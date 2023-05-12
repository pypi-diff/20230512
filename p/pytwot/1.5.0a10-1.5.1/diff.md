# Comparing `tmp/pytwot-1.5.0a10.tar.gz` & `tmp/pytwot-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytwot-1.5.0a10.tar", last modified: Fri May 12 13:41:13 2023, max compression
+gzip compressed data, was "pytwot-1.5.1.tar", last modified: Fri May 12 16:17:56 2023, max compression
```

## Comparing `pytwot-1.5.0a10.tar` & `pytwot-1.5.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 13:41:13.424806 pytwot-1.5.0a10/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1135 2023-05-12 12:55:37.000000 pytwot-1.5.0a10/LICENSE
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      137 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/MANIFEST.in
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     4322 2023-05-12 13:41:13.424806 pytwot-1.5.0a10/PKG-INFO
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     3327 2023-05-12 13:35:35.000000 pytwot-1.5.0a10/README.md
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 13:41:13.420806 pytwot-1.5.0a10/pytwot/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1422 2023-05-12 12:54:25.000000 pytwot-1.5.0a10/pytwot/__init__.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     2306 2023-05-12 13:09:31.000000 pytwot-1.5.0a10/pytwot/__main__.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    25574 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/attachments.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    22270 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/auth.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    54387 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/client.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     5620 2023-05-12 12:57:08.000000 pytwot-1.5.0a10/pytwot/compliance.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     4204 2023-05-12 12:57:15.000000 pytwot-1.5.0a10/pytwot/constants.py
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 13:41:13.424806 pytwot-1.5.0a10/pytwot/dataclass/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      231 2023-05-12 12:45:40.000000 pytwot-1.5.0a10/pytwot/dataclass/__init__.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1353 2023-05-12 13:00:03.000000 pytwot-1.5.0a10/pytwot/dataclass/app.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1984 2023-05-12 13:00:11.000000 pytwot-1.5.0a10/pytwot/dataclass/attachments.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1579 2023-05-12 13:00:16.000000 pytwot-1.5.0a10/pytwot/dataclass/compliance.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     2076 2023-05-12 13:00:21.000000 pytwot-1.5.0a10/pytwot/dataclass/embed.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     2111 2023-05-12 13:00:27.000000 pytwot-1.5.0a10/pytwot/dataclass/locations.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1407 2023-05-12 13:00:32.000000 pytwot-1.5.0a10/pytwot/dataclass/message.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     4804 2023-05-12 13:00:38.000000 pytwot-1.5.0a10/pytwot/dataclass/metrics.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     2242 2023-05-12 13:00:44.000000 pytwot-1.5.0a10/pytwot/dataclass/settings.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1322 2023-05-12 13:00:52.000000 pytwot-1.5.0a10/pytwot/dataclass/space.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1403 2023-05-12 13:00:58.000000 pytwot-1.5.0a10/pytwot/dataclass/stream.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     4829 2023-05-12 12:57:24.000000 pytwot-1.5.0a10/pytwot/entities.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     7725 2023-05-12 12:57:31.000000 pytwot-1.5.0a10/pytwot/enums.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     8887 2023-05-12 12:57:38.000000 pytwot-1.5.0a10/pytwot/environment.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     7153 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/errors.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    10182 2023-05-12 12:57:51.000000 pytwot-1.5.0a10/pytwot/events.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    38470 2023-05-12 13:09:31.000000 pytwot-1.5.0a10/pytwot/http.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    11728 2023-05-12 12:58:04.000000 pytwot-1.5.0a10/pytwot/list.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    15002 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/message.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1584 2023-05-12 12:58:24.000000 pytwot-1.5.0a10/pytwot/objects.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    17422 2023-05-12 12:58:33.000000 pytwot-1.5.0a10/pytwot/paginations.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    14626 2023-05-12 12:58:42.000000 pytwot-1.5.0a10/pytwot/parser.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        0 2023-05-12 12:45:40.000000 pytwot-1.5.0a10/pytwot/py.typed
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     6834 2023-05-12 12:58:49.000000 pytwot-1.5.0a10/pytwot/relations.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     9722 2023-05-12 12:58:55.000000 pytwot-1.5.0a10/pytwot/space.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    13357 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/stream.py
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 13:41:13.424806 pytwot-1.5.0a10/pytwot/threads/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     3257 2023-05-12 12:59:50.000000 pytwot-1.5.0a10/pytwot/threads/__init__.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    25687 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/tweet.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1286 2023-05-12 12:59:15.000000 pytwot-1.5.0a10/pytwot/type.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)    34247 2023-05-12 13:02:32.000000 pytwot-1.5.0a10/pytwot/user.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     4729 2023-05-12 12:59:39.000000 pytwot-1.5.0a10/pytwot/utils.py
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 13:41:13.424806 pytwot-1.5.0a10/pytwot.egg-info/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     4322 2023-05-12 13:41:13.000000 pytwot-1.5.0a10/pytwot.egg-info/PKG-INFO
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1001 2023-05-12 13:41:13.000000 pytwot-1.5.0a10/pytwot.egg-info/SOURCES.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-05-12 13:41:13.000000 pytwot-1.5.0a10/pytwot.egg-info/dependency_links.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      136 2023-05-12 13:41:13.000000 pytwot-1.5.0a10/pytwot.egg-info/requires.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        7 2023-05-12 13:41:13.000000 pytwot-1.5.0a10/pytwot.egg-info/top_level.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       50 2023-05-12 12:45:40.000000 pytwot-1.5.0a10/requirements.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       38 2023-05-12 13:41:13.424806 pytwot-1.5.0a10/setup.cfg
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1873 2023-05-12 13:09:31.000000 pytwot-1.5.0a10/setup.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 16:17:56.565810 pytwot-1.5.1/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1135 2023-05-12 12:55:37.000000 pytwot-1.5.1/LICENSE
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      136 2023-05-12 15:01:02.000000 pytwot-1.5.1/MANIFEST.in
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     3879 2023-05-12 16:17:56.565810 pytwot-1.5.1/PKG-INFO
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2887 2023-05-12 13:55:31.000000 pytwot-1.5.1/README.md
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 16:17:56.561810 pytwot-1.5.1/pytwot/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1419 2023-05-12 16:13:25.000000 pytwot-1.5.1/pytwot/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2306 2023-05-12 15:26:27.000000 pytwot-1.5.1/pytwot/__main__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    25552 2023-05-12 15:01:54.000000 pytwot-1.5.1/pytwot/attachments.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    22236 2023-05-12 15:01:54.000000 pytwot-1.5.1/pytwot/auth.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    54269 2023-05-12 16:14:35.000000 pytwot-1.5.1/pytwot/client.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     5621 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/compliance.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     4207 2023-05-12 14:56:12.000000 pytwot-1.5.1/pytwot/constants.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 16:17:56.565810 pytwot-1.5.1/pytwot/dataclass/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      231 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1354 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/app.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1985 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/attachments.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1579 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/compliance.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2076 2023-05-12 13:00:21.000000 pytwot-1.5.1/pytwot/dataclass/embed.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2111 2023-05-12 13:00:27.000000 pytwot-1.5.1/pytwot/dataclass/locations.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1408 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/message.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     4804 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/metrics.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2243 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/settings.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1322 2023-05-12 13:00:52.000000 pytwot-1.5.1/pytwot/dataclass/space.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1404 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/dataclass/stream.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     4829 2023-05-12 12:57:24.000000 pytwot-1.5.1/pytwot/entities.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     7725 2023-05-12 12:57:31.000000 pytwot-1.5.1/pytwot/enums.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     8888 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/environment.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     7154 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/errors.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    10183 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/events.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    37706 2023-05-12 16:03:05.000000 pytwot-1.5.1/pytwot/http.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    11706 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/list.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    15002 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/message.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1584 2023-05-12 12:58:24.000000 pytwot-1.5.1/pytwot/objects.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    17423 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/paginations.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    14627 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/parser.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        0 2023-05-12 12:45:40.000000 pytwot-1.5.1/pytwot/py.typed
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     6834 2023-05-12 12:58:49.000000 pytwot-1.5.1/pytwot/relations.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     9693 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/space.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    13328 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/stream.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 16:17:56.565810 pytwot-1.5.1/pytwot/threads/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     3258 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/threads/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    25811 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/tweet.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1285 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/type.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)    34247 2023-05-12 15:01:55.000000 pytwot-1.5.1/pytwot/user.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     4761 2023-05-12 15:21:07.000000 pytwot-1.5.1/pytwot/utils.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-12 16:17:56.561810 pytwot-1.5.1/pytwot.egg-info/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     3879 2023-05-12 16:17:56.000000 pytwot-1.5.1/pytwot.egg-info/PKG-INFO
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1001 2023-05-12 16:17:56.000000 pytwot-1.5.1/pytwot.egg-info/SOURCES.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-05-12 16:17:56.000000 pytwot-1.5.1/pytwot.egg-info/dependency_links.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      136 2023-05-12 16:17:56.000000 pytwot-1.5.1/pytwot.egg-info/requires.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        7 2023-05-12 16:17:56.000000 pytwot-1.5.1/pytwot.egg-info/top_level.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       50 2023-05-12 12:45:40.000000 pytwot-1.5.1/requirements.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       38 2023-05-12 16:17:56.565810 pytwot-1.5.1/setup.cfg
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1860 2023-05-12 15:05:05.000000 pytwot-1.5.1/setup.py
```

### Comparing `pytwot-1.5.0a10/LICENSE` & `pytwot-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/PKG-INFO` & `pytwot-1.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytwot
-Version: 1.5.0a10
+Version: 1.5.1
 Summary: A Synchronous python API wrapper for twitter's api
 Home-page: https://github.com/sengolda/pytwot
 Author: Sengolda
 Maintainer: Sengolda
 License: MIT
 Project-URL: Documentation, https://py-tweet.readthedocs.io/
 Project-URL: HomePage/Github, https://github.com/sengolda/pytwot/
@@ -32,37 +32,27 @@
 <p><b>Another note:</b> the support server given is support server for the original PyTweet as this is approved by the devs they requested the support server stay the same</p>
 
 <div>
 <img src="https://img.shields.io/pypi/v/pytwot?logo=pypi&style=plastic">  
 
 <img src="https://img.shields.io/badge/code%20style-black-000000.svg">  
 
-<img alt="PyPI - License" src="https://img.shields.io/pypi/l/pytwot">
-
-<img alt="Total Downloads" src="https://pepy.tech/badge/pytwot">
 
 <img src="https://img.shields.io/github/commit-activity/m/sengolda/pytwot?color=turquoise&logo=github&logoColor=black">
 
 
 <img src="https://img.shields.io/github/issues-pr/sengolda/pytwot?color=yellow&label=Pull%20Requests&logo=github&logoColor=black">
 
 
 <img src="https://img.shields.io/discord/858312394236624957?color=blue&label=pytwot&logo=discord">
 
 
-<img src='https://readthedocs.org/projects/py-tweet/badge/?version=latest' alt='Documentation Status' />
-
-
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard">
-
-
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fpremium">
+<img src='https://readthedocs.org/projects/pytwot/badge/?version=latest' alt='Documentation Status' />
 
 
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2">
 
 </div>
 <br>
 <br>
 <p align="center">pytwot is a synchronous Python API wrapper for the Twitter API. It is filled with rich features and is very easy to use.</p>
 
 ## Installation
@@ -97,15 +87,15 @@
 client.tweet("Hello world, Hello twitter!") #This requires read & write app permissions also elevated access type.
 ```
 
 You can check in the `examples` directory for more example code.
 
 # Links
 
-- [Documentation](https://py-tweet.readthedocs.io/en/latest/)
+- [Documentation](https://pytwot.readthedocs.io/en/latest/)
 
 - [Support Server](https://discord.gg/XHBhg6A4jJ)
 
 - [GitHub](https://github.com/sengolda/pytwot)
 
 - [PyPi](https://pypi.org/project/pytwot)
```

#### html2text {}

```diff
@@ -1,39 +1,34 @@
-Metadata-Version: 2.1 Name: pytwot Version: 1.5.0a10 Summary: A Synchronous
-python API wrapper for twitter's api Home-page: https://github.com/sengolda/
-pytwot Author: Sengolda Maintainer: Sengolda License: MIT Project-URL:
-Documentation, https://py-tweet.readthedocs.io/ Project-URL: HomePage/Github,
-https://github.com/sengolda/pytwot/ Project-URL: Discord, https://discord.gg/
-XHBhg6A4jJ Keywords: twitter,tweet.py twitter.py Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Operating System :: OS Independent Classifier: Topic
-:: Internet Classifier: Topic :: Utilities Classifier: Development Status :: 5
-- Production/Stable Requires-Python: >=3.7.0 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: pytwot Version: 1.5.1 Summary: A Synchronous python
+API wrapper for twitter's api Home-page: https://github.com/sengolda/pytwot
+Author: Sengolda Maintainer: Sengolda License: MIT Project-URL: Documentation,
+https://py-tweet.readthedocs.io/ Project-URL: HomePage/Github, https://
+github.com/sengolda/pytwot/ Project-URL: Discord, https://discord.gg/XHBhg6A4jJ
+Keywords: twitter,tweet.py twitter.py Platform: UNKNOWN Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent Classifier: Topic :: Internet
+Classifier: Topic :: Utilities Classifier: Development Status :: 5 -
+Production/Stable Requires-Python: >=3.7.0 Description-Content-Type: text/
 markdown Provides-Extra: docs Provides-Extra: events License-File: LICENSE
                               ***** pytwot *****
 This project is a fork of the now archived PyTweet
 VERY IMPORTANT: This project is approved by the PyTweet devs themselves.
 Another note: the support server given is support server for the original
 PyTweet as this is approved by the devs they requested the support server stay
 the same
 [https://img.shields.io/pypi/v/pytwot?logo=pypi&style=plastic] [https://
-img.shields.io/badge/code%20style-black-000000.svg] [PyPI - License] [Total
-Downloads] [https://img.shields.io/github/commit-activity/m/sengolda/
+img.shields.io/badge/code%20style-black-000000.svg] [https://img.shields.io/
+github/commit-activity/m/sengolda/
 pytwot?color=turquoise&logo=github&logoColor=black] [https://img.shields.io/
 github/issues-pr/sengolda/
 pytwot?color=yellow&label=Pull%20Requests&logo=github&logoColor=black] [https:/
 /img.shields.io/discord/
 858312394236624957?color=blue&label=pytwot&logo=discord] [Documentation Status]
-[https://img.shields.io/
-endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard] [https://
-img.shields.io/
-endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fpremium] [https://
-img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2]
 
 
  pytwot is a synchronous Python API wrapper for the Twitter API. It is filled
                   with rich features and is very easy to use.
 ## Installation ### Windows ```bash py -m pip install pytwot ``` ### Linux/
 MacOS ```bash python3 -m pip install pytwot ``` ## Usage Before using pytwot
 you have to setup an application [here](https://apps.twitter.com). For a more
@@ -45,15 +40,15 @@
 /discord.gg/nxZCE9EbVr). ```py import pytwot client = pytwot.Client( "Your
 Bearer Token Here!!!", consumer_key="Your consumer key here",
 consumer_secret="Your consumer secret here", access_token="Your access token
 here", access_token_secret="Your access token secret here", ) #Before using
 pytwot, make sure to create an application in https://apps.twitter.com.
 client.tweet("Hello world, Hello twitter!") #This requires read & write app
 permissions also elevated access type. ``` You can check in the `examples`
-directory for more example code. # Links - [Documentation](https://py-
-tweet.readthedocs.io/en/latest/) - [Support Server](https://discord.gg/
+directory for more example code. # Links - [Documentation](https://
+pytwot.readthedocs.io/en/latest/) - [Support Server](https://discord.gg/
 XHBhg6A4jJ) - [GitHub](https://github.com/sengolda/pytwot) - [PyPi](https://
 pypi.org/project/pytwot) # Contribute You can Contribute or open an issue
 regarding pytwot in our [GitHub repository](https://github.com/sengolda/
 pytwot)! # Licence & Copyright All files of this repo are protected and
 licensed with the [MIT License](https://opensource.org/licenses/MIT), [LICENSE
 File](LICENSE)
```

### Comparing `pytwot-1.5.0a10/README.md` & `pytwot-1.5.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 <p><b>Another note:</b> the support server given is support server for the original PyTweet as this is approved by the devs they requested the support server stay the same</p>
 
 <div>
 <img src="https://img.shields.io/pypi/v/pytwot?logo=pypi&style=plastic">  
 
 <img src="https://img.shields.io/badge/code%20style-black-000000.svg">  
 
-<img alt="PyPI - License" src="https://img.shields.io/pypi/l/pytwot">
-
-<img alt="Total Downloads" src="https://pepy.tech/badge/pytwot">
 
 <img src="https://img.shields.io/github/commit-activity/m/sengolda/pytwot?color=turquoise&logo=github&logoColor=black">
 
 
 <img src="https://img.shields.io/github/issues-pr/sengolda/pytwot?color=yellow&label=Pull%20Requests&logo=github&logoColor=black">
 
 
 <img src="https://img.shields.io/discord/858312394236624957?color=blue&label=pytwot&logo=discord">
 
 
-<img src='https://readthedocs.org/projects/py-tweet/badge/?version=latest' alt='Documentation Status' />
-
-
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard">
-
-
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fpremium">
+<img src='https://readthedocs.org/projects/pytwot/badge/?version=latest' alt='Documentation Status' />
 
 
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2">
 
 </div>
 <br>
 <br>
 <p align="center">pytwot is a synchronous Python API wrapper for the Twitter API. It is filled with rich features and is very easy to use.</p>
 
 ## Installation
@@ -69,15 +59,15 @@
 client.tweet("Hello world, Hello twitter!") #This requires read & write app permissions also elevated access type.
 ```
 
 You can check in the `examples` directory for more example code.
 
 # Links
 
-- [Documentation](https://py-tweet.readthedocs.io/en/latest/)
+- [Documentation](https://pytwot.readthedocs.io/en/latest/)
 
 - [Support Server](https://discord.gg/XHBhg6A4jJ)
 
 - [GitHub](https://github.com/sengolda/pytwot)
 
 - [PyPi](https://pypi.org/project/pytwot)
```

#### html2text {}

```diff
@@ -1,26 +1,21 @@
                               ***** pytwot *****
 This project is a fork of the now archived PyTweet
 VERY IMPORTANT: This project is approved by the PyTweet devs themselves.
 Another note: the support server given is support server for the original
 PyTweet as this is approved by the devs they requested the support server stay
 the same
 [https://img.shields.io/pypi/v/pytwot?logo=pypi&style=plastic] [https://
-img.shields.io/badge/code%20style-black-000000.svg] [PyPI - License] [Total
-Downloads] [https://img.shields.io/github/commit-activity/m/sengolda/
+img.shields.io/badge/code%20style-black-000000.svg] [https://img.shields.io/
+github/commit-activity/m/sengolda/
 pytwot?color=turquoise&logo=github&logoColor=black] [https://img.shields.io/
 github/issues-pr/sengolda/
 pytwot?color=yellow&label=Pull%20Requests&logo=github&logoColor=black] [https:/
 /img.shields.io/discord/
 858312394236624957?color=blue&label=pytwot&logo=discord] [Documentation Status]
-[https://img.shields.io/
-endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard] [https://
-img.shields.io/
-endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fpremium] [https://
-img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2]
 
 
  pytwot is a synchronous Python API wrapper for the Twitter API. It is filled
                   with rich features and is very easy to use.
 ## Installation ### Windows ```bash py -m pip install pytwot ``` ### Linux/
 MacOS ```bash python3 -m pip install pytwot ``` ## Usage Before using pytwot
 you have to setup an application [here](https://apps.twitter.com). For a more
@@ -32,15 +27,15 @@
 /discord.gg/nxZCE9EbVr). ```py import pytwot client = pytwot.Client( "Your
 Bearer Token Here!!!", consumer_key="Your consumer key here",
 consumer_secret="Your consumer secret here", access_token="Your access token
 here", access_token_secret="Your access token secret here", ) #Before using
 pytwot, make sure to create an application in https://apps.twitter.com.
 client.tweet("Hello world, Hello twitter!") #This requires read & write app
 permissions also elevated access type. ``` You can check in the `examples`
-directory for more example code. # Links - [Documentation](https://py-
-tweet.readthedocs.io/en/latest/) - [Support Server](https://discord.gg/
+directory for more example code. # Links - [Documentation](https://
+pytwot.readthedocs.io/en/latest/) - [Support Server](https://discord.gg/
 XHBhg6A4jJ) - [GitHub](https://github.com/sengolda/pytwot) - [PyPi](https://
 pypi.org/project/pytwot) # Contribute You can Contribute or open an issue
 regarding pytwot in our [GitHub repository](https://github.com/sengolda/
 pytwot)! # Licence & Copyright All files of this repo are protected and
 licensed with the [MIT License](https://opensource.org/licenses/MIT), [LICENSE
 File](LICENSE)
```

### Comparing `pytwot-1.5.0a10/pytwot/__init__.py` & `pytwot-1.5.1/pytwot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,54 +6,55 @@
 
 :copyright: (c) 2021-present UnrealFar & TheGenocides, 2023-present Sengolda
 :license: MIT, see LICENSE for more details.
 """
 import logging
 from typing import Literal, NamedTuple
 
-from .dataclass import *
 from .attachments import *
 from .auth import *
 from .client import *
 from .compliance import *
+from .constants import *
+from .dataclass import *
 from .entities import *
 from .enums import *
 from .environment import *
 from .errors import *
 from .events import *
-from .constants import *
 from .http import *
 from .list import *
 from .message import *
 from .objects import *
 from .paginations import *
 from .parser import *
 from .relations import *
 from .space import *
 from .stream import *
 from .tweet import *
 from .user import *
 from .utils import *
 
 __title__ = "pytwot"
-__version__ = "1.5.0a10"
 __author__ = "Sengolda"
+__version__ = "1.5.1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2021-present UnrealFar & TheGenocides, 2023-present Sengolda"
 
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=1, minor=5, micro=0, releaselevel="alpha", serial=10)
+version_info: VersionInfo = VersionInfo(major=1, minor=5, micro=1, releaselevel="final", serial=1)
+
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 assert version_info.releaselevel in (
     "alpha",
     "beta",
     "candidate",
```

### Comparing `pytwot-1.5.0a10/pytwot/__main__.py` & `pytwot-1.5.1/pytwot/__main__.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/attachments.py` & `pytwot-1.5.1/pytwot/attachments.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,27 +24,26 @@
 """
 
 from __future__ import annotations
 
 import datetime
 import io
 import os
-from typing import Any, Dict, List, Optional, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-from .dataclass import PollOption, Option, Button
+from .constants import LANGUAGES_CODES
+from .dataclass import Button, NonPublicMediaMetrics, Option, OrganicMediaMetrics, PollOption, PromotedMediaMetrics
 from .enums import ButtonType, MediaType
-from .utils import time_parse_todt, guess_mimetype, convert
 from .errors import pytwotException
-from .constants import LANGUAGES_CODES
 from .objects import Comparable
-from .dataclass import NonPublicMediaMetrics, OrganicMediaMetrics, PromotedMediaMetrics
+from .utils import convert, guess_mimetype, time_parse_todt
 
 if TYPE_CHECKING:
-    from .type import ID
     from .http import HTTPClient
+    from .type import ID
 
 __all__ = ("Media", "Poll", "QuickReply", "Geo", "CTA", "File", "SubFile")
 
 
 class Media:
     """Represents a media attachment in a message.
```

### Comparing `pytwot-1.5.0a10/pytwot/auth.py` & `pytwot-1.5.1/pytwot/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
 import base64
+import datetime
 import random
 import string
-import datetime
-
 from random import randint
-from typing import Tuple, Optional, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal, Optional, Tuple
+
 from requests_oauthlib import OAuth1
+
 from .errors import pytwotException
 
 if TYPE_CHECKING:
     from .http import HTTPClient
 
 __all__ = ("OauthSession", "Scope")
 
@@ -235,16 +236,15 @@
 
 
         .. versionadded:: 1.5.0
         """
         value = ""
         for attr in dir(self):
             if "_read" in attr or "_write" in attr or "_access" in attr:
-                scope = getattr(self, attr, None)
-                if scope:
+                if scope := getattr(self, attr, None):
                     value += f"{attr.replace('_', '.')}%20"
 
         return value.rstrip("%20")  # Only remove the last %20.
 
 
 class OauthSession:
     """Represents an OauthSession for OAuth1 and OAuth2 Authorization.
@@ -310,37 +310,37 @@
 
     @property
     def basic_auth(self) -> str:
         """:class:`str`: The decoded base64 encoded client id and secret.
 
         .. versionadded:: 1.5.0
         """
-        if not self.client_id and not self.client_secret:
+        if self.client_id or self.client_secret:
+            return base64.b64encode(bytes(f"{self.client_id}:{self.client_secret}", "utf-8")).decode()
+        else:
             raise pytwotException("'client_id' and 'client_secret' argument is missing in your client instance!")
 
-        return base64.b64encode(bytes(f"{self.client_id}:{self.client_secret}", "utf-8")).decode()
-
     def invalidate_access_token(self) -> None:
         """Invalidate the access token and access token secret of yout client.
 
         .. warning::
             This staticmethod will invalidate your access token and access token secret of your client.
 
 
         .. versionadded:: 1.3.5
         """
         self.http_client.request("POST", "1.1", "/oauth/invalidate_token", auth=True)
 
     def verify_credentials(self, *, raise_error: bool = True) -> Optional[bool]:
-        """Verify the credentials are correct. Returns a boolean whether its succesful or not if raise_error turns to False. Default to True
+        """Verify the credentials are correct. Returns a boolean whether its successful or not if raise_error turns to False. Default to True
 
         Parameters
         ------------
         raise_error: :class:`bool`
-            Indicates whether to raise if the credentials are wrong. If sets to False, the method will returns a boolean, True for succesful and False for error.
+            Indicates whether to raise if the credentials are wrong. If sets to False, the method will returns a boolean, True for successful and False for error.
 
         Raises
         --------
         :class:`Forbidden`
             Raised if the credentials are wrong.
 
 
@@ -350,15 +350,15 @@
             error = None
             self.http_client.request("GET", "1.1", "/account/verify_credentials.json", auth=True)
         except Exception as e:
             error = e
         finally:
             if not error:
                 return True
-            elif error and raise_error:
+            elif raise_error:
                 raise error
             else:
                 return False
 
     def generate_request_tokens(
         self, access_type: Optional[Literal["read", "write", "direct_messages"]] = None
     ) -> dict:
@@ -384,15 +384,15 @@
         .. versionadded:: 1.3.5
         """
         try:
             if access_type:
                 url = f"/request_token?x_auth_access_type={access_type}"
 
             else:
-                url = f"/request_token"
+                url = "/request_token"
 
             request_tokens = self.http_client.request("POST", "oauth", url, auth=self.oauth1)
             data = {}
             for credential in request_tokens.split("&"):
                 k, v = credential.split("=")
                 data[k] = v
             return data
@@ -431,19 +431,19 @@
         assert access_type in (
             "read",
             "write",
             "direct_messages",
         ), "Wrong access type passed! must be 'read', 'write', or 'direct_messages')"
         request_tokens = self.generate_request_tokens(access_type)
         authorize_url = (
-            self.http_client.base_url + "oauth/authorize"
+            f"{self.http_client.base_url}oauth/authorize"
             if not signin_with_twitter
-            else self.http_client.base_url + "oauth/authenticate"
+            else f"{self.http_client.base_url}oauth/authenticate"
         )
-        return authorize_url + f"?oauth_token={request_tokens.get('oauth_token')}"
+        return f"{authorize_url}?oauth_token={request_tokens.get('oauth_token')}"
 
     def post_oauth_token(self, oauth_token: str, oauth_verifier: str) -> Optional[Tuple[str]]:
         """Posts the oauth token & verifier. This is the 2nd step(and the last step) of making a request on behalf of other users through oauth1.1 usercontext. Returns a pair of access token & secret also the user's username(present as screen_name) and id e.g ("access_token=xxxxxxxxxxxxx", "access_token_secret=xxxxxxxxxxxxx", "screen_name=TheGenocides", "user_id=1382006704171196419"). Uses the access token and secret to make request on behalf of users! You can use the raw api or construct another client with the access token and secret.
 
         Parameters
         ------------
         oauth_token: :class:`str`
@@ -489,30 +489,30 @@
 
         .. versionadded:: 1.5.0
         """
         if not self.callback_url:
             raise pytwotException("'callback_url' argument is missing in your client instance")
 
         code_challenge_method = code_challenge_method.lower()
-        assert code_challenge_method in [
+        assert code_challenge_method in {
             "plain",
             "s256",
-        ], "Wrong code_challenge_method passed: must be 'plain' or 's256'"
+        }, "Wrong code_challenge_method passed: must be 'plain' or 's256'"
 
         if not state:
             state = "".join(random.choices(string.ascii_uppercase + string.digits, k=10)).lower()
         else:
             state = base64.b64decode(state.encode())
 
         now = datetime.datetime.now()
         timestamp = now.strftime("%m%d%Y%H%M%S")
         random_append = randint(1000, 100000)
         rand_dec = randint(300, 800)
         state = base64.b64encode(state.encode()).decode()
-        code_challenge = "{}{}.{}".format(timestamp, random_append, rand_dec)
+        code_challenge = f"{timestamp}{random_append}.{rand_dec}"
         client_id = self.client_id
         response_type = "code"
         scope = scope.value
 
         return f"https://twitter.com/i/oauth2/authorize?response_type={response_type}&client_id={client_id}&redirect_uri={self.callback_url}&scope={scope}&state={state}&code_challenge={code_challenge}&code_challenge_method={code_challenge_method}"
 
     def post_auth_code(self, code: str, code_challenge: str):
```

### Comparing `pytwot-1.5.0a10/pytwot/client.py` & `pytwot-1.5.1/pytwot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,43 +22,44 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
 import base64
+import datetime
 import hashlib
 import hmac
 import json
 import logging
-import time
 import threading
-import datetime
-from urllib.parse import urlparse
+import time
 from asyncio import iscoroutinefunction
 from http import HTTPStatus
-from typing import Callable, List, Optional, Union, Any
+from typing import Any, Callable, List, Optional, Union
+from urllib.parse import urlparse
+
 from flask import Flask, request
 
-from .paginations import MessagePagination
 from .attachments import CTA, CustomProfile, File, Geo, Poll, QuickReply
-from .enums import ReplySetting, SpaceState, Granularity, JobType, JobStatus
-from .constants import TWEET_EXPANSION, USER_FIELD, MEDIA_FIELD, PLACE_FIELD, POLL_FIELD, TWEET_FIELD
-from .errors import pytwotException, UnKnownSpaceState
+from .compliance import Job
+from .constants import MEDIA_FIELD, PLACE_FIELD, POLL_FIELD, TWEET_EXPANSION, TWEET_FIELD, USER_FIELD
+from .dataclass import Location, Trend
+from .enums import Granularity, JobStatus, JobType, ReplySetting, SpaceState
+from .environment import Environment, Webhook
+from .errors import UnKnownSpaceState, pytwotException
 from .http import HTTPClient
+from .list import List as TwitterList
 from .message import DirectMessage, WelcomeMessage, WelcomeMessageRule
+from .paginations import MessagePagination
 from .space import Space
 from .stream import Stream
 from .tweet import Tweet
-from .user import User, ClientAccount
-from .environment import Environment, Webhook
-from .dataclass import Location, Trend
-from .list import List as TwitterList
 from .type import ID
-from .compliance import Job
+from .user import ClientAccount, User
 
 __all__ = ("Client",)
 
 _log = logging.getLogger(__name__)
 
 
 class Client:
@@ -82,16 +83,16 @@
         The oauth callback url, default to None. Makes sure the callback url is the same as the one in your application auth-settings or else it can't create and interact with oauth related methods.
     client_id: Optional[:class:`str`]
         The client's OAuth 2.0 Client ID from keys and tokens page.
     client_secret: Optional[:class:`str`]
         The client's OAuth 2.0 Client Secret from keys and tokens page.
     use_bearer_only: bool
         Indicates to only use bearer token for all methods. This mean the client is now a twitter-api-client v2 interface. Some methods are unavailable to use such as fetching trends and location, environment fetching methods, and features such as events. Some methods can be recover with OAuth 2 authorization code flow with PKCE with the correct scopes or permissions. Like users.read scope for reading users info which some methods provide a way like :meth:`Client.fetch_user`.
-    sleep_after_ratelimit: :class:`bool`
-        Indicates to sleep when your client is ratelimited, If set to True it won't raise :class:`TooManyRequests` error but it would print a message indicating to sleep, then it sleeps for how many seconds it needs to sleep, after that it continue to restart the request.
+    handle_ratelimits: :class:`bool`
+        Indicates to handle ratelimits and sleep when your client is ratelimited, If set to False it will raise :class:`TooManyRequests` error when ratelimited.
     verify_credentials: :class:`bool`
         Indicates to verify the credentials you specified, this includes consumer_key, consumer_secret, access_token, access_token_secret. make sure to specified all of them in your client, you cannot specified only one of them.
 
     Attributes
     ------------
     webhook: Optional[:class:`Webhook`]
         Returns the client's main webhook, Returns None if not found.
@@ -113,49 +114,49 @@
         access_token: Optional[str] = None,
         access_token_secret: Optional[str] = None,
         stream: Optional[Stream] = None,
         callback_url: Optional[str] = None,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         use_bearer_only: bool = False,
-        sleep_after_ratelimit: bool = False,
+        handle_ratelimits: bool = True,
         verify_credentials: bool = False,
     ) -> None:
         self.http = HTTPClient(
             bearer_token,
             consumer_key=consumer_key,
             consumer_secret=consumer_secret,
             access_token=access_token,
             access_token_secret=access_token_secret,
             stream=stream,
             callback_url=callback_url,
             client_id=client_id,
             client_secret=client_secret,
             use_bearer_only=use_bearer_only,
-            sleep_after_ratelimit=sleep_after_ratelimit,
+            handle_ratelimits=handle_ratelimits,
         )
         self._account_user: Optional[User] = None  # set in account property.
         self.webhook: Optional[Webhook] = None
         self.environment: Optional[Environment] = None
         self.webhook_url_path: Optional[str] = None
         self.executor = self.http.thread_manager.create_new_executor(thread_name="main-executor")
         self.verify_credentials = verify_credentials
         if self.verify_credentials:
             self.http.oauth_session.verify_credentials(raise_error=True)
 
     def __repr__(self) -> str:
         return "Client({0.account!r})".format(self)
 
     def account(self, *, update: bool = False) -> Optional[ClientAccount]:
-        """Returns :class:`ClientAccount` object which hold the client's informations as a twitter user.
+        """Returns :class:`ClientAccount` object which hold the client's information as a twitter user.
 
         Parameters
         ------------
         update: :class:`bool`
-            Indicates to update the client's account information, setting update to True would make a request to the api and returns a new and updated data everytime. If sets to False, it will either make a request (if used the first time) or use the previous data stored in an instance variable.
+            Indicates to update the client's account information, setting update to True would make a request to the api and returns a new and updated data every time. If sets to False, it will either make a request (if used the first time) or use the previous data stored in an instance variable.
 
             .. versionadded:: 1.5.0
 
 
         Returns
         ---------
         Optional[:class:`ClientAccount`]
@@ -173,15 +174,15 @@
 
     def me(self, *, update: bool = False) -> Optional[ClientAccount]:
         """An alias to :meth:`Client.account`.
 
         Parameters
         ------------
         update: :class:`bool`
-            Indicates to update the client's account information, setting update to True would make a request to the api and returns a new and updated data everytime. If sets to False, it will either make a request (if used the first time) or use the previous data stored in an instance variable.
+            Indicates to update the client's account information, setting update to True would make a request to the api and returns a new and updated data every time. If sets to False, it will either make a request (if used the first time) or use the previous data stored in an instance variable.
 
             .. versionadded:: 1.5.0
 
 
         Returns
         ---------
         Optional[:class:`ClientAccount`]
@@ -369,15 +370,15 @@
         return self.http.fetch_welcome_message_rule(welcome_message_rule_id)
 
     def fetch_space(self, space_id: ID, *, space_host: bool = False) -> Space:
         """Fetches a space.
 
         .. warning
 
-            This will cause error if `space_host` paramater is True and the client is not the host of the Space!
+            This will cause error if `space_host` parameter is True and the client is not the host of the Space!
 
 
         Parameters
         ------------
         space_id: :class:`ID`
             Represents the space ID that you wish to get info with.
         space_host: :class:`bool`
@@ -417,15 +418,15 @@
         ---------
         Optional[List[:class:`Space`]]
             This method returns a list of :class:`Space` objects.
 
 
         .. versionadded:: 1.3.5
         """
-        if state == SpaceState.live or state == SpaceState.scheduled:
+        if state in [SpaceState.live, SpaceState.scheduled]:
             return self.http.fetch_spaces_bytitle(title, state, space_host=space_host)
         else:
             raise UnKnownSpaceState(given_state=state)
 
     def fetch_list(self, id: ID) -> TwitterList:
         """Fetches a twitter list using its id
 
@@ -470,15 +471,18 @@
         res = self.http.request("GET", "1.1", "/direct_messages/events/list.json", auth=True, params=params)
 
         if not res or not res.get("events"):
             return []
 
         res = self.http.payload_parser.parse_message_to_pagination_data(res)
         return MessagePagination(
-            res, endpoint_request=f"/direct_messages/events/list.jsons", http_client=self.http, params=params
+            res,
+            endpoint_request="/direct_messages/events/list.jsons",
+            http_client=self.http,
+            params=params,
         )
 
     def fetch_job(self, id: ID) -> Optional[Job]:
         """Fetches a job.
 
         Parameters
         ------------
@@ -1148,15 +1152,15 @@
                     validation = hmac.new(
                         key=bytes(self.http.consumer_secret, "UTF-8"),
                         msg=bytes(crc, "UTF-8"),
                         digestmod=hashlib.sha256,
                     )
                     digested = base64.b64encode(validation.digest())
 
-                    response = {"response_token": "sha256=" + format(str(digested)[2:-1])}
+                    response = {"response_token": f"sha256={format(str(digested)[2:-1])}"}
 
                     return json.dumps(response)
 
                 json_data = request.get_json()
                 _log.debug(f"An event triggered! {json_data}")
                 self.executor.submit(self.http.handle_events, payload=json_data)
                 return ("", HTTPStatus.OK)
@@ -1199,15 +1203,15 @@
                 )
             thread.join()
         except Exception as e:
             _log.warn(f"An error was caught during listening: {e}")
             raise e
 
         finally:
-            _log.debug(f"Stop listening due to internal/external problem!")
+            _log.debug("Stop listening due to internal/external problem!")
 
     def listen_to(self, url: str, *, env_label: str, ngrok: bool = False, make_new: bool = True):
         """Listen to upcoming account activity events send by twitter to a web application url. This method differ from :meth:`Client.listen`, this method doesn't use the flask's web application url, rather your web application url. This is good for people that want to implement their web application outside flask.
 
         .. warning::
             With this method, you have to make your own CRC and event handlers in your web application. For the time being, the documentation doesn't provides information for the handlers, either go to twitter documentation about account activity api or wait until we write the documentation.
 
@@ -1257,15 +1261,15 @@
             for user in users:
                 self.http.user_cache[user.id] = user
 
             _log.debug(
                 f"Listening for events! user cache filled at {len(self.http.user_cache)} users! flask application is running with url: {url}({self.webhook_url_path}).\n Ngrok: {ngrok}\nMake a new webhook when not found: {make_new}\n In Environment: {repr(self.environment)} with webhook: {repr(self.webhook)}."
             )
 
-        elif check and not make_new:
+        elif check:
             raise pytwotException(
                 f"Cannot find url passed: {url} Invalid url passed, please check the spelling of your url"
             )
 
         else:
             self.webhook.trigger_crc()
             ids = self.environment.fetch_all_subscriptions()
```

### Comparing `pytwot-1.5.0a10/pytwot/compliance.py` & `pytwot-1.5.1/pytwot/compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
 import datetime
-import requests
 import json
+from typing import TYPE_CHECKING, List, Optional
+
+import requests
 
-from typing import Optional, List, TYPE_CHECKING
+from .dataclass import JobResult
+from .enums import JobResultAction, JobResultActionReason, JobStatus, JobType
 from .objects import Comparable
 from .utils import time_parse_todt
-from .enums import JobType, JobStatus, JobResultAction, JobResultActionReason
-from .dataclass import JobResult
 
 if TYPE_CHECKING:
     from .http import HTTPClient
     from .type import ID, Payload
 
 
 class Job(Comparable):
```

### Comparing `pytwot-1.5.0a10/pytwot/constants.py` & `pytwot-1.5.1/pytwot/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,28 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
+
 # Expansions & Fields use for extend object data.
 TWEET_EXPANSION = "attachments.poll_ids,attachments.media_keys,author_id,geo.place_id,in_reply_to_user_id,referenced_tweets.id,entities.mentions.username,referenced_tweets.id.author_id"
 SPACE_EXPANSION = "invited_user_ids,speaker_ids,creator_id,host_ids,topic_ids"
 LIST_EXPANSION = "owner_id"
 PINNED_TWEET_EXPANSION = "pinned_tweet_id"
 
 TWEET_FIELD = "attachments,author_id,context_annotations,conversation_id,created_at,geo,entities,in_reply_to_user_id,lang,possibly_sensitive,public_metrics,referenced_tweets,reply_settings,source,text,withheld"
-COMPLETE_TWEET_FIELD = TWEET_FIELD + ",organic_metrics,promoted_metrics"
-TWEET_FIELD_WITH_ORGANIC_METRICS = TWEET_FIELD + ",organic_metrics"
-TWEET_FIELD_WITH_PROMOTED_METRICS = TWEET_FIELD + ",promoted_metrics"
+COMPLETE_TWEET_FIELD = f"{TWEET_FIELD},organic_metrics,promoted_metrics"
+TWEET_FIELD_WITH_ORGANIC_METRICS = f"{TWEET_FIELD},organic_metrics"
+TWEET_FIELD_WITH_PROMOTED_METRICS = f"{TWEET_FIELD},promoted_metrics"
 USER_FIELD = "created_at,description,entities,id,location,name,profile_image_url,protected,public_metrics,url,username,verified,withheld,pinned_tweet_id"
 SPACE_FIELD = "host_ids,created_at,creator_id,id,lang,invited_user_ids,participant_count,speaker_ids,started_at,state,title,updated_at,scheduled_start,is_ticketed"
-COMPLETE_SPACE_FIELD = SPACE_FIELD + ",subscriber_count"
+COMPLETE_SPACE_FIELD = f"{SPACE_FIELD},subscriber_count"
 MEDIA_FIELD = "duration_ms,height,media_key,preview_image_url,public_metrics,type,url,width"
 PLACE_FIELD = "contained_within,country,country_code,full_name,geo,id,name,place_type"
 POLL_FIELD = "duration_minutes,end_datetime,id,options,voting_status"
 TOPIC_FIELD = "id,name,description"
 LIST_FIELD = "created_at,follower_count,member_count,private,description,owner_id"
 
 # Indicator for the return_when argument in wait_for_futures method.
@@ -85,16 +86,16 @@
     "it-IT": "Italian",
     "jp-JP": "Japanese",
     "ko-KR": "Korean",
     "nl-BE": "Dutch",
     "nl-NL": "Dutch",
     "no-NO": "Norwegian",
     "pl-PL": "Polish",
-    "pt-BR": "Portugese",
-    "pt-PT": "Portugese",
+    "pt-BR": "Portuguese",
+    "pt-PT": "Portuguese",
     "ro-RO": "Romanian",
     "ru-RU": "Russian",
     "sk-SK": "Slovak",
     "sv-SE": "Swedish",
     "ta-IN": "Tamil",
     "ta-LK": "Tamil",
     "th-TH": "Thai",
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/app.py` & `pytwot-1.5.1/pytwot/dataclass/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from dataclasses import dataclass
+
 from ..type import ID
 
 
 @dataclass
 class ApplicationInfo:
     """Represents an application's info.
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/attachments.py` & `pytwot-1.5.1/pytwot/dataclass/attachments.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from dataclasses import dataclass
-from typing import Union, Optional
+from typing import Optional, Union
+
 from ..enums import ButtonType
 
 
 @dataclass
 class Option:
     """Represents an Option object for :class:`QuickReply`. You can add an Option using :meth:`QuickReply.add_option`.
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/compliance.py` & `pytwot-1.5.1/pytwot/dataclass/compliance.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import datetime
-
 from dataclasses import dataclass
 from typing import Optional
-from ..type import ID
+
 from ..enums import JobResultAction, JobResultActionReason
+from ..type import ID
 
 
 @dataclass
 class JobResult:
     """Represents a download result from a job.
 
     .. versionadded:: 1.5.0
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/embed.py` & `pytwot-1.5.1/pytwot/dataclass/embed.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/locations.py` & `pytwot-1.5.1/pytwot/dataclass/locations.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/message.py` & `pytwot-1.5.1/pytwot/dataclass/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from dataclasses import dataclass
+
 from ..type import ID
 
 
 @dataclass
 class InitiatedVia:
     """Represents an object that stores 'initiated_via' key from direct message event data.
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/metrics.py` & `pytwot-1.5.1/pytwot/dataclass/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from dataclasses import dataclass
-from typing import Union, Optional
+from typing import Optional, Union
 
 # TODO: Finish adding metrics and stuff
 
 __all__ = (
     "PublicUserMetrics",
     "PublicTweetMetrics",
     "NonPublicTweetMetrics",
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/settings.py` & `pytwot-1.5.1/pytwot/dataclass/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from dataclasses import dataclass
 from typing import Optional
+
 from .locations import Location, TimezoneInfo
 
 
 @dataclass
 class SleepTimeSettings:
     """Represents a setting for sleep time from a user setting.
```

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/space.py` & `pytwot-1.5.1/pytwot/dataclass/space.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/dataclass/stream.py` & `pytwot-1.5.1/pytwot/dataclass/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from dataclasses import dataclass
 from typing import Optional
+
 from ..type import ID
 
 
 @dataclass
 class StreamRule:
     """Represents a stream rule.
```

### Comparing `pytwot-1.5.0a10/pytwot/entities.py` & `pytwot-1.5.1/pytwot/entities.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/enums.py` & `pytwot-1.5.1/pytwot/enums.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/environment.py` & `pytwot-1.5.1/pytwot/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
-import logging
 import datetime
-from typing import Any, List, Dict, TYPE_CHECKING
-from .utils import time_parse_todt
+import logging
+from typing import TYPE_CHECKING, Any, Dict, List
+
 from .objects import Comparable
+from .utils import time_parse_todt
 
 if TYPE_CHECKING:
     from .client import Client
     from .type import ID
 
 _log = logging.getLogger(__name__)
```

### Comparing `pytwot-1.5.0a10/pytwot/errors.py` & `pytwot-1.5.1/pytwot/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import requests
-from typing import Optional
 from json import decoder
+from typing import Optional
+
+import requests
 
 
 class pytwotException(Exception):
     """This is the base class of all exceptions Raise by pytwot. This inherits :class:`Exception`.
 
     .. versionadded:: 1.2.0
     """
```

### Comparing `pytwot-1.5.0a10/pytwot/events.py` & `pytwot-1.5.1/pytwot/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import datetime
-from typing import Union, Optional
-from .user import User
-from .tweet import Tweet
+from typing import Optional, Union
+
 from .enums import ActionEventType, UserActionEventType
+from .tweet import Tweet
 from .type import Payload
+from .user import User
 from .utils import time_parse_todt
 
 # Events type
 
 
 class Event:
     """The base class of all event, this provides a type property that the event belongs to.
```

### Comparing `pytwot-1.5.0a10/pytwot/http.py` & `pytwot-1.5.1/pytwot/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,65 +25,66 @@
 
 from __future__ import annotations
 
 import io
 import logging
 import sys
 import time
-import requests
 from json import JSONDecodeError
-from typing import Any, List, NoReturn, Optional, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, List, NoReturn, Optional, Union
+
+import requests
 
 from .attachments import CTA, CustomProfile, File, Geo, Poll, QuickReply
 from .auth import OauthSession
-from .enums import ReplySetting, SpaceState, Granularity, JobType, JobStatus
-from .errors import (
-    BadRequests,
-    Conflict,
-    Forbidden,
-    NotFound,
-    TooManyRequests,
-    pytwotException,
-    Unauthorized,
-    FieldsTooLarge,
-    UnauthorizedForResource,
-    ResourceNotFound,
-    DisallowedResource,
-)
+from .compliance import Job
 from .constants import (
-    TWEET_EXPANSION,
-    SPACE_EXPANSION,
+    COMPLETE_SPACE_FIELD,
+    COMPLETE_TWEET_FIELD,
     LIST_EXPANSION,
-    PINNED_TWEET_EXPANSION,
+    LIST_FIELD,
     MEDIA_FIELD,
+    PINNED_TWEET_EXPANSION,
     PLACE_FIELD,
     POLL_FIELD,
+    SPACE_EXPANSION,
     SPACE_FIELD,
-    COMPLETE_SPACE_FIELD,
+    TOPIC_FIELD,
+    TWEET_EXPANSION,
     TWEET_FIELD,
-    COMPLETE_TWEET_FIELD,
     TWEET_FIELD_WITH_ORGANIC_METRICS,
     TWEET_FIELD_WITH_PROMOTED_METRICS,
     USER_FIELD,
-    TOPIC_FIELD,
-    LIST_FIELD,
 )
+from .enums import Granularity, JobStatus, JobType, ReplySetting, SpaceState
+from .errors import (
+    BadRequests,
+    Conflict,
+    DisallowedResource,
+    FieldsTooLarge,
+    Forbidden,
+    NotFound,
+    ResourceNotFound,
+    TooManyRequests,
+    Unauthorized,
+    UnauthorizedForResource,
+    pytwotException,
+)
+from .list import List as TwitterList
 from .message import DirectMessage, WelcomeMessage, WelcomeMessageRule
 from .parser import EventParser
+from .relations import RelationUpdate
 from .space import Space
-from .tweet import Tweet
-from .user import User, ClientAccount
 from .threads import ThreadManager
-from .relations import RelationUpdate
-from .list import List as TwitterList
-from .compliance import Job
+from .tweet import Tweet
+from .user import ClientAccount, User
 
 if TYPE_CHECKING:
-    from .type import ID, Payload, ResponsePayload
     from .stream import Stream
+    from .type import ID, Payload, ResponsePayload
 
 _log = logging.getLogger(__name__)
 
 
 class HTTPClient:
     def __init__(
         self,
@@ -94,15 +95,15 @@
         access_token: Optional[str],
         access_token_secret: Optional[str],
         stream: Optional[Stream] = None,
         callback_url: Optional[str] = None,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         use_bearer_only: bool = False,
-        sleep_after_ratelimit: bool = False,
+        handle_ratelimits: bool = True,
     ):
         self.credentials = {
             "bearer_token": bearer_token,
             "consumer_key": consumer_key,
             "consumer_secret": consumer_secret,
             "access_token": access_token,
             "access_token_secret": access_token_secret,
@@ -144,15 +145,15 @@
             client_id=self.client_id,
             client_secret=self.client_secret,
         )
         self.use_bearer_only = use_bearer_only
         self.event_parser = EventParser(self)
         self.payload_parser = self.event_parser.payload_parser
         self.thread_manager = ThreadManager()
-        self.sleep_after_ratelimit = sleep_after_ratelimit
+        self.handle_ratelimits = handle_ratelimits
         self.current_header = None
         self.message_cache = {}
         self.tweet_cache = {}
         self.user_cache = {}
         self.events = {}
         if self.stream:
             self.stream.http_client = self
@@ -193,15 +194,15 @@
         is_json: bool = True,
     ) -> ResponsePayload:
         if use_base_url:
             url = self.base_url + version + path
         else:
             url = self.upload_url + version + path
 
-        user_agent = "Py-Tweet (https://github.com/sengolda/pytwot/) Python/{0[0]}.{0[1]}.{0[2]} requests/{1}"
+        user_agent = "pytwot(https://github.com/sengolda/pytwot/) Python/{0[0]}.{0[1]}.{0[2]} requests/{1}"
         if "Authorization" not in headers.keys():
             headers["Authorization"] = f"Bearer {self.bearer_token}"
 
         headers["User-Agent"] = user_agent.format(sys.version_info, requests.__version__)
 
         if not self.use_bearer_only:
             if auth:
@@ -222,28 +223,26 @@
 
         if json:
             data = None
 
         method = method.upper()
         if thread_session:
             executor = self.thread_manager.create_new_executor(thread_name=thread_name, session_id=thread_session)
-            future = executor.submit(
+            return executor.submit(
                 self.request,
                 method,
                 version,
                 path,
                 headers=headers,
                 params=params,
                 data=data,
                 json=json,
                 files=files,
                 auth=auth,
             )
-            return future
-
         else:
             response = self.__session.request(
                 method,
                 url,
                 headers=headers,
                 params=params,
                 data=data,
@@ -260,22 +259,21 @@
                 f"Headers: {response.headers}\n"
                 f"Content: {response.content}\n"
                 f"Json-payload: {json}\n"
                 f"Parameters: {params}\n"
             )
 
             if code in (201, 202, 204):
-                if is_json:
-                    try:
-                        res = response.json()
-                    except JSONDecodeError:
-                        return response.text
-                else:
+                if not is_json:
                     return response.text
 
+                try:
+                    res = response.json()
+                except JSONDecodeError:
+                    return response.text
                 return res
 
             elif code == 400:
                 raise BadRequests(response)
 
             elif code == 401:
                 raise Unauthorized(response)
@@ -286,51 +284,48 @@
             elif code == 404:
                 raise NotFound(response)
 
             elif code == 409:
                 raise Conflict(response)
 
             elif code in (420, 429):  # 420 status code is an unofficial extension by Twitter.
-                if self.sleep_after_ratelimit:
-                    remaining = int(response.headers["x-rate-limit-reset"])
-                    sleep_for = (remaining - int(time.time())) + 1
-                    _log.warn(f"Client is ratelimited. Sleeping for {sleep_for}")
-                    print(f"Client is ratelimited. Sleeping for {sleep_for}")
-                    time.sleep(sleep_for)
-                    return self.request(
-                        method,
-                        version,
-                        path,
-                        headers=headers,
-                        params=params,
-                        data=data,
-                        json=json,
-                        files=files,
-                        auth=auth,
-                    )
-
-                else:
+                if not self.handle_ratelimits:
                     raise TooManyRequests(response)
 
+                remaining = int(response.headers["x-rate-limit-reset"])
+                sleep_for = (remaining - int(time.time())) + 1
+                _log.warn(f"Client is ratelimited. Sleeping for {sleep_for}")
+                time.sleep(sleep_for)
+                return self.request(
+                    method,
+                    version,
+                    path,
+                    headers=headers,
+                    params=params,
+                    data=data,
+                    json=json,
+                    files=files,
+                    auth=auth,
+                )
+
             elif code == 431:
                 raise FieldsTooLarge(response)
 
-            if is_json:
-                try:
-                    res = response.json()
-                except JSONDecodeError:
-                    res = response.text
-            else:
+            if not is_json:
                 return response.text
 
+            try:
+                res = response.json()
+            except JSONDecodeError:
+                res = response.text
             if isinstance(res, dict):
                 if res.get("errors"):
                     error = res["errors"][0]
                     if error["type"] == "https://api.twitter.com/2/problems/not-authorized-for-resource":
-                        if not error["parameter"] == "pinned_tweet_id":
+                        if error["parameter"] != "pinned_tweet_id":
                             raise UnauthorizedForResource(error["detail"])
                     elif (
                         error["type"] == "https://api.twitter.com/2/problems/resource-not-found"
                         and res.get("data", None) is None
                     ):
                         raise ResourceNotFound(error["detail"])
 
@@ -343,15 +338,15 @@
                             return []
                     except KeyError:
                         pass
 
             return res
 
     def upload(self, file: File, command: str):
-        assert command.upper() in ("INIT", "APPEND", "FINALIZE", "STATUS")
+        assert command.upper() in {"INIT", "APPEND", "FINALIZE", "STATUS"}
         thread_session = self.thread_manager.generate_thread_session()
 
         def check_status(processing_info, media_id):
             if not processing_info:
                 return
 
             state = processing_info["state"]
@@ -400,19 +395,15 @@
             file._File__media_id = res["media_id"]
             return res["media_id"]
 
         elif command.upper() == "APPEND":
             segment_id = 0
             bytes_sent = 0
             path = file.path
-            if isinstance(path, io.IOBase):
-                open_file = path
-            else:
-                open_file = open(path, "rb")
-
+            open_file = path if isinstance(path, io.IOBase) else open(path, "rb")
             if not file.media_id:
                 raise ValueError("'media_id' is None! Please specified it.")
 
             while bytes_sent < file.total_bytes:
                 self.request(
                     "POST",
                     version="1.1",
@@ -511,15 +502,15 @@
         self.upload(file, "FINALIZE")
         return file
 
     def fetch_me(self):
         data = self.request(
             "GET",
             "2",
-            f"/users/me",
+            "/users/me",
             params={
                 "expansions": PINNED_TWEET_EXPANSION,
                 "user.fields": USER_FIELD,
                 "tweet.fields": TWEET_FIELD,
             },
             auth=True,
         )
@@ -622,15 +613,15 @@
         self.tweet_cache[tweet.id] = tweet
         return tweet
 
     def fetch_space(self, space_id: str, *, space_host: bool) -> Space:
         res = self.request(
             "GET",
             "2",
-            f"/spaces/{str(space_id)}",
+            f"/spaces/{space_id}",
             params={
                 "expansions": SPACE_EXPANSION if not space_host else COMPLETE_SPACE_FIELD,
                 "space.fields": SPACE_FIELD,
                 "topic.fields": TOPIC_FIELD,
                 "user.fields": USER_FIELD,
             },
         )
@@ -732,15 +723,15 @@
         except ValueError:
             raise ValueError("welcome_message_id must be an integer or a string of digits.")
 
         res = self.request(
             "GET",
             "1.1",
             "/direct_messages/welcome_messages/show.json",
-            params={"id": str(welcome_message_id)},
+            params={"id": welcome_message_id},
             auth=True,
         )
 
         data = res.get("welcome_message")
         message_data = data.get("message_data")
         id = data.get("id")
         timestamp = data.get("created_timestamp")
@@ -770,22 +761,22 @@
 
         return Job(res.get("data"), http_client=self)
 
     def fetch_jobs(self, type: JobType, status: Optional[JobStatus] = None) -> Optional[List[Job]]:
         res = self.request(
             "GET",
             "2",
-            f"/compliance/jobs",
-            params={"type": type.value, "status": status.value if isinstance(status, JobStatus) else status},
+            "/compliance/jobs",
+            params={
+                "type": type.value,
+                "status": status.value if isinstance(status, JobStatus) else status,
+            },
         )
 
-        if not res:
-            return []
-
-        return [Job(data) for data in res["data"]]
+        return [] if not res else [Job(data) for data in res["data"]]
 
     def search_geo(
         self,
         query: str,
         max_result: Optional[ID] = None,
         *,
         lat: Optional[int] = None,
@@ -834,15 +825,15 @@
             }
         }
 
         executor = self.thread_manager.create_new_executor(
             thread_name="post-tweet-file-request", session_id=thread_session
         )
         message_data = data["event"]["message_create"]["message_data"]
-        message_data["text"] = str(text)
+        message_data["text"] = text
 
         if file:
             future = executor.submit(self.quick_upload, file)
 
         if custom_profile:
             message_data["custom_profile_id"] = str(custom_profile.id)
 
@@ -853,17 +844,15 @@
             }
 
         if cta:
             message_data["ctas"] = cta.raw_buttons
 
         if file:
             file = future.result()
-            message_data["attachment"] = {}
-            message_data["attachment"]["type"] = "media"
-            message_data["attachment"]["media"] = {}
+            message_data["attachment"] = {"type": "media", "media": {}}
             message_data["attachment"]["media"]["id"] = str(file.media_id)
 
         res = self.request(
             "POST",
             "1.1",
             "/direct_messages/events/new.json",
             json=data,
@@ -899,36 +888,32 @@
         executor = self.thread_manager.create_new_executor(thread_name="post-tweet-request", session_id=thread_session)
 
         payload = {}
         if text:
             payload["text"] = text
 
         if file:
-            payload["media"] = {}
-            payload["media"]["media_ids"] = []
+            payload["media"] = {"media_ids": []}
             executor.submit(self.quick_upload, file)
 
         if files:
             if len(files) + 1 if file else len(files) > 4:
                 raise BadRequests(message="Cannot upload more then 4 files!")
 
-            payload["media"] = {}
-            payload["media"]["media_ids"] = []
+            payload["media"] = {"media_ids": []}
             for file in files:
                 executor.submit(self.quick_upload, file)
 
         if poll:
-            payload["poll"] = {}
-            payload["poll"]["duration_minutes"] = int(poll.duration)
-            payload["poll"]["options"] = [option.label for option in poll.options]
-
+            payload["poll"] = {
+                "duration_minutes": int(poll.duration),
+                "options": [option.label for option in poll.options],
+            }
         if geo:
-            payload["geo"] = {}
-            payload["geo"]["place_id"] = geo.id if isinstance(geo, Geo) else geo
-
+            payload["geo"] = {"place_id": geo.id if isinstance(geo, Geo) else geo}
         if direct_message_deep_link:
             payload["direct_message_deep_link"] = direct_message_deep_link
 
         if reply_setting:
             payload["reply_settings"] = (
                 reply_setting.value if isinstance(reply_setting, ReplySetting) else reply_setting
             )
@@ -941,20 +926,17 @@
 
         if quote_tweet:
             payload["quote_tweet_id"] = str(quote_tweet.id) if isinstance(quote_tweet, Tweet) else str(quote_tweet)
 
         if exclude_reply_users:
             ids = [str(user.id) if isinstance(user, User) else str(user) for user in exclude_reply_users]
 
-            if "reply" in payload.keys():
-                payload["reply"]["exclude_reply_user_ids"] = ids
-            else:
+            if "reply" not in payload.keys():
                 payload["reply"] = {}
-                payload["reply"]["exclude_reply_user_ids"] = ids
-
+            payload["reply"]["exclude_reply_user_ids"] = ids
         if media_tagged_users:
             if not payload.get("media"):
                 raise pytwotException("Cannot tag users without any file!")
             payload["media"]["tagged_user_ids"] = [
                 str(user.id) if isinstance(user, (User, ClientAccount)) else str(user) for user in media_tagged_users
             ]
 
@@ -1046,17 +1028,15 @@
                 "options": quick_reply.raw_options,
             }
 
         if cta:
             message_data["ctas"] = cta.raw_buttons
 
         if file:
-            message_data["attachment"] = {}
-            message_data["attachment"]["type"] = "media"
-            message_data["attachment"]["media"] = {}
+            message_data["attachment"] = {"type": "media", "media": {}}
             message_data["attachment"]["media"]["id"] = str(file_future.result().media_id)
 
         res = self.request(
             "POST",
             "1.1",
             "/direct_messages/welcome_messages/new.json",
             json=data,
@@ -1100,17 +1080,15 @@
                 "options": quick_reply.raw_options,
             }
 
         if cta:
             message_data["ctas"] = cta.raw_buttons
 
         if file:
-            message_data["attachment"] = {}
-            message_data["attachment"]["type"] = "media"
-            message_data["attachment"]["media"] = {}
+            message_data["attachment"] = {"type": "media", "media": {}}
             message_data["attachment"]["media"]["id"] = str(file_future.result().media_id)
 
         res = self.request(
             "PUT",
             "1.1",
             "/direct_messages/welcome_messages/update.json",
             params={"id": str(welcome_message_id)},
```

### Comparing `pytwot-1.5.0a10/pytwot/list.py` & `pytwot-1.5.1/pytwot/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,20 @@
 """
 
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Optional
 
+from .constants import PINNED_TWEET_EXPANSION, TWEET_EXPANSION, TWEET_FIELD, USER_FIELD
+from .objects import Comparable
+from .paginations import TweetPagination, UserPagination
+from .relations import RelationDelete, RelationFollow, RelationPin, RelationUpdate
 from .type import ID, Payload
 from .utils import time_parse_todt
-from .paginations import UserPagination, TweetPagination
-from .constants import TWEET_EXPANSION, USER_FIELD, TWEET_FIELD, PINNED_TWEET_EXPANSION
-from .relations import RelationUpdate, RelationDelete, RelationPin
-from .objects import Comparable
-from .relations import RelationFollow
 
 if TYPE_CHECKING:
     from .http import HTTPClient
     from .user import User
 
 __all__ = ("List", "_CopyList")
```

### Comparing `pytwot-1.5.0a10/pytwot/message.py` & `pytwot-1.5.1/pytwot/message.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 """
 
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
-from .dataclass import ApplicationInfo, InitiatedVia
 from .attachments import CTA, File, QuickReply
+from .dataclass import ApplicationInfo, InitiatedVia
 from .entities import Hashtag, Symbol, Url, UserMention
 from .enums import MessageEventTypeEnum, MessageTypeEnum
-from .user import User
 from .objects import Comparable
+from .user import User
 
 if TYPE_CHECKING:
     from .http import HTTPClient
     from .type import ID
 
 __all__ = ("Message", "DirectMessage", "WelcomeMessage", "WelcomeMessageRule")
```

### Comparing `pytwot-1.5.0a10/pytwot/objects.py` & `pytwot-1.5.1/pytwot/objects.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/paginations.py` & `pytwot-1.5.1/pytwot/paginations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
-from typing import Any, List, Tuple, Optional, TYPE_CHECKING
-from .errors import NoPageAvailable
 
+from typing import TYPE_CHECKING, Any, List, Optional, Tuple
+
+from .errors import NoPageAvailable
 
 if TYPE_CHECKING:
     from .http import HTTPClient
     from .type import Payload
 
 
 class Pagination:
```

### Comparing `pytwot-1.5.0a10/pytwot/parser.py` & `pytwot-1.5.1/pytwot/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,37 +20,38 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
+from .dataclass import ApplicationInfo, Location, SleepTimeSettings, TimezoneInfo
 from .events import (
-    DirectMessageTypingEvent,
     DirectMessageReadEvent,
+    DirectMessageTypingEvent,
     TweetFavoriteActionEvent,
-    UserRevokeEvent,
-    UserFollowActionEvent,
-    UserUnfollowActionEvent,
     UserBlockActionEvent,
-    UserUnblockActionEvent,
+    UserFollowActionEvent,
     UserMuteActionEvent,
+    UserRevokeEvent,
+    UserUnblockActionEvent,
+    UserUnfollowActionEvent,
     UserUnmuteActionEvent,
 )
-from .message import Message, DirectMessage
-from .user import User
+from .message import DirectMessage, Message
 from .tweet import Tweet
-from .dataclass import TimezoneInfo, Location, SleepTimeSettings, ApplicationInfo
+from .user import User
 from .utils import convert
 
 if TYPE_CHECKING:
-    from .type import Payload
     from .http import HTTPClient
+    from .type import Payload
 
 __all__ = ("PayloadParser", "EventParser")
 
 
 class PayloadParser:
     __slots__ = "http_client"
```

### Comparing `pytwot-1.5.0a10/pytwot/relations.py` & `pytwot-1.5.1/pytwot/relations.py`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/pytwot/space.py` & `pytwot-1.5.1/pytwot/space.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,23 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import datetime
-from typing import Any, Union, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
+from .constants import MEDIA_FIELD, PLACE_FIELD, POLL_FIELD, TWEET_EXPANSION, TWEET_FIELD, USER_FIELD
+from .dataclass import Topic
 from .enums import SpaceState
-from .utils import time_parse_todt
-from .user import User
-from .tweet import Tweet
 from .objects import Comparable
-from .dataclass import Topic
-from .constants import (
-    TWEET_EXPANSION,
-    USER_FIELD,
-    MEDIA_FIELD,
-    PLACE_FIELD,
-    POLL_FIELD,
-    TWEET_FIELD,
-)
+from .tweet import Tweet
+from .user import User
+from .utils import time_parse_todt
 
 __all__ = ("Space",)
 
 
 class Space(Comparable):
     """Represents a twitter space.
```

### Comparing `pytwot-1.5.0a10/pytwot/stream.py` & `pytwot-1.5.1/pytwot/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,32 +22,25 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
 import json
-import requests
 import logging
 import time
+from typing import TYPE_CHECKING, Any, List, Optional, Type
+
+import requests
 
-from typing import TYPE_CHECKING, Any, List, Type, Optional
+from .constants import MEDIA_FIELD, PLACE_FIELD, POLL_FIELD, TWEET_EXPANSION, TWEET_FIELD, USER_FIELD
 from .dataclass import StreamRule
 from .errors import ConnectionException, pytwotException
-from .constants import (
-    MEDIA_FIELD,
-    PLACE_FIELD,
-    POLL_FIELD,
-    TWEET_EXPANSION,
-    TWEET_FIELD,
-    USER_FIELD,
-)
 from .tweet import Tweet
 
-
 if TYPE_CHECKING:
     from .http import HTTPClient
 
 _log = logging.getLogger(__name__)
 
 
 class StreamConnection:
@@ -86,15 +79,15 @@
     def closed(self) -> Optional[bool]:
         """Optional[:class:`bool`]: Returns True if the connection is closed, else False.
 
         .. versionadded:: 1.3.5
         """
         return not self.running
 
-    def is_close(self) -> Optional[bool]:
+    def is_closed(self) -> Optional[bool]:
         """An alias to :class:`StreamConnection.closed`.
 
         Returns
         ---------
         Optional[:class:`bool`]:
             This method returns a :class:`bool` object.
 
@@ -125,15 +118,15 @@
 
         .. versionadded:: 1.3.5
         """
         self.running = True
         http = self.http_client
         while self.running:
             try:
-                response = requests.get(
+                response = http.__session.get(
                     self.url,
                     headers={"Authorization": f"Bearer {http.bearer_token}"},
                     params={
                         "backfill_minutes": int(self.backfill_minutes),
                         "expansions": TWEET_EXPANSION,
                         "media.fields": MEDIA_FIELD,
                         "place.fields": PLACE_FIELD,
@@ -211,15 +204,15 @@
             "https://api.twitter.com/2/tweets/search/stream",
             self.backfill_minutes,
             reconnect_attempts,
             self.http_client,
         )
 
     @classmethod
-    def sample_stream(cls: Type[Stream], backfill_minutes: int = 0, reconnect_attempts: int = 15) -> Stream:
+    def sample(cls: Type[Stream], backfill_minutes: int = 0, reconnect_attempts: int = 15) -> Stream:
         """A class method that change the stream connection to a sample one, this would mean you dont have to set any stream rules. This would not recommended because it can make the progress of tweet cap much faster, if its out of limit you would not be able to stream.
 
         Parameters
         ------------
         backfill_minutes: :class:`int`
             This feature will deliver duplicate Tweets, meaning that if you were disconnected for 90 seconds, and you requested two minutes of backfill, you will receive 30 seconds worth of duplicate Tweets. Due to this, you should make sure your system is tolerant of duplicate data. This feature is currently only available to the Academic Research product track.
         reconnect_attempts: :class:`int`
```

### Comparing `pytwot-1.5.0a10/pytwot/threads/__init__.py` & `pytwot-1.5.1/pytwot/threads/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
-import threading
 import random
 import string
+import threading
 from concurrent.futures import ThreadPoolExecutor, wait
-from typing import Optional, Callable, Any
+from typing import Any, Callable, Optional
+
 from ..constants import ALL_COMPLETED
 
 __all__ = ("Executor", "ThreadManager")
 
 
 class Executor(ThreadPoolExecutor):
     def __init__(self, *args, **kwargs):
```

### Comparing `pytwot-1.5.0a10/pytwot/tweet.py` & `pytwot-1.5.1/pytwot/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,38 +24,38 @@
 """
 
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-from .attachments import Poll, Geo, File, Media
-from .enums import ReplySetting
+from .attachments import File, Geo, Media, Poll
 from .constants import (
-    TWEET_EXPANSION,
-    TWEET_FIELD,
-    USER_FIELD,
-    PINNED_TWEET_EXPANSION,
     MEDIA_FIELD,
+    PINNED_TWEET_EXPANSION,
     PLACE_FIELD,
     POLL_FIELD,
+    TWEET_EXPANSION,
+    TWEET_FIELD,
+    USER_FIELD,
 )
-from .relations import RelationHide, RelationLike, RelationRetweet, RelationDelete
-from .user import User
-from .utils import time_parse_todt, convert
-from .message import Message
-from .paginations import UserPagination, TweetPagination
 from .dataclass import (
     Embed,
     EmbedImage,
-    PublicTweetMetrics,
     NonPublicTweetMetrics,
     OrganicTweetMetrics,
     PromotedTweetMetrics,
+    PublicTweetMetrics,
 )
+from .enums import ReplySetting
+from .message import Message
+from .paginations import TweetPagination, UserPagination
+from .relations import RelationDelete, RelationHide, RelationLike, RelationRetweet
+from .user import User
+from .utils import convert, time_parse_todt
 
 if TYPE_CHECKING:
     from .http import HTTPClient
     from .type import ID
 
 __all__ = ("Tweet",)
 
@@ -262,17 +262,19 @@
 
         .. versionchanged:: 1.5.0
 
             Now returns a list of :class:`User` objects rather then a list of :class:`str` objects.
         """
         users = []
         for user in self._includes.get("users", {}):
-            for mention in self._entities.get("mentions", {}):
-                if user["id"] == mention["id"]:
-                    users.append(User(user, http_client=self.http_client))
+            users.extend(
+                User(user, http_client=self.http_client)
+                for mention in self._entities.get("mentions", {})
+                if user["id"] == mention["id"]
+            )
         return users
 
     @property
     def poll(self) -> Optional[Poll]:
         """:class:`Poll`: Returns a Poll object with the tweet's poll.
 
         .. versionadded:: 1.1.0
@@ -288,16 +290,16 @@
                 )
                 for option in data.get("options"):
                     poll.add_option(**option)
                 return poll
         return None
 
     @property
-    def medias(self) -> Optional[List[Media]]:
-        """Optional[List[:class:`Media`]]: Returns a list of media(s) in a tweet.
+    def media(self) -> Optional[List[Media]]:
+        """Optional[List[:class:`Media`]]: Returns a list of media objects in a tweet.
 
         .. versionadded:: 1.1.0
         """
         if self._includes and self._includes.get("media"):
             return [Media(img, http_client=self.http_client) for img in self._includes.get("media")]
         return None
 
@@ -609,74 +611,71 @@
         ---------
         Optional[:class:`UserPagination`]
             This method returns a :class:`UserPagination` object.
 
 
         .. versionadded:: 1.1.3
         """
-        res = self.http_client.request(
+        if res := self.http_client.request(
             "GET",
             "2",
             f"/tweets/{self.id}/retweeted_by",
             params={
                 "expansions": PINNED_TWEET_EXPANSION,
                 "user.fields": USER_FIELD,
                 "tweet.fields": TWEET_FIELD,
             },
-        )
-        if not res:
+        ):
+            return UserPagination(
+                res,
+                endpoint_request=f"/tweets/{self.id}/retweeted_by",
+                http_client=self.http_client,
+                params={
+                    "expansions": PINNED_TWEET_EXPANSION,
+                    "user.fields": USER_FIELD,
+                    "tweet.fields": TWEET_FIELD,
+                },
+            )
+        else:
             return []
 
-        return UserPagination(
-            res,
-            endpoint_request=f"/tweets/{self.id}/retweeted_by",
-            http_client=self.http_client,
-            params={
-                "expansions": PINNED_TWEET_EXPANSION,
-                "user.fields": USER_FIELD,
-                "tweet.fields": TWEET_FIELD,
-            },
-        )
-
     def fetch_likers(self) -> Optional[UserPagination]:
         """Returns a pagination object with the users that liked the tweet.
 
         Returns
         ---------
         Optional[:class:`UserPagination`]
             This method returns a :class:`UserPagination` object.
 
 
         .. versionadded:: 1.1.3
         """
-        res = self.http_client.request(
+        if res := self.http_client.request(
             "GET",
             "2",
             f"/tweets/{self.id}/liking_users",
             params={
                 "expansions": PINNED_TWEET_EXPANSION,
                 "user.fields": USER_FIELD,
                 "tweet.fields": TWEET_FIELD,
             },
-        )
-
-        if not res:
+        ):
+            return UserPagination(
+                res,
+                endpoint_request=f"/tweets/{self.id}/liking_users",
+                http_client=self.http_client,
+                params={
+                    "expansions": PINNED_TWEET_EXPANSION,
+                    "user.fields": USER_FIELD,
+                    "tweet.fields": TWEET_FIELD,
+                },
+            )
+        else:
             return []
 
-        return UserPagination(
-            res,
-            endpoint_request=f"/tweets/{self.id}/liking_users",
-            http_client=self.http_client,
-            params={
-                "expansions": PINNED_TWEET_EXPANSION,
-                "user.fields": USER_FIELD,
-                "tweet.fields": TWEET_FIELD,
-            },
-        )
-
     def fetch_quoted_tweets(self) -> Optional[TweetPagination]:
         """Returns a pagination object for tweets that quoted the tweet
 
         Returns
         ---------
         Optional[:class:`TweetPagination`]
             This method returns :class:`TweetPagination` or an empty list if the tweet does not contain any quoted tweets.
@@ -690,18 +689,16 @@
             "tweet.fields": TWEET_FIELD,
             "media.fields": MEDIA_FIELD,
             "place.fields": PLACE_FIELD,
             "poll.fields": POLL_FIELD,
             "max_results": 100,
         }
 
-        res = self.http_client.request("GET", "2", f"/tweets/{self.id}/quote_tweets", params=params)
-
-        if not res:
+        if res := self.http_client.request("GET", "2", f"/tweets/{self.id}/quote_tweets", params=params):
+            return TweetPagination(
+                res,
+                endpoint_request=f"/tweets/{self.id}/quote_tweets",
+                http_client=self.http_client,
+                params=params,
+            )
+        else:
             return []
-
-        return TweetPagination(
-            res,
-            endpoint_request=f"/tweets/{self.id}/quote_tweets",
-            http_client=self.http_client,
-            params=params,
-        )
```

### Comparing `pytwot-1.5.0a10/pytwot/type.py` & `pytwot-1.5.1/pytwot/type.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,13 +19,12 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from typing import Any, Dict, Union, Optional
-
+from typing import Any, Dict, Optional, Union
 
 ID = Union[str, int]
 Payload = Dict[str, Any]
 ResponsePayload = Optional[Union[str, Payload]]
```

### Comparing `pytwot-1.5.0a10/pytwot/user.py` & `pytwot-1.5.1/pytwot/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,43 +21,43 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
 
-import io
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union, List
+import io
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from .constants import (
-    TWEET_EXPANSION,
     LIST_EXPANSION,
-    PINNED_TWEET_EXPANSION,
+    LIST_FIELD,
     MEDIA_FIELD,
+    PINNED_TWEET_EXPANSION,
     PLACE_FIELD,
     POLL_FIELD,
+    TWEET_EXPANSION,
     TWEET_FIELD,
     USER_FIELD,
-    LIST_FIELD,
 )
-from .relations import RelationFollow
-from .utils import time_parse_todt, convert
-from .dataclass import UserSettings, Location
-from .paginations import UserPagination, TweetPagination, ListPagination
+from .dataclass import Location, UserSettings
 from .list import List as TwitterList
 from .objects import Comparable
+from .paginations import ListPagination, TweetPagination, UserPagination
+from .relations import RelationFollow
+from .utils import convert, time_parse_todt
 
 if TYPE_CHECKING:
-    from .message import DirectMessage
+    from .attachments import CTA, CustomProfile, File, Geo, QuickReply
+    from .enums import Timezone
     from .http import HTTPClient
-    from .type import ID
+    from .message import DirectMessage
     from .tweet import Tweet
-    from .enums import Timezone
-    from .attachments import Geo, CTA, CustomProfile, File, QuickReply
+    from .type import ID
 
 
 class User(Comparable):
     """Represents a user in Twitter.
     User is an identity in twitter, its very interactive. Can send message, post a tweet, and even send messages to other user through Dms.
```

### Comparing `pytwot-1.5.0a10/pytwot/utils.py` & `pytwot-1.5.1/pytwot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 SOFTWARE.
 """
 
 
 from __future__ import annotations
 
 import datetime
-from typing import Any, Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
+
 from dateutil import parser
 
 if TYPE_CHECKING:
     from .type import ID
 
 
-def convert(o: object, annotations: Any):
+def convert(o: object, annotations: Any) -> object:
     try:
         return annotations(o)
     except (ValueError, TypeError):
         return object
 
 
-def guess_mimetype(byts: bytes):
+def guess_mimetype(byts: bytes) -> str:
     if byts[6:10] == b"\x1a\n\x00\x00":
         return "image/png"
 
     elif byts[6:10] == b"JFIF":
         return "image/jpeg"
 
     elif byts[6:10] == b"ypis":
@@ -105,15 +106,15 @@
         if not text
         else f"https://twitter.com/intent/tweet" + f"?text={text}"
         if text
         else f"https://twitter.com/intent/tweet"
     )
 
 
-def compose_user_action(user_id: str, action: str, text: str = None):
+def compose_user_action(user_id: str, action: str, text: str = None) -> str:
     """Make a link that let's you interact with a user with certain actions.
 
     Parameters
     ------------
     user_id: :class:`str`
         The user's id.
     action: :class:`str`
@@ -138,15 +139,15 @@
         if action.lower() == "follow"
         else f"https://twitter.com/messages/compose?recipient_id={user_id}" + f"?text={text}"
         if text
         else f"https://twitter.com/messages/compose?recipient_id={user_id}"
     )
 
 
-def compose_tweet_action(tweet_id: ID, action: str = None):
+def compose_tweet_action(tweet_id: ID, action: str = None) -> str:
     """Make a link that let's you interact with a tweet with certain actions.
 
     Parameters
     ------------
     tweet_id: `ID`
         The tweet id you want to compose.
     action: :class:`str`
```

### Comparing `pytwot-1.5.0a10/pytwot.egg-info/PKG-INFO` & `pytwot-1.5.1/pytwot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytwot
-Version: 1.5.0a10
+Version: 1.5.1
 Summary: A Synchronous python API wrapper for twitter's api
 Home-page: https://github.com/sengolda/pytwot
 Author: Sengolda
 Maintainer: Sengolda
 License: MIT
 Project-URL: Documentation, https://py-tweet.readthedocs.io/
 Project-URL: HomePage/Github, https://github.com/sengolda/pytwot/
@@ -32,37 +32,27 @@
 <p><b>Another note:</b> the support server given is support server for the original PyTweet as this is approved by the devs they requested the support server stay the same</p>
 
 <div>
 <img src="https://img.shields.io/pypi/v/pytwot?logo=pypi&style=plastic">  
 
 <img src="https://img.shields.io/badge/code%20style-black-000000.svg">  
 
-<img alt="PyPI - License" src="https://img.shields.io/pypi/l/pytwot">
-
-<img alt="Total Downloads" src="https://pepy.tech/badge/pytwot">
 
 <img src="https://img.shields.io/github/commit-activity/m/sengolda/pytwot?color=turquoise&logo=github&logoColor=black">
 
 
 <img src="https://img.shields.io/github/issues-pr/sengolda/pytwot?color=yellow&label=Pull%20Requests&logo=github&logoColor=black">
 
 
 <img src="https://img.shields.io/discord/858312394236624957?color=blue&label=pytwot&logo=discord">
 
 
-<img src='https://readthedocs.org/projects/py-tweet/badge/?version=latest' alt='Documentation Status' />
-
-
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard">
-
-
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fpremium">
+<img src='https://readthedocs.org/projects/pytwot/badge/?version=latest' alt='Documentation Status' />
 
 
-<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2">
 
 </div>
 <br>
 <br>
 <p align="center">pytwot is a synchronous Python API wrapper for the Twitter API. It is filled with rich features and is very easy to use.</p>
 
 ## Installation
@@ -97,15 +87,15 @@
 client.tweet("Hello world, Hello twitter!") #This requires read & write app permissions also elevated access type.
 ```
 
 You can check in the `examples` directory for more example code.
 
 # Links
 
-- [Documentation](https://py-tweet.readthedocs.io/en/latest/)
+- [Documentation](https://pytwot.readthedocs.io/en/latest/)
 
 - [Support Server](https://discord.gg/XHBhg6A4jJ)
 
 - [GitHub](https://github.com/sengolda/pytwot)
 
 - [PyPi](https://pypi.org/project/pytwot)
```

#### html2text {}

```diff
@@ -1,39 +1,34 @@
-Metadata-Version: 2.1 Name: pytwot Version: 1.5.0a10 Summary: A Synchronous
-python API wrapper for twitter's api Home-page: https://github.com/sengolda/
-pytwot Author: Sengolda Maintainer: Sengolda License: MIT Project-URL:
-Documentation, https://py-tweet.readthedocs.io/ Project-URL: HomePage/Github,
-https://github.com/sengolda/pytwot/ Project-URL: Discord, https://discord.gg/
-XHBhg6A4jJ Keywords: twitter,tweet.py twitter.py Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Operating System :: OS Independent Classifier: Topic
-:: Internet Classifier: Topic :: Utilities Classifier: Development Status :: 5
-- Production/Stable Requires-Python: >=3.7.0 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: pytwot Version: 1.5.1 Summary: A Synchronous python
+API wrapper for twitter's api Home-page: https://github.com/sengolda/pytwot
+Author: Sengolda Maintainer: Sengolda License: MIT Project-URL: Documentation,
+https://py-tweet.readthedocs.io/ Project-URL: HomePage/Github, https://
+github.com/sengolda/pytwot/ Project-URL: Discord, https://discord.gg/XHBhg6A4jJ
+Keywords: twitter,tweet.py twitter.py Platform: UNKNOWN Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent Classifier: Topic :: Internet
+Classifier: Topic :: Utilities Classifier: Development Status :: 5 -
+Production/Stable Requires-Python: >=3.7.0 Description-Content-Type: text/
 markdown Provides-Extra: docs Provides-Extra: events License-File: LICENSE
                               ***** pytwot *****
 This project is a fork of the now archived PyTweet
 VERY IMPORTANT: This project is approved by the PyTweet devs themselves.
 Another note: the support server given is support server for the original
 PyTweet as this is approved by the devs they requested the support server stay
 the same
 [https://img.shields.io/pypi/v/pytwot?logo=pypi&style=plastic] [https://
-img.shields.io/badge/code%20style-black-000000.svg] [PyPI - License] [Total
-Downloads] [https://img.shields.io/github/commit-activity/m/sengolda/
+img.shields.io/badge/code%20style-black-000000.svg] [https://img.shields.io/
+github/commit-activity/m/sengolda/
 pytwot?color=turquoise&logo=github&logoColor=black] [https://img.shields.io/
 github/issues-pr/sengolda/
 pytwot?color=yellow&label=Pull%20Requests&logo=github&logoColor=black] [https:/
 /img.shields.io/discord/
 858312394236624957?color=blue&label=pytwot&logo=discord] [Documentation Status]
-[https://img.shields.io/
-endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard] [https://
-img.shields.io/
-endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fpremium] [https://
-img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2]
 
 
  pytwot is a synchronous Python API wrapper for the Twitter API. It is filled
                   with rich features and is very easy to use.
 ## Installation ### Windows ```bash py -m pip install pytwot ``` ### Linux/
 MacOS ```bash python3 -m pip install pytwot ``` ## Usage Before using pytwot
 you have to setup an application [here](https://apps.twitter.com). For a more
@@ -45,15 +40,15 @@
 /discord.gg/nxZCE9EbVr). ```py import pytwot client = pytwot.Client( "Your
 Bearer Token Here!!!", consumer_key="Your consumer key here",
 consumer_secret="Your consumer secret here", access_token="Your access token
 here", access_token_secret="Your access token secret here", ) #Before using
 pytwot, make sure to create an application in https://apps.twitter.com.
 client.tweet("Hello world, Hello twitter!") #This requires read & write app
 permissions also elevated access type. ``` You can check in the `examples`
-directory for more example code. # Links - [Documentation](https://py-
-tweet.readthedocs.io/en/latest/) - [Support Server](https://discord.gg/
+directory for more example code. # Links - [Documentation](https://
+pytwot.readthedocs.io/en/latest/) - [Support Server](https://discord.gg/
 XHBhg6A4jJ) - [GitHub](https://github.com/sengolda/pytwot) - [PyPi](https://
 pypi.org/project/pytwot) # Contribute You can Contribute or open an issue
 regarding pytwot in our [GitHub repository](https://github.com/sengolda/
 pytwot)! # Licence & Copyright All files of this repo are protected and
 licensed with the [MIT License](https://opensource.org/licenses/MIT), [LICENSE
 File](LICENSE)
```

### Comparing `pytwot-1.5.0a10/pytwot.egg-info/SOURCES.txt` & `pytwot-1.5.1/pytwot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytwot-1.5.0a10/setup.py` & `pytwot-1.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from setuptools import setup
 import re
 
+from setuptools import setup
+
 short_description = "A Synchronous python API wrapper for twitter's api"
 version = ""
 with open("pytwot/__init__.py") as f:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
 
 if not version:
     raise RuntimeError("version is not set")
@@ -34,19 +35,15 @@
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
     "Topic :: Internet",
     "Topic :: Utilities",
     "Development Status :: 5 - Production/Stable",
 ]
 
-packages = [
-    "pytwot",
-    "pytwot.dataclass",
-    "pytwot.threads"
-]
+packages = ["pytwot", "pytwot.dataclass", "pytwot.threads"]
 
 # fmt: off
 
 # fmt: on
 
 setup(
     name="pytwot",
```


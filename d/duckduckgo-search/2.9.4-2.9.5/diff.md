# Comparing `tmp/duckduckgo_search-2.9.4.tar.gz` & `tmp/duckduckgo_search-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.9.4.tar", last modified: Thu May 11 20:07:21 2023, max compression
+gzip compressed data, was "duckduckgo_search-2.9.5.tar", last modified: Fri May 12 17:56:15 2023, max compression
```

## Comparing `duckduckgo_search-2.9.4.tar` & `duckduckgo_search-2.9.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.348626 duckduckgo_search-2.9.4/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.348626 duckduckgo_search-2.9.4/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6309 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2856 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6557 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7190 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3953 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1605 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3939 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.348626 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34645 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.443162 duckduckgo_search-2.9.5/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/duckduckgo_search/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/cli/ddgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7206 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/ddg_videos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 17:56:15.000000 duckduckgo_search-2.9.5/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:56:15.447162 duckduckgo_search-2.9.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-12 17:55:58.000000 duckduckgo_search-2.9.5/tests/test_ddg_videos.py
```

### Comparing `duckduckgo_search-2.9.4/LICENSE.md` & `duckduckgo_search-2.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/PKG-INFO` & `duckduckgo_search-2.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 2.9.4
+Version: 2.9.5
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![Python >= 3.7](https://img.shields.io/badge/python->=3.7-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search)
-# Duckduckgo_search<a name="TOP"></a>
+# Duckduckgo_search<a name="TOP"></a> 
+***_Attention. Versions before v2.9.4 no longer work as of May 12, 2023!_***
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
```

### Comparing `duckduckgo_search-2.9.4/README.md` & `duckduckgo_search-2.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![Python >= 3.7](https://img.shields.io/badge/python->=3.7-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search)
-# Duckduckgo_search<a name="TOP"></a>
+# Duckduckgo_search<a name="TOP"></a> 
+***_Attention. Versions before v2.9.4 no longer work as of May 12, 2023!_***
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/__init__.py` & `duckduckgo_search-2.9.5/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/cli/ddgs.py` & `duckduckgo_search-2.9.5/duckduckgo_search/cli/ddgs.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
         for i in range(2):
             try:
                 resp = SESSION.get("https://links.duckduckgo.com/d.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
             except Exception as ex:
-                logger.debug(f"get_ddg_page() {keywords=} {type(ex).__name__} {ex}")
+                logger.debug(
+                    f"get_ddg_page() keywords={keywords} {type(ex).__name__} {ex}"
+                )
 
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
 
         page_results = []
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_answers.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_answers.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     }
     page_data = []
     try:
         resp = SESSION.get("https://api.duckduckgo.com/", params=payload)
         resp.raise_for_status()
         page_data = resp.json()
     except Exception as ex:
-        logger.debug(f"ddg_answers() {keywords=} {type(ex).__name__} {ex}")
+        logger.debug(f"ddg_answers() keywords={keywords} {type(ex).__name__} {ex}")
     if page_data:
         answer = page_data.get("AbstractText", None)
         if answer:
             results.append(
                 {
                     "icon": None,
                     "text": answer,
@@ -58,15 +58,15 @@
         }
         page_data = []
         try:
             resp = SESSION.get("https://api.duckduckgo.com/", params=payload)
             resp.raise_for_status()
             page_data = resp.json().get("RelatedTopics", [])
         except Exception as ex:
-            logger.debug(f"ddg_answers() {keywords=} {type(ex).__name__} {ex}")
+            logger.debug(f"ddg_answers() keywords={keywords} {type(ex).__name__} {ex}")
 
         for i, row in enumerate(page_data):
             topic = row.get("Name", None)
             if not topic:
                 icon = row["Icon"].get("URL", None)
                 results.append(
                     {
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_images.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             try:
                 resp = SESSION.get("https://duckduckgo.com/i.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
             except Exception as ex:
                 logger.debug(
-                    f"get_ddg_images_page() {keywords=} {type(ex).__name__} {ex}"
+                    f"get_ddg_images_page() keywords={keywords} {type(ex).__name__} {ex}"
                 )
 
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_maps.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 headers=headers,
             )
             resp.raise_for_status()
             coordinates = resp.json()[0]["boundingbox"]
             lat_t, lon_l = Decimal(coordinates[1]), Decimal(coordinates[2])
             lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
         except Exception as ex:
-            logger.debug(f"ddg_maps() {keywords=} {type(ex).__name__} {ex}")
+            logger.debug(f"ddg_maps() keywords={keywords} {type(ex).__name__} {ex}")
             return
 
     # if a radius is specified, expand the search square
     lat_t += Decimal(radius) * Decimal(0.008983)
     lat_b -= Decimal(radius) * Decimal(0.008983)
     lon_l -= Decimal(radius) * Decimal(0.008983)
     lon_r += Decimal(radius) * Decimal(0.008983)
@@ -148,15 +148,15 @@
         }
         page_data = None
         try:
             resp = SESSION.get("https://duckduckgo.com/local.js", params=params)
             resp.raise_for_status()
             page_data = resp.json()["results"]
         except Exception as ex:
-            logger.debug(f"ddg_maps() {keywords=} {type(ex).__name__} {ex}")
+            logger.debug(f"ddg_maps() keywords={keywords} {type(ex).__name__} {ex}")
             break
 
         if not page_data:
             break
 
         for res in page_data:
             result = MapsResult()
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_news.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             try:
                 resp = SESSION.get("https://duckduckgo.com/news.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
             except Exception as ex:
                 logger.debug(
-                    f"get_ddg_news_page() {keywords=} {type(ex).__name__} {ex}"
+                    f"get_ddg_news_page() keywords={keywords} {type(ex).__name__} {ex}"
                 )
 
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_suggestions.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_suggestions.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,13 +32,13 @@
         "kl": region,
     }
     try:
         resp = SESSION.get("https://duckduckgo.com/ac", params=payload)
         resp.raise_for_status()
         results = resp.json()
     except Exception as ex:
-        logger.debug(f"ddg_suggestions() {keywords=} {type(ex).__name__} {ex}")
+        logger.debug(f"ddg_suggestions() keywords={keywords} {type(ex).__name__} {ex}")
 
     if output:
         _do_output("ddg_suggestions", keywords, output, results)
 
     return results
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_translate.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_translate.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,13 +52,15 @@
             )
             resp.raise_for_status()
             result = resp.json()
             result["original"] = data
             results.append(result)
         except Exception as ex:
             VQD_CACHE.pop("translate", None)
-            logger.debug(f"ddg_translate() {keywords=} {type(ex).__name__} {ex}")
+            logger.debug(
+                f"ddg_translate() keywords={keywords} {type(ex).__name__} {ex}"
+            )
 
     if output:
         keywords = keywords[0]
         _do_output("ddg_translate", keywords, output, results)
     return results
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/ddg_videos.py` & `duckduckgo_search-2.9.5/duckduckgo_search/ddg_videos.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             try:
                 resp = SESSION.get("https://duckduckgo.com/v.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
             except Exception as ex:
                 logger.debug(
-                    f"get_ddg_videos_page() {keywords=} {type(ex).__name__} {ex}"
+                    f"get_ddg_videos_page() keywords={keywords} {type(ex).__name__} {ex}"
                 )
 
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search/utils.py` & `duckduckgo_search-2.9.5/duckduckgo_search/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             vqd_bytes = resp.content[vqd_index_start:vqd_index_end]
 
             if vqd_bytes:
                 VQD_CACHE[keywords] = vqd_bytes
                 return vqd_bytes.decode()
 
         except Exception as ex:
-            logger.info(f"_get_vqd() {keywords=} {type(ex).__name__} {ex}")
+            logger.info(f"_get_vqd() keywords={keywords} {type(ex).__name__} {ex}")
 
         # refresh SESSION if not vqd
         prev_proxies = SESSION.proxies
         SESSION = requests.Session()
         SESSION.headers = HEADERS
         SESSION.proxies = prev_proxies
         logger.warning("keywords=%s. _get_vqd() is None, refreshing SESSION", keywords)
@@ -100,15 +100,15 @@
         ) as resp:
             resp.raise_for_status()
             resp.raw.decode_content = True
             with open(os.path.join(dir_path, filename), "wb") as file:
                 copyfileobj(resp.raw, file)
             logger.info(f"File downloaded {url}")
     except Exception as ex:
-        logger.debug(f"_download_file {url=} {type(ex).__name__} {ex}")
+        logger.debug(f"_download_file url={url} {type(ex).__name__} {ex}")
 
 
 def _normalize(raw_html):
     """strip HTML tags"""
     if raw_html:
         return unescape(re.sub(RE_STRIP_TAGS, "", raw_html))
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-2.9.5/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 2.9.4
+Version: 2.9.5
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![Python >= 3.7](https://img.shields.io/badge/python->=3.7-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search)
-# Duckduckgo_search<a name="TOP"></a>
+# Duckduckgo_search<a name="TOP"></a> 
+***_Attention. Versions before v2.9.4 no longer work as of May 12, 2023!_***
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
```

### Comparing `duckduckgo_search-2.9.4/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-2.9.5/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/pyproject.toml` & `duckduckgo_search-2.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg.py` & `duckduckgo_search-2.9.5/tests/test_ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg_answers.py` & `duckduckgo_search-2.9.5/tests/test_ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg_images.py` & `duckduckgo_search-2.9.5/tests/test_ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg_news.py` & `duckduckgo_search-2.9.5/tests/test_ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg_suggestions.py` & `duckduckgo_search-2.9.5/tests/test_ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg_translate.py` & `duckduckgo_search-2.9.5/tests/test_ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.4/tests/test_ddg_videos.py` & `duckduckgo_search-2.9.5/tests/test_ddg_videos.py`

 * *Files identical despite different names*


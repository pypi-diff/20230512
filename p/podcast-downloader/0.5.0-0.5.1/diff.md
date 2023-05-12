# Comparing `tmp/podcast_downloader-0.5.0.tar.gz` & `tmp/podcast_downloader-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_downloader-0.5.0.tar", last modified: Thu Apr 27 20:06:25 2023, max compression
+gzip compressed data, was "podcast_downloader-0.5.1.tar", last modified: Fri May 12 20:08:14 2023, max compression
```

## Comparing `podcast_downloader-0.5.0.tar` & `podcast_downloader-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/podcast_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/downloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/podcast_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/podcast_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 20:06:25.000000 podcast_downloader-0.5.0/podcast_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:06:25.317252 podcast_downloader-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-27 20:06:02.000000 podcast_downloader-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/podcast_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/downloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/podcast_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/podcast_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 20:08:14.000000 podcast_downloader-0.5.1/podcast_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:08:14.695814 podcast_downloader-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-12 20:08:04.000000 podcast_downloader-0.5.1/setup.py
```

### Comparing `podcast_downloader-0.5.0/LICENSE` & `podcast_downloader-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/PKG-INFO` & `podcast_downloader-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast_downloader
-Version: 0.5.0
+Version: 0.5.1
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
```

### Comparing `podcast_downloader-0.5.0/README.md` & `podcast_downloader-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/podcast_downloader/__main__.py` & `podcast_downloader-0.5.1/podcast_downloader/__main__.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/podcast_downloader/configuration.py` & `podcast_downloader-0.5.1/podcast_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/podcast_downloader/downloaded.py` & `podcast_downloader-0.5.1/podcast_downloader/downloaded.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/podcast_downloader/parameters.py` & `podcast_downloader-0.5.1/podcast_downloader/parameters.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/podcast_downloader/rss.py` & `podcast_downloader-0.5.1/podcast_downloader/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return link.rpartition(".")[-1]
 
     return ""
 
 
 def str_to_filename(value: str) -> str:
     value = unicodedata.normalize("NFKC", value)
-    value = re.sub(r"[\u0000-\u001F\u007F\*/:<>\?\\\|]", " ", value)
+    value = re.sub(r"[\u0000-\u001F\u007F\*/:<>\"\?\\\|]", " ", value)
 
     return value.strip()
 
 
 def file_template_to_file_name(name_template: str, entity: RSSEntity) -> str:
     return (
         name_template.replace("%file_name%", link_to_file_name(entity.link))
```

### Comparing `podcast_downloader-0.5.0/podcast_downloader/utils.py` & `podcast_downloader-0.5.1/podcast_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.5.0/podcast_downloader.egg-info/PKG-INFO` & `podcast_downloader-0.5.1/podcast_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-downloader
-Version: 0.5.0
+Version: 0.5.1
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
```

### Comparing `podcast_downloader-0.5.0/setup.py` & `podcast_downloader-0.5.1/setup.py`

 * *Files identical despite different names*


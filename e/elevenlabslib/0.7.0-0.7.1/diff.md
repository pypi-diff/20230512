# Comparing `tmp/elevenlabslib-0.7.0.tar.gz` & `tmp/elevenlabslib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.7.0.tar", last modified: Wed May 10 20:41:45 2023, max compression
+gzip compressed data, was "elevenlabslib-0.7.1.tar", last modified: Fri May 12 19:59:47 2023, max compression
```

## Comparing `elevenlabslib-0.7.0.tar` & `elevenlabslib-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 20:41:45.597517 elevenlabslib-0.7.0/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-05-10 20:41:45.596521 elevenlabslib-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 20:41:45.581520 elevenlabslib-0.7.0/elevenlabslib/
--rw-rw-rw-   0        0        0     4629 2023-05-10 20:06:36.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    15016 2023-05-10 20:10:15.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    36538 2023-05-10 20:40:35.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.0/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-10 20:36:24.000000 elevenlabslib-0.7.0/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:41:45.595517 elevenlabslib-0.7.0/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-10 20:38:23.000000 elevenlabslib-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 20:41:45.597517 elevenlabslib-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 19:59:47.985493 elevenlabslib-0.7.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-05-12 19:59:47.984493 elevenlabslib-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 19:59:47.966493 elevenlabslib-0.7.1/elevenlabslib/
+-rw-rw-rw-   0        0        0     6421 2023-05-12 19:58:46.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    15016 2023-05-10 20:10:15.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    36538 2023-05-10 20:40:35.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.1/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-10 20:36:24.000000 elevenlabslib-0.7.1/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:59:47.983492 elevenlabslib-0.7.1/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-12 19:59:26.000000 elevenlabslib-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 19:59:47.985493 elevenlabslib-0.7.1/setup.cfg
```

### Comparing `elevenlabslib-0.7.0/LICENSE` & `elevenlabslib-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/PKG-INFO` & `elevenlabslib-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.0
+Version: 0.7.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.0/README.md` & `elevenlabslib-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsVoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/elevenlabslib/__init__.py` & `elevenlabslib-0.7.1/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/elevenlabslib/helpers.py` & `elevenlabslib-0.7.1/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.0/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.7.1/elevenlabslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.0
+Version: 0.7.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.0/pyproject.toml` & `elevenlabslib-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```


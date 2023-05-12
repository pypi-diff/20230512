# Comparing `tmp/wyoming_piper-0.0.2.tar.gz` & `tmp/wyoming_piper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_piper-0.0.2.tar", last modified: Wed Apr 19 20:16:08 2023, max compression
+gzip compressed data, was "wyoming_piper-0.0.3.tar", last modified: Fri May 12 20:29:57 2023, max compression
```

## Comparing `wyoming_piper-0.0.2.tar` & `wyoming_piper-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-19 16:16:21.000000 wyoming_piper-0.0.2/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      627 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-19 18:47:39.000000 wyoming_piper-0.0.2/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1205 2023-04-19 20:14:32.000000 wyoming_piper-0.0.2/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/wyoming_piper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-19 19:04:59.000000 wyoming_piper-0.0.2/wyoming_piper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4503 2023-04-19 20:03:45.000000 wyoming_piper-0.0.2/wyoming_piper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-19 15:13:49.000000 wyoming_piper-0.0.2/wyoming_piper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     1106 2023-04-19 19:08:21.000000 wyoming_piper-0.0.2/wyoming_piper/download.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3634 2023-04-19 19:09:15.000000 wyoming_piper-0.0.2/wyoming_piper/handler.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 20:16:08.750707 wyoming_piper-0.0.2/wyoming_piper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      627 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      347 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-04-19 20:16:08.000000 wyoming_piper-0.0.2/wyoming_piper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1205 2023-05-10 19:58:40.000000 wyoming_piper-0.0.3/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/wyoming_piper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/wyoming_piper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4503 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/wyoming_piper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/wyoming_piper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     2603 2023-05-10 20:32:19.000000 wyoming_piper-0.0.3/wyoming_piper/download.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-0.0.3/wyoming_piper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3689 2023-05-11 15:57:03.000000 wyoming_piper-0.0.3/wyoming_piper/handler.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     9186 2023-05-12 17:05:02.000000 wyoming_piper-0.0.3/wyoming_piper/voice_hashes.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/wyoming_piper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      404 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/top_level.txt
```

### Comparing `wyoming_piper-0.0.2/PKG-INFO` & `wyoming_piper-0.0.3/wyoming_piper.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1
-Name: wyoming_piper
-Version: 0.0.2
+Metadata-Version: 1.1
+Name: wyoming-piper
+Version: 0.0.3
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
+Description: UNKNOWN
 Keywords: rhasspy wyoming piper
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `wyoming_piper-0.0.2/setup.py` & `wyoming_piper-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(requirements_path, "r", encoding="utf-8") as requirements_file:
         requirements = requirements_file.read().splitlines()
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_piper",
-    version="0.0.2",
+    version="0.0.3",
     description="Wyoming Server for Piper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `wyoming_piper-0.0.2/wyoming_piper/__main__.py` & `wyoming_piper-0.0.3/wyoming_piper/__main__.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.2/wyoming_piper/const.py` & `wyoming_piper-0.0.3/wyoming_piper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.2/wyoming_piper/handler.py` & `wyoming_piper-0.0.3/wyoming_piper/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,18 @@
 
         if not Synthesize.is_type(event.type):
             _LOGGER.warning("Unexpected event: %s", event)
             return True
 
         synthesize = Synthesize.from_event(event)
         raw_text = synthesize.text
-        text = raw_text.strip()
+
+        # Join multiple lines
+        text = " ".join(raw_text.strip().splitlines())
+
         if self.cli_args.auto_punctuation and text:
             # Add automatic punctuation (important for some voices)
             has_punctuation = False
             for punc_char in self.cli_args.auto_punctuation:
                 if text[-1] == punc_char:
                     has_punctuation = True
                     break
```

### Comparing `wyoming_piper-0.0.2/wyoming_piper.egg-info/PKG-INFO` & `wyoming_piper-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1
-Name: wyoming-piper
-Version: 0.0.2
+Metadata-Version: 1.1
+Name: wyoming_piper
+Version: 0.0.3
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
+Description: UNKNOWN
 Keywords: rhasspy wyoming piper
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


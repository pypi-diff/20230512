# Comparing `tmp/streaming_indicators-0.0.1.tar.gz` & `tmp/streaming_indicators-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.1.tar", last modified: Fri May 12 16:41:50 2023, max compression
+gzip compressed data, was "streaming_indicators-0.0.1b0.tar", last modified: Fri May 12 17:33:34 2023, max compression
```

## Comparing `streaming_indicators-0.0.1.tar` & `streaming_indicators-0.0.1b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 16:41:50.405068 streaming_indicators-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2830 2023-05-12 16:41:50.406063 streaming_indicators-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      887 2023-05-12 16:41:50.417859 streaming_indicators-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 16:41:50.374345 streaming_indicators-0.0.1/streaming_indicators/
-drwxrwxrwx   0        0        0        0 2023-05-12 16:41:50.403053 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 17:33:34.144430 streaming_indicators-0.0.1b0/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.1b0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2826 2023-05-12 17:33:34.145161 streaming_indicators-0.0.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.1b0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0      882 2023-05-12 17:33:34.151152 streaming_indicators-0.0.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 17:33:33.784962 streaming_indicators-0.0.1b0/streaming_indicators/
+drwxrwxrwx   0        0        0        0 2023-05-12 17:33:33.813965 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     2826 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.1/LICENSE.txt` & `streaming_indicators-0.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.1/PKG-INFO` & `streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: streaming_indicators
-Version: 0.0.1
+Name: streaming-indicators
+Version: 0.0.1b0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
-Project-URL: repository, https://github.com/mr-easy/streaming_indicators
+Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `streaming_indicators-0.0.1/README.md` & `streaming_indicators-0.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/PKG-INFO` & `streaming_indicators-0.0.1b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: streaming-indicators
-Version: 0.0.1
+Name: streaming_indicators
+Version: 0.0.1b0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
-Project-URL: repository, https://github.com/mr-easy/streaming_indicators
+Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```


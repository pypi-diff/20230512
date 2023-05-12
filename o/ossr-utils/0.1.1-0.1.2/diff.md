# Comparing `tmp/ossr_utils-0.1.1.tar.gz` & `tmp/ossr_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossr_utils-0.1.1.tar", max compression
+gzip compressed data, was "ossr_utils-0.1.2.tar", max compression
```

## Comparing `ossr_utils-0.1.1.tar` & `ossr_utils-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       67 2023-05-12 16:15:06.843492 ossr_utils-0.1.1/README.md
--rw-r--r--   0        0        0      355 2023-05-12 16:19:39.159961 ossr_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-12 16:09:00.188445 ossr_utils-0.1.1/src/ossr_utils/__init__.py
--rw-r--r--   0        0        0      443 2023-05-12 16:08:56.032271 ossr_utils-0.1.1/src/ossr_utils/audio_utils.py
--rw-r--r--   0        0        0      981 2023-01-10 22:55:56.183254 ossr_utils-0.1.1/src/ossr_utils/fft_utils.py
--rw-r--r--   0        0        0      492 2023-05-11 15:05:58.393123 ossr_utils-0.1.1/src/ossr_utils/io_utils.py
--rw-r--r--   0        0        0     4831 2023-05-11 15:18:51.415248 ossr_utils-0.1.1/src/ossr_utils/misc_utils.py
--rw-r--r--   0        0        0      992 2023-01-27 15:44:16.196447 ossr_utils-0.1.1/src/ossr_utils/model_utils.py
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 ossr_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-05-12 16:15:06.843492 ossr_utils-0.1.2/README.md
+-rw-r--r--   0        0        0      355 2023-05-12 18:44:30.526672 ossr_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-12 18:39:40.636726 ossr_utils-0.1.2/src/ossr_utils/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-12 16:08:56.032271 ossr_utils-0.1.2/src/ossr_utils/audio_utils.py
+-rw-r--r--   0        0        0      981 2023-01-10 22:55:56.183254 ossr_utils-0.1.2/src/ossr_utils/fft_utils.py
+-rw-r--r--   0        0        0      492 2023-05-11 15:05:58.393123 ossr_utils-0.1.2/src/ossr_utils/io_utils.py
+-rw-r--r--   0        0        0     4831 2023-05-11 15:18:51.415248 ossr_utils-0.1.2/src/ossr_utils/misc_utils.py
+-rw-r--r--   0        0        0      992 2023-01-27 15:44:16.196447 ossr_utils-0.1.2/src/ossr_utils/model_utils.py
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 ossr_utils-0.1.2/PKG-INFO
```

### Comparing `ossr_utils-0.1.1/src/ossr_utils/fft_utils.py` & `ossr_utils-0.1.2/src/ossr_utils/fft_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.1/src/ossr_utils/misc_utils.py` & `ossr_utils-0.1.2/src/ossr_utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.1/src/ossr_utils/model_utils.py` & `ossr_utils-0.1.2/src/ossr_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.1/PKG-INFO` & `ossr_utils-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossr-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils for the Open-Set Sound Recognition (OSSR) system
 License: MIT
 Author: Johannes Traa
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


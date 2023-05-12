# Comparing `tmp/sca_rhythm-0.4.4.tar.gz` & `tmp/sca_rhythm-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.4.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.5.tar", max compression
```

## Comparing `sca_rhythm-0.4.4.tar` & `sca_rhythm-0.4.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.4/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.4/README.md
--rw-r--r--   0        0        0      357 2023-05-12 03:16:58.661586 sca_rhythm-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.4/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.4/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.5/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.5/README.md
+-rw-r--r--   0        0        0      360 2023-05-12 20:24:14.051216 sca_rhythm-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.5/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.5/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sca_rhythm-0.4.5/PKG-INFO
```

### Comparing `sca_rhythm-0.4.4/LICENSE.md` & `sca_rhythm-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.4/README.md` & `sca_rhythm-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.4/sca_rhythm/__init__.py` & `sca_rhythm-0.4.5/sca_rhythm/__init__.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.4/sca_rhythm/progress.py` & `sca_rhythm-0.4.5/sca_rhythm/progress.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.4/PKG-INFO` & `sca_rhythm-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.4
+Version: 0.4.5
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: celery (>=5.2.7,<6.0.0)
+Requires-Dist: celery (>=5.3.0rc1,<6.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Rhythm
 Rhythm allows you to design and control workflows made of Celery tasks. A workflow is a sequence of steps to run one after the other. Rhythm simplifies the process of executing workflows consisting of long-running tasks with reliability.
 
 The following are the features of Rhythm workflows:
```


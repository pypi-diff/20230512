# Comparing `tmp/downstream_fairness-0.0.1.tar.gz` & `tmp/downstream_fairness-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downstream_fairness-0.0.1.tar", last modified: Thu May  4 14:22:20 2023, max compression
+gzip compressed data, was "downstream_fairness-0.1.0.tar", last modified: Fri May 12 15:45:06 2023, max compression
```

## Comparing `downstream_fairness-0.0.1.tar` & `downstream_fairness-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 reese      (501) admin       (80)        0 2023-05-04 14:22:20.947023 downstream_fairness-0.0.1/
--rw-r--r--   0 reese      (501) admin       (80)     1066 2023-05-04 14:11:41.000000 downstream_fairness-0.0.1/LICENSE.txt
--rw-r--r--   0 reese      (501) admin       (80)     2831 2023-05-04 14:22:20.946921 downstream_fairness-0.0.1/PKG-INFO
--rw-r--r--   0 reese      (501) admin       (80)     2233 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/README.md
-drwxr-xr-x   0 reese      (501) admin       (80)        0 2023-05-04 14:22:20.945615 downstream_fairness-0.0.1/downstream_fairness/
--rw-r--r--   0 reese      (501) admin       (80)       33 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/downstream_fairness/__init__.py
--rw-r--r--   0 reese      (501) admin       (80)     5827 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/downstream_fairness/process.py
--rw-r--r--   0 reese      (501) admin       (80)     8140 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/downstream_fairness/train.py
-drwxr-xr-x   0 reese      (501) admin       (80)        0 2023-05-04 14:22:20.946412 downstream_fairness-0.0.1/downstream_fairness/utils/
--rw-r--r--   0 reese      (501) admin       (80)     8385 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/downstream_fairness/utils/barycenter.py
--rw-r--r--   0 reese      (501) admin       (80)      282 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/downstream_fairness/utils/constants.py
--rw-r--r--   0 reese      (501) admin       (80)    11147 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/downstream_fairness/utils/metrics.py
--rw-r--r--   0 reese      (501) admin       (80)      344 2023-05-04 14:11:41.000000 downstream_fairness-0.0.1/downstream_fairness/version.py
-drwxr-xr-x   0 reese      (501) admin       (80)        0 2023-05-04 14:22:20.946118 downstream_fairness-0.0.1/downstream_fairness.egg-info/
--rw-r--r--   0 reese      (501) admin       (80)     2831 2023-05-04 14:22:20.000000 downstream_fairness-0.0.1/downstream_fairness.egg-info/PKG-INFO
--rw-r--r--   0 reese      (501) admin       (80)      553 2023-05-04 14:22:20.000000 downstream_fairness-0.0.1/downstream_fairness.egg-info/SOURCES.txt
--rw-r--r--   0 reese      (501) admin       (80)        1 2023-05-04 14:22:20.000000 downstream_fairness-0.0.1/downstream_fairness.egg-info/dependency_links.txt
--rw-r--r--   0 reese      (501) admin       (80)      108 2023-05-04 14:22:20.000000 downstream_fairness-0.0.1/downstream_fairness.egg-info/requires.txt
--rw-r--r--   0 reese      (501) admin       (80)       20 2023-05-04 14:22:20.000000 downstream_fairness-0.0.1/downstream_fairness.egg-info/top_level.txt
--rw-r--r--   0 reese      (501) admin       (80)     1186 2023-05-04 14:19:21.000000 downstream_fairness-0.0.1/pyproject.toml
--rw-r--r--   0 reese      (501) admin       (80)       38 2023-05-04 14:22:20.947050 downstream_fairness-0.0.1/setup.cfg
-drwxr-xr-x   0 reese      (501) admin       (80)        0 2023-05-04 14:22:20.946742 downstream_fairness-0.0.1/test/
--rw-r--r--   0 reese      (501) admin       (80)     2874 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/test/test_barycenter.py
--rw-r--r--   0 reese      (501) admin       (80)     2520 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/test/test_process.py
--rw-r--r--   0 reese      (501) admin       (80)     1449 2023-05-03 17:08:16.000000 downstream_fairness-0.0.1/test/test_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 15:45:06.531467 downstream_fairness-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-05-12 15:45:06.531467 downstream_fairness-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 15:45:06.526467 downstream_fairness-0.1.0/downstream_fairness/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     8140 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 15:45:06.529467 downstream_fairness-0.1.0/downstream_fairness/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     8385 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/utils/barycenter.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11147 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/utils/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/downstream_fairness/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 15:45:06.528467 downstream_fairness-0.1.0/downstream_fairness.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-05-12 15:45:06.000000 downstream_fairness-0.1.0/downstream_fairness.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      553 2023-05-12 15:45:06.000000 downstream_fairness-0.1.0/downstream_fairness.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 15:45:06.000000 downstream_fairness-0.1.0/downstream_fairness.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-12 15:45:06.000000 downstream_fairness-0.1.0/downstream_fairness.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-12 15:45:06.000000 downstream_fairness-0.1.0/downstream_fairness.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 15:45:06.531467 downstream_fairness-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 15:45:06.530467 downstream_fairness-0.1.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2874 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/test/test_barycenter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/test/test_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2023-05-12 15:44:46.000000 downstream_fairness-0.1.0/test/test_train.py
```

### Comparing `downstream_fairness-0.0.1/LICENSE.txt` & `downstream_fairness-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/PKG-INFO` & `downstream_fairness-0.1.0/downstream_fairness.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
-Name: downstream_fairness
-Version: 0.0.1
+Name: downstream-fairness
+Version: 0.1.0
 Summary: A new post-processing fairness algorithm that operates on the output probabilities of a binary classifier
 Author-email: Arthur <info@arthur.ai>, Daniel Nissani <daniel.nissani@arthur.ai>
 License: MIT
+Project-URL: Homepage, http://arthur.ai
+Project-URL: Repository, https://github.com/arthur-ai/downstream-fairness
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `downstream_fairness-0.0.1/README.md` & `downstream_fairness-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/downstream_fairness/process.py` & `downstream_fairness-0.1.0/downstream_fairness/process.py`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/downstream_fairness/train.py` & `downstream_fairness-0.1.0/downstream_fairness/train.py`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/downstream_fairness/utils/barycenter.py` & `downstream_fairness-0.1.0/downstream_fairness/utils/barycenter.py`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/downstream_fairness/utils/metrics.py` & `downstream_fairness-0.1.0/downstream_fairness/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/downstream_fairness.egg-info/PKG-INFO` & `downstream_fairness-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
-Name: downstream-fairness
-Version: 0.0.1
+Name: downstream_fairness
+Version: 0.1.0
 Summary: A new post-processing fairness algorithm that operates on the output probabilities of a binary classifier
 Author-email: Arthur <info@arthur.ai>, Daniel Nissani <daniel.nissani@arthur.ai>
 License: MIT
+Project-URL: Homepage, http://arthur.ai
+Project-URL: Repository, https://github.com/arthur-ai/downstream-fairness
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `downstream_fairness-0.0.1/downstream_fairness.egg-info/SOURCES.txt` & `downstream_fairness-0.1.0/downstream_fairness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/pyproject.toml` & `downstream_fairness-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,20 +22,21 @@
 
 dependencies = [
     "numpy>=1.19.0,<2",
     "pandas>=1.2.0",
     "POT==0.9.0",
     "python-dateutil>=2.7,<3",
     "pytz>=2020.1",
-    "scipy>=1.8,<2",
+    "scipy~=1.10.1",
     "tzdata==2020.1"
 ]
 
-[metadata]
-url = 'http://arthur.ai'
+[project.urls]
+Homepage = 'http://arthur.ai'
+Repository = "https://github.com/arthur-ai/downstream-fairness"
 
 [tool.setuptools.packages.find]
 include = ["downstream_fairness", "downstream_fairness.*"]
 exclude = ["test", "test.*"]
 
  [tool.setuptools.dynamic]
  version = {attr = "downstream_fairness.__version__"}
```

### Comparing `downstream_fairness-0.0.1/test/test_barycenter.py` & `downstream_fairness-0.1.0/test/test_barycenter.py`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/test/test_process.py` & `downstream_fairness-0.1.0/test/test_process.py`

 * *Files identical despite different names*

### Comparing `downstream_fairness-0.0.1/test/test_train.py` & `downstream_fairness-0.1.0/test/test_train.py`

 * *Files identical despite different names*


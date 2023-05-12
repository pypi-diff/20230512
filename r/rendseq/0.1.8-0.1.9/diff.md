# Comparing `tmp/rendseq-0.1.8.tar.gz` & `tmp/rendseq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendseq-0.1.8.tar", last modified: Wed Apr  5 17:46:39 2023, max compression
+gzip compressed data, was "rendseq-0.1.9.tar", last modified: Fri May 12 16:21:26 2023, max compression
```

## Comparing `rendseq-0.1.8.tar` & `rendseq-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 17:46:39.138526 rendseq-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-05 17:46:21.000000 rendseq-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-05 17:46:39.138526 rendseq-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-05 17:46:21.000000 rendseq-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-05 17:46:21.000000 rendseq-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 17:46:39.138526 rendseq-0.1.8/rendseq/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-05 17:46:21.000000 rendseq-0.1.8/rendseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-04-05 17:46:21.000000 rendseq-0.1.8/rendseq/file_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10403 2023-04-05 17:46:21.000000 rendseq-0.1.8/rendseq/make_peaks.py
--rw-r--r--   0 runner    (1001) docker     (122)    15401 2023-04-05 17:46:21.000000 rendseq-0.1.8/rendseq/ramps_steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-05 17:46:21.000000 rendseq-0.1.8/rendseq/utility_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     7620 2023-04-05 17:46:21.000000 rendseq-0.1.8/rendseq/zscores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 17:46:39.138526 rendseq-0.1.8/rendseq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-05 17:46:39.000000 rendseq-0.1.8/rendseq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-05 17:46:39.000000 rendseq-0.1.8/rendseq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-05 17:46:39.000000 rendseq-0.1.8/rendseq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-05 17:46:39.000000 rendseq-0.1.8/rendseq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-05 17:46:39.138526 rendseq-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-05 17:46:21.000000 rendseq-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:21:26.902562 rendseq-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-12 16:21:12.000000 rendseq-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-05-12 16:21:26.902562 rendseq-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-12 16:21:12.000000 rendseq-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-12 16:21:12.000000 rendseq-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:21:26.902562 rendseq-0.1.9/rendseq/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-12 16:21:12.000000 rendseq-0.1.9/rendseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-05-12 16:21:12.000000 rendseq-0.1.9/rendseq/file_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10409 2023-05-12 16:21:12.000000 rendseq-0.1.9/rendseq/make_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15401 2023-05-12 16:21:12.000000 rendseq-0.1.9/rendseq/ramps_steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-12 16:21:12.000000 rendseq-0.1.9/rendseq/utility_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6064 2023-05-12 16:21:12.000000 rendseq-0.1.9/rendseq/zscores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:21:26.902562 rendseq-0.1.9/rendseq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-05-12 16:21:26.000000 rendseq-0.1.9/rendseq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-12 16:21:26.000000 rendseq-0.1.9/rendseq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 16:21:26.000000 rendseq-0.1.9/rendseq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-12 16:21:26.000000 rendseq-0.1.9/rendseq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-05-12 16:21:26.902562 rendseq-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-05-12 16:21:12.000000 rendseq-0.1.9/setup.py
```

### Comparing `rendseq-0.1.8/LICENSE` & `rendseq-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rendseq-0.1.8/PKG-INFO` & `rendseq-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendseq
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for RendSeq Data Analysis
 Home-page: https://github.com/miraep8/rendseq
 Author: Mirae Parker
 Author-email: rendseq@mit.edu
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rendseq Version: 0.1.8 Summary: Package for RendSeq
+Metadata-Version: 2.1 Name: rendseq Version: 0.1.9 Summary: Package for RendSeq
 Data Analysis Home-page: https://github.com/miraep8/rendseq Author: Mirae
 Parker Author-email: rendseq@mit.edu License: MIT Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # rendseq
 *** A python package to facilitate your End-Enriched RNA Sequencing (Rend) data
                              analysis dreams! ***
 [Documentation_Link] [Lifecycle:_experimental] [https://codecov.io/gh/miraep8/
              rendseq/branch/main/graph/badge.svg?token=SIGSJGCZPI]
```

### Comparing `rendseq-0.1.8/README.md` & `rendseq-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rendseq-0.1.8/rendseq/file_funcs.py` & `rendseq-0.1.9/rendseq/file_funcs.py`

 * *Files identical despite different names*

### Comparing `rendseq-0.1.8/rendseq/make_peaks.py` & `rendseq-0.1.9/rendseq/make_peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,17 +199,17 @@
         - thresh - the threshold value to use.  If none is provided it will be
             automatically calculated.
         - method - the method to use to automatically calculate the z score
             if none is provided.  Default method is "kink"
     """
     if thresh is None:
         thresh = _calc_thresh(z_scores, method)
-    peaks = np.zeros([len(z_scores), 2])
+    peaks = 100 * np.ones([len(z_scores), 2])
     peaks[:, 0] = z_scores[:, 0]
-    peaks[:, 1] = (z_scores[:, 1] > thresh).astype(int)
+    peaks = np.delete(peaks, z_scores[:, 1] < thresh, 0)
     return peaks
 
 
 def parse_args_make_peaks(args):
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description="Can run from the\
```

### Comparing `rendseq-0.1.8/rendseq/ramps_steps.py` & `rendseq-0.1.9/rendseq/ramps_steps.py`

 * *Files identical despite different names*

### Comparing `rendseq-0.1.8/rendseq/utility_funcs.py` & `rendseq-0.1.9/rendseq/utility_funcs.py`

 * *Files identical despite different names*

### Comparing `rendseq-0.1.8/rendseq.egg-info/PKG-INFO` & `rendseq-0.1.9/rendseq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendseq
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for RendSeq Data Analysis
 Home-page: https://github.com/miraep8/rendseq
 Author: Mirae Parker
 Author-email: rendseq@mit.edu
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rendseq Version: 0.1.8 Summary: Package for RendSeq
+Metadata-Version: 2.1 Name: rendseq Version: 0.1.9 Summary: Package for RendSeq
 Data Analysis Home-page: https://github.com/miraep8/rendseq Author: Mirae
 Parker Author-email: rendseq@mit.edu License: MIT Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # rendseq
 *** A python package to facilitate your End-Enriched RNA Sequencing (Rend) data
                              analysis dreams! ***
 [Documentation_Link] [Lifecycle:_experimental] [https://codecov.io/gh/miraep8/
              rendseq/branch/main/graph/badge.svg?token=SIGSJGCZPI]
```

### Comparing `rendseq-0.1.8/setup.py` & `rendseq-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rendseq",
-    version="0.1.8",
+    version="0.1.9",
     description="Package for RendSeq Data Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miraep8/rendseq",
     author="Mirae Parker",
     author_email="rendseq@mit.edu",
     license="MIT",
```


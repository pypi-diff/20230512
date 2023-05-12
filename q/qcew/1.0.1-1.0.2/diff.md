# Comparing `tmp/qcew-1.0.1.tar.gz` & `tmp/qcew-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcew-1.0.1.tar", last modified: Fri May 12 17:10:19 2023, max compression
+gzip compressed data, was "qcew-1.0.2.tar", last modified: Fri May 12 17:20:03 2023, max compression
```

## Comparing `qcew-1.0.1.tar` & `qcew-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:10:19.041760 qcew-1.0.1/
--rw-r--r--   0 TrentThompson   (501) staff       (20)     1090 2023-05-12 11:30:42.000000 qcew-1.0.1/LICENSE
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2774 2023-05-12 17:10:19.041317 qcew-1.0.1/PKG-INFO
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2128 2023-05-12 16:57:32.000000 qcew-1.0.1/README.md
--rw-r--r--   0 TrentThompson   (501) staff       (20)       38 2023-05-12 17:10:19.041883 qcew-1.0.1/setup.cfg
--rw-r--r--   0 TrentThompson   (501) staff       (20)      979 2023-05-12 17:09:57.000000 qcew-1.0.1/setup.py
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:10:19.033443 qcew-1.0.1/src/
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:10:19.040579 qcew-1.0.1/src/qcew.egg-info/
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2774 2023-05-12 17:10:19.000000 qcew-1.0.1/src/qcew.egg-info/PKG-INFO
--rw-r--r--   0 TrentThompson   (501) staff       (20)      166 2023-05-12 17:10:19.000000 qcew-1.0.1/src/qcew.egg-info/SOURCES.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 17:10:19.000000 qcew-1.0.1/src/qcew.egg-info/dependency_links.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)        5 2023-05-12 17:10:19.000000 qcew-1.0.1/src/qcew.egg-info/top_level.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)    11681 2023-05-12 11:30:42.000000 qcew-1.0.1/src/qcew.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:20:03.063572 qcew-1.0.2/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     1090 2023-05-12 11:30:42.000000 qcew-1.0.2/LICENSE
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2775 2023-05-12 17:20:03.063070 qcew-1.0.2/PKG-INFO
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2128 2023-05-12 16:57:32.000000 qcew-1.0.2/README.md
+-rw-r--r--   0 TrentThompson   (501) staff       (20)       38 2023-05-12 17:20:03.063707 qcew-1.0.2/setup.cfg
+-rw-r--r--   0 TrentThompson   (501) staff       (20)      980 2023-05-12 17:12:09.000000 qcew-1.0.2/setup.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:20:03.056198 qcew-1.0.2/src/
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:20:03.062395 qcew-1.0.2/src/qcew.egg-info/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2775 2023-05-12 17:20:03.000000 qcew-1.0.2/src/qcew.egg-info/PKG-INFO
+-rw-r--r--   0 TrentThompson   (501) staff       (20)      166 2023-05-12 17:20:03.000000 qcew-1.0.2/src/qcew.egg-info/SOURCES.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 17:20:03.000000 qcew-1.0.2/src/qcew.egg-info/dependency_links.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        5 2023-05-12 17:20:03.000000 qcew-1.0.2/src/qcew.egg-info/top_level.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)    11681 2023-05-12 11:30:42.000000 qcew-1.0.2/src/qcew.py
```

### Comparing `qcew-1.0.1/LICENSE` & `qcew-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qcew-1.0.1/PKG-INFO` & `qcew-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qcew
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for retrieving Quarterly Census of Employment and Wages (QCEW) data.
 Home-page: https://github.com/TrentLThompson/qcew
 Author: Trent Thompson
 Author-email: 808trent@gmail.com
 Keywords: QCEW,BLS,employment,wages,statistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # qcew
 
 A package for retrieving Quarterly Census of Employment and Wages ([QCEW](https://www.bls.gov/cew/)) data from the Bureau of Labor Statistics' [database](https://www.bls.gov/cew/downloadable-data-files.htm).
```

### Comparing `qcew-1.0.1/README.md` & `qcew-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qcew-1.0.1/src/qcew.egg-info/PKG-INFO` & `qcew-1.0.2/src/qcew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qcew
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for retrieving Quarterly Census of Employment and Wages (QCEW) data.
 Home-page: https://github.com/TrentLThompson/qcew
 Author: Trent Thompson
 Author-email: 808trent@gmail.com
 Keywords: QCEW,BLS,employment,wages,statistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # qcew
 
 A package for retrieving Quarterly Census of Employment and Wages ([QCEW](https://www.bls.gov/cew/)) data from the Bureau of Labor Statistics' [database](https://www.bls.gov/cew/downloadable-data-files.htm).
```

### Comparing `qcew-1.0.1/src/qcew.py` & `qcew-1.0.2/src/qcew.py`

 * *Files identical despite different names*


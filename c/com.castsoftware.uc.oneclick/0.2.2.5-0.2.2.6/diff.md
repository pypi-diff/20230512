# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.5.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.5.tar", last modified: Fri May 12 14:41:02 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.6.tar", last modified: Fri May 12 16:04:59 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.5.tar` & `com.castsoftware.uc.oneclick-0.2.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 14:41:02.354397 com.castsoftware.uc.oneclick-0.2.2.5/
--rw-rw-rw-   0        0        0      517 2023-05-12 14:41:02.280074 com.castsoftware.uc.oneclick-0.2.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 14:41:01.986522 com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-12 14:41:01.000000 com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-05-12 14:41:01.000000 com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 14:41:01.000000 com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      163 2023-05-12 14:41:01.000000 com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 14:41:01.000000 com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 14:41:02.080906 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/
--rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 14:41:02.134135 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3454 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19841 2023-05-12 13:25:09.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-05-12 14:41:02.267025 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9049 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6835 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11247 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     6039 2023-05-12 13:56:42.000000 com.castsoftware.uc.oneclick-0.2.2.5/oneclick/setup.py
--rw-rw-rw-   0        0        0      738 2023-05-12 14:15:36.000000 com.castsoftware.uc.oneclick-0.2.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 14:41:02.354397 com.castsoftware.uc.oneclick-0.2.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:59.946872 com.castsoftware.uc.oneclick-0.2.2.6/
+-rw-rw-rw-   0        0        0      517 2023-05-12 16:04:59.936767 com.castsoftware.uc.oneclick-0.2.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:59.601204 com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-12 16:04:59.000000 com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-05-12 16:04:59.000000 com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:04:59.000000 com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-05-12 16:04:59.000000 com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 16:04:59.000000 com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:59.755688 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:59.816837 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     3454 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    19841 2023-05-12 13:25:09.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:59.923918 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9049 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    11247 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     6039 2023-05-12 13:56:42.000000 com.castsoftware.uc.oneclick-0.2.2.6/oneclick/setup.py
+-rw-rw-rw-   0        0        0      759 2023-05-12 16:04:25.000000 com.castsoftware.uc.oneclick-0.2.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 16:04:59.948157 com.castsoftware.uc.oneclick-0.2.2.6/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.5
+Version: 0.2.2.6
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.5
+Version: 0.2.2.6
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.2.6/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/highlight_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/cloc.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/discovery/unzip.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/oneclick/setup.py` & `com.castsoftware.uc.oneclick-0.2.2.6/oneclick/setup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.5/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.2.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2.5' #prod version
+version='0.2.2.6' #prod version
 dependencies = [
     'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
+    'URLValidator',
     'com.castsoftware.uc.python.common>=0.1.11',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```


# Comparing `tmp/flaretool-0.1.7.tar.gz` & `tmp/flaretool-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaretool-0.1.7.tar", last modified: Fri May 12 06:16:52 2023, max compression
+gzip compressed data, was "flaretool-0.1.8.tar", last modified: Fri May 12 06:50:31 2023, max compression
```

## Comparing `flaretool-0.1.7.tar` & `flaretool-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 white     (1000) white     (1000)        0 2023-05-12 06:16:52.311966 flaretool-0.1.7/
--rw-rw-r--   0 white     (1000) white     (1000)     1066 2023-05-11 13:18:09.000000 flaretool-0.1.7/LICENSE
--rw-rw-r--   0 white     (1000) white     (1000)       48 2023-05-11 13:22:25.000000 flaretool-0.1.7/MANIFEST.in
--rw-rw-r--   0 white     (1000) white     (1000)     1405 2023-05-12 06:16:52.307966 flaretool-0.1.7/PKG-INFO
--rw-rw-r--   0 white     (1000) white     (1000)      849 2023-05-11 23:54:03.000000 flaretool-0.1.7/README.md
-drwxrwxr-x   0 white     (1000) white     (1000)        0 2023-05-12 06:16:52.303966 flaretool-0.1.7/repos/
-drwxrwxr-x   0 white     (1000) white     (1000)        0 2023-05-12 06:16:52.307966 flaretool-0.1.7/repos/flaretool/
--rw-rw-r--   0 white     (1000) white     (1000)       56 2023-05-12 06:16:51.000000 flaretool-0.1.7/repos/flaretool/VERSION.py
--rw-rw-r--   0 white     (1000) white     (1000)      394 2023-05-11 14:19:48.000000 flaretool-0.1.7/repos/flaretool/__init__.py
--rw-rw-r--   0 white     (1000) white     (1000)     1565 2023-05-12 00:30:35.000000 flaretool-0.1.7/repos/flaretool/command.py
--rw-rw-r--   0 white     (1000) white     (1000)     2054 2023-05-11 14:23:20.000000 flaretool-0.1.7/repos/flaretool/error.py
-drwxrwxr-x   0 white     (1000) white     (1000)        0 2023-05-12 06:16:52.307966 flaretool-0.1.7/repos/flaretool/nettool/
--rw-rw-r--   0 white     (1000) white     (1000)      289 2023-05-11 16:29:53.000000 flaretool-0.1.7/repos/flaretool/nettool/__init__.py
--rw-rw-r--   0 white     (1000) white     (1000)     3613 2023-05-12 00:37:37.000000 flaretool-0.1.7/repos/flaretool/nettool/common.py
--rw-rw-r--   0 white     (1000) white     (1000)      298 2023-05-12 00:36:43.000000 flaretool-0.1.7/repos/flaretool/nettool/model.py
--rw-rw-r--   0 white     (1000) white     (1000)        0 2023-05-11 13:33:00.000000 flaretool-0.1.7/repos/flaretool/settings.py
-drwxrwxr-x   0 white     (1000) white     (1000)        0 2023-05-12 06:16:52.307966 flaretool-0.1.7/repos/flaretool.egg-info/
--rw-rw-r--   0 white     (1000) white     (1000)     1405 2023-05-12 06:16:52.000000 flaretool-0.1.7/repos/flaretool.egg-info/PKG-INFO
--rw-rw-r--   0 white     (1000) white     (1000)      579 2023-05-12 06:16:52.000000 flaretool-0.1.7/repos/flaretool.egg-info/SOURCES.txt
--rw-rw-r--   0 white     (1000) white     (1000)        1 2023-05-12 06:16:52.000000 flaretool-0.1.7/repos/flaretool.egg-info/dependency_links.txt
--rw-rw-r--   0 white     (1000) white     (1000)       54 2023-05-12 06:16:52.000000 flaretool-0.1.7/repos/flaretool.egg-info/entry_points.txt
--rw-rw-r--   0 white     (1000) white     (1000)        1 2023-05-11 13:43:16.000000 flaretool-0.1.7/repos/flaretool.egg-info/not-zip-safe
--rw-rw-r--   0 white     (1000) white     (1000)      196 2023-05-12 06:16:52.000000 flaretool-0.1.7/repos/flaretool.egg-info/requires.txt
--rw-rw-r--   0 white     (1000) white     (1000)       50 2023-05-12 06:16:52.000000 flaretool-0.1.7/repos/flaretool.egg-info/top_level.txt
--rw-rw-r--   0 white     (1000) white     (1000)      196 2023-05-12 06:16:51.000000 flaretool-0.1.7/requirements.txt
--rw-rw-r--   0 white     (1000) white     (1000)       38 2023-05-12 06:16:52.311966 flaretool-0.1.7/setup.cfg
--rw-rw-r--   0 white     (1000) white     (1000)     1515 2023-05-12 05:27:29.000000 flaretool-0.1.7/setup.py
--rw-rw-r--   0 white     (1000) white     (1000)        5 2023-05-12 06:16:51.000000 flaretool-0.1.7/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:31.089436 flaretool-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 06:50:12.000000 flaretool-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 06:50:12.000000 flaretool-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-12 06:50:31.089436 flaretool-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-12 06:50:12.000000 flaretool-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:31.085436 flaretool-0.1.8/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:31.089436 flaretool-0.1.8/repos/flaretool/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:31.089436 flaretool-0.1.8/repos/flaretool/nettool/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/nettool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/nettool/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/nettool/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:12.000000 flaretool-0.1.8/repos/flaretool/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:31.089436 flaretool-0.1.8/repos/flaretool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 06:50:31.000000 flaretool-0.1.8/repos/flaretool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 06:50:12.000000 flaretool-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 06:50:31.089436 flaretool-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-12 06:50:12.000000 flaretool-0.1.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 06:50:12.000000 flaretool-0.1.8/version.txt
```

### Comparing `flaretool-0.1.7/LICENSE` & `flaretool-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flaretool-0.1.7/PKG-INFO` & `flaretool-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: flaretool
-Version: 0.1.7
+Version: 0.1.8
 Summary: this is flarebrow package
 Home-page: https://main.flarebrow.com
 Author: flarebrow
 License: MIT
 Project-URL: Documentation, https://flarebrow.github.io/flaretool/
 Project-URL: Source, https://github.com/flarebrow/flaretool
 Keywords: flaretool
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flaretool
 
 **flaretool** is flarebrow Library.  
 
 ![](https://img.shields.io/badge/python-%3E%3D3.8-blue)
 
-[API Doc](https://flarebrow.github.io/flaretool/flaretool.nettool.html#module-flaretool.nettool)
+[API Doc](https://flarebrow.github.io/flaretool/flaretool.nettool.html)
 
 **Attention**  
 This library is under development and may exhibit unexpected behavior. New features will be released soon. Please stay tuned.
 
 
 ## install (dev)
 ```bash
@@ -49,9 +48,7 @@
 
 ```bash
 flaretool nettool get_global_ipaddr_info
 ```
 
 All methods within Netttol can be executed as commands.
 
-
-
```

### Comparing `flaretool-0.1.7/README.md` & `flaretool-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flaretool
 
 **flaretool** is flarebrow Library.  
 
 ![](https://img.shields.io/badge/python-%3E%3D3.8-blue)
 
-[API Doc](https://flarebrow.github.io/flaretool/flaretool.nettool.html#module-flaretool.nettool)
+[API Doc](https://flarebrow.github.io/flaretool/flaretool.nettool.html)
 
 **Attention**  
 This library is under development and may exhibit unexpected behavior. New features will be released soon. Please stay tuned.
 
 
 ## install (dev)
 ```bash
```

### Comparing `flaretool-0.1.7/repos/flaretool/command.py` & `flaretool-0.1.8/repos/flaretool/command.py`

 * *Files identical despite different names*

### Comparing `flaretool-0.1.7/repos/flaretool/error.py` & `flaretool-0.1.8/repos/flaretool/error.py`

 * *Files identical despite different names*

### Comparing `flaretool-0.1.7/repos/flaretool/nettool/common.py` & `flaretool-0.1.8/repos/flaretool/nettool/common.py`

 * *Files identical despite different names*

### Comparing `flaretool-0.1.7/repos/flaretool.egg-info/PKG-INFO` & `flaretool-0.1.8/repos/flaretool.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: flaretool
-Version: 0.1.7
+Version: 0.1.8
 Summary: this is flarebrow package
 Home-page: https://main.flarebrow.com
 Author: flarebrow
 License: MIT
 Project-URL: Documentation, https://flarebrow.github.io/flaretool/
 Project-URL: Source, https://github.com/flarebrow/flaretool
 Keywords: flaretool
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flaretool
 
 **flaretool** is flarebrow Library.  
 
 ![](https://img.shields.io/badge/python-%3E%3D3.8-blue)
 
-[API Doc](https://flarebrow.github.io/flaretool/flaretool.nettool.html#module-flaretool.nettool)
+[API Doc](https://flarebrow.github.io/flaretool/flaretool.nettool.html)
 
 **Attention**  
 This library is under development and may exhibit unexpected behavior. New features will be released soon. Please stay tuned.
 
 
 ## install (dev)
 ```bash
@@ -49,9 +48,7 @@
 
 ```bash
 flaretool nettool get_global_ipaddr_info
 ```
 
 All methods within Netttol can be executed as commands.
 
-
-
```

### Comparing `flaretool-0.1.7/repos/flaretool.egg-info/SOURCES.txt` & `flaretool-0.1.8/repos/flaretool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flaretool-0.1.7/setup.py` & `flaretool-0.1.8/setup.py`

 * *Files identical despite different names*


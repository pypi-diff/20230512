# Comparing `tmp/ink_extensions-1.2.0.tar.gz` & `tmp/ink_extensions-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ink_extensions-1.2.0.tar", last modified: Sun Dec 11 19:29:40 2022, max compression
+gzip compressed data, was "ink_extensions-1.3.0.tar", last modified: Thu May 11 22:01:19 2023, max compression
```

## Comparing `ink_extensions-1.2.0.tar` & `ink_extensions-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:40.963245 ink_extensions-1.2.0/
--rw-r--r--   0 oskay      (504) staff       (20)    18092 2018-12-10 18:38:07.000000 ink_extensions-1.2.0/LICENSE
--rw-r--r--   0 oskay      (504) staff       (20)      655 2022-12-11 19:29:40.963121 ink_extensions-1.2.0/PKG-INFO
--rw-r--r--   0 oskay      (504) staff       (20)      439 2019-07-21 17:18:17.000000 ink_extensions-1.2.0/README.md
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:40.961658 ink_extensions-1.2.0/ink_extensions/
--rwxr-xr-x   0 oskay      (504) staff       (20)      245 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/__init__.py
--rwxr-xr-x   0 oskay      (504) staff       (20)     9004 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/bezmisc.py
--rwxr-xr-x   0 oskay      (504) staff       (20)      908 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/cspsubdiv.py
--rwxr-xr-x   0 oskay      (504) staff       (20)     5234 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/cubicsuperpath.py
--rw-r--r--   0 oskay      (504) staff       (20)     4931 2022-12-10 02:00:22.000000 ink_extensions-1.2.0/ink_extensions/ffgeom.py
--rwxr-xr-x   0 oskay      (504) staff       (20)     4723 2022-12-10 01:58:22.000000 ink_extensions-1.2.0/ink_extensions/ffgeom_legacy.py
--rwx------   0 oskay      (504) staff       (20)    15539 2020-05-25 16:20:11.000000 ink_extensions-1.2.0/ink_extensions/inkex.py
--rwxr-xr-x   0 oskay      (504) staff       (20)     7052 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/simplepath.py
--rwxr-xr-x   0 oskay      (504) staff       (20)     7204 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/simplestyle.py
--rwxr-xr-x   0 oskay      (504) staff       (20)     9639 2019-02-25 23:13:22.000000 ink_extensions-1.2.0/ink_extensions/simpletransform.py
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:40.962389 ink_extensions-1.2.0/ink_extensions.egg-info/
--rw-r--r--   0 oskay      (504) staff       (20)      655 2022-12-11 19:29:40.000000 ink_extensions-1.2.0/ink_extensions.egg-info/PKG-INFO
--rw-r--r--   0 oskay      (504) staff       (20)      604 2022-12-11 19:29:40.000000 ink_extensions-1.2.0/ink_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 oskay      (504) staff       (20)        1 2022-12-11 19:29:40.000000 ink_extensions-1.2.0/ink_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 oskay      (504) staff       (20)       34 2022-12-11 19:29:40.000000 ink_extensions-1.2.0/ink_extensions.egg-info/requires.txt
--rw-r--r--   0 oskay      (504) staff       (20)       36 2022-12-11 19:29:40.000000 ink_extensions-1.2.0/ink_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 oskay      (504) staff       (20)        0 2022-12-11 19:29:40.962923 ink_extensions-1.2.0/ink_extensions_utils/
--rw-r--r--   0 oskay      (504) staff       (20)        1 2019-07-21 17:18:17.000000 ink_extensions-1.2.0/ink_extensions_utils/__init__.py
--rw-r--r--   0 oskay      (504) staff       (20)     1133 2019-07-21 17:18:17.000000 ink_extensions-1.2.0/ink_extensions_utils/exit_status.py
--rw-r--r--   0 oskay      (504) staff       (20)      708 2019-09-04 16:43:48.000000 ink_extensions-1.2.0/ink_extensions_utils/message.py
--rw-r--r--   0 oskay      (504) staff       (20)       38 2022-12-11 19:29:40.963284 ink_extensions-1.2.0/setup.cfg
--rw-r--r--   0 oskay      (504) staff       (20)      878 2022-12-10 02:46:08.000000 ink_extensions-1.2.0/setup.py
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-05-11 22:01:19.136350 ink_extensions-1.3.0/
+-rw-r--r--   0 oskay      (504) staff       (20)    18092 2018-12-10 18:38:07.000000 ink_extensions-1.3.0/LICENSE
+-rw-r--r--   0 oskay      (504) staff       (20)      655 2023-05-11 22:01:19.136163 ink_extensions-1.3.0/PKG-INFO
+-rw-r--r--   0 oskay      (504) staff       (20)      439 2019-07-21 17:18:17.000000 ink_extensions-1.3.0/README.md
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-05-11 22:01:19.134243 ink_extensions-1.3.0/ink_extensions/
+-rwxr-xr-x   0 oskay      (504) staff       (20)      245 2019-02-25 23:13:22.000000 ink_extensions-1.3.0/ink_extensions/__init__.py
+-rwxr-xr-x   0 oskay      (504) staff       (20)     9004 2019-02-25 23:13:22.000000 ink_extensions-1.3.0/ink_extensions/bezmisc.py
+-rwxr-xr-x   0 oskay      (504) staff       (20)      908 2019-02-25 23:13:22.000000 ink_extensions-1.3.0/ink_extensions/cspsubdiv.py
+-rwxr-xr-x   0 oskay      (504) staff       (20)     5234 2019-02-25 23:13:22.000000 ink_extensions-1.3.0/ink_extensions/cubicsuperpath.py
+-rw-r--r--   0 oskay      (504) staff       (20)     4931 2022-12-10 02:00:22.000000 ink_extensions-1.3.0/ink_extensions/ffgeom.py
+-rwxr-xr-x   0 oskay      (504) staff       (20)     4723 2022-12-10 01:58:22.000000 ink_extensions-1.3.0/ink_extensions/ffgeom_legacy.py
+-rwx------   0 oskay      (504) staff       (20)    15539 2020-05-25 16:20:11.000000 ink_extensions-1.3.0/ink_extensions/inkex.py
+-rw-r--r--   0 oskay      (504) staff       (20)     8082 2023-05-11 21:51:53.000000 ink_extensions-1.3.0/ink_extensions/simplepath.py
+-rwxr-xr-x   0 oskay      (504) staff       (20)     7204 2019-02-25 23:13:22.000000 ink_extensions-1.3.0/ink_extensions/simplestyle.py
+-rwxr-xr-x   0 oskay      (504) staff       (20)     9639 2019-02-25 23:13:22.000000 ink_extensions-1.3.0/ink_extensions/simpletransform.py
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-05-11 22:01:19.135055 ink_extensions-1.3.0/ink_extensions.egg-info/
+-rw-r--r--   0 oskay      (504) staff       (20)      655 2023-05-11 22:01:19.000000 ink_extensions-1.3.0/ink_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 oskay      (504) staff       (20)      604 2023-05-11 22:01:19.000000 ink_extensions-1.3.0/ink_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 oskay      (504) staff       (20)        1 2023-05-11 22:01:19.000000 ink_extensions-1.3.0/ink_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 oskay      (504) staff       (20)       34 2023-05-11 22:01:19.000000 ink_extensions-1.3.0/ink_extensions.egg-info/requires.txt
+-rw-r--r--   0 oskay      (504) staff       (20)       36 2023-05-11 22:01:19.000000 ink_extensions-1.3.0/ink_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 oskay      (504) staff       (20)        0 2023-05-11 22:01:19.135920 ink_extensions-1.3.0/ink_extensions_utils/
+-rw-r--r--   0 oskay      (504) staff       (20)        1 2019-07-21 17:18:17.000000 ink_extensions-1.3.0/ink_extensions_utils/__init__.py
+-rw-r--r--   0 oskay      (504) staff       (20)     1133 2019-07-21 17:18:17.000000 ink_extensions-1.3.0/ink_extensions_utils/exit_status.py
+-rw-r--r--   0 oskay      (504) staff       (20)      708 2019-09-04 16:43:48.000000 ink_extensions-1.3.0/ink_extensions_utils/message.py
+-rw-r--r--   0 oskay      (504) staff       (20)       38 2023-05-11 22:01:19.136419 ink_extensions-1.3.0/setup.cfg
+-rw-r--r--   0 oskay      (504) staff       (20)      878 2023-05-11 21:51:53.000000 ink_extensions-1.3.0/setup.py
```

### Comparing `ink_extensions-1.2.0/LICENSE` & `ink_extensions-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/PKG-INFO` & `ink_extensions-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ink_extensions
-Version: 1.2.0
+Version: 1.3.0
 Home-page: https://github.com/evil-mad/ink_extensions
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # ink_extensions
```

### Comparing `ink_extensions-1.2.0/ink_extensions/bezmisc.py` & `ink_extensions-1.3.0/ink_extensions/bezmisc.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/cspsubdiv.py` & `ink_extensions-1.3.0/ink_extensions/cspsubdiv.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/cubicsuperpath.py` & `ink_extensions-1.3.0/ink_extensions/cubicsuperpath.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/ffgeom.py` & `ink_extensions-1.3.0/ink_extensions/ffgeom.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/ffgeom_legacy.py` & `ink_extensions-1.3.0/ink_extensions/ffgeom_legacy.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/inkex.py` & `ink_extensions-1.3.0/ink_extensions/inkex.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/simplestyle.py` & `ink_extensions-1.3.0/ink_extensions/simplestyle.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions/simpletransform.py` & `ink_extensions-1.3.0/ink_extensions/simpletransform.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions.egg-info/PKG-INFO` & `ink_extensions-1.3.0/ink_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ink-extensions
-Version: 1.2.0
+Version: 1.3.0
 Home-page: https://github.com/evil-mad/ink_extensions
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # ink_extensions
```

### Comparing `ink_extensions-1.2.0/ink_extensions.egg-info/SOURCES.txt` & `ink_extensions-1.3.0/ink_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions_utils/exit_status.py` & `ink_extensions-1.3.0/ink_extensions_utils/exit_status.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/ink_extensions_utils/message.py` & `ink_extensions-1.3.0/ink_extensions_utils/message.py`

 * *Files identical despite different names*

### Comparing `ink_extensions-1.2.0/setup.py` & `ink_extensions-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ink_extensions',
-    version='1.2.0',
+    version='1.3.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/evil-mad/ink_extensions',
 
     packages=find_packages(exclude=['contrib', 'docs', 'test', 'test.*']),
     install_requires=[
         'lxml'
```


# Comparing `tmp/dicopp-1.0.35.tar.gz` & `tmp/dicopp-1.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicopp-1.0.35.tar", last modified: Fri Apr 21 19:29:24 2023, max compression
+gzip compressed data, was "dicopp-1.0.36.tar", last modified: Fri May 12 13:08:08 2023, max compression
```

## Comparing `dicopp-1.0.35.tar` & `dicopp-1.0.36.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-04-21 19:29:24.593887 dicopp-1.0.35/
--rw-rw-r--   0 bc        (1000) bc        (1000)      385 2023-04-21 19:29:24.593887 dicopp-1.0.35/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      894 2023-03-23 11:57:18.000000 dicopp-1.0.35/README.md
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-04-21 19:29:24.585887 dicopp-1.0.35/dicopp/
--rw-rw-r--   0 bc        (1000) bc        (1000)     1236 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/base.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1909 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/com.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      359 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/con.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1468 2022-07-07 04:32:27.000000 dicopp-1.0.35/dicopp/daem.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1553 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/details.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     2640 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/dload.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1429 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/extension.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      688 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/first.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1976 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/flist.py
--rw-rw-r--   0 bc        (1000) bc        (1000)    31289 2023-04-21 19:16:29.000000 dicopp-1.0.35/dicopp/hublist.xml.gz.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     4382 2023-04-21 19:22:44.000000 dicopp-1.0.35/dicopp/hubs.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1195 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/hubscon.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1519 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/hubson.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1436 2022-05-05 03:24:34.000000 dicopp-1.0.35/dicopp/layout.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1323 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/limit.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1028 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/log.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      994 2022-05-07 04:49:33.000000 dicopp-1.0.35/dicopp/main.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      895 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/nick.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      205 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/overrides.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      980 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/reqs.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     4641 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/search.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1374 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/sets.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      612 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/share.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1503 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/stor2.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      661 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/userinfo.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1514 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/users.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      540 2022-01-31 07:04:25.000000 dicopp-1.0.35/dicopp/usersloc.py
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-04-21 19:29:24.593887 dicopp-1.0.35/dicopp.egg-info/
--rw-rw-r--   0 bc        (1000) bc        (1000)      385 2023-04-21 19:29:23.000000 dicopp-1.0.35/dicopp.egg-info/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      649 2023-04-21 19:29:24.000000 dicopp-1.0.35/dicopp.egg-info/SOURCES.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        1 2023-04-21 19:29:23.000000 dicopp-1.0.35/dicopp.egg-info/dependency_links.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       44 2023-04-21 19:29:23.000000 dicopp-1.0.35/dicopp.egg-info/entry_points.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       60 2023-04-21 19:29:23.000000 dicopp-1.0.35/dicopp.egg-info/requires.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        7 2023-04-21 19:29:23.000000 dicopp-1.0.35/dicopp.egg-info/top_level.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       38 2023-04-21 19:29:24.593887 dicopp-1.0.35/setup.cfg
--rw-rw-r--   0 bc        (1000) bc        (1000)      884 2023-04-21 19:22:44.000000 dicopp-1.0.35/setup.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-05-12 13:08:08.645580 dicopp-1.0.36/
+-rw-rw-r--   0 bc        (1000) bc        (1000)       30 2023-05-12 11:46:51.000000 dicopp-1.0.36/MANIFEST.in
+-rw-rw-r--   0 bc        (1000) bc        (1000)      385 2023-05-12 13:08:08.645580 dicopp-1.0.36/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      894 2023-03-23 11:57:18.000000 dicopp-1.0.36/README.md
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-05-12 13:08:08.629580 dicopp-1.0.36/dicopp/
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1236 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/base.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1909 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/com.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      359 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/con.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1468 2022-07-07 04:32:27.000000 dicopp-1.0.36/dicopp/daem.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1553 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/details.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2640 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/dload.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1429 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/extension.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      688 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/first.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1976 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/flist.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)    29689 2023-05-12 11:12:57.000000 dicopp-1.0.36/dicopp/hublist.xml.gz
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4379 2023-05-12 11:46:51.000000 dicopp-1.0.36/dicopp/hubs.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1195 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/hubscon.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1519 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/hubson.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1436 2022-05-05 03:24:34.000000 dicopp-1.0.36/dicopp/layout.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1323 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/limit.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1028 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/log.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      994 2022-05-07 04:49:33.000000 dicopp-1.0.36/dicopp/main.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      895 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/nick.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      205 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/overrides.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      980 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/reqs.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4641 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/search.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1374 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/sets.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      612 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/share.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1503 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/stor2.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      661 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/userinfo.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1514 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/users.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      540 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/usersloc.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-05-12 13:08:08.641580 dicopp-1.0.36/dicopp.egg-info/
+-rw-rw-r--   0 bc        (1000) bc        (1000)      385 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      658 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/SOURCES.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        1 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/dependency_links.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       44 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/entry_points.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       60 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/requires.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        7 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/top_level.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       38 2023-05-12 13:08:08.645580 dicopp-1.0.36/setup.cfg
+-rw-rw-r--   0 bc        (1000) bc        (1000)      912 2023-05-12 11:46:51.000000 dicopp-1.0.36/setup.py
```

### Comparing `dicopp-1.0.35/README.md` & `dicopp-1.0.36/README.md`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/base.py` & `dicopp-1.0.36/dicopp/base.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/com.py` & `dicopp-1.0.36/dicopp/com.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/daem.py` & `dicopp-1.0.36/dicopp/daem.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/details.py` & `dicopp-1.0.36/dicopp/details.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/dload.py` & `dicopp-1.0.36/dicopp/dload.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/extension.py` & `dicopp-1.0.36/dicopp/extension.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/first.py` & `dicopp-1.0.36/dicopp/first.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/flist.py` & `dicopp-1.0.36/dicopp/flist.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/hubs.py` & `dicopp-1.0.36/dicopp/hubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 			if file.get_text():
 				tree = ET.parse(file.get_text())
 				root = tree.getroot()
 			else:
 				#if the module has never been imported before (== not present in sys.modules), then it is loaded and added to sys.modules.
 				import gzip
 				import os.path
-				with gzip.open(os.path.join(os.path.dirname(__file__),'hublist.xml.gz.py'), mode='r') as zipfile:
+				with gzip.open(os.path.join(os.path.dirname(__file__),'hublist.xml.gz'), mode='r') as zipfile:
 					root = ET.fromstring(zipfile.read())
 		ini_result(root)
 	return False
 def ini_result(root):
 	try:
 		hbs=root.find("Hubs").findall("Hub")
 	except Exception:
```

### Comparing `dicopp-1.0.35/dicopp/hubscon.py` & `dicopp-1.0.36/dicopp/hubscon.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/hubson.py` & `dicopp-1.0.36/dicopp/hubson.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/layout.py` & `dicopp-1.0.36/dicopp/layout.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/limit.py` & `dicopp-1.0.36/dicopp/limit.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/log.py` & `dicopp-1.0.36/dicopp/log.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/main.py` & `dicopp-1.0.36/dicopp/main.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/nick.py` & `dicopp-1.0.36/dicopp/nick.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/reqs.py` & `dicopp-1.0.36/dicopp/reqs.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/search.py` & `dicopp-1.0.36/dicopp/search.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/sets.py` & `dicopp-1.0.36/dicopp/sets.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/share.py` & `dicopp-1.0.36/dicopp/share.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/stor2.py` & `dicopp-1.0.36/dicopp/stor2.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/userinfo.py` & `dicopp-1.0.36/dicopp/userinfo.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/users.py` & `dicopp-1.0.36/dicopp/users.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp/usersloc.py` & `dicopp-1.0.36/dicopp/usersloc.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.35/dicopp.egg-info/SOURCES.txt` & `dicopp-1.0.36/dicopp.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+MANIFEST.in
 README.md
 setup.py
 dicopp/base.py
 dicopp/com.py
 dicopp/con.py
 dicopp/daem.py
 dicopp/details.py
 dicopp/dload.py
 dicopp/extension.py
 dicopp/first.py
 dicopp/flist.py
-dicopp/hublist.xml.gz.py
+dicopp/hublist.xml.gz
 dicopp/hubs.py
 dicopp/hubscon.py
 dicopp/hubson.py
 dicopp/layout.py
 dicopp/limit.py
 dicopp/log.py
 dicopp/main.py
```

### Comparing `dicopp-1.0.35/setup.py` & `dicopp-1.0.36/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from setuptools import setup
 setup(name=pkname,
 	packages=[pkname],
 	#data_files = [('', [pkname+'/hublist.xml.gz'])], #still is not placing it in the same folder
 	version=ver,
 	#opt
+	include_package_data=True,
 	python_requires='>=3',
 	install_requires=["PyGObject>=3.40","requests>=2.21","appdirs>=1.4.3",\
 		"psutil>=5.5.1"],
 	description='Direct Connect ++ client',
 	long_description=README,
 	long_description_content_type="text/markdown",
 	url='https://github.com/colin-i/dico',
```


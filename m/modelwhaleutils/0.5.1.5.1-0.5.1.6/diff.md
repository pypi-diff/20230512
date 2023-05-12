# Comparing `tmp/modelwhaleutils-0.5.1.5.1.tar.gz` & `tmp/modelwhaleutils-0.5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modelwhaleutils-0.5.1.5.1.tar", last modified: Wed May 10 07:03:47 2023, max compression
+gzip compressed data, was "dist/modelwhaleutils-0.5.1.6.tar", last modified: Fri May 12 06:10:37 2023, max compression
```

## Comparing `modelwhaleutils-0.5.1.5.1.tar` & `modelwhaleutils-0.5.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/
--rw-r--r--   0 YiranTao   (502) staff       (20)      383 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/PKG-INFO
--rw-r--r--   0 YiranTao   (502) staff       (20)     3078 2021-04-16 07:51:27.000000 modelwhaleutils-0.5.1.5.1/README.md
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/modelwhaleutils.egg-info/
--rw-r--r--   0 YiranTao   (502) staff       (20)      383 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/modelwhaleutils.egg-info/PKG-INFO
--rw-r--r--   0 YiranTao   (502) staff       (20)      360 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/modelwhaleutils.egg-info/SOURCES.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)        1 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/modelwhaleutils.egg-info/dependency_links.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)       35 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/modelwhaleutils.egg-info/requires.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)        8 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/modelwhaleutils.egg-info/top_level.txt
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/mwutils/
--rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/__init__.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     1580 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/keras.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     4410 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/logs.py
--rw-r--r--   0 YiranTao   (502) staff       (20)    22754 2023-05-06 08:16:09.000000 modelwhaleutils-0.5.1.5.1/mwutils/run.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     6284 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/sys_stat.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     1163 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/tf_utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)      562 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/torch_utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.5.1/mwutils/utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)       38 2023-05-10 07:03:47.000000 modelwhaleutils-0.5.1.5.1/setup.cfg
--rw-r--r--   0 YiranTao   (502) staff       (20)      514 2023-05-10 07:03:45.000000 modelwhaleutils-0.5.1.5.1/setup.py
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/
+-rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/PKG-INFO
+-rw-r--r--   0 YiranTao   (502) staff       (20)     3078 2021-04-16 07:51:27.000000 modelwhaleutils-0.5.1.6/README.md
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/
+-rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/PKG-INFO
+-rw-r--r--   0 YiranTao   (502) staff       (20)      360 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/SOURCES.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)        1 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/dependency_links.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)       35 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/requires.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)        8 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/top_level.txt
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/mwutils/
+-rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/__init__.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     1580 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/keras.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     4410 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/logs.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)    22758 2023-05-12 06:09:49.000000 modelwhaleutils-0.5.1.6/mwutils/run.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     6284 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/sys_stat.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     1163 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/tf_utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)      562 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/torch_utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)       38 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/setup.cfg
+-rw-r--r--   0 YiranTao   (502) staff       (20)      512 2023-05-12 06:09:57.000000 modelwhaleutils-0.5.1.6/setup.py
```

### Comparing `modelwhaleutils-0.5.1.5.1/README.md` & `modelwhaleutils-0.5.1.6/README.md`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.5.1/mwutils/keras.py` & `modelwhaleutils-0.5.1.6/mwutils/keras.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.5.1/mwutils/logs.py` & `modelwhaleutils-0.5.1.6/mwutils/logs.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.5.1/mwutils/run.py` & `modelwhaleutils-0.5.1.6/mwutils/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,15 @@
                                          region_name=region,
                                          aws_access_key_id=AK,
                                          aws_secret_access_key=SK,
                                          aws_session_token=Session
                                          )
                 if oss_config["host"] != "":
                     s3_client = boto3.client('s3',
-                                             endpoint=oss_config["host"],
+                                             endpoint_url=oss_config["host"],
                                              region_name=region,
                                              aws_access_key_id=AK,
                                              aws_secret_access_key=SK,
                                              aws_session_token=Session
                                              )
 
                 upload_dir = _path
```

### Comparing `modelwhaleutils-0.5.1.5.1/mwutils/sys_stat.py` & `modelwhaleutils-0.5.1.6/mwutils/sys_stat.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.5.1/mwutils/tf_utils.py` & `modelwhaleutils-0.5.1.6/mwutils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.5.1/mwutils/torch_utils.py` & `modelwhaleutils-0.5.1.6/mwutils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.5.1/setup.py` & `modelwhaleutils-0.5.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="modelwhaleutils",
-    version="0.5.1.5.1",
+    version="0.5.1.6",
     author="modalwhale team",
     description="use in mw",
     url="https://github.com/Kesci/modelwhaleutils",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```


# Comparing `tmp/opendatalab-0.0.7.tar.gz` & `tmp/opendatalab-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatalab-0.0.7.tar", last modified: Fri Apr 28 08:06:44 2023, max compression
+gzip compressed data, was "opendatalab-0.0.8.tar", last modified: Fri May 12 09:38:57 2023, max compression
```

## Comparing `opendatalab-0.0.7.tar` & `opendatalab-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 08:06:44.062734 opendatalab-0.0.7/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1078 2023-02-23 08:14:20.000000 opendatalab-0.0.7/LICENSE
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6129 2023-04-28 08:06:44.062734 opendatalab-0.0.7/PKG-INFO
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     5014 2023-04-18 05:57:49.000000 opendatalab-0.0.7/README.md
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 08:06:44.058734 opendatalab-0.0.7/opendatalab/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      295 2023-03-06 07:19:58.000000 opendatalab-0.0.7/opendatalab/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      391 2023-04-28 08:06:39.000000 opendatalab-0.0.7/opendatalab/__version__.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 08:06:44.058734 opendatalab-0.0.7/opendatalab/cli/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      137 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/cli/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4515 2023-03-22 05:51:23.000000 opendatalab-0.0.7/opendatalab/cli/cmd.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      762 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/cli/config.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1618 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/cli/custom.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     5607 2023-04-28 07:50:03.000000 opendatalab-0.0.7/opendatalab/cli/get.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3100 2023-02-23 08:15:29.000000 opendatalab-0.0.7/opendatalab/cli/info.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      589 2023-03-06 10:56:03.000000 opendatalab-0.0.7/opendatalab/cli/login.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      620 2023-02-23 08:15:29.000000 opendatalab-0.0.7/opendatalab/cli/logout.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1986 2023-03-08 08:53:00.000000 opendatalab-0.0.7/opendatalab/cli/ls.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      150 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/cli/policy.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3775 2023-04-20 05:33:58.000000 opendatalab-0.0.7/opendatalab/cli/search.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4776 2023-04-06 08:11:36.000000 opendatalab-0.0.7/opendatalab/cli/upgrade.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4941 2023-04-11 09:43:56.000000 opendatalab-0.0.7/opendatalab/cli/utility.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 08:06:44.062734 opendatalab-0.0.7/opendatalab/client/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      264 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/client/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)    11070 2023-04-28 08:02:54.000000 opendatalab-0.0.7/opendatalab/client/api.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1224 2023-03-06 09:18:13.000000 opendatalab-0.0.7/opendatalab/client/client.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)    13852 2023-04-20 06:16:53.000000 opendatalab-0.0.7/opendatalab/client/downloader.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3579 2023-03-06 09:57:42.000000 opendatalab-0.0.7/opendatalab/client/uaa.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 08:06:44.062734 opendatalab-0.0.7/opendatalab/dataset/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      224 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/dataset/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      772 2023-03-06 09:18:08.000000 opendatalab-0.0.7/opendatalab/dataset/dataset.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1416 2023-02-23 08:15:29.000000 opendatalab-0.0.7/opendatalab/exception.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       65 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/py.typed
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     2495 2023-02-23 08:14:20.000000 opendatalab-0.0.7/opendatalab/utils.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 08:06:44.058734 opendatalab-0.0.7/opendatalab.egg-info/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6129 2023-04-28 08:06:44.000000 opendatalab-0.0.7/opendatalab.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      903 2023-04-28 08:06:44.000000 opendatalab-0.0.7/opendatalab.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        1 2023-04-28 08:06:44.000000 opendatalab-0.0.7/opendatalab.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       48 2023-04-28 08:06:44.000000 opendatalab-0.0.7/opendatalab.egg-info/entry_points.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      102 2023-04-28 08:06:44.000000 opendatalab-0.0.7/opendatalab.egg-info/requires.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       12 2023-04-28 08:06:44.000000 opendatalab-0.0.7/opendatalab.egg-info/top_level.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1295 2023-04-28 08:06:44.062734 opendatalab-0.0.7/setup.cfg
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      486 2023-03-06 11:46:16.000000 opendatalab-0.0.7/setup.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-05-12 09:38:57.272763 opendatalab-0.0.8/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1078 2023-02-23 08:14:20.000000 opendatalab-0.0.8/LICENSE
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6129 2023-05-12 09:38:57.272763 opendatalab-0.0.8/PKG-INFO
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     5014 2023-04-18 05:57:49.000000 opendatalab-0.0.8/README.md
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-05-12 09:38:57.268763 opendatalab-0.0.8/opendatalab/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      295 2023-03-06 07:19:58.000000 opendatalab-0.0.8/opendatalab/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      391 2023-05-11 07:21:23.000000 opendatalab-0.0.8/opendatalab/__version__.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-05-12 09:38:57.272763 opendatalab-0.0.8/opendatalab/cli/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      137 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/cli/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4515 2023-03-22 05:51:23.000000 opendatalab-0.0.8/opendatalab/cli/cmd.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      762 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/cli/config.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1618 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/cli/custom.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6228 2023-05-12 09:36:08.000000 opendatalab-0.0.8/opendatalab/cli/get.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3100 2023-02-23 08:15:29.000000 opendatalab-0.0.8/opendatalab/cli/info.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      589 2023-03-06 10:56:03.000000 opendatalab-0.0.8/opendatalab/cli/login.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      620 2023-02-23 08:15:29.000000 opendatalab-0.0.8/opendatalab/cli/logout.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1986 2023-03-08 08:53:00.000000 opendatalab-0.0.8/opendatalab/cli/ls.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      150 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/cli/policy.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3775 2023-04-20 05:33:58.000000 opendatalab-0.0.8/opendatalab/cli/search.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4776 2023-04-06 08:11:36.000000 opendatalab-0.0.8/opendatalab/cli/upgrade.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4941 2023-04-11 09:43:56.000000 opendatalab-0.0.8/opendatalab/cli/utility.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-05-12 09:38:57.272763 opendatalab-0.0.8/opendatalab/client/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      264 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/client/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)    11070 2023-04-28 08:02:54.000000 opendatalab-0.0.8/opendatalab/client/api.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1224 2023-03-06 09:18:13.000000 opendatalab-0.0.8/opendatalab/client/client.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)    13852 2023-04-20 06:16:53.000000 opendatalab-0.0.8/opendatalab/client/downloader.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3579 2023-03-06 09:57:42.000000 opendatalab-0.0.8/opendatalab/client/uaa.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-05-12 09:38:57.272763 opendatalab-0.0.8/opendatalab/dataset/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      224 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/dataset/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      772 2023-03-06 09:18:08.000000 opendatalab-0.0.8/opendatalab/dataset/dataset.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1416 2023-02-23 08:15:29.000000 opendatalab-0.0.8/opendatalab/exception.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       65 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/py.typed
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     2495 2023-02-23 08:14:20.000000 opendatalab-0.0.8/opendatalab/utils.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-05-12 09:38:57.268763 opendatalab-0.0.8/opendatalab.egg-info/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6129 2023-05-12 09:38:57.000000 opendatalab-0.0.8/opendatalab.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      903 2023-05-12 09:38:57.000000 opendatalab-0.0.8/opendatalab.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        1 2023-05-12 09:38:57.000000 opendatalab-0.0.8/opendatalab.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       48 2023-05-12 09:38:57.000000 opendatalab-0.0.8/opendatalab.egg-info/entry_points.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      102 2023-05-12 09:38:57.000000 opendatalab-0.0.8/opendatalab.egg-info/requires.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       12 2023-05-12 09:38:57.000000 opendatalab-0.0.8/opendatalab.egg-info/top_level.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1295 2023-05-12 09:38:57.272763 opendatalab-0.0.8/setup.cfg
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      486 2023-03-06 11:46:16.000000 opendatalab-0.0.8/setup.py
```

### Comparing `opendatalab-0.0.7/LICENSE` & `opendatalab-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/PKG-INFO` & `opendatalab-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatalab
-Version: 0.0.7
+Version: 0.0.8
 Summary: OpenDataLab Python SDK
 Home-page: https://github.com/opendatalab/opendatalab-python-sdk
 Author: OpenDataLab
 Author-email: OpenDataLab@pjlab.org.cn
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opendatalab/opendatalab-python-sdk/issues
 Keywords: opendatalab,dataset,test
```

### Comparing `opendatalab-0.0.7/README.md` & `opendatalab-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/cmd.py` & `opendatalab-0.0.8/opendatalab/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/config.py` & `opendatalab-0.0.8/opendatalab/cli/config.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/custom.py` & `opendatalab-0.0.8/opendatalab/cli/custom.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/get.py` & `opendatalab-0.0.8/opendatalab/cli/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,21 +49,25 @@
     # print(name)
     ds_split = name.split("/")
     dataset_name = ds_split[0]
     if ds_split[-1] == '':
         ds_split.pop()
     single_file_flag = False
     sub_dir = "/".join(ds_split[1:])
-    if len(ds_split) > 2:
-        # if a single file
-        if ('.' in ds_split[-1]):
-            single_file_flag = True
+    
+    if ('.' in ds_split[-1]):
+        single_file_flag = True
+        if len(ds_split) == 2:
+            # indicate README.md
+            file_name = ds_split[-1]
+            sub_dir = ''
+        elif len(ds_split) > 2:
             sub_dir = "/".join(ds_split[1:-1])
-        
-    # client init    
+            file_name = sub_dir + '/' + ds_split[-1]
+                # client init
     client = obj.get_client()
     data_info = client.get_api().get_info(dataset_name)
     
     # basic info of dataset
     info_dataset_name = data_info['name']
     info_dataset_id = data_info['id']
     
@@ -80,29 +84,39 @@
         click.echo(f"Direct download for {dataset_name} is currently not available."
                    f"\nPlease visit the homepage {info_dataset_url} for more information.")
         sys.exit(1)
 
     
     dataset_res_dict = client.get_api().get_dataset_files(dataset_name=info_dataset_name,
                                                           prefix = sub_dir)
-    total_object = dataset_res_dict['total']
-
-    # obj list constuct
-    obj_info_list = []
-    for info in dataset_res_dict['list']:
-        curr_dict = {}
-        if not info['isDir']:
-            curr_dict['size'] = info['size']
-            if single_file_flag:
-                curr_dict['name'] = info['path']
-            elif len(sub_dir.split('/')) > 1:
-                curr_dict['name'] = sub_dir
-            else:
+    if not single_file_flag:
+        total_object = dataset_res_dict['total']
+        # obj list constuct
+        obj_info_list = []
+        for info in dataset_res_dict['list']:
+            curr_dict = {}
+            if not info['isDir']:
+                curr_dict['size'] = info['size']
+                if single_file_flag:
+                    curr_dict['name'] = info['path']
+                elif len(sub_dir.split('/')) > 1:
+                    # curr_dict['name'] = sub_dir
+                    curr_dict['name'] = info['path']
+                else:
+                    curr_dict['name'] = info['path']
+                obj_info_list.append(curr_dict)
+    else:
+        total_object = 1
+        obj_info_list = []
+        for info in dataset_res_dict['list']:
+            curr_dict = {}
+            if info['path'] == str(file_name):
+                curr_dict['size'] = info['size']
                 curr_dict['name'] = info['path']
-            obj_info_list.append(curr_dict)
+                obj_info_list.append(curr_dict)
 
     local_dir = destination
     
     download_data = client.get_api().get_download_record(info_dataset_name)
     has_download = download_data['hasDownload']
 
     if not has_download:
```

### Comparing `opendatalab-0.0.7/opendatalab/cli/info.py` & `opendatalab-0.0.8/opendatalab/cli/info.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/login.py` & `opendatalab-0.0.8/opendatalab/cli/login.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/logout.py` & `opendatalab-0.0.8/opendatalab/cli/logout.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/ls.py` & `opendatalab-0.0.8/opendatalab/cli/ls.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/search.py` & `opendatalab-0.0.8/opendatalab/cli/search.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/upgrade.py` & `opendatalab-0.0.8/opendatalab/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/cli/utility.py` & `opendatalab-0.0.8/opendatalab/cli/utility.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/client/api.py` & `opendatalab-0.0.8/opendatalab/client/api.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/client/client.py` & `opendatalab-0.0.8/opendatalab/client/client.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/client/downloader.py` & `opendatalab-0.0.8/opendatalab/client/downloader.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/client/uaa.py` & `opendatalab-0.0.8/opendatalab/client/uaa.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/dataset/dataset.py` & `opendatalab-0.0.8/opendatalab/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/exception.py` & `opendatalab-0.0.8/opendatalab/exception.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab/utils.py` & `opendatalab-0.0.8/opendatalab/utils.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/opendatalab.egg-info/PKG-INFO` & `opendatalab-0.0.8/opendatalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatalab
-Version: 0.0.7
+Version: 0.0.8
 Summary: OpenDataLab Python SDK
 Home-page: https://github.com/opendatalab/opendatalab-python-sdk
 Author: OpenDataLab
 Author-email: OpenDataLab@pjlab.org.cn
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opendatalab/opendatalab-python-sdk/issues
 Keywords: opendatalab,dataset,test
```

### Comparing `opendatalab-0.0.7/opendatalab.egg-info/SOURCES.txt` & `opendatalab-0.0.8/opendatalab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.7/setup.cfg` & `opendatalab-0.0.8/setup.cfg`

 * *Files identical despite different names*


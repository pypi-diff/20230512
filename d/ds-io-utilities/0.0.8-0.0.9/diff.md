# Comparing `tmp/ds-io-utilities-0.0.8.tar.gz` & `tmp/ds-io-utilities-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ds-io-utilities-0.0.8.tar", last modified: Tue Jul 12 08:07:52 2022, max compression
+gzip compressed data, was "dist/ds-io-utilities-0.0.9.tar", last modified: Tue Jul 12 11:19:21 2022, max compression
```

## Comparing `ds-io-utilities-0.0.8.tar` & `ds-io-utilities-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 08:07:52.109346 ds-io-utilities-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      422 2022-07-12 08:07:52.110346 ds-io-utilities-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 08:07:52.109346 ds-io-utilities-0.0.8/ds_io_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)      422 2022-07-12 08:07:52.000000 ds-io-utilities-0.0.8/ds_io_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-07-12 08:07:52.000000 ds-io-utilities-0.0.8/ds_io_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 08:07:52.000000 ds-io-utilities-0.0.8/ds_io_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2022-07-12 08:07:52.000000 ds-io-utilities-0.0.8/ds_io_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-07-12 08:07:52.000000 ds-io-utilities-0.0.8/ds_io_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 08:07:52.109346 ds-io-utilities-0.0.8/dsioutilities/
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 08:07:52.109346 ds-io-utilities-0.0.8/dsioutilities/tabular/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/tabular/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/tabular/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/tabular/hive.py
--rw-rw-rw-   0 root         (0) root         (0)     3007 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/tabular/minio.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/tabular/tabular.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/dsioutilities/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-07-12 08:07:52.110346 ds-io-utilities-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      640 2022-07-12 08:07:42.000000 ds-io-utilities-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 11:19:21.184274 ds-io-utilities-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      426 2022-07-12 11:19:21.184274 ds-io-utilities-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 11:19:21.183274 ds-io-utilities-0.0.9/ds_io_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      426 2022-07-12 11:19:21.000000 ds-io-utilities-0.0.9/ds_io_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2022-07-12 11:19:21.000000 ds-io-utilities-0.0.9/ds_io_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 11:19:21.000000 ds-io-utilities-0.0.9/ds_io_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2022-07-12 11:19:21.000000 ds-io-utilities-0.0.9/ds_io_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-07-12 11:19:21.000000 ds-io-utilities-0.0.9/ds_io_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 11:19:21.183274 ds-io-utilities-0.0.9/dsioutilities/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 11:19:21.184274 ds-io-utilities-0.0.9/dsioutilities/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/tabular/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/tabular/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/tabular/hive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3228 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/tabular/minio.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/tabular/tabular.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/dsioutilities/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2022-07-12 11:19:21.184274 ds-io-utilities-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      644 2022-07-12 11:19:12.000000 ds-io-utilities-0.0.9/setup.py
```

### Comparing `ds-io-utilities-0.0.8/dsioutilities/dataset.py` & `ds-io-utilities-0.0.9/dsioutilities/dataset.py`

 * *Files identical despite different names*

### Comparing `ds-io-utilities-0.0.8/dsioutilities/tabular/hive.py` & `ds-io-utilities-0.0.9/dsioutilities/tabular/hive.py`

 * *Files identical despite different names*

### Comparing `ds-io-utilities-0.0.8/dsioutilities/tabular/minio.py` & `ds-io-utilities-0.0.9/dsioutilities/tabular/minio.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,50 +23,53 @@
                                                     client_kwargs={'endpoint_url': endpoint_url},
                                                     **kw)
             print('S3FileSystem is patched with url:  ' + endpoint_url)
 
     s3fs.S3FileSystem = S3FileSystemPatched
 
 
-def minio_ls(address, access_key, secret_key, bucket_name, folder, extention):
+def minio_ls(address, access_key, secret_key, bucket_name, folder, extention, use_ssl=False):
 
     if folder[-1] != "/":
         folder = folder + "/"
 
     client = Minio(
         address,
         access_key=access_key,
-        secret_key=secret_key#,
-        #secure=False
+        secret_key=secret_key,
+        secure=use_ssl
     )
     objects = client.list_objects(bucket_name=bucket_name, prefix=folder)
 
     return [x._object_name for x in objects if extention in x._object_name[-len(extention):]]
 
 
 
+
 def get_path(name):
     
     # Get credentials
     minio_url = get_asset_property(asset_name=name, property="minIO_URL")
     access_key = get_asset_property(asset_name=name, property="minIO_ACCESS_KEY")
     secret_key = get_asset_property(asset_name=name, property="minIO_SECRET_KEY")
     bucket_name = get_asset_property(asset_name=name, property="minio_bucket")
     
     # Set connection for pandas reading
     set_connection(access_key=access_key, secret_key=secret_key, url=minio_url)
 
     if input_or_output(name) == "input":
+        use_ssl = get_asset_property(asset_name=name, property="use_ssl") if get_asset_property(asset_name=name, property="use_ssl") is not None else False
         # List all files in dataset folder
         files_list = minio_ls(address=minio_url.replace("http://", "").replace("https://", ""), 
                                 access_key=access_key, 
                                 secret_key=secret_key, 
                                 bucket_name=bucket_name, 
                                 folder=get_asset_property(name),
-                                extention=".csv")
+                                extention=".csv",
+                                use_ssl=use_ssl)
         if len(files_list) > 1:
             return ["s3://" + bucket_name + "/" + x for x in files_list]
         elif len(files_list) == 1:
             return "s3://" + bucket_name + "/" + files_list[0]
         else:
             raise Exception("Dataset is empty!")
```

### Comparing `ds-io-utilities-0.0.8/setup.py` & `ds-io-utilities-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 setuptools.setup(
     name="ds-io-utilities",
-    version="0.0.8",
+    version="0.0.9",
     author="Alida research team",
-    author_email="salvatore.cipolla@eng.it",
+    author_email="engineering-alida-lab@eng.it",
     description="Utils for datasets IO operations in Alida.",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```


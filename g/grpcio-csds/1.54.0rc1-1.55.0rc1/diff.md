# Comparing `tmp/grpcio-csds-1.54.0rc1.tar.gz` & `tmp/grpcio-csds-1.55.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-csds-1.54.0rc1.tar", last modified: Fri Mar 31 21:34:19 2023, max compression
+gzip compressed data, was "grpcio-csds-1.55.0rc1.tar", last modified: Wed Apr 26 10:35:50 2023, max compression
```

## Comparing `grpcio-csds-1.54.0rc1.tar` & `grpcio-csds-1.55.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:19.575797 grpcio-csds-1.54.0rc1/
--rw-r--r--   0 root         (0) root         (0)       94 2023-03-31 21:09:23.000000 grpcio-csds-1.54.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-31 21:34:19.575797 grpcio-csds-1.54.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-03-31 21:09:23.000000 grpcio-csds-1.54.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:19.571797 grpcio-csds-1.54.0rc1/grpc_csds/
--rw-r--r--   0 root         (0) root         (0)     2149 2023-03-31 21:09:23.000000 grpcio-csds-1.54.0rc1/grpc_csds/__init__.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-03-31 21:09:23.000000 grpcio-csds-1.54.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:19.575797 grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-31 21:34:19.000000 grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2023-03-31 21:34:19.000000 grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 21:34:19.000000 grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-31 21:34:19.000000 grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-31 21:34:19.000000 grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 21:34:19.575797 grpcio-csds-1.54.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2120 2023-03-31 21:09:23.000000 grpcio-csds-1.54.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:50.828451 grpcio-csds-1.55.0rc1/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-26 10:25:03.000000 grpcio-csds-1.55.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-26 10:35:50.828451 grpcio-csds-1.55.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-04-26 10:25:03.000000 grpcio-csds-1.55.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:50.820451 grpcio-csds-1.55.0rc1/grpc_csds/
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-04-26 10:25:03.000000 grpcio-csds-1.55.0rc1/grpc_csds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-26 10:25:03.000000 grpcio-csds-1.55.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:50.828451 grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-26 10:35:50.000000 grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-26 10:35:50.000000 grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:35:50.000000 grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-26 10:35:50.000000 grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 10:35:50.000000 grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:35:50.828451 grpcio-csds-1.55.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-26 10:25:03.000000 grpcio-csds-1.55.0rc1/setup.py
```

### Comparing `grpcio-csds-1.54.0rc1/PKG-INFO` & `grpcio-csds-1.55.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.54.0rc1
+Version: 1.55.0rc1
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-csds-1.54.0rc1/grpc_csds/__init__.py` & `grpcio-csds-1.55.0rc1/grpc_csds/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-csds-1.54.0rc1/grpcio_csds.egg-info/PKG-INFO` & `grpcio-csds-1.55.0rc1/grpcio_csds.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.54.0rc1
+Version: 1.55.0rc1
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-csds-1.54.0rc1/setup.py` & `grpcio-csds-1.55.0rc1/setup.py`

 * *Files identical despite different names*


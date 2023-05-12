# Comparing `tmp/xpublish_edr-0.1.0.tar.gz` & `tmp/xpublish_edr-0.1.dev29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish_edr-0.1.0.tar", last modified: Fri May 12 07:55:59 2023, max compression
+gzip compressed data, was "xpublish_edr-0.1.dev29.tar", last modified: Thu May 11 20:52:52 2023, max compression
```

## Comparing `xpublish_edr-0.1.0.tar` & `xpublish_edr-0.1.dev29.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:55:59.816466 xpublish_edr-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/xpublish_edr/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/xpublish_edr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 07:55:59.000000 xpublish_edr-0.1.0/xpublish_edr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/xpublish_edr/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/xpublish_edr/formats/to_covjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/xpublish_edr/formats/to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/xpublish_edr/formats/to_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/xpublish_edr/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-12 07:55:50.000000 xpublish_edr-0.1.0/xpublish_edr/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:55:59.820466 xpublish_edr-0.1.0/xpublish_edr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-12 07:55:59.000000 xpublish_edr-0.1.0/xpublish_edr.egg-info/SOURCES.txt
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.427673 xpublish_edr-0.1.dev29/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.419377 xpublish_edr-0.1.dev29/.github/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.423488 xpublish_edr-0.1.dev29/.github/workflows/
+-rw-r--r--   0 akerney    (502) staff       (20)      237 2022-07-15 20:50:57.000000 xpublish_edr-0.1.dev29/.github/workflows/pre-commit.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1766 2023-05-11 20:47:24.000000 xpublish_edr-0.1.dev29/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 akerney    (502) staff       (20)      963 2022-12-11 16:56:31.000000 xpublish_edr-0.1.dev29/.github/workflows/tests.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1472 2022-05-11 10:40:36.000000 xpublish_edr-0.1.dev29/LICENSE.txt
+-rw-r--r--   0 akerney    (502) staff       (20)      251 2023-05-11 20:51:17.000000 xpublish_edr-0.1.dev29/MANIFEST.in
+-rw-r--r--   0 akerney    (502) staff       (20)     3705 2023-05-11 20:52:52.427112 xpublish_edr-0.1.dev29/PKG-INFO
+-rw-r--r--   0 akerney    (502) staff       (20)     1309 2022-05-11 12:12:08.000000 xpublish_edr-0.1.dev29/README.md
+-rw-r--r--   0 akerney    (502) staff       (20)     1799 2023-05-11 20:51:01.000000 xpublish_edr-0.1.dev29/pyproject.toml
+-rw-r--r--   0 akerney    (502) staff       (20)      277 2022-06-14 16:26:23.000000 xpublish_edr-0.1.dev29/requirements-dev.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       38 2023-05-11 20:48:24.000000 xpublish_edr-0.1.dev29/requirements.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       38 2023-05-11 20:52:52.427803 xpublish_edr-0.1.dev29/setup.cfg
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.424976 xpublish_edr-0.1.dev29/xpublish_edr/
+-rw-r--r--   0 akerney    (502) staff       (20)      247 2023-05-11 20:46:59.000000 xpublish_edr-0.1.dev29/xpublish_edr/__init__.py
+-rw-r--r--   0 akerney    (502) staff       (20)      170 2023-05-11 20:52:52.000000 xpublish_edr-0.1.dev29/xpublish_edr/_version.py
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.426107 xpublish_edr-0.1.dev29/xpublish_edr/formats/
+-rw-r--r--   0 akerney    (502) staff       (20)     4141 2022-07-15 20:50:57.000000 xpublish_edr-0.1.dev29/xpublish_edr/formats/to_covjson.py
+-rw-r--r--   0 akerney    (502) staff       (20)      424 2022-07-15 20:43:58.000000 xpublish_edr-0.1.dev29/xpublish_edr/formats/to_csv.py
+-rw-r--r--   0 akerney    (502) staff       (20)      616 2022-07-15 20:43:58.000000 xpublish_edr-0.1.dev29/xpublish_edr/formats/to_netcdf.py
+-rw-r--r--   0 akerney    (502) staff       (20)     5125 2023-05-11 20:46:59.000000 xpublish_edr-0.1.dev29/xpublish_edr/plugin.py
+-rw-r--r--   0 akerney    (502) staff       (20)     1956 2022-07-15 20:43:58.000000 xpublish_edr-0.1.dev29/xpublish_edr/query.py
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.426490 xpublish_edr-0.1.dev29/xpublish_edr.egg-info/
+-rw-r--r--   0 akerney    (502) staff       (20)      380 2023-05-11 20:52:52.000000 xpublish_edr-0.1.dev29/xpublish_edr.egg-info/SOURCES.txt
```

### Comparing `xpublish_edr-0.1.0/.github/workflows/publish-to-pypi.yml` & `xpublish_edr-0.1.dev29/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.0/LICENSE.txt` & `xpublish_edr-0.1.dev29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.0/PKG-INFO` & `xpublish_edr-0.1.dev29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpublish_edr
-Version: 0.1.0
+Version: 0.1.dev29
 License: Copyright 2017 AUTHOR NAME
         
         
         Redistribution and use in source and binary forms,
         with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `xpublish_edr-0.1.0/README.md` & `xpublish_edr-0.1.dev29/README.md`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.0/pyproject.toml` & `xpublish_edr-0.1.dev29/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -34,24 +34,25 @@
 csv = "xpublish_edr.formats.to_csv:to_csv"
 nc = "xpublish_edr.formats.to_netcdf:to_netcdf"
 netcdf = "xpublish_edr.formats.to_netcdf:to_netcdf"
 nc4 = "xpublish_edr.formats.to_netcdf:to_netcdf"
 netcdf4 = "xpublish_edr.formats.to_netcdf:to_netcdf"
 
 [tool.check-manifest]
-ignore = ["xpublish_edr/_version.py"]
+ignore = ["xpublish_opendap/_version.py"]
 
 [tool.setuptools]
 packages = ["xpublish_edr"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools_scm]
 write_to = "xpublish_edr/_version.py"
+local_scheme = "no-local-version"
 
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
```

### Comparing `xpublish_edr-0.1.0/xpublish_edr/formats/to_covjson.py` & `xpublish_edr-0.1.dev29/xpublish_edr/formats/to_covjson.py`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.0/xpublish_edr/formats/to_netcdf.py` & `xpublish_edr-0.1.dev29/xpublish_edr/formats/to_netcdf.py`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.0/xpublish_edr/plugin.py` & `xpublish_edr-0.1.dev29/xpublish_edr/plugin.py`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.0/xpublish_edr/query.py` & `xpublish_edr-0.1.dev29/xpublish_edr/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,36 +40,30 @@
         None,
         title="Z axis",
         description="Height or depth of query",
     ),
     datetime: Optional[str] = Query(
         None,
         title="Datetime or datetime range",
-        description=(
-            "Query by a single ISO time or a range of ISO times. "
-            "To query by a range, split the times with a slash"
-        ),
+        description="Query by a single ISO time or a range of ISO times. To query by a range, split the times with a slash",
     ),
     parameters: Optional[str] = Query(
         None,
         alias="parameter-name",
         description="xarray variables to query",
     ),
     crs: Optional[str] = Query(
         None,
         deprecated=True,
         description="CRS is not yet implemented",
     ),
     f: Optional[str] = Query(
         None,
         title="Response format",
-        description=(
-            "Data is returned as a CoverageJSON by default. "
-            "Get `/formats` to discover what other formats are accessible"
-        ),
+        description="Data is returned as a CoverageJSON by default. Get `/formats` to discover what other formats are accessible",
     ),
 ):
     """Extract EDR query params from request query strings"""
     return EDRQuery(
         coords=coords,
         z=z,
         datetime=datetime,
```


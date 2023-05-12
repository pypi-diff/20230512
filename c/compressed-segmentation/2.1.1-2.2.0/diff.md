# Comparing `tmp/compressed_segmentation-2.1.1.tar.gz` & `tmp/compressed_segmentation-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressed_segmentation-2.1.1.tar", last modified: Sun Jan 23 05:57:35 2022, max compression
+gzip compressed data, was "compressed_segmentation-2.2.0.tar", last modified: Wed Mar 16 03:47:11 2022, max compression
```

## Comparing `compressed_segmentation-2.1.1.tar` & `compressed_segmentation-2.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.810910 compressed_segmentation-2.1.1/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.802874 compressed_segmentation-2.1.1/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.806889 compressed_segmentation-2.1.1/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      949 2021-12-28 19:43:59.000000 compressed_segmentation-2.1.1/.github/workflows/build_wheel.yml
--rw-r--r--   0 wms        (501) staff       (20)      877 2021-12-28 19:43:59.000000 compressed_segmentation-2.1.1/.github/workflows/run_tests.yaml
--rw-r--r--   0 wms        (501) staff       (20)      146 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     3415 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/CMakeLists.txt
--rw-r--r--   0 wms        (501) staff       (20)     2601 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    11359 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/LICENSE.txt
--rw-r--r--   0 wms        (501) staff       (20)     1582 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/LICENSE_JANELIA.txt
--rw-r--r--   0 wms        (501) staff       (20)     1726 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/LICENSE_PYTHON.txt
--rw-r--r--   0 wms        (501) staff       (20)      140 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     4763 2022-01-23 05:57:35.811016 compressed_segmentation-2.1.1/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     3711 2021-12-30 04:41:38.000000 compressed_segmentation-2.1.1/README.md
--rw-r--r--   0 wms        (501) staff       (20)     5349 2022-01-23 05:54:14.000000 compressed_segmentation-2.1.1/automated_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)      603 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/build_linux.sh
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.808189 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     4763 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1013 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       40 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 00:54:55.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       19 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       24 2022-01-23 05:57:35.000000 compressed_segmentation-2.1.1/compressed_segmentation.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.808476 compressed_segmentation-2.1.1/cseg_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2021-12-28 19:43:59.000000 compressed_segmentation-2.1.1/cseg_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     3669 2021-12-28 19:43:59.000000 compressed_segmentation-2.1.1/cseg_cli/cli.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.808761 compressed_segmentation-2.1.1/include/
--rw-r--r--   0 wms        (501) staff       (20)     4216 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/include/compress_segmentation.h
--rw-r--r--   0 wms        (501) staff       (20)     2085 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/include/decompress_segmentation.h
--rw-r--r--   0 wms        (501) staff       (20)     1188 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/manylinux1.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1220 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/manylinux2010.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1460 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/manylinux2014.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1632 2021-01-11 02:45:21.000000 compressed_segmentation-2.1.1/perf.py
--rw-r--r--   0 wms        (501) staff       (20)       82 2021-12-28 19:43:59.000000 compressed_segmentation-2.1.1/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)       18 2021-12-28 19:43:59.000000 compressed_segmentation-2.1.1/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)      955 2022-01-23 05:57:35.811704 compressed_segmentation-2.1.1/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      993 2022-01-23 05:55:10.000000 compressed_segmentation-2.1.1/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-01-23 05:57:35.810655 compressed_segmentation-2.1.1/src/
--rw-r--r--   0 wms        (501) staff       (20)    10360 2021-12-30 04:08:11.000000 compressed_segmentation-2.1.1/src/compress_segmentation.cc
--rw-r--r--   0 wms        (501) staff       (20)     7984 2021-12-28 01:15:34.000000 compressed_segmentation-2.1.1/src/compress_segmentation_test.cc
--rw-r--r--   0 wms        (501) staff       (20)  1312863 2022-01-23 05:54:14.000000 compressed_segmentation-2.1.1/src/compressed_segmentation.cpp
--rw-r--r--   0 wms        (501) staff       (20)    11349 2022-01-23 05:54:14.000000 compressed_segmentation-2.1.1/src/compressed_segmentation.pyx
--rw-r--r--   0 wms        (501) staff       (20)     4910 2021-12-30 05:33:48.000000 compressed_segmentation-2.1.1/src/decompress_segmentation.cc
--rw-r--r--   0 wms        (501) staff       (20)     2671 2021-12-28 01:15:34.000000 compressed_segmentation-2.1.1/src/decompress_segmentation_test.cc
--rw-r--r--   0 wms        (501) staff       (20)      134 2022-01-23 05:42:57.000000 compressed_segmentation-2.1.1/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.264525 compressed_segmentation-2.2.0/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.257610 compressed_segmentation-2.2.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.260767 compressed_segmentation-2.2.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      949 2021-12-28 19:43:59.000000 compressed_segmentation-2.2.0/.github/workflows/build_wheel.yml
+-rw-r--r--   0 wms        (501) staff       (20)      877 2021-12-28 19:43:59.000000 compressed_segmentation-2.2.0/.github/workflows/run_tests.yaml
+-rw-r--r--   0 wms        (501) staff       (20)      146 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3415 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/CMakeLists.txt
+-rw-r--r--   0 wms        (501) staff       (20)     2684 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    11359 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/LICENSE.txt
+-rw-r--r--   0 wms        (501) staff       (20)     1582 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/LICENSE_JANELIA.txt
+-rw-r--r--   0 wms        (501) staff       (20)     1726 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/LICENSE_PYTHON.txt
+-rw-r--r--   0 wms        (501) staff       (20)      140 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     4910 2022-03-16 03:47:11.264649 compressed_segmentation-2.2.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     3858 2022-03-16 03:42:28.000000 compressed_segmentation-2.2.0/README.md
+-rw-r--r--   0 wms        (501) staff       (20)     6082 2022-03-16 03:41:35.000000 compressed_segmentation-2.2.0/automated_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)      603 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/build_linux.sh
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.261907 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     4910 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1013 2022-03-16 03:47:11.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       40 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 00:54:55.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       19 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       24 2022-03-16 03:47:10.000000 compressed_segmentation-2.2.0/compressed_segmentation.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.262169 compressed_segmentation-2.2.0/cseg_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2021-12-28 19:43:59.000000 compressed_segmentation-2.2.0/cseg_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     3669 2021-12-28 19:43:59.000000 compressed_segmentation-2.2.0/cseg_cli/cli.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.262436 compressed_segmentation-2.2.0/include/
+-rw-r--r--   0 wms        (501) staff       (20)     4216 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/include/compress_segmentation.h
+-rw-r--r--   0 wms        (501) staff       (20)     2085 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/include/decompress_segmentation.h
+-rw-r--r--   0 wms        (501) staff       (20)     1188 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/manylinux1.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1220 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/manylinux2010.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1460 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/manylinux2014.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1632 2021-01-11 02:45:21.000000 compressed_segmentation-2.2.0/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)       82 2021-12-28 19:43:59.000000 compressed_segmentation-2.2.0/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)       18 2021-12-28 19:43:59.000000 compressed_segmentation-2.2.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)      955 2022-03-16 03:47:11.265160 compressed_segmentation-2.2.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      993 2022-01-23 05:55:10.000000 compressed_segmentation-2.2.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-03-16 03:47:11.264390 compressed_segmentation-2.2.0/src/
+-rw-r--r--   0 wms        (501) staff       (20)    10360 2021-12-30 04:08:11.000000 compressed_segmentation-2.2.0/src/compress_segmentation.cc
+-rw-r--r--   0 wms        (501) staff       (20)     7984 2021-12-28 01:15:34.000000 compressed_segmentation-2.2.0/src/compress_segmentation_test.cc
+-rw-r--r--   0 wms        (501) staff       (20)  1393592 2022-03-16 03:41:35.000000 compressed_segmentation-2.2.0/src/compressed_segmentation.cpp
+-rw-r--r--   0 wms        (501) staff       (20)    13011 2022-03-16 03:44:46.000000 compressed_segmentation-2.2.0/src/compressed_segmentation.pyx
+-rw-r--r--   0 wms        (501) staff       (20)     4910 2021-12-30 05:33:48.000000 compressed_segmentation-2.2.0/src/decompress_segmentation.cc
+-rw-r--r--   0 wms        (501) staff       (20)     2671 2021-12-28 01:15:34.000000 compressed_segmentation-2.2.0/src/decompress_segmentation_test.cc
+-rw-r--r--   0 wms        (501) staff       (20)      130 2022-01-23 05:59:24.000000 compressed_segmentation-2.2.0/tox.ini
```

### Comparing `compressed_segmentation-2.1.1/.github/workflows/build_wheel.yml` & `compressed_segmentation-2.2.0/.github/workflows/build_wheel.yml`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/.github/workflows/run_tests.yaml` & `compressed_segmentation-2.2.0/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/CMakeLists.txt` & `compressed_segmentation-2.2.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/ChangeLog` & `compressed_segmentation-2.2.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 CHANGES
 =======
 
+2.2.0
+-----
+
+* docs: update date
+* docs: show how to use remap
+* feat: remap (#9)
+
 2.1.1
 -----
 
 * install: ensure windows compiles in release mode
 * fix: empty random access (#8)
+* chore: update TROVE identifiers
 
 2.1.0
 -----
 
-* chore: update TROVE identifiers
 * fix: add bounds check for get
 * fix: missing x offset in bitpos
 * refactor: change volume\_size to shape
 * docs: add highlights
 * docs: show how to use CompressedSegmentationArray
 * fix: add default block size to constructor
 * feat: adds CompressedSegmentationArray class for random access to voxels
```

### Comparing `compressed_segmentation-2.1.1/LICENSE.txt` & `compressed_segmentation-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/LICENSE_JANELIA.txt` & `compressed_segmentation-2.2.0/LICENSE_JANELIA.txt`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/LICENSE_PYTHON.txt` & `compressed_segmentation-2.2.0/LICENSE_PYTHON.txt`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/PKG-INFO` & `compressed_segmentation-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressed_segmentation
-Version: 2.1.1
+Version: 2.2.0
 Summary: Neuroglancer compressed_segmentation codec.
 Home-page: https://github.com/janelia-flyem/compressedseg
 Author: Jeremy Maitin-Shepard, Stephen Plaza, and William Silversmith
 Author-email: ws9@princeton.edu
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,15 @@
 )
 
 arr = CompressedSegmentationArray(
     compressed, shape=(sx,sy,sz), dtype=dtype
 )
 label = arr[54,32,103] # random access to single voxels w/o decompressing
 uniq_labels = arr.labels() # get all distinct values w/o decompressing
+binary2 = arr.remap({ 1: 2 }, preserve_missing_labels=False) # remap labels in segmentation w/o decompressing
 recovered = arr.numpy() # decompress to a numpy array, same as decompress
 124213 in arr # test if a value is in the array
 ```
 
 ```bash
 cseg compress connectomics.npy
 cseg decompress connectomics.npy.cseg --volume-size 512,512,512 --bytes 4
@@ -66,14 +67,15 @@
 
 
 ### Features
 
 * Compression and decompression
 * Random access to voxels without decompression
 * Read out unique values without decompression
+* Remap labels without decompression
 * Command line interface for numpy files
 * (TBD) Interface to relabel and manipulate segmentation from the compressed data
 * C++, Python, and Go interface (see original repo for Golang)
 
 ### C++ Compilation
 
 Compiling as a shared library. Feel free to subsititute e.g. clang for the C++ compiler.
```

### Comparing `compressed_segmentation-2.1.1/README.md` & `compressed_segmentation-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 
 arr = CompressedSegmentationArray(
     compressed, shape=(sx,sy,sz), dtype=dtype
 )
 label = arr[54,32,103] # random access to single voxels w/o decompressing
 uniq_labels = arr.labels() # get all distinct values w/o decompressing
+binary2 = arr.remap({ 1: 2 }, preserve_missing_labels=False) # remap labels in segmentation w/o decompressing
 recovered = arr.numpy() # decompress to a numpy array, same as decompress
 124213 in arr # test if a value is in the array
 ```
 
 ```bash
 cseg compress connectomics.npy
 cseg decompress connectomics.npy.cseg --volume-size 512,512,512 --bytes 4
@@ -39,14 +40,15 @@
 
 
 ### Features
 
 * Compression and decompression
 * Random access to voxels without decompression
 * Read out unique values without decompression
+* Remap labels without decompression
 * Command line interface for numpy files
 * (TBD) Interface to relabel and manipulate segmentation from the compressed data
 * C++, Python, and Go interface (see original repo for Golang)
 
 ### C++ Compilation
 
 Compiling as a shared library. Feel free to subsititute e.g. clang for the C++ compiler.
```

### Comparing `compressed_segmentation-2.1.1/automated_test.py` & `compressed_segmentation-2.2.0/automated_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,7 +149,28 @@
         binary, shape=(sx,sy,sz), dtype=dtype, block_size=block_size
     )
 
     for i in range(10):
         x,y,z = np.random.randint(0, sx, size=(3,), dtype=int)
         assert arr[x,y,z] == labels[x,y,z]
 
+@pytest.mark.parametrize('dtype', [ np.uint32, np.uint64 ])
+@pytest.mark.parametrize('preserve_missing_labels', [ True, False ])
+def test_remap(dtype, preserve_missing_labels):
+    shape = (61,63,67)
+    labels = np.random.randint(0, 15, size=shape).astype(dtype)
+
+    remap = { i: i+20 for i in range(15) }
+    binary = cseg.compress(labels)
+    recovered = cseg.decompress(binary, shape, dtype)
+
+    assert np.all(labels == recovered)
+    assert np.all(cseg.labels(binary, shape, dtype) == list(range(15)))
+
+    binary2 = cseg.remap(
+        binary, shape, dtype, 
+        mapping=remap, 
+        preserve_missing_labels=preserve_missing_labels,
+    )
+    assert np.all(cseg.labels(binary2, shape, dtype) == list(range(20, 35)))
+
+
```

### Comparing `compressed_segmentation-2.1.1/build_linux.sh` & `compressed_segmentation-2.2.0/build_linux.sh`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/compressed_segmentation.egg-info/PKG-INFO` & `compressed_segmentation-2.2.0/compressed_segmentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressed-segmentation
-Version: 2.1.1
+Version: 2.2.0
 Summary: Neuroglancer compressed_segmentation codec.
 Home-page: https://github.com/janelia-flyem/compressedseg
 Author: Jeremy Maitin-Shepard, Stephen Plaza, and William Silversmith
 Author-email: ws9@princeton.edu
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,15 @@
 )
 
 arr = CompressedSegmentationArray(
     compressed, shape=(sx,sy,sz), dtype=dtype
 )
 label = arr[54,32,103] # random access to single voxels w/o decompressing
 uniq_labels = arr.labels() # get all distinct values w/o decompressing
+binary2 = arr.remap({ 1: 2 }, preserve_missing_labels=False) # remap labels in segmentation w/o decompressing
 recovered = arr.numpy() # decompress to a numpy array, same as decompress
 124213 in arr # test if a value is in the array
 ```
 
 ```bash
 cseg compress connectomics.npy
 cseg decompress connectomics.npy.cseg --volume-size 512,512,512 --bytes 4
@@ -66,14 +67,15 @@
 
 
 ### Features
 
 * Compression and decompression
 * Random access to voxels without decompression
 * Read out unique values without decompression
+* Remap labels without decompression
 * Command line interface for numpy files
 * (TBD) Interface to relabel and manipulate segmentation from the compressed data
 * C++, Python, and Go interface (see original repo for Golang)
 
 ### C++ Compilation
 
 Compiling as a shared library. Feel free to subsititute e.g. clang for the C++ compiler.
```

### Comparing `compressed_segmentation-2.1.1/compressed_segmentation.egg-info/SOURCES.txt` & `compressed_segmentation-2.2.0/compressed_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/cseg_cli/cli.py` & `compressed_segmentation-2.2.0/cseg_cli/cli.py`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/include/compress_segmentation.h` & `compressed_segmentation-2.2.0/include/compress_segmentation.h`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/include/decompress_segmentation.h` & `compressed_segmentation-2.2.0/include/decompress_segmentation.h`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/manylinux1.Dockerfile` & `compressed_segmentation-2.2.0/manylinux1.Dockerfile`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/manylinux2010.Dockerfile` & `compressed_segmentation-2.2.0/manylinux2010.Dockerfile`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/manylinux2014.Dockerfile` & `compressed_segmentation-2.2.0/manylinux2014.Dockerfile`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/perf.py` & `compressed_segmentation-2.2.0/perf.py`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/setup.cfg` & `compressed_segmentation-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/setup.py` & `compressed_segmentation-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/src/compress_segmentation.cc` & `compressed_segmentation-2.2.0/src/compress_segmentation.cc`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/src/compress_segmentation_test.cc` & `compressed_segmentation-2.2.0/src/compress_segmentation_test.cc`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/src/compressed_segmentation.cpp` & `compressed_segmentation-2.2.0/src/compressed_segmentation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1812,14 +1812,21 @@
 static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
     __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
 static void __Pyx_ZeroBuffer(Py_buffer* buf);
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
 #define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_SubtractObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
@@ -1888,21 +1895,14 @@
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_LshiftObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_LshiftObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceLshift(op1, op2) : PyNumber_Lshift(op1, op2))
 #endif
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* GetTopmostException.proto */
@@ -2814,34 +2814,36 @@
   static const char __pyx_k_s[] = "(%s)";
   static const char __pyx_k_x[] = "x";
   static const char __pyx_k_y[] = "y";
   static const char __pyx_k_z[] = "z";
   static const char __pyx_k_id[] = "id";
   static const char __pyx_k_np[] = "np";
   static const char __pyx_k_pt[] = "pt";
-  static const char __pyx_k__14[] = "<";
-  static const char __pyx_k__15[] = ",";
-  static const char __pyx_k__36[] = "^";
-  static const char __pyx_k__37[] = "";
-  static const char __pyx_k__38[] = ":";
-static const char __pyx_k__39[] = "}";
+  static const char __pyx_k__15[] = "<";
+  static const char __pyx_k__16[] = ",";
+  static const char __pyx_k__37[] = "^";
+  static const char __pyx_k__38[] = "";
+  static const char __pyx_k__39[] = ":";
+static const char __pyx_k__40[] = "}";
 static const char __pyx_k_any[] = "any";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_end[] = "end";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_gpt[] = "gpt";
 static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_mul[] = "mul";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_val[] = "val";
 static const char __pyx_k_xyz[] = "xyz";
+static const char __pyx_k_axis[] = "axis";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_ceil[] = "ceil";
+static const char __pyx_k_copy[] = "copy";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
@@ -2858,17 +2860,19 @@
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_int64[] = "int64";
+static const char __pyx_k_label[] = "label";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_order[] = "order";
 static const char __pyx_k_range[] = "range";
+static const char __pyx_k_remap[] = "remap";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_astype[] = "astype";
 static const char __pyx_k_binary[] = "binary";
 static const char __pyx_k_bitpos[] = "bitpos";
 static const char __pyx_k_bitval[] = "bitval";
@@ -2889,20 +2893,22 @@
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_bitmask[] = "bitmask";
 static const char __pyx_k_encoded[] = "encoded";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_getitem[] = "__getitem__";
 static const char __pyx_k_headers[] = "headers";
+static const char __pyx_k_mapping[] = "mapping";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_newaxis[] = "newaxis";
 static const char __pyx_k_offsets[] = "offsets";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_reshape[] = "reshape";
 static const char __pyx_k_tbl_off[] = "tbl_off";
+static const char __pyx_k_tobytes[] = "tobytes";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_arraypos[] = "arraypos";
 static const char __pyx_k_bitshift[] = "bitshift";
 static const char __pyx_k_compress[] = "compress";
 static const char __pyx_k_contains[] = "__contains__";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
@@ -2947,34 +2953,37 @@
 static const char __pyx_k_OverflowError[] = "OverflowError";
 static const char __pyx_k_arr_memview32[] = "arr_memview32";
 static const char __pyx_k_arr_memview64[] = "arr_memview64";
 static const char __pyx_k_block_sizeptr[] = "block_sizeptr";
 static const char __pyx_k_input_strides[] = "input_strides";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_channel_length[] = "channel_length";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_table_entry_size[] = "table_entry_size";
 static const char __pyx_k_Empty_data_stream[] = "Empty data stream.";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_DEFAULT_BLOCK_SIZE[] = "DEFAULT_BLOCK_SIZE";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_lookup_table_offset[] = "lookup_table_offset";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
+static const char __pyx_k_compute_label_offsets[] = "_compute_label_offsets";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_encoded_values_offset[] = "encoded_values_offset";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_Unable_to_locate_value[] = "Unable to locate value: ";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_compressed_segmentation[] = "compressed_segmentation";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
+static const char __pyx_k_preserve_missing_labels[] = "preserve_missing_labels";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_must_be_contained_within[] = "> must be contained within ";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_CompressedSegmentationArray[] = "CompressedSegmentationArray";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
@@ -2988,14 +2997,15 @@
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_CompressedSegmentationArray___co[] = "CompressedSegmentationArray.__contains__";
 static const char __pyx_k_CompressedSegmentationArray___ge[] = "CompressedSegmentationArray.__getitem__";
 static const char __pyx_k_CompressedSegmentationArray___in[] = "CompressedSegmentationArray.__init__";
 static const char __pyx_k_CompressedSegmentationArray_grid[] = "CompressedSegmentationArray.grid_size";
 static const char __pyx_k_CompressedSegmentationArray_labe[] = "CompressedSegmentationArray.labels";
 static const char __pyx_k_CompressedSegmentationArray_nump[] = "CompressedSegmentationArray.numpy";
+static const char __pyx_k_CompressedSegmentationArray_rema[] = "CompressedSegmentationArray.remap";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_Only_single_channel_is_currently[] = "Only single channel is currently supported in this function.";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_The_input_data_were_too_large_an[] = "The input data were too large and varied and generated a table offset larger than 24-bits.\nSee lookupTableOffset: https://github.com/google/neuroglancer/blob/c9a6b9948dd416997c91e655ec3d67bf6b7e771b/src/neuroglancer/sliceview/compressed_segmentation/README.md#format-specification";
@@ -3017,14 +3027,15 @@
 static PyObject *__pyx_n_s_CompressedSegmentationArray___co;
 static PyObject *__pyx_n_s_CompressedSegmentationArray___ge;
 static PyObject *__pyx_n_s_CompressedSegmentationArray___in;
 static PyObject *__pyx_n_s_CompressedSegmentationArray_get;
 static PyObject *__pyx_n_s_CompressedSegmentationArray_grid;
 static PyObject *__pyx_n_s_CompressedSegmentationArray_labe;
 static PyObject *__pyx_n_s_CompressedSegmentationArray_nump;
+static PyObject *__pyx_n_s_CompressedSegmentationArray_rema;
 static PyObject *__pyx_n_s_DEFAULT_BLOCK_SIZE;
 static PyObject *__pyx_n_s_DecodeError;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_u_Empty_data_stream;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_u_F;
 static PyObject *__pyx_n_s_ImportError;
@@ -3045,47 +3056,51 @@
 static PyObject *__pyx_kp_u_The_input_data_were_too_large_an;
 static PyObject *__pyx_kp_u_This_function_only_handles_singl;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_kp_u_Unable_to_locate_value;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
-static PyObject *__pyx_kp_u__14;
 static PyObject *__pyx_kp_u__15;
-static PyObject *__pyx_kp_b__36;
+static PyObject *__pyx_kp_u__16;
 static PyObject *__pyx_kp_b__37;
 static PyObject *__pyx_kp_b__38;
 static PyObject *__pyx_kp_b__39;
+static PyObject *__pyx_kp_b__40;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_any;
 static PyObject *__pyx_n_s_arr_memview32;
 static PyObject *__pyx_n_s_arr_memview64;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_arraypos;
 static PyObject *__pyx_n_s_astype;
+static PyObject *__pyx_n_s_axis;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_binary;
 static PyObject *__pyx_n_s_bitmask;
 static PyObject *__pyx_n_s_bitpos;
 static PyObject *__pyx_n_s_bitshift;
 static PyObject *__pyx_n_s_bitval;
 static PyObject *__pyx_n_s_block_size;
 static PyObject *__pyx_n_s_block_sizeptr;
 static PyObject *__pyx_n_s_bytestrout;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_ceil;
+static PyObject *__pyx_n_s_channel_length;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_compress;
 static PyObject *__pyx_n_s_compressed_segmentation;
+static PyObject *__pyx_n_s_compute_label_offsets;
 static PyObject *__pyx_n_s_concatenate;
 static PyObject *__pyx_n_s_contains;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
+static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_decompress;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_bytes;
 static PyObject *__pyx_n_s_dtype_is_object;
@@ -3120,18 +3135,20 @@
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_input_strides;
 static PyObject *__pyx_n_s_int64;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_join;
+static PyObject *__pyx_n_s_label;
 static PyObject *__pyx_n_s_labels;
 static PyObject *__pyx_n_s_labels_2;
 static PyObject *__pyx_n_s_lookup_table_offset;
 static PyObject *__pyx_n_s_main;
+static PyObject *__pyx_n_s_mapping;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_mul;
 static PyObject *__pyx_kp_u_must_be_contained_within;
 static PyObject *__pyx_n_s_name;
@@ -3151,14 +3168,15 @@
 static PyObject *__pyx_n_s_order;
 static PyObject *__pyx_n_s_output;
 static PyObject *__pyx_n_s_output_ptr;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_packed_off;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_prepare;
+static PyObject *__pyx_n_s_preserve_missing_labels;
 static PyObject *__pyx_n_s_property;
 static PyObject *__pyx_n_s_pt;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
@@ -3167,14 +3185,15 @@
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_2;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
+static PyObject *__pyx_n_s_remap;
 static PyObject *__pyx_n_s_reshape;
 static PyObject *__pyx_kp_u_s;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
@@ -3188,14 +3207,15 @@
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_sys;
 static PyObject *__pyx_n_s_table_entry_size;
 static PyObject *__pyx_n_s_tbl_off;
 static PyObject *__pyx_n_s_test;
+static PyObject *__pyx_n_s_tobytes;
 static PyObject *__pyx_n_s_uint32;
 static PyObject *__pyx_n_s_uint64;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unique;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
@@ -3207,22 +3227,25 @@
 static PyObject *__pyx_n_s_xyz;
 static PyObject *__pyx_n_s_y;
 static PyObject *__pyx_n_s_z;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_pf_23compressed_segmentation_compress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_block_size, PyObject *__pyx_v_order); /* proto */
 static PyObject *__pyx_pf_23compressed_segmentation_2decompress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_volume_size, PyObject *__pyx_v_dtype, PyObject *__pyx_v_block_size, PyObject *__pyx_v_order); /* proto */
 static PyObject *__pyx_pf_23compressed_segmentation_4labels(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_block_size); /* proto */
-static PyObject *__pyx_pf_23compressed_segmentation_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_6remap(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_mapping, PyObject *__pyx_v_preserve_missing_labels, PyObject *__pyx_v_block_size); /* proto */
+static PyArrayObject *__pyx_pf_23compressed_segmentation_8_compute_label_offsets(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_block_size); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_binary, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_block_size); /* proto */
 static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_2grid_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_4labels(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_6numpy(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_8get(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_y, PyObject *__pyx_v_z); /* proto */
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_10__contains__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_12__getitem__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_slcs); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_6remap(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mapping, PyObject *__pyx_v_preserve_missing_labels); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_8numpy(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_10get(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_y, PyObject *__pyx_v_z); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_12__contains__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_14__getitem__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_slcs); /* proto */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -3277,26 +3300,26 @@
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_k_;
 static PyObject *__pyx_k__8;
 static PyObject *__pyx_k__9;
 static PyObject *__pyx_k__10;
 static PyObject *__pyx_k__11;
-static uint32_t __pyx_k__43;
-static uint64_t __pyx_k__44;
+static PyObject *__pyx_k__14;
+static uint32_t __pyx_k__44;
+static uint64_t __pyx_k__45;
 static PyObject *__pyx_slice__2;
 static PyObject *__pyx_slice__3;
 static PyObject *__pyx_slice__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_slice__16;
+static PyObject *__pyx_slice__17;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
@@ -3307,42 +3330,50 @@
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
-static PyObject *__pyx_tuple__40;
+static PyObject *__pyx_tuple__36;
 static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_tuple__45;
-static PyObject *__pyx_tuple__47;
-static PyObject *__pyx_tuple__49;
-static PyObject *__pyx_tuple__51;
-static PyObject *__pyx_tuple__53;
-static PyObject *__pyx_tuple__55;
-static PyObject *__pyx_tuple__57;
-static PyObject *__pyx_tuple__59;
-static PyObject *__pyx_tuple__61;
+static PyObject *__pyx_tuple__42;
+static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_tuple__50;
+static PyObject *__pyx_tuple__52;
+static PyObject *__pyx_tuple__54;
+static PyObject *__pyx_tuple__56;
+static PyObject *__pyx_tuple__58;
+static PyObject *__pyx_tuple__60;
+static PyObject *__pyx_tuple__62;
 static PyObject *__pyx_tuple__63;
-static PyObject *__pyx_tuple__64;
 static PyObject *__pyx_tuple__65;
-static PyObject *__pyx_tuple__66;
 static PyObject *__pyx_tuple__67;
-static PyObject *__pyx_tuple__68;
-static PyObject *__pyx_codeobj__42;
-static PyObject *__pyx_codeobj__46;
-static PyObject *__pyx_codeobj__48;
-static PyObject *__pyx_codeobj__50;
-static PyObject *__pyx_codeobj__52;
-static PyObject *__pyx_codeobj__54;
-static PyObject *__pyx_codeobj__56;
-static PyObject *__pyx_codeobj__58;
-static PyObject *__pyx_codeobj__60;
-static PyObject *__pyx_codeobj__62;
-static PyObject *__pyx_codeobj__69;
+static PyObject *__pyx_tuple__69;
+static PyObject *__pyx_tuple__71;
+static PyObject *__pyx_tuple__72;
+static PyObject *__pyx_tuple__73;
+static PyObject *__pyx_tuple__74;
+static PyObject *__pyx_tuple__75;
+static PyObject *__pyx_tuple__76;
+static PyObject *__pyx_codeobj__43;
+static PyObject *__pyx_codeobj__47;
+static PyObject *__pyx_codeobj__49;
+static PyObject *__pyx_codeobj__51;
+static PyObject *__pyx_codeobj__53;
+static PyObject *__pyx_codeobj__55;
+static PyObject *__pyx_codeobj__57;
+static PyObject *__pyx_codeobj__59;
+static PyObject *__pyx_codeobj__61;
+static PyObject *__pyx_codeobj__64;
+static PyObject *__pyx_codeobj__66;
+static PyObject *__pyx_codeobj__68;
+static PyObject *__pyx_codeobj__70;
+static PyObject *__pyx_codeobj__77;
 /* Late includes */
 
 /* "compressed_segmentation.pyx":58
  *   pass
  * 
  * def compress(data, block_size=DEFAULT_BLOCK_SIZE, order='C'):             # <<<<<<<<<<<<<<
  *   """
@@ -5450,89 +5481,47 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_23compressed_segmentation_4labels(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_block_size) {
-  PyObject *__pyx_v_grid_size = NULL;
+  PyObject *__pyx_v_index = NULL;
   size_t __pyx_v_num_headers;
-  size_t __pyx_v_header_bytes;
-  PyArrayObject *__pyx_v_headers = 0;
   PyArrayObject *__pyx_v_data = 0;
-  PyArrayObject *__pyx_v_offsets = 0;
-  size_t __pyx_v_i;
-  size_t __pyx_v_lookup_table_offset;
-  size_t __pyx_v_encoded_values_offset;
   PyObject *__pyx_v_labels = NULL;
-  CYTHON_UNUSED size_t __pyx_v_dtype_bytes;
-  CYTHON_UNUSED size_t __pyx_v_start;
-  CYTHON_UNUSED size_t __pyx_v_end;
-  int64_t __pyx_v_idx;
-  int64_t __pyx_v_size;
-  PyArrayObject *__pyx_v_index = 0;
-  int64_t __pyx_8genexpr2__pyx_v_idx;
+  size_t __pyx_8genexpr2__pyx_v_idx;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_data;
   __Pyx_Buffer __pyx_pybuffer_data;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_headers;
-  __Pyx_Buffer __pyx_pybuffer_headers;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_index;
-  __Pyx_Buffer __pyx_pybuffer_index;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_offsets;
-  __Pyx_Buffer __pyx_pybuffer_offsets;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  size_t __pyx_t_9;
+  size_t __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
   PyArrayObject *__pyx_t_10 = NULL;
-  PyArrayObject *__pyx_t_11 = NULL;
-  PyArrayObject *__pyx_t_12 = NULL;
-  size_t __pyx_t_13;
-  size_t __pyx_t_14;
-  size_t __pyx_t_15;
-  PyObject *__pyx_t_16 = NULL;
-  PyObject *__pyx_t_17 = NULL;
-  PyObject *__pyx_t_18 = NULL;
-  int64_t __pyx_t_19;
-  PyArrayObject *__pyx_t_20 = NULL;
-  Py_ssize_t __pyx_t_21;
-  Py_ssize_t __pyx_t_22;
-  uint32_t __pyx_t_23;
-  PyObject *__pyx_t_24 = NULL;
-  PyObject *__pyx_t_25 = NULL;
+  size_t __pyx_t_11;
+  size_t __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("labels", 0);
   __Pyx_INCREF(__pyx_v_encoded);
   __Pyx_INCREF(__pyx_v_shape);
-  __Pyx_INCREF(__pyx_v_block_size);
-  __pyx_pybuffer_headers.pybuffer.buf = NULL;
-  __pyx_pybuffer_headers.refcount = 0;
-  __pyx_pybuffernd_headers.data = NULL;
-  __pyx_pybuffernd_headers.rcbuffer = &__pyx_pybuffer_headers;
   __pyx_pybuffer_data.pybuffer.buf = NULL;
   __pyx_pybuffer_data.refcount = 0;
   __pyx_pybuffernd_data.data = NULL;
   __pyx_pybuffernd_data.rcbuffer = &__pyx_pybuffer_data;
-  __pyx_pybuffer_offsets.pybuffer.buf = NULL;
-  __pyx_pybuffer_offsets.refcount = 0;
-  __pyx_pybuffernd_offsets.data = NULL;
-  __pyx_pybuffernd_offsets.rcbuffer = &__pyx_pybuffer_offsets;
-  __pyx_pybuffer_index.pybuffer.buf = NULL;
-  __pyx_pybuffer_index.refcount = 0;
-  __pyx_pybuffernd_index.data = NULL;
-  __pyx_pybuffernd_index.rcbuffer = &__pyx_pybuffer_index;
 
   /* "compressed_segmentation.pyx":230
  *   """Extract labels without decompressing."""
  * 
  *   if len(encoded) == 0:             # <<<<<<<<<<<<<<
  *     raise DecodeError("Empty data stream.")
  * 
@@ -5635,16 +5624,16 @@
  */
   }
 
   /* "compressed_segmentation.pyx":236
  *     raise DecodeError("This function only handles single channel images.")
  * 
  *   shape = np.array(shape)             # <<<<<<<<<<<<<<
- *   block_size = np.array(block_size)
- * 
+ *   if any(shape == 0):
+ *     return np.zeros((0,), dtype=dtype)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
@@ -5664,1069 +5653,2498 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_shape, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "compressed_segmentation.pyx":237
  * 
  *   shape = np.array(shape)
- *   block_size = np.array(block_size)             # <<<<<<<<<<<<<<
+ *   if any(shape == 0):             # <<<<<<<<<<<<<<
+ *     return np.zeros((0,), dtype=dtype)
  * 
+ */
+  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_shape, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_any, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__pyx_t_2) {
+
+    /* "compressed_segmentation.pyx":238
+ *   shape = np.array(shape)
  *   if any(shape == 0):
+ *     return np.zeros((0,), dtype=dtype)             # <<<<<<<<<<<<<<
+ * 
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_v_dtype) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__13, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+
+    /* "compressed_segmentation.pyx":237
+ * 
+ *   shape = np.array(shape)
+ *   if any(shape == 0):             # <<<<<<<<<<<<<<
+ *     return np.zeros((0,), dtype=dtype)
+ * 
+ */
+  }
+
+  /* "compressed_segmentation.pyx":240
+ *     return np.zeros((0,), dtype=dtype)
+ * 
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)             # <<<<<<<<<<<<<<
+ *   index = np.unique(index, axis=0)
+ *   cdef size_t num_headers = index.shape[0]
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_compute_label_offsets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = NULL;
+  __pyx_t_6 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __pyx_t_6 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[5] = {__pyx_t_4, __pyx_v_encoded, __pyx_v_shape, __pyx_v_dtype, __pyx_v_block_size};
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[5] = {__pyx_t_4, __pyx_v_encoded, __pyx_v_shape, __pyx_v_dtype, __pyx_v_block_size};
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_6, 4+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+  } else
+  #endif
+  {
+    __pyx_t_7 = PyTuple_New(4+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_encoded);
+    __Pyx_GIVEREF(__pyx_v_encoded);
+    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_encoded);
+    __Pyx_INCREF(__pyx_v_shape);
+    __Pyx_GIVEREF(__pyx_v_shape);
+    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_shape);
+    __Pyx_INCREF(__pyx_v_dtype);
+    __Pyx_GIVEREF(__pyx_v_dtype);
+    PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_v_dtype);
+    __Pyx_INCREF(__pyx_v_block_size);
+    __Pyx_GIVEREF(__pyx_v_block_size);
+    PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_6, __pyx_v_block_size);
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_v_index = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "compressed_segmentation.pyx":241
+ * 
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
+ *   index = np.unique(index, axis=0)             # <<<<<<<<<<<<<<
+ *   cdef size_t num_headers = index.shape[0]
+ * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_unique); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(__pyx_v_index);
+  __Pyx_GIVEREF(__pyx_v_index);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "compressed_segmentation.pyx":242
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
+ *   index = np.unique(index, axis=0)
+ *   cdef size_t num_headers = index.shape[0]             # <<<<<<<<<<<<<<
+ * 
+ *   encoded = encoded[4:] # skip the channel length
+ */
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_8 = __Pyx_PyInt_As_size_t(__pyx_t_7); if (unlikely((__pyx_t_8 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_v_num_headers = __pyx_t_8;
+
+  /* "compressed_segmentation.pyx":244
+ *   cdef size_t num_headers = index.shape[0]
+ * 
+ *   encoded = encoded[4:] # skip the channel length             # <<<<<<<<<<<<<<
+ *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
+ * 
+ */
+  if (unlikely(__pyx_v_encoded == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 244, __pyx_L1_error)
+  }
+  __pyx_t_7 = PySequence_GetSlice(__pyx_v_encoded, 4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF_SET(__pyx_v_encoded, ((PyObject*)__pyx_t_7));
+  __pyx_t_7 = 0;
+
+  /* "compressed_segmentation.pyx":245
+ * 
+ *   encoded = encoded[4:] # skip the channel length
+ *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)             # <<<<<<<<<<<<<<
+ * 
+ *   labels = np.concatenate([
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_INCREF(__pyx_v_encoded);
+  __Pyx_GIVEREF(__pyx_v_encoded);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_encoded);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (!(likely(((__pyx_t_9) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_9, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_10 = ((PyArrayObject *)__pyx_t_9);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_data = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_data.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 245, __pyx_L1_error)
+    } else {__pyx_pybuffernd_data.diminfo[0].strides = __pyx_pybuffernd_data.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data.diminfo[0].shape = __pyx_pybuffernd_data.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_10 = 0;
+  __pyx_v_data = ((PyArrayObject *)__pyx_t_9);
+  __pyx_t_9 = 0;
+
+  /* "compressed_segmentation.pyx":247
+ *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
+ * 
+ *   labels = np.concatenate([             # <<<<<<<<<<<<<<
+ *     data[index[idx,0]:index[idx,1]]
+ *     for idx in range(num_headers)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_concatenate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  { /* enter inner scope */
+    __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+
+    /* "compressed_segmentation.pyx":249
+ *   labels = np.concatenate([
+ *     data[index[idx,0]:index[idx,1]]
+ *     for idx in range(num_headers)             # <<<<<<<<<<<<<<
+ *   ]).view(dtype)
+ * 
+ */
+    __pyx_t_8 = __pyx_v_num_headers;
+    __pyx_t_11 = __pyx_t_8;
+    for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+      __pyx_8genexpr2__pyx_v_idx = __pyx_t_12;
+
+      /* "compressed_segmentation.pyx":248
+ * 
+ *   labels = np.concatenate([
+ *     data[index[idx,0]:index[idx,1]]             # <<<<<<<<<<<<<<
+ *     for idx in range(num_headers)
+ *   ]).view(dtype)
+ */
+      __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_8genexpr2__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_GIVEREF(__pyx_t_5);
+      PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_5);
+      __Pyx_INCREF(__pyx_int_0);
+      __Pyx_GIVEREF(__pyx_int_0);
+      PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_int_0);
+      __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_index, __pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+      __pyx_t_13 = __Pyx_PyInt_FromSize_t(__pyx_8genexpr2__pyx_v_idx); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_14);
+      __Pyx_GIVEREF(__pyx_t_13);
+      PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13);
+      __Pyx_INCREF(__pyx_int_1);
+      __Pyx_GIVEREF(__pyx_int_1);
+      PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_int_1);
+      __pyx_t_13 = 0;
+      __pyx_t_13 = __Pyx_PyObject_GetItem(__pyx_v_index, __pyx_t_14); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      __pyx_t_14 = PySlice_New(__pyx_t_5, __pyx_t_13, Py_None); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_14);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+      __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_data), __pyx_t_14); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 248, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_13))) __PYX_ERR(0, 247, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    }
+  } /* exit inner scope */
+  __pyx_t_13 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_13)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_13);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_v_block_size) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_block_size);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_3 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_13, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "compressed_segmentation.pyx":250
+ *     data[index[idx,0]:index[idx,1]]
+ *     for idx in range(num_headers)
+ *   ]).view(dtype)             # <<<<<<<<<<<<<<
+ * 
+ *   return np.unique(labels)
+ */
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_view); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF_SET(__pyx_v_block_size, __pyx_t_4);
-  __pyx_t_4 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_9 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_dtype) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_dtype);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_labels = __pyx_t_9;
+  __pyx_t_9 = 0;
 
-  /* "compressed_segmentation.pyx":239
- *   block_size = np.array(block_size)
+  /* "compressed_segmentation.pyx":252
+ *   ]).view(dtype)
  * 
- *   if any(shape == 0):             # <<<<<<<<<<<<<<
- *     return np.zeros((0,), dtype=dtype)
+ *   return np.unique(labels)             # <<<<<<<<<<<<<<
  * 
+ * def remap(
  */
-  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_shape, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_any, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unique); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_9 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_labels) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_labels);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__pyx_t_2) {
+  __pyx_r = __pyx_t_9;
+  __pyx_t_9 = 0;
+  goto __pyx_L0;
 
-    /* "compressed_segmentation.pyx":240
+  /* "compressed_segmentation.pyx":224
+ *     raise TypeError("dtype ({}) must be one of uint32 or uint64.".format(dtype))
  * 
- *   if any(shape == 0):
- *     return np.zeros((0,), dtype=dtype)             # <<<<<<<<<<<<<<
+ * def labels(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype,
+ *   block_size=DEFAULT_BLOCK_SIZE
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_14);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("compressed_segmentation.labels", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF(__pyx_v_index);
+  __Pyx_XDECREF((PyObject *)__pyx_v_data);
+  __Pyx_XDECREF(__pyx_v_labels);
+  __Pyx_XDECREF(__pyx_v_encoded);
+  __Pyx_XDECREF(__pyx_v_shape);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "compressed_segmentation.pyx":254
+ *   return np.unique(labels)
  * 
- *   grid_size = np.ceil(shape / block_size).astype(np.uint64)
+ * def remap(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,
  */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
+
+/* Python wrapper */
+static PyObject *__pyx_pw_23compressed_segmentation_7remap(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_23compressed_segmentation_6remap[] = "Extract labels without decompressing.";
+static PyMethodDef __pyx_mdef_23compressed_segmentation_7remap = {"remap", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_7remap, METH_VARARGS|METH_KEYWORDS, __pyx_doc_23compressed_segmentation_6remap};
+static PyObject *__pyx_pw_23compressed_segmentation_7remap(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_encoded = 0;
+  PyObject *__pyx_v_shape = 0;
+  PyObject *__pyx_v_dtype = 0;
+  PyObject *__pyx_v_mapping = 0;
+  PyObject *__pyx_v_preserve_missing_labels = 0;
+  PyObject *__pyx_v_block_size = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("remap (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_encoded,&__pyx_n_s_shape,&__pyx_n_s_dtype,&__pyx_n_s_mapping,&__pyx_n_s_preserve_missing_labels,&__pyx_n_s_block_size,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+
+    /* "compressed_segmentation.pyx":256
+ * def remap(
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,             # <<<<<<<<<<<<<<
+ *   block_size=DEFAULT_BLOCK_SIZE
+ * ):
+ */
+    values[4] = ((PyObject *)Py_False);
+    values[5] = __pyx_k__14;
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoded)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("remap", 0, 4, 6, 1); __PYX_ERR(0, 254, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("remap", 0, 4, 6, 2); __PYX_ERR(0, 254, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mapping)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("remap", 0, 4, 6, 3); __PYX_ERR(0, 254, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_preserve_missing_labels);
+          if (value) { values[4] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_block_size);
+          if (value) { values[5] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "remap") < 0)) __PYX_ERR(0, 254, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_encoded = ((PyObject*)values[0]);
+    __pyx_v_shape = values[1];
+    __pyx_v_dtype = values[2];
+    __pyx_v_mapping = values[3];
+    __pyx_v_preserve_missing_labels = values[4];
+    __pyx_v_block_size = values[5];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("remap", 0, 4, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 254, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("compressed_segmentation.remap", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encoded), (&PyBytes_Type), 1, "encoded", 1))) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_r = __pyx_pf_23compressed_segmentation_6remap(__pyx_self, __pyx_v_encoded, __pyx_v_shape, __pyx_v_dtype, __pyx_v_mapping, __pyx_v_preserve_missing_labels, __pyx_v_block_size);
+
+  /* "compressed_segmentation.pyx":254
+ *   return np.unique(labels)
+ * 
+ * def remap(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_23compressed_segmentation_6remap(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_mapping, PyObject *__pyx_v_preserve_missing_labels, PyObject *__pyx_v_block_size) {
+  PyObject *__pyx_v_index = NULL;
+  size_t __pyx_v_num_headers;
+  PyObject *__pyx_v_channel_length = NULL;
+  PyArrayObject *__pyx_v_data = 0;
+  size_t __pyx_v_idx;
+  PyObject *__pyx_v_labels = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_label = NULL;
+  PyObject *__pyx_8genexpr4__pyx_v_label = NULL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_data;
+  __Pyx_Buffer __pyx_pybuffer_data;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  size_t __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyArrayObject *__pyx_t_12 = NULL;
+  size_t __pyx_t_13;
+  size_t __pyx_t_14;
+  PyObject *(*__pyx_t_15)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("remap", 0);
+  __Pyx_INCREF(__pyx_v_shape);
+  __pyx_pybuffer_data.pybuffer.buf = NULL;
+  __pyx_pybuffer_data.refcount = 0;
+  __pyx_pybuffernd_data.data = NULL;
+  __pyx_pybuffernd_data.rcbuffer = &__pyx_pybuffer_data;
+
+  /* "compressed_segmentation.pyx":261
+ *   """Extract labels without decompressing."""
+ * 
+ *   if len(encoded) == 0:             # <<<<<<<<<<<<<<
+ *     raise DecodeError("Empty data stream.")
+ * 
+ */
+  if (unlikely(__pyx_v_encoded == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 261, __pyx_L1_error)
+  }
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_encoded); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_2 = ((__pyx_t_1 == 0) != 0);
+  if (unlikely(__pyx_t_2)) {
+
+    /* "compressed_segmentation.pyx":262
+ * 
+ *   if len(encoded) == 0:
+ *     raise DecodeError("Empty data stream.")             # <<<<<<<<<<<<<<
+ * 
+ *   if encoded[0] != 1:
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DecodeError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_Empty_data_stream) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_Empty_data_stream);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_dtype) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__13, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 240, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
-    goto __pyx_L0;
+    __PYX_ERR(0, 262, __pyx_L1_error)
 
-    /* "compressed_segmentation.pyx":239
- *   block_size = np.array(block_size)
+    /* "compressed_segmentation.pyx":261
+ *   """Extract labels without decompressing."""
  * 
- *   if any(shape == 0):             # <<<<<<<<<<<<<<
- *     return np.zeros((0,), dtype=dtype)
+ *   if len(encoded) == 0:             # <<<<<<<<<<<<<<
+ *     raise DecodeError("Empty data stream.")
  * 
  */
   }
 
-  /* "compressed_segmentation.pyx":242
- *     return np.zeros((0,), dtype=dtype)
+  /* "compressed_segmentation.pyx":264
+ *     raise DecodeError("Empty data stream.")
+ * 
+ *   if encoded[0] != 1:             # <<<<<<<<<<<<<<
+ *     raise DecodeError("This function only handles single channel images.")
  * 
- *   grid_size = np.ceil(shape / block_size).astype(np.uint64)             # <<<<<<<<<<<<<<
- *   cdef size_t num_headers = reduce(operator.mul, grid_size)
- *   cdef size_t header_bytes = 8 * num_headers
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_encoded, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyInt_NeObjC(__pyx_t_3, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ceil); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyNumber_Divide(__pyx_v_shape, __pyx_v_block_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (unlikely(__pyx_t_2)) {
+
+    /* "compressed_segmentation.pyx":265
+ * 
+ *   if encoded[0] != 1:
+ *     raise DecodeError("This function only handles single channel images.")             # <<<<<<<<<<<<<<
+ * 
+ *   shape = np.array(shape)
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DecodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u_This_function_only_handles_singl) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_This_function_only_handles_singl);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_ERR(0, 265, __pyx_L1_error)
+
+    /* "compressed_segmentation.pyx":264
+ *     raise DecodeError("Empty data stream.")
+ * 
+ *   if encoded[0] != 1:             # <<<<<<<<<<<<<<
+ *     raise DecodeError("This function only handles single channel images.")
+ * 
+ */
+  }
+
+  /* "compressed_segmentation.pyx":267
+ *     raise DecodeError("This function only handles single channel images.")
+ * 
+ *   shape = np.array(shape)             # <<<<<<<<<<<<<<
+ *   if np.any(shape == 0):
+ *     return encoded
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+    }
+  }
+  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_v_shape) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_shape);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF_SET(__pyx_v_shape, __pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "compressed_segmentation.pyx":268
+ * 
+ *   shape = np.array(shape)
+ *   if np.any(shape == 0):             # <<<<<<<<<<<<<<
+ *     return encoded
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_any); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_EqObjC(__pyx_v_shape, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "compressed_segmentation.pyx":269
+ *   shape = np.array(shape)
+ *   if np.any(shape == 0):
+ *     return encoded             # <<<<<<<<<<<<<<
+ * 
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_v_encoded);
+    __pyx_r = __pyx_v_encoded;
+    goto __pyx_L0;
+
+    /* "compressed_segmentation.pyx":268
+ * 
+ *   shape = np.array(shape)
+ *   if np.any(shape == 0):             # <<<<<<<<<<<<<<
+ *     return encoded
+ * 
+ */
+  }
+
+  /* "compressed_segmentation.pyx":271
+ *     return encoded
+ * 
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)             # <<<<<<<<<<<<<<
+ *   index = np.unique(index, axis=0)
+ *   cdef size_t num_headers = index.shape[0]
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compute_label_offsets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = NULL;
+  __pyx_t_7 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[5] = {__pyx_t_5, __pyx_v_encoded, __pyx_v_shape, __pyx_v_dtype, __pyx_v_block_size};
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 4+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_GOTREF(__pyx_t_4);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[5] = {__pyx_t_5, __pyx_v_encoded, __pyx_v_shape, __pyx_v_dtype, __pyx_v_block_size};
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 4+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_GOTREF(__pyx_t_4);
+  } else
+  #endif
+  {
+    __pyx_t_6 = PyTuple_New(4+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (__pyx_t_5) {
+      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_encoded);
+    __Pyx_GIVEREF(__pyx_v_encoded);
+    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_v_encoded);
+    __Pyx_INCREF(__pyx_v_shape);
+    __Pyx_GIVEREF(__pyx_v_shape);
+    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_v_shape);
+    __Pyx_INCREF(__pyx_v_dtype);
+    __Pyx_GIVEREF(__pyx_v_dtype);
+    PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_7, __pyx_v_dtype);
+    __Pyx_INCREF(__pyx_v_block_size);
+    __Pyx_GIVEREF(__pyx_v_block_size);
+    PyTuple_SET_ITEM(__pyx_t_6, 3+__pyx_t_7, __pyx_v_block_size);
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_index = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "compressed_segmentation.pyx":272
+ * 
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
+ *   index = np.unique(index, axis=0)             # <<<<<<<<<<<<<<
+ *   cdef size_t num_headers = index.shape[0]
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unique); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_INCREF(__pyx_v_index);
+  __Pyx_GIVEREF(__pyx_v_index);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_index);
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_5);
+  __pyx_t_5 = 0;
+
+  /* "compressed_segmentation.pyx":273
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
+ *   index = np.unique(index, axis=0)
+ *   cdef size_t num_headers = index.shape[0]             # <<<<<<<<<<<<<<
+ * 
+ *   channel_length = encoded[:4]
+ */
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_8 = __Pyx_PyInt_As_size_t(__pyx_t_6); if (unlikely((__pyx_t_8 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 273, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_v_num_headers = __pyx_t_8;
+
+  /* "compressed_segmentation.pyx":275
+ *   cdef size_t num_headers = index.shape[0]
+ * 
+ *   channel_length = encoded[:4]             # <<<<<<<<<<<<<<
+ *   cdef np.ndarray[uint32_t] data = np.copy(np.frombuffer(encoded[4:], dtype=np.uint32))
+ * 
+ */
+  if (unlikely(__pyx_v_encoded == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 275, __pyx_L1_error)
+  }
+  __pyx_t_6 = PySequence_GetSlice(__pyx_v_encoded, 0, 4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_v_channel_length = ((PyObject*)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "compressed_segmentation.pyx":276
+ * 
+ *   channel_length = encoded[:4]
+ *   cdef np.ndarray[uint32_t] data = np.copy(np.frombuffer(encoded[4:], dtype=np.uint32))             # <<<<<<<<<<<<<<
+ * 
+ *   for idx in range(num_headers):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_copy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(__pyx_v_encoded == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(0, 276, __pyx_L1_error)
+  }
+  __pyx_t_5 = PySequence_GetSlice(__pyx_v_encoded, 4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_uint32); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_12 = ((PyArrayObject *)__pyx_t_6);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data.rcbuffer->pybuffer, (PyObject*)__pyx_t_12, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_data = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_data.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 276, __pyx_L1_error)
+    } else {__pyx_pybuffernd_data.diminfo[0].strides = __pyx_pybuffernd_data.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data.diminfo[0].shape = __pyx_pybuffernd_data.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_12 = 0;
+  __pyx_v_data = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "compressed_segmentation.pyx":278
+ *   cdef np.ndarray[uint32_t] data = np.copy(np.frombuffer(encoded[4:], dtype=np.uint32))
+ * 
+ *   for idx in range(num_headers):             # <<<<<<<<<<<<<<
+ *     labels = data[index[idx,0]:index[idx,1]].view(dtype)
+ * 
+ */
+  __pyx_t_8 = __pyx_v_num_headers;
+  __pyx_t_13 = __pyx_t_8;
+  for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
+    __pyx_v_idx = __pyx_t_14;
+
+    /* "compressed_segmentation.pyx":279
+ * 
+ *   for idx in range(num_headers):
+ *     labels = data[index[idx,0]:index[idx,1]].view(dtype)             # <<<<<<<<<<<<<<
+ * 
+ *     if preserve_missing_labels:
+ */
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_idx); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_4);
+    __Pyx_INCREF(__pyx_int_0);
+    __Pyx_GIVEREF(__pyx_int_0);
+    PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_0);
+    __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_index, __pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyInt_FromSize_t(__pyx_v_idx); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_11);
+    __Pyx_INCREF(__pyx_int_1);
+    __Pyx_GIVEREF(__pyx_int_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_int_1);
+    __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_v_index, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PySlice_New(__pyx_t_4, __pyx_t_11, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_data), __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_view); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_11)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_11);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+      }
+    }
+    __pyx_t_6 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_11, __pyx_v_dtype) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_dtype);
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_labels, __pyx_t_6);
+    __pyx_t_6 = 0;
+
+    /* "compressed_segmentation.pyx":281
+ *     labels = data[index[idx,0]:index[idx,1]].view(dtype)
+ * 
+ *     if preserve_missing_labels:             # <<<<<<<<<<<<<<
+ *       labels = np.array([ mapping.get(label, label) for label in labels ], dtype=dtype)
+ *     else:
+ */
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_preserve_missing_labels); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 281, __pyx_L1_error)
+    if (__pyx_t_2) {
+
+      /* "compressed_segmentation.pyx":282
+ * 
+ *     if preserve_missing_labels:
+ *       labels = np.array([ mapping.get(label, label) for label in labels ], dtype=dtype)             # <<<<<<<<<<<<<<
+ *     else:
+ *       labels = np.array([ mapping[label] for label in labels ], dtype=dtype)
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 282, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 282, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      { /* enter inner scope */
+        __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 282, __pyx_L11_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        if (likely(PyList_CheckExact(__pyx_v_labels)) || PyTuple_CheckExact(__pyx_v_labels)) {
+          __pyx_t_11 = __pyx_v_labels; __Pyx_INCREF(__pyx_t_11); __pyx_t_1 = 0;
+          __pyx_t_15 = NULL;
+        } else {
+          __pyx_t_1 = -1; __pyx_t_11 = PyObject_GetIter(__pyx_v_labels); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 282, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_15 = Py_TYPE(__pyx_t_11)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 282, __pyx_L11_error)
+        }
+        for (;;) {
+          if (likely(!__pyx_t_15)) {
+            if (likely(PyList_CheckExact(__pyx_t_11))) {
+              if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_11)) break;
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_4 = PyList_GET_ITEM(__pyx_t_11, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 282, __pyx_L11_error)
+              #else
+              __pyx_t_4 = PySequence_ITEM(__pyx_t_11, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L11_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              #endif
+            } else {
+              if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_11)) break;
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_11, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 282, __pyx_L11_error)
+              #else
+              __pyx_t_4 = PySequence_ITEM(__pyx_t_11, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L11_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              #endif
+            }
+          } else {
+            __pyx_t_4 = __pyx_t_15(__pyx_t_11);
+            if (unlikely(!__pyx_t_4)) {
+              PyObject* exc_type = PyErr_Occurred();
+              if (exc_type) {
+                if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+                else __PYX_ERR(0, 282, __pyx_L11_error)
+              }
+              break;
+            }
+            __Pyx_GOTREF(__pyx_t_4);
+          }
+          __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_label, __pyx_t_4);
+          __pyx_t_4 = 0;
+          __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_mapping, __pyx_n_s_get); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 282, __pyx_L11_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          __pyx_t_3 = NULL;
+          __pyx_t_7 = 0;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+            __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
+            if (likely(__pyx_t_3)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+              __Pyx_INCREF(__pyx_t_3);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_9, function);
+              __pyx_t_7 = 1;
+            }
+          }
+          #if CYTHON_FAST_PYCALL
+          if (PyFunction_Check(__pyx_t_9)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_8genexpr3__pyx_v_label, __pyx_8genexpr3__pyx_v_label};
+            __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L11_error)
+            __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __Pyx_GOTREF(__pyx_t_4);
+          } else
+          #endif
+          #if CYTHON_FAST_PYCCALL
+          if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_8genexpr3__pyx_v_label, __pyx_8genexpr3__pyx_v_label};
+            __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L11_error)
+            __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __Pyx_GOTREF(__pyx_t_4);
+          } else
+          #endif
+          {
+            __pyx_t_10 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 282, __pyx_L11_error)
+            __Pyx_GOTREF(__pyx_t_10);
+            if (__pyx_t_3) {
+              __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_3); __pyx_t_3 = NULL;
+            }
+            __Pyx_INCREF(__pyx_8genexpr3__pyx_v_label);
+            __Pyx_GIVEREF(__pyx_8genexpr3__pyx_v_label);
+            PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_7, __pyx_8genexpr3__pyx_v_label);
+            __Pyx_INCREF(__pyx_8genexpr3__pyx_v_label);
+            __Pyx_GIVEREF(__pyx_8genexpr3__pyx_v_label);
+            PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_7, __pyx_8genexpr3__pyx_v_label);
+            __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L11_error)
+            __Pyx_GOTREF(__pyx_t_4);
+            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          }
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 282, __pyx_L11_error)
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_label); __pyx_8genexpr3__pyx_v_label = 0;
+        goto __pyx_L14_exit_scope;
+        __pyx_L11_error:;
+        __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_label); __pyx_8genexpr3__pyx_v_label = 0;
+        goto __pyx_L1_error;
+        __pyx_L14_exit_scope:;
+      } /* exit inner scope */
+      __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 282, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_GIVEREF(__pyx_t_6);
+      PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
+      __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 282, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_v_dtype) < 0) __PYX_ERR(0, 282, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_11, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_4);
+      __pyx_t_4 = 0;
+
+      /* "compressed_segmentation.pyx":281
+ *     labels = data[index[idx,0]:index[idx,1]].view(dtype)
+ * 
+ *     if preserve_missing_labels:             # <<<<<<<<<<<<<<
+ *       labels = np.array([ mapping.get(label, label) for label in labels ], dtype=dtype)
+ *     else:
+ */
+      goto __pyx_L8;
+    }
+
+    /* "compressed_segmentation.pyx":284
+ *       labels = np.array([ mapping.get(label, label) for label in labels ], dtype=dtype)
+ *     else:
+ *       labels = np.array([ mapping[label] for label in labels ], dtype=dtype)             # <<<<<<<<<<<<<<
+ * 
+ *     data[index[idx,0]:index[idx,1]] = labels.view(np.uint32)
+ */
+    /*else*/ {
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      { /* enter inner scope */
+        __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L17_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        if (likely(PyList_CheckExact(__pyx_v_labels)) || PyTuple_CheckExact(__pyx_v_labels)) {
+          __pyx_t_11 = __pyx_v_labels; __Pyx_INCREF(__pyx_t_11); __pyx_t_1 = 0;
+          __pyx_t_15 = NULL;
+        } else {
+          __pyx_t_1 = -1; __pyx_t_11 = PyObject_GetIter(__pyx_v_labels); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 284, __pyx_L17_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_15 = Py_TYPE(__pyx_t_11)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 284, __pyx_L17_error)
+        }
+        for (;;) {
+          if (likely(!__pyx_t_15)) {
+            if (likely(PyList_CheckExact(__pyx_t_11))) {
+              if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_11)) break;
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_5 = PyList_GET_ITEM(__pyx_t_11, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 284, __pyx_L17_error)
+              #else
+              __pyx_t_5 = PySequence_ITEM(__pyx_t_11, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              #endif
+            } else {
+              if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_11)) break;
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_11, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 284, __pyx_L17_error)
+              #else
+              __pyx_t_5 = PySequence_ITEM(__pyx_t_11, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              #endif
+            }
+          } else {
+            __pyx_t_5 = __pyx_t_15(__pyx_t_11);
+            if (unlikely(!__pyx_t_5)) {
+              PyObject* exc_type = PyErr_Occurred();
+              if (exc_type) {
+                if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+                else __PYX_ERR(0, 284, __pyx_L17_error)
+              }
+              break;
+            }
+            __Pyx_GOTREF(__pyx_t_5);
+          }
+          __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_label, __pyx_t_5);
+          __pyx_t_5 = 0;
+          __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_mapping, __pyx_8genexpr4__pyx_v_label); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L17_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 284, __pyx_L17_error)
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        }
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_label); __pyx_8genexpr4__pyx_v_label = 0;
+        goto __pyx_L20_exit_scope;
+        __pyx_L17_error:;
+        __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_label); __pyx_8genexpr4__pyx_v_label = 0;
+        goto __pyx_L1_error;
+        __pyx_L20_exit_scope:;
+      } /* exit inner scope */
+      __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_GIVEREF(__pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_4);
+      __pyx_t_4 = 0;
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_v_dtype) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_5);
+      __pyx_t_5 = 0;
+    }
+    __pyx_L8:;
+
+    /* "compressed_segmentation.pyx":286
+ *       labels = np.array([ mapping[label] for label in labels ], dtype=dtype)
+ * 
+ *     data[index[idx,0]:index[idx,1]] = labels.view(np.uint32)             # <<<<<<<<<<<<<<
+ * 
+ *   return channel_length + data.tobytes()
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_labels, __pyx_n_s_view); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_uint32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_11)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_11);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_5 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_11, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_idx); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
+    __Pyx_INCREF(__pyx_int_0);
+    __Pyx_GIVEREF(__pyx_int_0);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_int_0);
+    __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_index, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_idx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
+    __Pyx_INCREF(__pyx_int_1);
+    __Pyx_GIVEREF(__pyx_int_1);
+    PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_1);
+    __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_index, __pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = PySlice_New(__pyx_t_4, __pyx_t_6, Py_None); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_data), __pyx_t_11, __pyx_t_5) < 0)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
+
+  /* "compressed_segmentation.pyx":288
+ *     data[index[idx,0]:index[idx,1]] = labels.view(np.uint32)
+ * 
+ *   return channel_length + data.tobytes()             # <<<<<<<<<<<<<<
+ * 
+ * def _compute_label_offsets(
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_6 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_11);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_11, function);
+    }
+  }
+  __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __pyx_t_11 = PyNumber_Add(__pyx_v_channel_length, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_11;
+  __pyx_t_11 = 0;
+  goto __pyx_L0;
+
+  /* "compressed_segmentation.pyx":254
+ *   return np.unique(labels)
+ * 
+ * def remap(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("compressed_segmentation.remap", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF(__pyx_v_index);
+  __Pyx_XDECREF(__pyx_v_channel_length);
+  __Pyx_XDECREF((PyObject *)__pyx_v_data);
+  __Pyx_XDECREF(__pyx_v_labels);
+  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_label);
+  __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_label);
+  __Pyx_XDECREF(__pyx_v_shape);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "compressed_segmentation.pyx":290
+ *   return channel_length + data.tobytes()
+ * 
+ * def _compute_label_offsets(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype, block_size
+ * ) -> np.ndarray:
+ */
+
+/* Python wrapper */
+static PyArrayObject *__pyx_pw_23compressed_segmentation_9_compute_label_offsets(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_23compressed_segmentation_9_compute_label_offsets = {"_compute_label_offsets", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_9_compute_label_offsets, METH_VARARGS|METH_KEYWORDS, 0};
+static PyArrayObject *__pyx_pw_23compressed_segmentation_9_compute_label_offsets(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_encoded = 0;
+  PyObject *__pyx_v_shape = 0;
+  PyObject *__pyx_v_dtype = 0;
+  PyObject *__pyx_v_block_size = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyArrayObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_compute_label_offsets (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_encoded,&__pyx_n_s_shape,&__pyx_n_s_dtype,&__pyx_n_s_block_size,0};
+    PyObject* values[4] = {0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoded)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_compute_label_offsets", 1, 4, 4, 1); __PYX_ERR(0, 290, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_compute_label_offsets", 1, 4, 4, 2); __PYX_ERR(0, 290, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_block_size)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_compute_label_offsets", 1, 4, 4, 3); __PYX_ERR(0, 290, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_compute_label_offsets") < 0)) __PYX_ERR(0, 290, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+    }
+    __pyx_v_encoded = ((PyObject*)values[0]);
+    __pyx_v_shape = values[1];
+    __pyx_v_dtype = values[2];
+    __pyx_v_block_size = values[3];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("_compute_label_offsets", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 290, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("compressed_segmentation._compute_label_offsets", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encoded), (&PyBytes_Type), 1, "encoded", 1))) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_r = __pyx_pf_23compressed_segmentation_8_compute_label_offsets(__pyx_self, __pyx_v_encoded, __pyx_v_shape, __pyx_v_dtype, __pyx_v_block_size);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyArrayObject *__pyx_pf_23compressed_segmentation_8_compute_label_offsets(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_encoded, PyObject *__pyx_v_shape, PyObject *__pyx_v_dtype, PyObject *__pyx_v_block_size) {
+  PyObject *__pyx_v_grid_size = NULL;
+  size_t __pyx_v_num_headers;
+  size_t __pyx_v_header_bytes;
+  PyArrayObject *__pyx_v_headers = 0;
+  PyArrayObject *__pyx_v_data = 0;
+  PyArrayObject *__pyx_v_offsets = 0;
+  size_t __pyx_v_i;
+  size_t __pyx_v_lookup_table_offset;
+  size_t __pyx_v_encoded_values_offset;
+  CYTHON_UNUSED PyObject *__pyx_v_labels = NULL;
+  CYTHON_UNUSED size_t __pyx_v_dtype_bytes;
+  CYTHON_UNUSED size_t __pyx_v_start;
+  CYTHON_UNUSED size_t __pyx_v_end;
+  int64_t __pyx_v_idx;
+  int64_t __pyx_v_size;
+  PyArrayObject *__pyx_v_index = 0;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_data;
+  __Pyx_Buffer __pyx_pybuffer_data;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_headers;
+  __Pyx_Buffer __pyx_pybuffer_headers;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_index;
+  __Pyx_Buffer __pyx_pybuffer_index;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_offsets;
+  __Pyx_Buffer __pyx_pybuffer_offsets;
+  PyArrayObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  size_t __pyx_t_7;
+  PyArrayObject *__pyx_t_8 = NULL;
+  PyArrayObject *__pyx_t_9 = NULL;
+  PyArrayObject *__pyx_t_10 = NULL;
+  size_t __pyx_t_11;
+  size_t __pyx_t_12;
+  size_t __pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
+  int64_t __pyx_t_17;
+  PyArrayObject *__pyx_t_18 = NULL;
+  int __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  Py_ssize_t __pyx_t_21;
+  uint32_t __pyx_t_22;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_compute_label_offsets", 0);
+  __Pyx_INCREF(__pyx_v_encoded);
+  __Pyx_INCREF(__pyx_v_shape);
+  __Pyx_INCREF(__pyx_v_block_size);
+  __pyx_pybuffer_headers.pybuffer.buf = NULL;
+  __pyx_pybuffer_headers.refcount = 0;
+  __pyx_pybuffernd_headers.data = NULL;
+  __pyx_pybuffernd_headers.rcbuffer = &__pyx_pybuffer_headers;
+  __pyx_pybuffer_data.pybuffer.buf = NULL;
+  __pyx_pybuffer_data.refcount = 0;
+  __pyx_pybuffernd_data.data = NULL;
+  __pyx_pybuffernd_data.rcbuffer = &__pyx_pybuffer_data;
+  __pyx_pybuffer_offsets.pybuffer.buf = NULL;
+  __pyx_pybuffer_offsets.refcount = 0;
+  __pyx_pybuffernd_offsets.data = NULL;
+  __pyx_pybuffernd_offsets.rcbuffer = &__pyx_pybuffer_offsets;
+  __pyx_pybuffer_index.pybuffer.buf = NULL;
+  __pyx_pybuffer_index.refcount = 0;
+  __pyx_pybuffernd_index.data = NULL;
+  __pyx_pybuffernd_index.rcbuffer = &__pyx_pybuffer_index;
+
+  /* "compressed_segmentation.pyx":293
+ *   bytes encoded, shape, dtype, block_size
+ * ) -> np.ndarray:
+ *   shape = np.array(shape)             # <<<<<<<<<<<<<<
+ *   block_size = np.array(block_size)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_shape) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_shape);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF_SET(__pyx_v_shape, __pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "compressed_segmentation.pyx":294
+ * ) -> np.ndarray:
+ *   shape = np.array(shape)
+ *   block_size = np.array(block_size)             # <<<<<<<<<<<<<<
+ * 
+ *   grid_size = np.ceil(shape / block_size).astype(np.uint64)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_4);
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_block_size) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_block_size);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(__pyx_v_block_size, __pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "compressed_segmentation.pyx":296
+ *   block_size = np.array(block_size)
+ * 
+ *   grid_size = np.ceil(shape / block_size).astype(np.uint64)             # <<<<<<<<<<<<<<
+ *   cdef size_t num_headers = reduce(operator.mul, grid_size)
+ *   cdef size_t header_bytes = 8 * num_headers
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ceil); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_v_shape, __pyx_v_block_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_grid_size = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_grid_size = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-  /* "compressed_segmentation.pyx":243
+  /* "compressed_segmentation.pyx":297
  * 
  *   grid_size = np.ceil(shape / block_size).astype(np.uint64)
  *   cdef size_t num_headers = reduce(operator.mul, grid_size)             # <<<<<<<<<<<<<<
  *   cdef size_t header_bytes = 8 * num_headers
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_reduce); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_operator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_reduce); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mul); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_operator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  __pyx_t_8 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  __pyx_t_6 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-      __pyx_t_8 = 1;
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_grid_size};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyFunction_Check(__pyx_t_4)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_2, __pyx_v_grid_size};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_grid_size};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_2, __pyx_v_grid_size};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_4) {
-      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (__pyx_t_3) {
+      __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_grid_size);
     __Pyx_GIVEREF(__pyx_v_grid_size);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_grid_size);
-    __pyx_t_3 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_v_grid_size);
+    __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_9 = __Pyx_PyInt_As_size_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_num_headers = __pyx_t_9;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_7 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_7 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_num_headers = __pyx_t_7;
 
-  /* "compressed_segmentation.pyx":244
+  /* "compressed_segmentation.pyx":298
  *   grid_size = np.ceil(shape / block_size).astype(np.uint64)
  *   cdef size_t num_headers = reduce(operator.mul, grid_size)
  *   cdef size_t header_bytes = 8 * num_headers             # <<<<<<<<<<<<<<
  * 
  *   encoded = encoded[4:] # skip the channel length
  */
   __pyx_v_header_bytes = (8 * __pyx_v_num_headers);
 
-  /* "compressed_segmentation.pyx":246
+  /* "compressed_segmentation.pyx":300
  *   cdef size_t header_bytes = 8 * num_headers
  * 
  *   encoded = encoded[4:] # skip the channel length             # <<<<<<<<<<<<<<
  *   cdef np.ndarray[uint64_t] headers = np.frombuffer(encoded[:header_bytes], dtype=np.uint64)
  *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
  */
   if (unlikely(__pyx_v_encoded == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 246, __pyx_L1_error)
+    __PYX_ERR(0, 300, __pyx_L1_error)
   }
-  __pyx_t_5 = PySequence_GetSlice(__pyx_v_encoded, 4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF_SET(__pyx_v_encoded, ((PyObject*)__pyx_t_5));
-  __pyx_t_5 = 0;
+  __pyx_t_1 = PySequence_GetSlice(__pyx_v_encoded, 4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF_SET(__pyx_v_encoded, ((PyObject*)__pyx_t_1));
+  __pyx_t_1 = 0;
 
-  /* "compressed_segmentation.pyx":247
+  /* "compressed_segmentation.pyx":301
  * 
  *   encoded = encoded[4:] # skip the channel length
  *   cdef np.ndarray[uint64_t] headers = np.frombuffer(encoded[:header_bytes], dtype=np.uint64)             # <<<<<<<<<<<<<<
  *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PySequence_GetSlice(__pyx_v_encoded, 0, __pyx_v_header_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PySequence_GetSlice(__pyx_v_encoded, 0, __pyx_v_header_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 247, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 247, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 247, __pyx_L1_error)
-  __pyx_t_10 = ((PyArrayObject *)__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_8 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_headers.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_headers.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_headers = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 247, __pyx_L1_error)
+      __PYX_ERR(0, 301, __pyx_L1_error)
     } else {__pyx_pybuffernd_headers.diminfo[0].strides = __pyx_pybuffernd_headers.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_headers.diminfo[0].shape = __pyx_pybuffernd_headers.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_10 = 0;
-  __pyx_v_headers = ((PyArrayObject *)__pyx_t_4);
-  __pyx_t_4 = 0;
+  __pyx_t_8 = 0;
+  __pyx_v_headers = ((PyArrayObject *)__pyx_t_3);
+  __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":248
+  /* "compressed_segmentation.pyx":302
  *   encoded = encoded[4:] # skip the channel length
  *   cdef np.ndarray[uint64_t] headers = np.frombuffer(encoded[:header_bytes], dtype=np.uint64)
  *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
  *   cdef np.ndarray[uint32_t] offsets = np.zeros((2*num_headers,), dtype=np.uint32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_INCREF(__pyx_v_encoded);
-  __Pyx_GIVEREF(__pyx_v_encoded);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_encoded);
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 248, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_uint32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 302, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 302, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_v_encoded);
+  __Pyx_GIVEREF(__pyx_v_encoded);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_encoded);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 248, __pyx_L1_error)
-  __pyx_t_11 = ((PyArrayObject *)__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_9 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data.rcbuffer->pybuffer, (PyObject*)__pyx_t_11, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_data = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_data.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 248, __pyx_L1_error)
+      __PYX_ERR(0, 302, __pyx_L1_error)
     } else {__pyx_pybuffernd_data.diminfo[0].strides = __pyx_pybuffernd_data.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data.diminfo[0].shape = __pyx_pybuffernd_data.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_11 = 0;
-  __pyx_v_data = ((PyArrayObject *)__pyx_t_3);
-  __pyx_t_3 = 0;
+  __pyx_t_9 = 0;
+  __pyx_v_data = ((PyArrayObject *)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "compressed_segmentation.pyx":250
+  /* "compressed_segmentation.pyx":304
  *   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
  * 
  *   cdef np.ndarray[uint32_t] offsets = np.zeros((2*num_headers,), dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
  *   cdef size_t i = 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t((2 * __pyx_v_num_headers)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t((2 * __pyx_v_num_headers)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
-  __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 250, __pyx_L1_error)
-  __pyx_t_12 = ((PyArrayObject *)__pyx_t_6);
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_10 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_t_12, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_offsets = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 250, __pyx_L1_error)
+      __PYX_ERR(0, 304, __pyx_L1_error)
     } else {__pyx_pybuffernd_offsets.diminfo[0].strides = __pyx_pybuffernd_offsets.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_offsets.diminfo[0].shape = __pyx_pybuffernd_offsets.rcbuffer->pybuffer.shape[0];
     }
   }
-  __pyx_t_12 = 0;
-  __pyx_v_offsets = ((PyArrayObject *)__pyx_t_6);
-  __pyx_t_6 = 0;
+  __pyx_t_10 = 0;
+  __pyx_v_offsets = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
 
-  /* "compressed_segmentation.pyx":252
+  /* "compressed_segmentation.pyx":306
  *   cdef np.ndarray[uint32_t] offsets = np.zeros((2*num_headers,), dtype=np.uint32)
  * 
  *   cdef size_t i = 0             # <<<<<<<<<<<<<<
  *   cdef size_t lookup_table_offset = 0
  *   cdef size_t encoded_values_offset = 0
  */
   __pyx_v_i = 0;
 
-  /* "compressed_segmentation.pyx":253
+  /* "compressed_segmentation.pyx":307
  * 
  *   cdef size_t i = 0
  *   cdef size_t lookup_table_offset = 0             # <<<<<<<<<<<<<<
  *   cdef size_t encoded_values_offset = 0
  *   for i in range(num_headers):
  */
   __pyx_v_lookup_table_offset = 0;
 
-  /* "compressed_segmentation.pyx":254
+  /* "compressed_segmentation.pyx":308
  *   cdef size_t i = 0
  *   cdef size_t lookup_table_offset = 0
  *   cdef size_t encoded_values_offset = 0             # <<<<<<<<<<<<<<
  *   for i in range(num_headers):
  *     lookup_table_offset = headers[i] & 0xffffff
  */
   __pyx_v_encoded_values_offset = 0;
 
-  /* "compressed_segmentation.pyx":255
+  /* "compressed_segmentation.pyx":309
  *   cdef size_t lookup_table_offset = 0
  *   cdef size_t encoded_values_offset = 0
  *   for i in range(num_headers):             # <<<<<<<<<<<<<<
  *     lookup_table_offset = headers[i] & 0xffffff
  *     encoded_values_offset = headers[i] >> 32
  */
-  __pyx_t_9 = __pyx_v_num_headers;
-  __pyx_t_13 = __pyx_t_9;
-  for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
-    __pyx_v_i = __pyx_t_14;
+  __pyx_t_7 = __pyx_v_num_headers;
+  __pyx_t_11 = __pyx_t_7;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_i = __pyx_t_12;
 
-    /* "compressed_segmentation.pyx":256
+    /* "compressed_segmentation.pyx":310
  *   cdef size_t encoded_values_offset = 0
  *   for i in range(num_headers):
  *     lookup_table_offset = headers[i] & 0xffffff             # <<<<<<<<<<<<<<
  *     encoded_values_offset = headers[i] >> 32
  *     offsets[2 * i] = lookup_table_offset
  */
-    __pyx_t_15 = __pyx_v_i;
-    __pyx_t_8 = -1;
-    if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_headers.diminfo[0].shape)) __pyx_t_8 = 0;
-    if (unlikely(__pyx_t_8 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_8);
-      __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_13 = __pyx_v_i;
+    __pyx_t_6 = -1;
+    if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_headers.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (unlikely(__pyx_t_6 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_6);
+      __PYX_ERR(0, 310, __pyx_L1_error)
     }
-    __pyx_v_lookup_table_offset = ((*__Pyx_BufPtrStrided1d(uint64_t *, __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_headers.diminfo[0].strides)) & 0xffffff);
+    __pyx_v_lookup_table_offset = ((*__Pyx_BufPtrStrided1d(uint64_t *, __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_headers.diminfo[0].strides)) & 0xffffff);
 
-    /* "compressed_segmentation.pyx":257
+    /* "compressed_segmentation.pyx":311
  *   for i in range(num_headers):
  *     lookup_table_offset = headers[i] & 0xffffff
  *     encoded_values_offset = headers[i] >> 32             # <<<<<<<<<<<<<<
  *     offsets[2 * i] = lookup_table_offset
  *     offsets[2 * i + 1] = encoded_values_offset
  */
-    __pyx_t_15 = __pyx_v_i;
-    __pyx_t_8 = -1;
-    if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_headers.diminfo[0].shape)) __pyx_t_8 = 0;
-    if (unlikely(__pyx_t_8 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_8);
-      __PYX_ERR(0, 257, __pyx_L1_error)
+    __pyx_t_13 = __pyx_v_i;
+    __pyx_t_6 = -1;
+    if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_headers.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (unlikely(__pyx_t_6 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_6);
+      __PYX_ERR(0, 311, __pyx_L1_error)
     }
-    __pyx_v_encoded_values_offset = ((*__Pyx_BufPtrStrided1d(uint64_t *, __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_headers.diminfo[0].strides)) >> 32);
+    __pyx_v_encoded_values_offset = ((*__Pyx_BufPtrStrided1d(uint64_t *, __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_headers.diminfo[0].strides)) >> 32);
 
-    /* "compressed_segmentation.pyx":258
+    /* "compressed_segmentation.pyx":312
  *     lookup_table_offset = headers[i] & 0xffffff
  *     encoded_values_offset = headers[i] >> 32
  *     offsets[2 * i] = lookup_table_offset             # <<<<<<<<<<<<<<
  *     offsets[2 * i + 1] = encoded_values_offset
  * 
  */
-    __pyx_t_15 = (2 * __pyx_v_i);
-    __pyx_t_8 = -1;
-    if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_8 = 0;
-    if (unlikely(__pyx_t_8 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_8);
-      __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_13 = (2 * __pyx_v_i);
+    __pyx_t_6 = -1;
+    if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (unlikely(__pyx_t_6 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_6);
+      __PYX_ERR(0, 312, __pyx_L1_error)
     }
-    *__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_offsets.diminfo[0].strides) = __pyx_v_lookup_table_offset;
+    *__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_offsets.diminfo[0].strides) = __pyx_v_lookup_table_offset;
 
-    /* "compressed_segmentation.pyx":259
+    /* "compressed_segmentation.pyx":313
  *     encoded_values_offset = headers[i] >> 32
  *     offsets[2 * i] = lookup_table_offset
  *     offsets[2 * i + 1] = encoded_values_offset             # <<<<<<<<<<<<<<
  * 
  *   # use unique rather than simply sort b/c
  */
-    __pyx_t_15 = ((2 * __pyx_v_i) + 1);
-    __pyx_t_8 = -1;
-    if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_8 = 0;
-    if (unlikely(__pyx_t_8 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_8);
-      __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_13 = ((2 * __pyx_v_i) + 1);
+    __pyx_t_6 = -1;
+    if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (unlikely(__pyx_t_6 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_6);
+      __PYX_ERR(0, 313, __pyx_L1_error)
     }
-    *__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_offsets.diminfo[0].strides) = __pyx_v_encoded_values_offset;
+    *__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_offsets.diminfo[0].strides) = __pyx_v_encoded_values_offset;
   }
 
-  /* "compressed_segmentation.pyx":263
+  /* "compressed_segmentation.pyx":317
  *   # use unique rather than simply sort b/c
  *   # label offsets can be reused.
  *   offsets = np.unique(offsets)             # <<<<<<<<<<<<<<
  * 
  *   labels = np.zeros((0,), dtype=dtype)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unique); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_unique); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_offsets)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_offsets));
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 263, __pyx_L1_error)
-  __pyx_t_12 = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_offsets)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_offsets));
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_10 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer);
-    __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_t_12, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
-    if (unlikely(__pyx_t_8 < 0)) {
-      PyErr_Fetch(&__pyx_t_16, &__pyx_t_17, &__pyx_t_18);
+    __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
+    if (unlikely(__pyx_t_6 < 0)) {
+      PyErr_Fetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
       if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_v_offsets, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
-        Py_XDECREF(__pyx_t_16); Py_XDECREF(__pyx_t_17); Py_XDECREF(__pyx_t_18);
+        Py_XDECREF(__pyx_t_14); Py_XDECREF(__pyx_t_15); Py_XDECREF(__pyx_t_16);
         __Pyx_RaiseBufferFallbackError();
       } else {
-        PyErr_Restore(__pyx_t_16, __pyx_t_17, __pyx_t_18);
+        PyErr_Restore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
       }
-      __pyx_t_16 = __pyx_t_17 = __pyx_t_18 = 0;
+      __pyx_t_14 = __pyx_t_15 = __pyx_t_16 = 0;
     }
     __pyx_pybuffernd_offsets.diminfo[0].strides = __pyx_pybuffernd_offsets.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_offsets.diminfo[0].shape = __pyx_pybuffernd_offsets.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 317, __pyx_L1_error)
   }
-  __pyx_t_12 = 0;
-  __Pyx_DECREF_SET(__pyx_v_offsets, ((PyArrayObject *)__pyx_t_6));
-  __pyx_t_6 = 0;
+  __pyx_t_10 = 0;
+  __Pyx_DECREF_SET(__pyx_v_offsets, ((PyArrayObject *)__pyx_t_4));
+  __pyx_t_4 = 0;
 
-  /* "compressed_segmentation.pyx":265
+  /* "compressed_segmentation.pyx":319
  *   offsets = np.unique(offsets)
  * 
  *   labels = np.zeros((0,), dtype=dtype)             # <<<<<<<<<<<<<<
  * 
  *   cdef size_t dtype_bytes = np.dtype(dtype).itemsize
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_v_dtype) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__13, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_labels = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_v_dtype) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__13, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_labels = __pyx_t_3;
+  __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":267
+  /* "compressed_segmentation.pyx":321
  *   labels = np.zeros((0,), dtype=dtype)
  * 
  *   cdef size_t dtype_bytes = np.dtype(dtype).itemsize             # <<<<<<<<<<<<<<
  *   cdef size_t start = 0
  *   cdef size_t end = 0
  */
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5numpy_dtype), __pyx_v_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 267, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = ((PyArray_Descr *)__pyx_t_4)->elsize;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_v_dtype_bytes = __pyx_t_8;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5numpy_dtype), __pyx_v_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = ((PyArray_Descr *)__pyx_t_3)->elsize;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_dtype_bytes = __pyx_t_6;
 
-  /* "compressed_segmentation.pyx":268
+  /* "compressed_segmentation.pyx":322
  * 
  *   cdef size_t dtype_bytes = np.dtype(dtype).itemsize
  *   cdef size_t start = 0             # <<<<<<<<<<<<<<
  *   cdef size_t end = 0
  * 
  */
   __pyx_v_start = 0;
 
-  /* "compressed_segmentation.pyx":269
+  /* "compressed_segmentation.pyx":323
  *   cdef size_t dtype_bytes = np.dtype(dtype).itemsize
  *   cdef size_t start = 0
  *   cdef size_t end = 0             # <<<<<<<<<<<<<<
  * 
  *   cdef int64_t idx = 0
  */
   __pyx_v_end = 0;
 
-  /* "compressed_segmentation.pyx":271
+  /* "compressed_segmentation.pyx":325
  *   cdef size_t end = 0
  * 
  *   cdef int64_t idx = 0             # <<<<<<<<<<<<<<
  *   cdef int64_t size = offsets.size - 1
  * 
  */
   __pyx_v_idx = 0;
 
-  /* "compressed_segmentation.pyx":272
+  /* "compressed_segmentation.pyx":326
  * 
  *   cdef int64_t idx = 0
  *   cdef int64_t size = offsets.size - 1             # <<<<<<<<<<<<<<
  * 
  *   cdef np.ndarray[uint32_t, ndim=2] index = np.zeros((num_headers, 2), dtype=np.uint32)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_offsets), __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_offsets), __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_17 = __Pyx_PyInt_As_int64_t(__pyx_t_4); if (unlikely((__pyx_t_17 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_19 = __Pyx_PyInt_As_int64_t(__pyx_t_6); if (unlikely((__pyx_t_19 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 272, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_size = __pyx_t_19;
+  __pyx_v_size = __pyx_t_17;
 
-  /* "compressed_segmentation.pyx":274
+  /* "compressed_segmentation.pyx":328
  *   cdef int64_t size = offsets.size - 1
  * 
  *   cdef np.ndarray[uint32_t, ndim=2] index = np.zeros((num_headers, 2), dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
  *   for i in range(num_headers):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_num_headers); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_num_headers); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_2);
-  __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_2);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 274, __pyx_L1_error)
-  __pyx_t_20 = ((PyArrayObject *)__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_18 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_index.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_index.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_index = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_index.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 274, __pyx_L1_error)
+      __PYX_ERR(0, 328, __pyx_L1_error)
     } else {__pyx_pybuffernd_index.diminfo[0].strides = __pyx_pybuffernd_index.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_index.diminfo[0].shape = __pyx_pybuffernd_index.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_index.diminfo[1].strides = __pyx_pybuffernd_index.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_index.diminfo[1].shape = __pyx_pybuffernd_index.rcbuffer->pybuffer.shape[1];
     }
   }
-  __pyx_t_20 = 0;
-  __pyx_v_index = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
+  __pyx_t_18 = 0;
+  __pyx_v_index = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "compressed_segmentation.pyx":276
+  /* "compressed_segmentation.pyx":330
  *   cdef np.ndarray[uint32_t, ndim=2] index = np.zeros((num_headers, 2), dtype=np.uint32)
  * 
  *   for i in range(num_headers):             # <<<<<<<<<<<<<<
  *     lookup_table_offset = headers[i] & 0xffffff
  *     idx = _search(offsets, lookup_table_offset)
  */
-  __pyx_t_9 = __pyx_v_num_headers;
-  __pyx_t_13 = __pyx_t_9;
-  for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
-    __pyx_v_i = __pyx_t_14;
+  __pyx_t_7 = __pyx_v_num_headers;
+  __pyx_t_11 = __pyx_t_7;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_i = __pyx_t_12;
 
-    /* "compressed_segmentation.pyx":277
+    /* "compressed_segmentation.pyx":331
  * 
  *   for i in range(num_headers):
  *     lookup_table_offset = headers[i] & 0xffffff             # <<<<<<<<<<<<<<
  *     idx = _search(offsets, lookup_table_offset)
  *     if idx == -1:
  */
-    __pyx_t_15 = __pyx_v_i;
-    __pyx_t_8 = -1;
-    if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_headers.diminfo[0].shape)) __pyx_t_8 = 0;
-    if (unlikely(__pyx_t_8 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_8);
-      __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_13 = __pyx_v_i;
+    __pyx_t_6 = -1;
+    if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_headers.diminfo[0].shape)) __pyx_t_6 = 0;
+    if (unlikely(__pyx_t_6 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_6);
+      __PYX_ERR(0, 331, __pyx_L1_error)
     }
-    __pyx_v_lookup_table_offset = ((*__Pyx_BufPtrStrided1d(uint64_t *, __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_headers.diminfo[0].strides)) & 0xffffff);
+    __pyx_v_lookup_table_offset = ((*__Pyx_BufPtrStrided1d(uint64_t *, __pyx_pybuffernd_headers.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_headers.diminfo[0].strides)) & 0xffffff);
 
-    /* "compressed_segmentation.pyx":278
+    /* "compressed_segmentation.pyx":332
  *   for i in range(num_headers):
  *     lookup_table_offset = headers[i] & 0xffffff
  *     idx = _search(offsets, lookup_table_offset)             # <<<<<<<<<<<<<<
  *     if idx == -1:
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")
  */
     __pyx_v_idx = __pyx_f_23compressed_segmentation__search(((PyArrayObject *)__pyx_v_offsets), __pyx_v_lookup_table_offset);
 
-    /* "compressed_segmentation.pyx":279
+    /* "compressed_segmentation.pyx":333
  *     lookup_table_offset = headers[i] & 0xffffff
  *     idx = _search(offsets, lookup_table_offset)
  *     if idx == -1:             # <<<<<<<<<<<<<<
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")
  *     elif idx == size:
  */
-    __pyx_t_2 = ((__pyx_v_idx == -1L) != 0);
-    if (unlikely(__pyx_t_2)) {
+    __pyx_t_19 = ((__pyx_v_idx == -1L) != 0);
+    if (unlikely(__pyx_t_19)) {
 
-      /* "compressed_segmentation.pyx":280
+      /* "compressed_segmentation.pyx":334
  *     idx = _search(offsets, lookup_table_offset)
  *     if idx == -1:
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")             # <<<<<<<<<<<<<<
  *     elif idx == size:
  *       index[i, 0] = offsets[idx]
  */
-      __pyx_t_5 = __Pyx_PyUnicode_From_size_t(__pyx_v_lookup_table_offset, 0, ' ', 'd'); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 280, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unable_to_locate_value, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 280, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 280, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 280, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyUnicode_From_size_t(__pyx_v_lookup_table_offset, 0, ' ', 'd'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unable_to_locate_value, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __PYX_ERR(0, 334, __pyx_L1_error)
 
-      /* "compressed_segmentation.pyx":279
+      /* "compressed_segmentation.pyx":333
  *     lookup_table_offset = headers[i] & 0xffffff
  *     idx = _search(offsets, lookup_table_offset)
  *     if idx == -1:             # <<<<<<<<<<<<<<
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")
  *     elif idx == size:
  */
     }
 
-    /* "compressed_segmentation.pyx":281
+    /* "compressed_segmentation.pyx":335
  *     if idx == -1:
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")
  *     elif idx == size:             # <<<<<<<<<<<<<<
  *       index[i, 0] = offsets[idx]
  *       index[i, 1] = data.size
  */
-    __pyx_t_2 = ((__pyx_v_idx == __pyx_v_size) != 0);
-    if (__pyx_t_2) {
+    __pyx_t_19 = ((__pyx_v_idx == __pyx_v_size) != 0);
+    if (__pyx_t_19) {
 
-      /* "compressed_segmentation.pyx":282
+      /* "compressed_segmentation.pyx":336
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")
  *     elif idx == size:
  *       index[i, 0] = offsets[idx]             # <<<<<<<<<<<<<<
  *       index[i, 1] = data.size
  *     else:
  */
-      __pyx_t_21 = __pyx_v_idx;
-      __pyx_t_8 = -1;
+      __pyx_t_20 = __pyx_v_idx;
+      __pyx_t_6 = -1;
+      if (__pyx_t_20 < 0) {
+        __pyx_t_20 += __pyx_pybuffernd_offsets.diminfo[0].shape;
+        if (unlikely(__pyx_t_20 < 0)) __pyx_t_6 = 0;
+      } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_6 = 0;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 336, __pyx_L1_error)
+      }
+      __pyx_t_13 = __pyx_v_i;
+      __pyx_t_21 = 0;
+      __pyx_t_6 = -1;
+      if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_6 = 0;
       if (__pyx_t_21 < 0) {
-        __pyx_t_21 += __pyx_pybuffernd_offsets.diminfo[0].shape;
-        if (unlikely(__pyx_t_21 < 0)) __pyx_t_8 = 0;
-      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 282, __pyx_L1_error)
-      }
-      __pyx_t_15 = __pyx_v_i;
-      __pyx_t_22 = 0;
-      __pyx_t_8 = -1;
-      if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (__pyx_t_22 < 0) {
-        __pyx_t_22 += __pyx_pybuffernd_index.diminfo[1].shape;
-        if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 1;
-      } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_8 = 1;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 282, __pyx_L1_error)
+        __pyx_t_21 += __pyx_pybuffernd_index.diminfo[1].shape;
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_6 = 1;
+      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_6 = 1;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 336, __pyx_L1_error)
       }
-      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_index.diminfo[1].strides) = (*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_offsets.diminfo[0].strides));
+      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_21, __pyx_pybuffernd_index.diminfo[1].strides) = (*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_offsets.diminfo[0].strides));
 
-      /* "compressed_segmentation.pyx":283
+      /* "compressed_segmentation.pyx":337
  *     elif idx == size:
  *       index[i, 0] = offsets[idx]
  *       index[i, 1] = data.size             # <<<<<<<<<<<<<<
  *     else:
  *       index[i, 0] = offsets[idx]
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 283, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_23 = __Pyx_PyInt_As_uint32_t(__pyx_t_5); if (unlikely((__pyx_t_23 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_15 = __pyx_v_i;
-      __pyx_t_21 = 1;
-      __pyx_t_8 = -1;
-      if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (__pyx_t_21 < 0) {
-        __pyx_t_21 += __pyx_pybuffernd_index.diminfo[1].shape;
-        if (unlikely(__pyx_t_21 < 0)) __pyx_t_8 = 1;
-      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_8 = 1;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_22 = __Pyx_PyInt_As_uint32_t(__pyx_t_1); if (unlikely((__pyx_t_22 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 337, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_13 = __pyx_v_i;
+      __pyx_t_20 = 1;
+      __pyx_t_6 = -1;
+      if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_6 = 0;
+      if (__pyx_t_20 < 0) {
+        __pyx_t_20 += __pyx_pybuffernd_index.diminfo[1].shape;
+        if (unlikely(__pyx_t_20 < 0)) __pyx_t_6 = 1;
+      } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_6 = 1;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 337, __pyx_L1_error)
       }
-      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_21, __pyx_pybuffernd_index.diminfo[1].strides) = __pyx_t_23;
+      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_20, __pyx_pybuffernd_index.diminfo[1].strides) = __pyx_t_22;
 
-      /* "compressed_segmentation.pyx":281
+      /* "compressed_segmentation.pyx":335
  *     if idx == -1:
  *       raise IndexError(f"Unable to locate value: {lookup_table_offset}")
  *     elif idx == size:             # <<<<<<<<<<<<<<
  *       index[i, 0] = offsets[idx]
  *       index[i, 1] = data.size
  */
-      goto __pyx_L10;
+      goto __pyx_L7;
     }
 
-    /* "compressed_segmentation.pyx":285
+    /* "compressed_segmentation.pyx":339
  *       index[i, 1] = data.size
  *     else:
  *       index[i, 0] = offsets[idx]             # <<<<<<<<<<<<<<
  *       index[i, 1] = offsets[idx+1]
  * 
  */
     /*else*/ {
-      __pyx_t_21 = __pyx_v_idx;
-      __pyx_t_8 = -1;
+      __pyx_t_20 = __pyx_v_idx;
+      __pyx_t_6 = -1;
+      if (__pyx_t_20 < 0) {
+        __pyx_t_20 += __pyx_pybuffernd_offsets.diminfo[0].shape;
+        if (unlikely(__pyx_t_20 < 0)) __pyx_t_6 = 0;
+      } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_6 = 0;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 339, __pyx_L1_error)
+      }
+      __pyx_t_13 = __pyx_v_i;
+      __pyx_t_21 = 0;
+      __pyx_t_6 = -1;
+      if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_6 = 0;
       if (__pyx_t_21 < 0) {
-        __pyx_t_21 += __pyx_pybuffernd_offsets.diminfo[0].shape;
-        if (unlikely(__pyx_t_21 < 0)) __pyx_t_8 = 0;
-      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 285, __pyx_L1_error)
-      }
-      __pyx_t_15 = __pyx_v_i;
-      __pyx_t_22 = 0;
-      __pyx_t_8 = -1;
-      if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (__pyx_t_22 < 0) {
-        __pyx_t_22 += __pyx_pybuffernd_index.diminfo[1].shape;
-        if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 1;
-      } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_8 = 1;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 285, __pyx_L1_error)
+        __pyx_t_21 += __pyx_pybuffernd_index.diminfo[1].shape;
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_6 = 1;
+      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_6 = 1;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 339, __pyx_L1_error)
       }
-      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_index.diminfo[1].strides) = (*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_offsets.diminfo[0].strides));
+      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_21, __pyx_pybuffernd_index.diminfo[1].strides) = (*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_offsets.diminfo[0].strides));
 
-      /* "compressed_segmentation.pyx":286
+      /* "compressed_segmentation.pyx":340
  *     else:
  *       index[i, 0] = offsets[idx]
  *       index[i, 1] = offsets[idx+1]             # <<<<<<<<<<<<<<
  * 
- *   labels = np.concatenate([
- */
-      __pyx_t_21 = (__pyx_v_idx + 1);
-      __pyx_t_8 = -1;
-      if (__pyx_t_21 < 0) {
-        __pyx_t_21 += __pyx_pybuffernd_offsets.diminfo[0].shape;
-        if (unlikely(__pyx_t_21 < 0)) __pyx_t_8 = 0;
-      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 286, __pyx_L1_error)
-      }
-      __pyx_t_15 = __pyx_v_i;
-      __pyx_t_22 = 1;
-      __pyx_t_8 = -1;
-      if (unlikely(__pyx_t_15 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (__pyx_t_22 < 0) {
-        __pyx_t_22 += __pyx_pybuffernd_index.diminfo[1].shape;
-        if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 1;
-      } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_8 = 1;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 286, __pyx_L1_error)
-      }
-      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_index.diminfo[1].strides) = (*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_offsets.diminfo[0].strides));
-    }
-    __pyx_L10:;
-  }
-
-  /* "compressed_segmentation.pyx":288
- *       index[i, 1] = offsets[idx+1]
- * 
- *   labels = np.concatenate([             # <<<<<<<<<<<<<<
- *     data[index[idx,0]:index[idx,1]]
- *     for idx in range(num_headers)
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_concatenate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 288, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-
-    /* "compressed_segmentation.pyx":290
- *   labels = np.concatenate([
- *     data[index[idx,0]:index[idx,1]]
- *     for idx in range(num_headers)             # <<<<<<<<<<<<<<
- *   ]).view(dtype)
- * 
- */
-    __pyx_t_9 = __pyx_v_num_headers;
-    __pyx_t_13 = __pyx_t_9;
-    for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_13; __pyx_t_19+=1) {
-      __pyx_8genexpr2__pyx_v_idx = __pyx_t_19;
-
-      /* "compressed_segmentation.pyx":289
- * 
- *   labels = np.concatenate([
- *     data[index[idx,0]:index[idx,1]]             # <<<<<<<<<<<<<<
- *     for idx in range(num_headers)
- *   ]).view(dtype)
+ *   return index
  */
-      __pyx_t_21 = __pyx_8genexpr2__pyx_v_idx;
-      __pyx_t_22 = 0;
-      __pyx_t_8 = -1;
-      if (__pyx_t_21 < 0) {
-        __pyx_t_21 += __pyx_pybuffernd_index.diminfo[0].shape;
-        if (unlikely(__pyx_t_21 < 0)) __pyx_t_8 = 0;
-      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_8 = 0;
-      if (__pyx_t_22 < 0) {
-        __pyx_t_22 += __pyx_pybuffernd_index.diminfo[1].shape;
-        if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 1;
-      } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_8 = 1;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 289, __pyx_L1_error)
+      __pyx_t_20 = (__pyx_v_idx + 1);
+      __pyx_t_6 = -1;
+      if (__pyx_t_20 < 0) {
+        __pyx_t_20 += __pyx_pybuffernd_offsets.diminfo[0].shape;
+        if (unlikely(__pyx_t_20 < 0)) __pyx_t_6 = 0;
+      } else if (unlikely(__pyx_t_20 >= __pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_6 = 0;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 340, __pyx_L1_error)
       }
-      __pyx_t_7 = __Pyx_PyInt_From_uint32_t((*__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_index.diminfo[1].strides))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 289, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_22 = __pyx_8genexpr2__pyx_v_idx;
+      __pyx_t_13 = __pyx_v_i;
       __pyx_t_21 = 1;
-      __pyx_t_8 = -1;
-      if (__pyx_t_22 < 0) {
-        __pyx_t_22 += __pyx_pybuffernd_index.diminfo[0].shape;
-        if (unlikely(__pyx_t_22 < 0)) __pyx_t_8 = 0;
-      } else if (unlikely(__pyx_t_22 >= __pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_8 = 0;
+      __pyx_t_6 = -1;
+      if (unlikely(__pyx_t_13 >= (size_t)__pyx_pybuffernd_index.diminfo[0].shape)) __pyx_t_6 = 0;
       if (__pyx_t_21 < 0) {
         __pyx_t_21 += __pyx_pybuffernd_index.diminfo[1].shape;
-        if (unlikely(__pyx_t_21 < 0)) __pyx_t_8 = 1;
-      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_8 = 1;
-      if (unlikely(__pyx_t_8 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_8);
-        __PYX_ERR(0, 289, __pyx_L1_error)
-      }
-      __pyx_t_24 = __Pyx_PyInt_From_uint32_t((*__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_21, __pyx_pybuffernd_index.diminfo[1].strides))); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 289, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_24);
-      __pyx_t_25 = PySlice_New(__pyx_t_7, __pyx_t_24, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 289, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_25);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-      __pyx_t_24 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_data), __pyx_t_25); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 289, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_24);
-      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_24))) __PYX_ERR(0, 288, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-    }
-  } /* exit inner scope */
-  __pyx_t_24 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_24 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_24)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_24);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-    }
-  }
-  __pyx_t_3 = (__pyx_t_24) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_24, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_24); __pyx_t_24 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-
-  /* "compressed_segmentation.pyx":291
- *     data[index[idx,0]:index[idx,1]]
- *     for idx in range(num_headers)
- *   ]).view(dtype)             # <<<<<<<<<<<<<<
- * 
- *   return np.unique(labels)
- */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_view); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_6 = 1;
+      } else if (unlikely(__pyx_t_21 >= __pyx_pybuffernd_index.diminfo[1].shape)) __pyx_t_6 = 1;
+      if (unlikely(__pyx_t_6 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_6);
+        __PYX_ERR(0, 340, __pyx_L1_error)
+      }
+      *__Pyx_BufPtrStrided2d(uint32_t *, __pyx_pybuffernd_index.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_index.diminfo[0].strides, __pyx_t_21, __pyx_pybuffernd_index.diminfo[1].strides) = (*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_offsets.diminfo[0].strides));
     }
+    __pyx_L7:;
   }
-  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_dtype) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_dtype);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_5);
-  __pyx_t_5 = 0;
 
-  /* "compressed_segmentation.pyx":293
- *   ]).view(dtype)
+  /* "compressed_segmentation.pyx":342
+ *       index[i, 1] = offsets[idx+1]
  * 
- *   return np.unique(labels)             # <<<<<<<<<<<<<<
+ *   return index             # <<<<<<<<<<<<<<
  * 
  * cdef int64_t _search(np.ndarray[uint32_t] offsets, uint32_t value):
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unique); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_labels) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_labels);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __Pyx_XDECREF(((PyObject *)__pyx_r));
+  __Pyx_INCREF(((PyObject *)__pyx_v_index));
+  __pyx_r = ((PyArrayObject *)__pyx_v_index);
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":224
- *     raise TypeError("dtype ({}) must be one of uint32 or uint64.".format(dtype))
+  /* "compressed_segmentation.pyx":290
+ *   return channel_length + data.tobytes()
  * 
- * def labels(             # <<<<<<<<<<<<<<
- *   bytes encoded, shape, dtype,
- *   block_size=DEFAULT_BLOCK_SIZE
+ * def _compute_label_offsets(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype, block_size
+ * ) -> np.ndarray:
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_24);
-  __Pyx_XDECREF(__pyx_t_25);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_headers.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_index.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("compressed_segmentation.labels", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("compressed_segmentation._compute_label_offsets", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_headers.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_index.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer);
@@ -6736,21 +8154,21 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_data);
   __Pyx_XDECREF((PyObject *)__pyx_v_offsets);
   __Pyx_XDECREF(__pyx_v_labels);
   __Pyx_XDECREF((PyObject *)__pyx_v_index);
   __Pyx_XDECREF(__pyx_v_encoded);
   __Pyx_XDECREF(__pyx_v_shape);
   __Pyx_XDECREF(__pyx_v_block_size);
-  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":295
- *   return np.unique(labels)
+/* "compressed_segmentation.pyx":344
+ *   return index
  * 
  * cdef int64_t _search(np.ndarray[uint32_t] offsets, uint32_t value):             # <<<<<<<<<<<<<<
  *   cdef size_t first = 0
  *   cdef size_t last = offsets.size - 1
  */
 
 static int64_t __pyx_f_23compressed_segmentation__search(PyArrayObject *__pyx_v_offsets, uint32_t __pyx_v_value) {
@@ -6772,241 +8190,241 @@
   __Pyx_RefNannySetupContext("_search", 0);
   __pyx_pybuffer_offsets.pybuffer.buf = NULL;
   __pyx_pybuffer_offsets.refcount = 0;
   __pyx_pybuffernd_offsets.data = NULL;
   __pyx_pybuffernd_offsets.rcbuffer = &__pyx_pybuffer_offsets;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_v_offsets, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 295, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer, (PyObject*)__pyx_v_offsets, &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 344, __pyx_L1_error)
   }
   __pyx_pybuffernd_offsets.diminfo[0].strides = __pyx_pybuffernd_offsets.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_offsets.diminfo[0].shape = __pyx_pybuffernd_offsets.rcbuffer->pybuffer.shape[0];
 
-  /* "compressed_segmentation.pyx":296
+  /* "compressed_segmentation.pyx":345
  * 
  * cdef int64_t _search(np.ndarray[uint32_t] offsets, uint32_t value):
  *   cdef size_t first = 0             # <<<<<<<<<<<<<<
  *   cdef size_t last = offsets.size - 1
  *   cdef size_t middle = (first // 2 + last // 2)
  */
   __pyx_v_first = 0;
 
-  /* "compressed_segmentation.pyx":297
+  /* "compressed_segmentation.pyx":346
  * cdef int64_t _search(np.ndarray[uint32_t] offsets, uint32_t value):
  *   cdef size_t first = 0
  *   cdef size_t last = offsets.size - 1             # <<<<<<<<<<<<<<
  *   cdef size_t middle = (first // 2 + last // 2)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_offsets), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_offsets), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_last = __pyx_t_3;
 
-  /* "compressed_segmentation.pyx":298
+  /* "compressed_segmentation.pyx":347
  *   cdef size_t first = 0
  *   cdef size_t last = offsets.size - 1
  *   cdef size_t middle = (first // 2 + last // 2)             # <<<<<<<<<<<<<<
  * 
  *   while (last - first) > 1:
  */
   __pyx_v_middle = ((__pyx_v_first / 2) + (__pyx_v_last / 2));
 
-  /* "compressed_segmentation.pyx":300
+  /* "compressed_segmentation.pyx":349
  *   cdef size_t middle = (first // 2 + last // 2)
  * 
  *   while (last - first) > 1:             # <<<<<<<<<<<<<<
  *     if offsets[middle] == value:
  *       return middle
  */
   while (1) {
     __pyx_t_4 = (((__pyx_v_last - __pyx_v_first) > 1) != 0);
     if (!__pyx_t_4) break;
 
-    /* "compressed_segmentation.pyx":301
+    /* "compressed_segmentation.pyx":350
  * 
  *   while (last - first) > 1:
  *     if offsets[middle] == value:             # <<<<<<<<<<<<<<
  *       return middle
  *     elif offsets[middle] > value:
  */
     __pyx_t_3 = __pyx_v_middle;
     __pyx_t_5 = -1;
     if (unlikely(__pyx_t_3 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_5 = 0;
     if (unlikely(__pyx_t_5 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_5);
-      __PYX_ERR(0, 301, __pyx_L1_error)
+      __PYX_ERR(0, 350, __pyx_L1_error)
     }
     __pyx_t_4 = (((*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_offsets.diminfo[0].strides)) == __pyx_v_value) != 0);
     if (__pyx_t_4) {
 
-      /* "compressed_segmentation.pyx":302
+      /* "compressed_segmentation.pyx":351
  *   while (last - first) > 1:
  *     if offsets[middle] == value:
  *       return middle             # <<<<<<<<<<<<<<
  *     elif offsets[middle] > value:
  *       last = middle
  */
       __pyx_r = __pyx_v_middle;
       goto __pyx_L0;
 
-      /* "compressed_segmentation.pyx":301
+      /* "compressed_segmentation.pyx":350
  * 
  *   while (last - first) > 1:
  *     if offsets[middle] == value:             # <<<<<<<<<<<<<<
  *       return middle
  *     elif offsets[middle] > value:
  */
     }
 
-    /* "compressed_segmentation.pyx":303
+    /* "compressed_segmentation.pyx":352
  *     if offsets[middle] == value:
  *       return middle
  *     elif offsets[middle] > value:             # <<<<<<<<<<<<<<
  *       last = middle
  *     else:
  */
     __pyx_t_3 = __pyx_v_middle;
     __pyx_t_5 = -1;
     if (unlikely(__pyx_t_3 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_5 = 0;
     if (unlikely(__pyx_t_5 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_5);
-      __PYX_ERR(0, 303, __pyx_L1_error)
+      __PYX_ERR(0, 352, __pyx_L1_error)
     }
     __pyx_t_4 = (((*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_offsets.diminfo[0].strides)) > __pyx_v_value) != 0);
     if (__pyx_t_4) {
 
-      /* "compressed_segmentation.pyx":304
+      /* "compressed_segmentation.pyx":353
  *       return middle
  *     elif offsets[middle] > value:
  *       last = middle             # <<<<<<<<<<<<<<
  *     else:
  *       first = middle
  */
       __pyx_v_last = __pyx_v_middle;
 
-      /* "compressed_segmentation.pyx":303
+      /* "compressed_segmentation.pyx":352
  *     if offsets[middle] == value:
  *       return middle
  *     elif offsets[middle] > value:             # <<<<<<<<<<<<<<
  *       last = middle
  *     else:
  */
       goto __pyx_L5;
     }
 
-    /* "compressed_segmentation.pyx":306
+    /* "compressed_segmentation.pyx":355
  *       last = middle
  *     else:
  *       first = middle             # <<<<<<<<<<<<<<
  * 
  *     middle = (first // 2 + last // 2 + ((first & 0b1) + (last & 0b1)) // 2)
  */
     /*else*/ {
       __pyx_v_first = __pyx_v_middle;
     }
     __pyx_L5:;
 
-    /* "compressed_segmentation.pyx":308
+    /* "compressed_segmentation.pyx":357
  *       first = middle
  * 
  *     middle = (first // 2 + last // 2 + ((first & 0b1) + (last & 0b1)) // 2)             # <<<<<<<<<<<<<<
  * 
  *   if offsets[first] == value:
  */
     __pyx_v_middle = (((__pyx_v_first / 2) + (__pyx_v_last / 2)) + (((__pyx_v_first & 1) + (__pyx_v_last & 1)) / 2));
   }
 
-  /* "compressed_segmentation.pyx":310
+  /* "compressed_segmentation.pyx":359
  *     middle = (first // 2 + last // 2 + ((first & 0b1) + (last & 0b1)) // 2)
  * 
  *   if offsets[first] == value:             # <<<<<<<<<<<<<<
  *     return first
  * 
  */
   __pyx_t_3 = __pyx_v_first;
   __pyx_t_5 = -1;
   if (unlikely(__pyx_t_3 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_5 = 0;
   if (unlikely(__pyx_t_5 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 310, __pyx_L1_error)
+    __PYX_ERR(0, 359, __pyx_L1_error)
   }
   __pyx_t_4 = (((*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_offsets.diminfo[0].strides)) == __pyx_v_value) != 0);
   if (__pyx_t_4) {
 
-    /* "compressed_segmentation.pyx":311
+    /* "compressed_segmentation.pyx":360
  * 
  *   if offsets[first] == value:
  *     return first             # <<<<<<<<<<<<<<
  * 
  *   if offsets[last] == value:
  */
     __pyx_r = __pyx_v_first;
     goto __pyx_L0;
 
-    /* "compressed_segmentation.pyx":310
+    /* "compressed_segmentation.pyx":359
  *     middle = (first // 2 + last // 2 + ((first & 0b1) + (last & 0b1)) // 2)
  * 
  *   if offsets[first] == value:             # <<<<<<<<<<<<<<
  *     return first
  * 
  */
   }
 
-  /* "compressed_segmentation.pyx":313
+  /* "compressed_segmentation.pyx":362
  *     return first
  * 
  *   if offsets[last] == value:             # <<<<<<<<<<<<<<
  *     return last
  * 
  */
   __pyx_t_3 = __pyx_v_last;
   __pyx_t_5 = -1;
   if (unlikely(__pyx_t_3 >= (size_t)__pyx_pybuffernd_offsets.diminfo[0].shape)) __pyx_t_5 = 0;
   if (unlikely(__pyx_t_5 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_5);
-    __PYX_ERR(0, 313, __pyx_L1_error)
+    __PYX_ERR(0, 362, __pyx_L1_error)
   }
   __pyx_t_4 = (((*__Pyx_BufPtrStrided1d(uint32_t *, __pyx_pybuffernd_offsets.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_offsets.diminfo[0].strides)) == __pyx_v_value) != 0);
   if (__pyx_t_4) {
 
-    /* "compressed_segmentation.pyx":314
+    /* "compressed_segmentation.pyx":363
  * 
  *   if offsets[last] == value:
  *     return last             # <<<<<<<<<<<<<<
  * 
  *   return -1
  */
     __pyx_r = __pyx_v_last;
     goto __pyx_L0;
 
-    /* "compressed_segmentation.pyx":313
+    /* "compressed_segmentation.pyx":362
  *     return first
  * 
  *   if offsets[last] == value:             # <<<<<<<<<<<<<<
  *     return last
  * 
  */
   }
 
-  /* "compressed_segmentation.pyx":316
+  /* "compressed_segmentation.pyx":365
  *     return last
  * 
  *   return -1             # <<<<<<<<<<<<<<
  * 
  * class CompressedSegmentationArray:
  */
   __pyx_r = -1L;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":295
- *   return np.unique(labels)
+  /* "compressed_segmentation.pyx":344
+ *   return index
  * 
  * cdef int64_t _search(np.ndarray[uint32_t] offsets, uint32_t value):             # <<<<<<<<<<<<<<
  *   cdef size_t first = 0
  *   cdef size_t last = offsets.size - 1
  */
 
   /* function exit code */
@@ -7025,38 +8443,38 @@
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_offsets.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":319
+/* "compressed_segmentation.pyx":368
  * 
  * class CompressedSegmentationArray:
  *   def __init__(             # <<<<<<<<<<<<<<
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  *   ):
  */
 
-static PyObject *__pyx_pf_23compressed_segmentation_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_23compressed_segmentation_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_block_size);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_block_size);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_block_size);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -7118,37 +8536,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_binary)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 1); __PYX_ERR(0, 319, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 1); __PYX_ERR(0, 368, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 2); __PYX_ERR(0, 319, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 2); __PYX_ERR(0, 368, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 3); __PYX_ERR(0, 319, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 3); __PYX_ERR(0, 368, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_block_size);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 319, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 368, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -7162,15 +8580,15 @@
     __pyx_v_binary = values[1];
     __pyx_v_shape = values[2];
     __pyx_v_dtype = values[3];
     __pyx_v_block_size = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 319, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 368, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("compressed_segmentation.CompressedSegmentationArray.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray___init__(__pyx_self, __pyx_v_self, __pyx_v_binary, __pyx_v_shape, __pyx_v_dtype, __pyx_v_block_size);
 
@@ -7188,113 +8606,113 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "compressed_segmentation.pyx":322
+  /* "compressed_segmentation.pyx":371
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  *   ):
  *     self.binary = binary             # <<<<<<<<<<<<<<
  *     self.shape = np.array(shape, dtype=np.int64)
  *     self.dtype = np.dtype(dtype)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_binary, __pyx_v_binary) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_binary, __pyx_v_binary) < 0) __PYX_ERR(0, 371, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":323
+  /* "compressed_segmentation.pyx":372
  *   ):
  *     self.binary = binary
  *     self.shape = np.array(shape, dtype=np.int64)             # <<<<<<<<<<<<<<
  *     self.dtype = np.dtype(dtype)
  *     self.block_size = np.array(block_size, dtype=np.int64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_shape);
   __Pyx_GIVEREF(__pyx_v_shape);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_shape);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_shape, __pyx_t_5) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_shape, __pyx_t_5) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "compressed_segmentation.pyx":324
+  /* "compressed_segmentation.pyx":373
  *     self.binary = binary
  *     self.shape = np.array(shape, dtype=np.int64)
  *     self.dtype = np.dtype(dtype)             # <<<<<<<<<<<<<<
  *     self.block_size = np.array(block_size, dtype=np.int64)
  *     self._labels = None
  */
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5numpy_dtype), __pyx_v_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5numpy_dtype), __pyx_v_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 324, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "compressed_segmentation.pyx":325
+  /* "compressed_segmentation.pyx":374
  *     self.shape = np.array(shape, dtype=np.int64)
  *     self.dtype = np.dtype(dtype)
  *     self.block_size = np.array(block_size, dtype=np.int64)             # <<<<<<<<<<<<<<
  *     self._labels = None
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_block_size);
   __Pyx_GIVEREF(__pyx_v_block_size);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_block_size);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_block_size, __pyx_t_4) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_block_size, __pyx_t_4) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "compressed_segmentation.pyx":326
+  /* "compressed_segmentation.pyx":375
  *     self.dtype = np.dtype(dtype)
  *     self.block_size = np.array(block_size, dtype=np.int64)
  *     self._labels = None             # <<<<<<<<<<<<<<
  * 
  *   @property
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, Py_None) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, Py_None) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":319
+  /* "compressed_segmentation.pyx":368
  * 
  * class CompressedSegmentationArray:
  *   def __init__(             # <<<<<<<<<<<<<<
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  *   ):
  */
 
@@ -7311,15 +8729,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":329
+/* "compressed_segmentation.pyx":378
  * 
  *   @property
  *   def grid_size(self):             # <<<<<<<<<<<<<<
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  */
 
@@ -7347,32 +8765,32 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("grid_size", 0);
 
-  /* "compressed_segmentation.pyx":330
+  /* "compressed_segmentation.pyx":379
  *   @property
  *   def grid_size(self):
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)             # <<<<<<<<<<<<<<
  * 
  *   def labels(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ceil); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ceil); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
@@ -7381,23 +8799,23 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7405,22 +8823,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":329
+  /* "compressed_segmentation.pyx":378
  * 
  *   @property
  *   def grid_size(self):             # <<<<<<<<<<<<<<
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  */
 
@@ -7436,15 +8854,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":332
+/* "compressed_segmentation.pyx":381
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  *   def labels(self):             # <<<<<<<<<<<<<<
  *     if self._labels is None:
  *       self._labels = labels(
  */
 
@@ -7472,130 +8890,130 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("labels", 0);
 
-  /* "compressed_segmentation.pyx":333
+  /* "compressed_segmentation.pyx":382
  * 
  *   def labels(self):
  *     if self._labels is None:             # <<<<<<<<<<<<<<
  *       self._labels = labels(
  *         self.binary, shape=self.shape,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "compressed_segmentation.pyx":334
+    /* "compressed_segmentation.pyx":383
  *   def labels(self):
  *     if self._labels is None:
  *       self._labels = labels(             # <<<<<<<<<<<<<<
  *         self.binary, shape=self.shape,
  *         dtype=self.dtype, block_size=self.block_size
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_labels_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_labels_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "compressed_segmentation.pyx":335
+    /* "compressed_segmentation.pyx":384
  *     if self._labels is None:
  *       self._labels = labels(
  *         self.binary, shape=self.shape,             # <<<<<<<<<<<<<<
  *         dtype=self.dtype, block_size=self.block_size
  *       )
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
 
-    /* "compressed_segmentation.pyx":334
+    /* "compressed_segmentation.pyx":383
  *   def labels(self):
  *     if self._labels is None:
  *       self._labels = labels(             # <<<<<<<<<<<<<<
  *         self.binary, shape=self.shape,
  *         dtype=self.dtype, block_size=self.block_size
  */
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "compressed_segmentation.pyx":335
+    /* "compressed_segmentation.pyx":384
  *     if self._labels is None:
  *       self._labels = labels(
  *         self.binary, shape=self.shape,             # <<<<<<<<<<<<<<
  *         dtype=self.dtype, block_size=self.block_size
  *       )
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_6) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_6) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "compressed_segmentation.pyx":336
+    /* "compressed_segmentation.pyx":385
  *       self._labels = labels(
  *         self.binary, shape=self.shape,
  *         dtype=self.dtype, block_size=self.block_size             # <<<<<<<<<<<<<<
  *       )
  *     return self._labels
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_block_size, __pyx_t_6) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_block_size, __pyx_t_6) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "compressed_segmentation.pyx":334
+    /* "compressed_segmentation.pyx":383
  *   def labels(self):
  *     if self._labels is None:
  *       self._labels = labels(             # <<<<<<<<<<<<<<
  *         self.binary, shape=self.shape,
  *         dtype=self.dtype, block_size=self.block_size
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 334, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_6) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_6) < 0) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "compressed_segmentation.pyx":333
+    /* "compressed_segmentation.pyx":382
  * 
  *   def labels(self):
  *     if self._labels is None:             # <<<<<<<<<<<<<<
  *       self._labels = labels(
  *         self.binary, shape=self.shape,
  */
   }
 
-  /* "compressed_segmentation.pyx":338
+  /* "compressed_segmentation.pyx":387
  *         dtype=self.dtype, block_size=self.block_size
  *       )
  *     return self._labels             # <<<<<<<<<<<<<<
  * 
- *   def numpy(self):
+ *   def remap(self, mapping, preserve_missing_labels=False):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":332
+  /* "compressed_segmentation.pyx":381
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  *   def labels(self):             # <<<<<<<<<<<<<<
  *     if self._labels is None:
  *       self._labels = labels(
  */
 
@@ -7609,37 +9027,271 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":340
+/* "compressed_segmentation.pyx":389
+ *     return self._labels
+ * 
+ *   def remap(self, mapping, preserve_missing_labels=False):             # <<<<<<<<<<<<<<
+ *     return remap(
+ *       self.binary, self.shape, self.dtype,
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_7remap(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_7remap = {"remap", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_7remap, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_7remap(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_self = 0;
+  PyObject *__pyx_v_mapping = 0;
+  PyObject *__pyx_v_preserve_missing_labels = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("remap (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_mapping,&__pyx_n_s_preserve_missing_labels,0};
+    PyObject* values[3] = {0,0,0};
+    values[2] = ((PyObject *)((PyObject *)Py_False));
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mapping)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("remap", 0, 2, 3, 1); __PYX_ERR(0, 389, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_preserve_missing_labels);
+          if (value) { values[2] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "remap") < 0)) __PYX_ERR(0, 389, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_self = values[0];
+    __pyx_v_mapping = values[1];
+    __pyx_v_preserve_missing_labels = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("remap", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 389, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("compressed_segmentation.CompressedSegmentationArray.remap", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_6remap(__pyx_self, __pyx_v_self, __pyx_v_mapping, __pyx_v_preserve_missing_labels);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_6remap(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mapping, PyObject *__pyx_v_preserve_missing_labels) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("remap", 0);
+
+  /* "compressed_segmentation.pyx":390
+ * 
+ *   def remap(self, mapping, preserve_missing_labels=False):
+ *     return remap(             # <<<<<<<<<<<<<<
+ *       self.binary, self.shape, self.dtype,
+ *       mapping, preserve_missing_labels,
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_remap); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "compressed_segmentation.pyx":391
+ *   def remap(self, mapping, preserve_missing_labels=False):
+ *     return remap(
+ *       self.binary, self.shape, self.dtype,             # <<<<<<<<<<<<<<
+ *       mapping, preserve_missing_labels,
+ *       self.block_size
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "compressed_segmentation.pyx":393
+ *       self.binary, self.shape, self.dtype,
+ *       mapping, preserve_missing_labels,
+ *       self.block_size             # <<<<<<<<<<<<<<
+ *     )
+ * 
+ */
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = NULL;
+  __pyx_t_8 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_8 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[7] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_v_mapping, __pyx_v_preserve_missing_labels, __pyx_t_6};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 6+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[7] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_v_mapping, __pyx_v_preserve_missing_labels, __pyx_t_6};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 6+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  } else
+  #endif
+  {
+    __pyx_t_9 = PyTuple_New(6+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    if (__pyx_t_7) {
+      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
+    }
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_t_5);
+    __Pyx_INCREF(__pyx_v_mapping);
+    __Pyx_GIVEREF(__pyx_v_mapping);
+    PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_v_mapping);
+    __Pyx_INCREF(__pyx_v_preserve_missing_labels);
+    __Pyx_GIVEREF(__pyx_v_preserve_missing_labels);
+    PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_8, __pyx_v_preserve_missing_labels);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_9, 5+__pyx_t_8, __pyx_t_6);
+    __pyx_t_3 = 0;
+    __pyx_t_4 = 0;
+    __pyx_t_5 = 0;
+    __pyx_t_6 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "compressed_segmentation.pyx":389
  *     return self._labels
  * 
+ *   def remap(self, mapping, preserve_missing_labels=False):             # <<<<<<<<<<<<<<
+ *     return remap(
+ *       self.binary, self.shape, self.dtype,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("compressed_segmentation.CompressedSegmentationArray.remap", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "compressed_segmentation.pyx":396
+ *     )
+ * 
  *   def numpy(self):             # <<<<<<<<<<<<<<
  *     return decompress(
  *       self.binary, self.shape,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_7numpy(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_7numpy = {"numpy", (PyCFunction)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_7numpy, METH_O, 0};
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_7numpy(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_9numpy(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_9numpy = {"numpy", (PyCFunction)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_9numpy, METH_O, 0};
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_9numpy(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("numpy (wrapper)", 0);
-  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_6numpy(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_8numpy(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_6numpy(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_8numpy(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -7648,47 +9300,47 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("numpy", 0);
 
-  /* "compressed_segmentation.pyx":341
+  /* "compressed_segmentation.pyx":397
  * 
  *   def numpy(self):
  *     return decompress(             # <<<<<<<<<<<<<<
  *       self.binary, self.shape,
  *       self.dtype, self.block_size
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_decompress); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_decompress); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "compressed_segmentation.pyx":342
+  /* "compressed_segmentation.pyx":398
  *   def numpy(self):
  *     return decompress(
  *       self.binary, self.shape,             # <<<<<<<<<<<<<<
  *       self.dtype, self.block_size
  *     )
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "compressed_segmentation.pyx":343
+  /* "compressed_segmentation.pyx":399
  *     return decompress(
  *       self.binary, self.shape,
  *       self.dtype, self.block_size             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7697,37 +9349,37 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 4+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 4+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_7, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 4+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 4+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(4+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(4+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 397, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
@@ -7736,25 +9388,25 @@
     PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_t_6);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":340
- *     return self._labels
+  /* "compressed_segmentation.pyx":396
+ *     )
  * 
  *   def numpy(self):             # <<<<<<<<<<<<<<
  *     return decompress(
  *       self.binary, self.shape,
  */
 
   /* function exit code */
@@ -7771,26 +9423,26 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":346
+/* "compressed_segmentation.pyx":402
  *     )
  * 
  *   def get(self, x,y,z):             # <<<<<<<<<<<<<<
  *     if (
  *       (x < 0 or x >= self.shape[0])
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_9get(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_9get = {"get", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_9get, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_9get(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_11get(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_11get = {"get", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_11get, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_11get(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_x = 0;
   PyObject *__pyx_v_y = 0;
   PyObject *__pyx_v_z = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -7820,31 +9472,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, 1); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, 1); __PYX_ERR(0, 402, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, 2); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, 2); __PYX_ERR(0, 402, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_z)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, 3); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, 3); __PYX_ERR(0, 402, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get") < 0)) __PYX_ERR(0, 346, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get") < 0)) __PYX_ERR(0, 402, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -7853,28 +9505,28 @@
     __pyx_v_self = values[0];
     __pyx_v_x = values[1];
     __pyx_v_y = values[2];
     __pyx_v_z = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 346, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 402, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("compressed_segmentation.CompressedSegmentationArray.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_8get(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
+  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_10get(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_8get(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_y, PyObject *__pyx_v_z) {
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_10get(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_y, PyObject *__pyx_v_z) {
   PyObject *__pyx_v_xyz = NULL;
   PyObject *__pyx_v_gpt = NULL;
   PyObject *__pyx_v_grid_size = NULL;
   PyObject *__pyx_v_binary = NULL;
   PyObject *__pyx_v_num_headers = NULL;
   PyObject *__pyx_v_header_idx = NULL;
   PyObject *__pyx_v_headers = NULL;
@@ -7906,750 +9558,750 @@
   uint64_t __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get", 0);
 
-  /* "compressed_segmentation.pyx":348
+  /* "compressed_segmentation.pyx":404
  *   def get(self, x,y,z):
  *     if (
  *       (x < 0 or x >= self.shape[0])             # <<<<<<<<<<<<<<
  *       or (y < 0 or y >= self.shape[1])
  *       or (z < 0 or z >= self.shape[2])
  */
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_x, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_x, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_x, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_x, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "compressed_segmentation.pyx":349
+  /* "compressed_segmentation.pyx":405
  *     if (
  *       (x < 0 or x >= self.shape[0])
  *       or (y < 0 or y >= self.shape[1])             # <<<<<<<<<<<<<<
  *       or (z < 0 or z >= self.shape[2])
  *     ):
  */
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_y, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_y, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_y, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_y, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "compressed_segmentation.pyx":350
+  /* "compressed_segmentation.pyx":406
  *       (x < 0 or x >= self.shape[0])
  *       or (y < 0 or y >= self.shape[1])
  *       or (z < 0 or z >= self.shape[2])             # <<<<<<<<<<<<<<
  *     ):
  *       raise IndexError(f"<{x},{y},{z}> must be contained within {self.shape}")
  */
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_z, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_z, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_2, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_z, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_z, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
 
-  /* "compressed_segmentation.pyx":347
+  /* "compressed_segmentation.pyx":403
  * 
  *   def get(self, x,y,z):
  *     if (             # <<<<<<<<<<<<<<
  *       (x < 0 or x >= self.shape[0])
  *       or (y < 0 or y >= self.shape[1])
  */
   if (unlikely(__pyx_t_1)) {
 
-    /* "compressed_segmentation.pyx":352
+    /* "compressed_segmentation.pyx":408
  *       or (z < 0 or z >= self.shape[2])
  *     ):
  *       raise IndexError(f"<{x},{y},{z}> must be contained within {self.shape}")             # <<<<<<<<<<<<<<
  * 
  *     xyz = np.array([x,y,z], dtype=np.int64)
  */
-    __pyx_t_2 = PyTuple_New(8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__14);
+    __Pyx_INCREF(__pyx_kp_u__15);
     __pyx_t_5 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__14);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__14);
-    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_x, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__15);
+    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__15);
+    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_x, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    __Pyx_INCREF(__pyx_kp_u__15);
+    __Pyx_INCREF(__pyx_kp_u__16);
     __pyx_t_5 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__15);
-    PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u__15);
-    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_y, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__16);
+    PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u__16);
+    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_y, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_4);
     __pyx_t_4 = 0;
-    __Pyx_INCREF(__pyx_kp_u__15);
+    __Pyx_INCREF(__pyx_kp_u__16);
     __pyx_t_5 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__15);
-    PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u__15);
-    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_z, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__16);
+    PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u__16);
+    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_z, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_INCREF(__pyx_kp_u_must_be_contained_within);
     __pyx_t_5 += 27;
     __Pyx_GIVEREF(__pyx_kp_u_must_be_contained_within);
     PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_kp_u_must_be_contained_within);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_2, 8, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_2, 8, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 352, __pyx_L1_error)
+    __PYX_ERR(0, 408, __pyx_L1_error)
 
-    /* "compressed_segmentation.pyx":347
+    /* "compressed_segmentation.pyx":403
  * 
  *   def get(self, x,y,z):
  *     if (             # <<<<<<<<<<<<<<
  *       (x < 0 or x >= self.shape[0])
  *       or (y < 0 or y >= self.shape[1])
  */
   }
 
-  /* "compressed_segmentation.pyx":354
+  /* "compressed_segmentation.pyx":410
  *       raise IndexError(f"<{x},{y},{z}> must be contained within {self.shape}")
  * 
  *     xyz = np.array([x,y,z], dtype=np.int64)             # <<<<<<<<<<<<<<
  *     gpt = xyz // self.block_size
  *     grid_size = self.grid_size
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_x);
   __Pyx_GIVEREF(__pyx_v_x);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_v_x);
   __Pyx_INCREF(__pyx_v_y);
   __Pyx_GIVEREF(__pyx_v_y);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_v_y);
   __Pyx_INCREF(__pyx_v_z);
   __Pyx_GIVEREF(__pyx_v_z);
   PyList_SET_ITEM(__pyx_t_2, 2, __pyx_v_z);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_int64); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_int64); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_xyz = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "compressed_segmentation.pyx":355
+  /* "compressed_segmentation.pyx":411
  * 
  *     xyz = np.array([x,y,z], dtype=np.int64)
  *     gpt = xyz // self.block_size             # <<<<<<<<<<<<<<
  *     grid_size = self.grid_size
  * 
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_2 = PyNumber_FloorDivide(__pyx_v_xyz, __pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_FloorDivide(__pyx_v_xyz, __pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_v_gpt = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "compressed_segmentation.pyx":356
+  /* "compressed_segmentation.pyx":412
  *     xyz = np.array([x,y,z], dtype=np.int64)
  *     gpt = xyz // self.block_size
  *     grid_size = self.grid_size             # <<<<<<<<<<<<<<
  * 
  *     if self.binary[0] != 1:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grid_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grid_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_grid_size = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "compressed_segmentation.pyx":358
+  /* "compressed_segmentation.pyx":414
  *     grid_size = self.grid_size
  * 
  *     if self.binary[0] != 1:             # <<<<<<<<<<<<<<
  *       raise DecodeError(
  *         "Only single channel is currently supported in this function."
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_t_9, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_t_9, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_1)) {
 
-    /* "compressed_segmentation.pyx":359
+    /* "compressed_segmentation.pyx":415
  * 
  *     if self.binary[0] != 1:
  *       raise DecodeError(             # <<<<<<<<<<<<<<
  *         "Only single channel is currently supported in this function."
  *       )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_DecodeError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 359, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_DecodeError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, __pyx_kp_u_Only_single_channel_is_currently) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_kp_u_Only_single_channel_is_currently);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 359, __pyx_L1_error)
+    __PYX_ERR(0, 415, __pyx_L1_error)
 
-    /* "compressed_segmentation.pyx":358
+    /* "compressed_segmentation.pyx":414
  *     grid_size = self.grid_size
  * 
  *     if self.binary[0] != 1:             # <<<<<<<<<<<<<<
  *       raise DecodeError(
  *         "Only single channel is currently supported in this function."
  */
   }
 
-  /* "compressed_segmentation.pyx":363
+  /* "compressed_segmentation.pyx":419
  *       )
  * 
  *     binary = self.binary[4:]             # <<<<<<<<<<<<<<
  *     num_headers = grid_size[0] * grid_size[1] * grid_size[2]
  *     header_idx = gpt[0] + grid_size[0] * (gpt[1] + grid_size[1] * gpt[2])
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_t_2, 4, 0, NULL, NULL, &__pyx_slice__16, 1, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_t_2, 4, 0, NULL, NULL, &__pyx_slice__17, 1, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_binary = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "compressed_segmentation.pyx":364
+  /* "compressed_segmentation.pyx":420
  * 
  *     binary = self.binary[4:]
  *     num_headers = grid_size[0] * grid_size[1] * grid_size[2]             # <<<<<<<<<<<<<<
  *     header_idx = gpt[0] + grid_size[0] * (gpt[1] + grid_size[1] * gpt[2])
  * 
  */
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_grid_size, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_grid_size, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_grid_size, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_grid_size, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_9, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_9, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_grid_size, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_grid_size, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = PyNumber_Multiply(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_9 = PyNumber_Multiply(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_num_headers = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "compressed_segmentation.pyx":365
+  /* "compressed_segmentation.pyx":421
  *     binary = self.binary[4:]
  *     num_headers = grid_size[0] * grid_size[1] * grid_size[2]
  *     header_idx = gpt[0] + grid_size[0] * (gpt[1] + grid_size[1] * gpt[2])             # <<<<<<<<<<<<<<
  * 
  *     headers = np.frombuffer(binary[:8*num_headers], dtype=np.uint64)
  */
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_gpt, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_gpt, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_grid_size, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_grid_size, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_gpt, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_gpt, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_grid_size, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_grid_size, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_GetItemInt(__pyx_v_gpt, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_GetItemInt(__pyx_v_gpt, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_10 = PyNumber_Multiply(__pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_10 = PyNumber_Multiply(__pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Add(__pyx_t_4, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Add(__pyx_t_4, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = PyNumber_Multiply(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_10 = PyNumber_Multiply(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Add(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Add(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_header_idx = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "compressed_segmentation.pyx":367
+  /* "compressed_segmentation.pyx":423
  *     header_idx = gpt[0] + grid_size[0] * (gpt[1] + grid_size[1] * gpt[2])
  * 
  *     headers = np.frombuffer(binary[:8*num_headers], dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     data = np.frombuffer(binary, dtype=np.uint32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Multiply(__pyx_int_8, __pyx_v_num_headers); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Multiply(__pyx_int_8, __pyx_v_num_headers); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_v_binary, 0, 0, NULL, &__pyx_t_8, NULL, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_v_binary, 0, 0, NULL, &__pyx_t_8, NULL, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_9);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_9);
   __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_v_headers = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "compressed_segmentation.pyx":368
+  /* "compressed_segmentation.pyx":424
  * 
  *     headers = np.frombuffer(binary[:8*num_headers], dtype=np.uint64)
  *     data = np.frombuffer(binary, dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
  *     cdef uint64_t header = headers[header_idx]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_binary);
   __Pyx_GIVEREF(__pyx_v_binary);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_binary);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 368, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "compressed_segmentation.pyx":370
+  /* "compressed_segmentation.pyx":426
  *     data = np.frombuffer(binary, dtype=np.uint32)
  * 
  *     cdef uint64_t header = headers[header_idx]             # <<<<<<<<<<<<<<
  *     cdef uint64_t tbl_off = header & 0xffffff
  *     cdef uint64_t encoded_bits = (header >> 24) & 0xff
  */
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_headers, __pyx_v_header_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_headers, __pyx_v_header_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_header = __pyx_t_11;
 
-  /* "compressed_segmentation.pyx":371
+  /* "compressed_segmentation.pyx":427
  * 
  *     cdef uint64_t header = headers[header_idx]
  *     cdef uint64_t tbl_off = header & 0xffffff             # <<<<<<<<<<<<<<
  *     cdef uint64_t encoded_bits = (header >> 24) & 0xff
  *     cdef uint64_t packed_off = header >> 32
  */
   __pyx_v_tbl_off = (__pyx_v_header & 0xffffff);
 
-  /* "compressed_segmentation.pyx":372
+  /* "compressed_segmentation.pyx":428
  *     cdef uint64_t header = headers[header_idx]
  *     cdef uint64_t tbl_off = header & 0xffffff
  *     cdef uint64_t encoded_bits = (header >> 24) & 0xff             # <<<<<<<<<<<<<<
  *     cdef uint64_t packed_off = header >> 32
  * 
  */
   __pyx_v_encoded_bits = ((__pyx_v_header >> 24) & 0xff);
 
-  /* "compressed_segmentation.pyx":373
+  /* "compressed_segmentation.pyx":429
  *     cdef uint64_t tbl_off = header & 0xffffff
  *     cdef uint64_t encoded_bits = (header >> 24) & 0xff
  *     cdef uint64_t packed_off = header >> 32             # <<<<<<<<<<<<<<
  * 
  *     pt = xyz % self.block_size
  */
   __pyx_v_packed_off = (__pyx_v_header >> 32);
 
-  /* "compressed_segmentation.pyx":375
+  /* "compressed_segmentation.pyx":431
  *     cdef uint64_t packed_off = header >> 32
  * 
  *     pt = xyz % self.block_size             # <<<<<<<<<<<<<<
  * 
  *     cdef uint64_t bitpos = encoded_bits * (
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = PyNumber_Remainder(__pyx_v_xyz, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Remainder(__pyx_v_xyz, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_pt = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "compressed_segmentation.pyx":377
+  /* "compressed_segmentation.pyx":433
  *     pt = xyz % self.block_size
  * 
  *     cdef uint64_t bitpos = encoded_bits * (             # <<<<<<<<<<<<<<
  *       pt[0] + self.block_size[0] * (pt[1] + self.block_size[1] * pt[2])
  *     )
  */
-  __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_encoded_bits); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_encoded_bits); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
 
-  /* "compressed_segmentation.pyx":378
+  /* "compressed_segmentation.pyx":434
  * 
  *     cdef uint64_t bitpos = encoded_bits * (
  *       pt[0] + self.block_size[0] * (pt[1] + self.block_size[1] * pt[2])             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pt, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pt, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pt, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pt, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_block_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_10, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_10, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_pt, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_pt, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_12 = PyNumber_Multiply(__pyx_t_7, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_12 = PyNumber_Multiply(__pyx_t_7, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = PyNumber_Add(__pyx_t_4, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_10 = PyNumber_Add(__pyx_t_4, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = PyNumber_Multiply(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_12 = PyNumber_Multiply(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = PyNumber_Add(__pyx_t_2, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_10 = PyNumber_Add(__pyx_t_2, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-  /* "compressed_segmentation.pyx":377
+  /* "compressed_segmentation.pyx":433
  *     pt = xyz % self.block_size
  * 
  *     cdef uint64_t bitpos = encoded_bits * (             # <<<<<<<<<<<<<<
  *       pt[0] + self.block_size[0] * (pt[1] + self.block_size[1] * pt[2])
  *     )
  */
-  __pyx_t_12 = PyNumber_Multiply(__pyx_t_8, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_12 = PyNumber_Multiply(__pyx_t_8, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_12); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_12); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_v_bitpos = __pyx_t_11;
 
-  /* "compressed_segmentation.pyx":381
+  /* "compressed_segmentation.pyx":437
  *     )
  * 
  *     cdef uint64_t bitshift = bitpos % 32             # <<<<<<<<<<<<<<
  *     cdef uint64_t arraypos = bitpos // 32
  *     cdef uint64_t bitmask = (1 << encoded_bits) - 1
  */
   __pyx_v_bitshift = (__pyx_v_bitpos % 32);
 
-  /* "compressed_segmentation.pyx":382
+  /* "compressed_segmentation.pyx":438
  * 
  *     cdef uint64_t bitshift = bitpos % 32
  *     cdef uint64_t arraypos = bitpos // 32             # <<<<<<<<<<<<<<
  *     cdef uint64_t bitmask = (1 << encoded_bits) - 1
  *     cdef uint64_t bitval = 0
  */
   __pyx_v_arraypos = (__pyx_v_bitpos / 32);
 
-  /* "compressed_segmentation.pyx":383
+  /* "compressed_segmentation.pyx":439
  *     cdef uint64_t bitshift = bitpos % 32
  *     cdef uint64_t arraypos = bitpos // 32
  *     cdef uint64_t bitmask = (1 << encoded_bits) - 1             # <<<<<<<<<<<<<<
  *     cdef uint64_t bitval = 0
  *     if encoded_bits > 0:
  */
   __pyx_v_bitmask = ((1 << __pyx_v_encoded_bits) - 1);
 
-  /* "compressed_segmentation.pyx":384
+  /* "compressed_segmentation.pyx":440
  *     cdef uint64_t arraypos = bitpos // 32
  *     cdef uint64_t bitmask = (1 << encoded_bits) - 1
  *     cdef uint64_t bitval = 0             # <<<<<<<<<<<<<<
  *     if encoded_bits > 0:
  *       bitval = (data[packed_off + arraypos] >> bitshift) & bitmask
  */
   __pyx_v_bitval = 0;
 
-  /* "compressed_segmentation.pyx":385
+  /* "compressed_segmentation.pyx":441
  *     cdef uint64_t bitmask = (1 << encoded_bits) - 1
  *     cdef uint64_t bitval = 0
  *     if encoded_bits > 0:             # <<<<<<<<<<<<<<
  *       bitval = (data[packed_off + arraypos] >> bitshift) & bitmask
  * 
  */
   __pyx_t_1 = ((__pyx_v_encoded_bits > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "compressed_segmentation.pyx":386
+    /* "compressed_segmentation.pyx":442
  *     cdef uint64_t bitval = 0
  *     if encoded_bits > 0:
  *       bitval = (data[packed_off + arraypos] >> bitshift) & bitmask             # <<<<<<<<<<<<<<
  * 
  *     cdef uint64_t table_entry_size = np.dtype(self.dtype).itemsize // 4
  */
     __pyx_t_11 = (__pyx_v_packed_off + __pyx_v_arraypos);
-    __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_11, uint64_t, 0, __Pyx_PyInt_From_uint64_t, 0, 0, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_11, uint64_t, 0, __Pyx_PyInt_From_uint64_t, 0, 0, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_bitshift); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_bitshift); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_8 = PyNumber_Rshift(__pyx_t_12, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_8 = PyNumber_Rshift(__pyx_t_12, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_bitmask); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_bitmask); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_12 = PyNumber_And(__pyx_t_8, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_12 = PyNumber_And(__pyx_t_8, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_12); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_12); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_v_bitval = __pyx_t_11;
 
-    /* "compressed_segmentation.pyx":385
+    /* "compressed_segmentation.pyx":441
  *     cdef uint64_t bitmask = (1 << encoded_bits) - 1
  *     cdef uint64_t bitval = 0
  *     if encoded_bits > 0:             # <<<<<<<<<<<<<<
  *       bitval = (data[packed_off + arraypos] >> bitshift) & bitmask
  * 
  */
   }
 
-  /* "compressed_segmentation.pyx":388
+  /* "compressed_segmentation.pyx":444
  *       bitval = (data[packed_off + arraypos] >> bitshift) & bitmask
  * 
  *     cdef uint64_t table_entry_size = np.dtype(self.dtype).itemsize // 4             # <<<<<<<<<<<<<<
  *     cdef uint64_t val = data[tbl_off + bitval * table_entry_size]
  *     if table_entry_size > 1:
  */
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dtype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5numpy_dtype), __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5numpy_dtype), __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_v_table_entry_size = __Pyx_div_long(((PyArray_Descr *)__pyx_t_10)->elsize, 4);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "compressed_segmentation.pyx":389
+  /* "compressed_segmentation.pyx":445
  * 
  *     cdef uint64_t table_entry_size = np.dtype(self.dtype).itemsize // 4
  *     cdef uint64_t val = data[tbl_off + bitval * table_entry_size]             # <<<<<<<<<<<<<<
  *     if table_entry_size > 1:
  *       val = val | (data[tbl_off + bitval * table_entry_size + 1] << 32)
  */
   __pyx_t_11 = (__pyx_v_tbl_off + (__pyx_v_bitval * __pyx_v_table_entry_size));
-  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_11, uint64_t, 0, __Pyx_PyInt_From_uint64_t, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_11, uint64_t, 0, __Pyx_PyInt_From_uint64_t, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_10); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_10); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_val = __pyx_t_11;
 
-  /* "compressed_segmentation.pyx":390
+  /* "compressed_segmentation.pyx":446
  *     cdef uint64_t table_entry_size = np.dtype(self.dtype).itemsize // 4
  *     cdef uint64_t val = data[tbl_off + bitval * table_entry_size]
  *     if table_entry_size > 1:             # <<<<<<<<<<<<<<
  *       val = val | (data[tbl_off + bitval * table_entry_size + 1] << 32)
  * 
  */
   __pyx_t_1 = ((__pyx_v_table_entry_size > 1) != 0);
   if (__pyx_t_1) {
 
-    /* "compressed_segmentation.pyx":391
+    /* "compressed_segmentation.pyx":447
  *     cdef uint64_t val = data[tbl_off + bitval * table_entry_size]
  *     if table_entry_size > 1:
  *       val = val | (data[tbl_off + bitval * table_entry_size + 1] << 32)             # <<<<<<<<<<<<<<
  * 
  *     return val
  */
-    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_val); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_val); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_11 = ((__pyx_v_tbl_off + (__pyx_v_bitval * __pyx_v_table_entry_size)) + 1);
-    __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_11, uint64_t, 0, __Pyx_PyInt_From_uint64_t, 0, 0, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_11, uint64_t, 0, __Pyx_PyInt_From_uint64_t, 0, 0, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_8 = __Pyx_PyInt_LshiftObjC(__pyx_t_12, __pyx_int_32, 32, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_LshiftObjC(__pyx_t_12, __pyx_int_32, 32, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = PyNumber_Or(__pyx_t_10, __pyx_t_8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_12 = PyNumber_Or(__pyx_t_10, __pyx_t_8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_12); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_uint64_t(__pyx_t_12); if (unlikely((__pyx_t_11 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_v_val = __pyx_t_11;
 
-    /* "compressed_segmentation.pyx":390
+    /* "compressed_segmentation.pyx":446
  *     cdef uint64_t table_entry_size = np.dtype(self.dtype).itemsize // 4
  *     cdef uint64_t val = data[tbl_off + bitval * table_entry_size]
  *     if table_entry_size > 1:             # <<<<<<<<<<<<<<
  *       val = val | (data[tbl_off + bitval * table_entry_size + 1] << 32)
  * 
  */
   }
 
-  /* "compressed_segmentation.pyx":393
+  /* "compressed_segmentation.pyx":449
  *       val = val | (data[tbl_off + bitval * table_entry_size + 1] << 32)
  * 
  *     return val             # <<<<<<<<<<<<<<
  * 
  *   def __contains__(self, val):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_12 = __Pyx_PyInt_From_uint64_t(__pyx_v_val); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_uint64_t(__pyx_v_val); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __pyx_r = __pyx_t_12;
   __pyx_t_12 = 0;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":346
+  /* "compressed_segmentation.pyx":402
  *     )
  * 
  *   def get(self, x,y,z):             # <<<<<<<<<<<<<<
  *     if (
  *       (x < 0 or x >= self.shape[0])
  */
 
@@ -8675,26 +10327,26 @@
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_pt);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":395
+/* "compressed_segmentation.pyx":451
  *     return val
  * 
  *   def __contains__(self, val):             # <<<<<<<<<<<<<<
  *     return val in self.labels()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_11__contains__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_11__contains__ = {"__contains__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_11__contains__, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_11__contains__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_13__contains__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_13__contains__ = {"__contains__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_13__contains__, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_13__contains__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_val = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -8718,90 +10370,90 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_val)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, 1); __PYX_ERR(0, 395, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, 1); __PYX_ERR(0, 451, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__contains__") < 0)) __PYX_ERR(0, 395, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__contains__") < 0)) __PYX_ERR(0, 451, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_val = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 395, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 451, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("compressed_segmentation.CompressedSegmentationArray.__contains__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_10__contains__(__pyx_self, __pyx_v_self, __pyx_v_val);
+  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_12__contains__(__pyx_self, __pyx_v_self, __pyx_v_val);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_10__contains__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_12__contains__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__contains__", 0);
 
-  /* "compressed_segmentation.pyx":396
+  /* "compressed_segmentation.pyx":452
  * 
  *   def __contains__(self, val):
  *     return val in self.labels()             # <<<<<<<<<<<<<<
  * 
  *   def __getitem__(self, slcs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_v_val, __pyx_t_1, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_v_val, __pyx_t_1, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":395
+  /* "compressed_segmentation.pyx":451
  *     return val
  * 
  *   def __contains__(self, val):             # <<<<<<<<<<<<<<
  *     return val in self.labels()
  * 
  */
 
@@ -8814,25 +10466,25 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "compressed_segmentation.pyx":398
+/* "compressed_segmentation.pyx":454
  *     return val in self.labels()
  * 
  *   def __getitem__(self, slcs):             # <<<<<<<<<<<<<<
  *     return self.get(*slcs)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_13__getitem__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_13__getitem__ = {"__getitem__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_13__getitem__, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_13__getitem__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_15__getitem__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_15__getitem__ = {"__getitem__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_15__getitem__, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_23compressed_segmentation_27CompressedSegmentationArray_15__getitem__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_slcs = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -8856,74 +10508,74 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slcs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 398, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, 1); __PYX_ERR(0, 454, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 398, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__getitem__") < 0)) __PYX_ERR(0, 454, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_slcs = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 398, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__getitem__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 454, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("compressed_segmentation.CompressedSegmentationArray.__getitem__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_12__getitem__(__pyx_self, __pyx_v_self, __pyx_v_slcs);
+  __pyx_r = __pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_14__getitem__(__pyx_self, __pyx_v_self, __pyx_v_slcs);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_12__getitem__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_slcs) {
+static PyObject *__pyx_pf_23compressed_segmentation_27CompressedSegmentationArray_14__getitem__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_slcs) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "compressed_segmentation.pyx":399
+  /* "compressed_segmentation.pyx":455
  * 
  *   def __getitem__(self, slcs):
  *     return self.get(*slcs)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_v_slcs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_v_slcs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "compressed_segmentation.pyx":398
+  /* "compressed_segmentation.pyx":454
  *     return val in self.labels()
  * 
  *   def __getitem__(self, slcs):             # <<<<<<<<<<<<<<
  *     return self.get(*slcs)
  */
 
   /* function exit code */
@@ -10119,15 +11771,15 @@
       /* "../../.virtualenvs/cseg/lib/python3.9/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -10251,15 +11903,15 @@
       /* "../../.virtualenvs/cseg/lib/python3.9/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -10383,15 +12035,15 @@
       /* "../../.virtualenvs/cseg/lib/python3.9/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -11136,15 +12788,15 @@
     /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 133, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 133, __pyx_L1_error)
 
     /* "View.MemoryView":132
  *         self.itemsize = itemsize
@@ -11168,15 +12820,15 @@
     /* "View.MemoryView":136
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 136, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 136, __pyx_L1_error)
 
     /* "View.MemoryView":135
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -11295,15 +12947,15 @@
     /* "View.MemoryView":148
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 148, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 148, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 148, __pyx_L1_error)
 
     /* "View.MemoryView":147
  *         self._strides = self._shape + self.ndim
@@ -11569,15 +13221,15 @@
       /* "View.MemoryView":176
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 176, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 176, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(3, 176, __pyx_L1_error)
 
       /* "View.MemoryView":175
  * 
@@ -11813,15 +13465,15 @@
     /* "View.MemoryView":192
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 192, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 192, __pyx_L1_error)
 
     /* "View.MemoryView":191
  *         elif self.mode == u"fortran":
@@ -12547,15 +14199,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -12603,15 +14255,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -14313,15 +15965,15 @@
     /* "View.MemoryView":418
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(3, 418, __pyx_L1_error)
 
     /* "View.MemoryView":417
  * 
@@ -15361,15 +17013,15 @@
       /* "View.MemoryView":495
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(3, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(3, 495, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(3, 495, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -15723,15 +17375,15 @@
     /* "View.MemoryView":520
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 520, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(3, 520, __pyx_L1_error)
 
     /* "View.MemoryView":519
  *     @cname('getbuffer')
@@ -16272,15 +17924,15 @@
     /* "View.MemoryView":570
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 570, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(3, 570, __pyx_L1_error)
 
     /* "View.MemoryView":568
  *     @property
@@ -16389,15 +18041,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__30, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__31, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":576
@@ -17427,15 +19079,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -17483,15 +19135,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -18144,15 +19796,15 @@
       /* "View.MemoryView":703
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 703, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(3, 703, __pyx_L1_error)
 
       /* "View.MemoryView":702
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -20328,15 +21980,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -20384,15 +22036,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(3, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -24043,16 +25695,16 @@
       /* "BufferFormatFromTypeInfo":1473
  * 
  *         if type.flags & __PYX_BUF_FLAGS_PACKED_STRUCT:
  *             alignment = b'^'             # <<<<<<<<<<<<<<
  *         else:
  *             alignment = b''
  */
-      __Pyx_INCREF(__pyx_kp_b__36);
-      __pyx_v_alignment = __pyx_kp_b__36;
+      __Pyx_INCREF(__pyx_kp_b__37);
+      __pyx_v_alignment = __pyx_kp_b__37;
 
       /* "BufferFormatFromTypeInfo":1472
  *         assert type.fields.type != NULL
  * 
  *         if type.flags & __PYX_BUF_FLAGS_PACKED_STRUCT:             # <<<<<<<<<<<<<<
  *             alignment = b'^'
  *         else:
@@ -24064,16 +25716,16 @@
  *             alignment = b'^'
  *         else:
  *             alignment = b''             # <<<<<<<<<<<<<<
  * 
  *         parts = [b"T{"]
  */
     /*else*/ {
-      __Pyx_INCREF(__pyx_kp_b__37);
-      __pyx_v_alignment = __pyx_kp_b__37;
+      __Pyx_INCREF(__pyx_kp_b__38);
+      __pyx_v_alignment = __pyx_kp_b__38;
     }
     __pyx_L4:;
 
     /* "BufferFormatFromTypeInfo":1477
  *             alignment = b''
  * 
  *         parts = [b"T{"]             # <<<<<<<<<<<<<<
@@ -24124,23 +25776,23 @@
       /* "BufferFormatFromTypeInfo":1482
  *         while field.type:
  *             part = format_from_typeinfo(field.type)
  *             parts.append(part + b':' + field.name + b':')             # <<<<<<<<<<<<<<
  *             field += 1
  * 
  */
-      __pyx_t_2 = PyNumber_Add(__pyx_v_part, __pyx_kp_b__38); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 1482, __pyx_L1_error)
+      __pyx_t_2 = PyNumber_Add(__pyx_v_part, __pyx_kp_b__39); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 1482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_field->name); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 1482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = PyNumber_Add(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyNumber_Add(__pyx_t_5, __pyx_kp_b__38); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 1482, __pyx_L1_error)
+      __pyx_t_4 = PyNumber_Add(__pyx_t_5, __pyx_kp_b__39); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 1482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_parts, __pyx_t_4); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(3, 1482, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "BufferFormatFromTypeInfo":1483
  *             part = format_from_typeinfo(field.type)
@@ -24157,15 +25809,15 @@
  * 
  *         result = alignment.join(parts) + b'}'             # <<<<<<<<<<<<<<
  *     else:
  *         fmt = __Pyx_TypeInfoToFormat(type)
  */
     __pyx_t_4 = __Pyx_PyBytes_Join(__pyx_v_alignment, __pyx_v_parts); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 1485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_b__39); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1485, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_b__40); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(3, 1485, __pyx_L1_error)
     __pyx_v_result = ((PyObject*)__pyx_t_5);
     __pyx_t_5 = 0;
 
     /* "BufferFormatFromTypeInfo":1468
@@ -24225,15 +25877,15 @@
       /* "BufferFormatFromTypeInfo":1490
  *         if type.arraysize[0]:
  *             extents = [unicode(type.arraysize[i]) for i in range(type.ndim)]
  *             result = (u"(%s)" % u','.join(extents)).encode('ascii') + fmt.string             # <<<<<<<<<<<<<<
  *         else:
  *             result = fmt.string
  */
-      __pyx_t_5 = PyUnicode_Join(__pyx_kp_u__15, __pyx_v_extents); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1490, __pyx_L1_error)
+      __pyx_t_5 = PyUnicode_Join(__pyx_kp_u__16, __pyx_v_extents); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1490, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_2 = PyUnicode_Format(__pyx_kp_u_s, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 1490, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = PyUnicode_AsASCIIString(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1490, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -25094,14 +26746,15 @@
   {&__pyx_n_s_CompressedSegmentationArray___co, __pyx_k_CompressedSegmentationArray___co, sizeof(__pyx_k_CompressedSegmentationArray___co), 0, 0, 1, 1},
   {&__pyx_n_s_CompressedSegmentationArray___ge, __pyx_k_CompressedSegmentationArray___ge, sizeof(__pyx_k_CompressedSegmentationArray___ge), 0, 0, 1, 1},
   {&__pyx_n_s_CompressedSegmentationArray___in, __pyx_k_CompressedSegmentationArray___in, sizeof(__pyx_k_CompressedSegmentationArray___in), 0, 0, 1, 1},
   {&__pyx_n_s_CompressedSegmentationArray_get, __pyx_k_CompressedSegmentationArray_get, sizeof(__pyx_k_CompressedSegmentationArray_get), 0, 0, 1, 1},
   {&__pyx_n_s_CompressedSegmentationArray_grid, __pyx_k_CompressedSegmentationArray_grid, sizeof(__pyx_k_CompressedSegmentationArray_grid), 0, 0, 1, 1},
   {&__pyx_n_s_CompressedSegmentationArray_labe, __pyx_k_CompressedSegmentationArray_labe, sizeof(__pyx_k_CompressedSegmentationArray_labe), 0, 0, 1, 1},
   {&__pyx_n_s_CompressedSegmentationArray_nump, __pyx_k_CompressedSegmentationArray_nump, sizeof(__pyx_k_CompressedSegmentationArray_nump), 0, 0, 1, 1},
+  {&__pyx_n_s_CompressedSegmentationArray_rema, __pyx_k_CompressedSegmentationArray_rema, sizeof(__pyx_k_CompressedSegmentationArray_rema), 0, 0, 1, 1},
   {&__pyx_n_s_DEFAULT_BLOCK_SIZE, __pyx_k_DEFAULT_BLOCK_SIZE, sizeof(__pyx_k_DEFAULT_BLOCK_SIZE), 0, 0, 1, 1},
   {&__pyx_n_s_DecodeError, __pyx_k_DecodeError, sizeof(__pyx_k_DecodeError), 0, 0, 1, 1},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_u_Empty_data_stream, __pyx_k_Empty_data_stream, sizeof(__pyx_k_Empty_data_stream), 0, 1, 0, 0},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_u_F, __pyx_k_F, sizeof(__pyx_k_F), 0, 1, 0, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
@@ -25122,47 +26775,51 @@
   {&__pyx_kp_u_The_input_data_were_too_large_an, __pyx_k_The_input_data_were_too_large_an, sizeof(__pyx_k_The_input_data_were_too_large_an), 0, 1, 0, 0},
   {&__pyx_kp_u_This_function_only_handles_singl, __pyx_k_This_function_only_handles_singl, sizeof(__pyx_k_This_function_only_handles_singl), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_kp_u_Unable_to_locate_value, __pyx_k_Unable_to_locate_value, sizeof(__pyx_k_Unable_to_locate_value), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
-  {&__pyx_kp_u__14, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 0},
   {&__pyx_kp_u__15, __pyx_k__15, sizeof(__pyx_k__15), 0, 1, 0, 0},
-  {&__pyx_kp_b__36, __pyx_k__36, sizeof(__pyx_k__36), 0, 0, 0, 0},
+  {&__pyx_kp_u__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 1, 0, 0},
   {&__pyx_kp_b__37, __pyx_k__37, sizeof(__pyx_k__37), 0, 0, 0, 0},
   {&__pyx_kp_b__38, __pyx_k__38, sizeof(__pyx_k__38), 0, 0, 0, 0},
   {&__pyx_kp_b__39, __pyx_k__39, sizeof(__pyx_k__39), 0, 0, 0, 0},
+  {&__pyx_kp_b__40, __pyx_k__40, sizeof(__pyx_k__40), 0, 0, 0, 0},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_any, __pyx_k_any, sizeof(__pyx_k_any), 0, 0, 1, 1},
   {&__pyx_n_s_arr_memview32, __pyx_k_arr_memview32, sizeof(__pyx_k_arr_memview32), 0, 0, 1, 1},
   {&__pyx_n_s_arr_memview64, __pyx_k_arr_memview64, sizeof(__pyx_k_arr_memview64), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_arraypos, __pyx_k_arraypos, sizeof(__pyx_k_arraypos), 0, 0, 1, 1},
   {&__pyx_n_s_astype, __pyx_k_astype, sizeof(__pyx_k_astype), 0, 0, 1, 1},
+  {&__pyx_n_s_axis, __pyx_k_axis, sizeof(__pyx_k_axis), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_binary, __pyx_k_binary, sizeof(__pyx_k_binary), 0, 0, 1, 1},
   {&__pyx_n_s_bitmask, __pyx_k_bitmask, sizeof(__pyx_k_bitmask), 0, 0, 1, 1},
   {&__pyx_n_s_bitpos, __pyx_k_bitpos, sizeof(__pyx_k_bitpos), 0, 0, 1, 1},
   {&__pyx_n_s_bitshift, __pyx_k_bitshift, sizeof(__pyx_k_bitshift), 0, 0, 1, 1},
   {&__pyx_n_s_bitval, __pyx_k_bitval, sizeof(__pyx_k_bitval), 0, 0, 1, 1},
   {&__pyx_n_s_block_size, __pyx_k_block_size, sizeof(__pyx_k_block_size), 0, 0, 1, 1},
   {&__pyx_n_s_block_sizeptr, __pyx_k_block_sizeptr, sizeof(__pyx_k_block_sizeptr), 0, 0, 1, 1},
   {&__pyx_n_s_bytestrout, __pyx_k_bytestrout, sizeof(__pyx_k_bytestrout), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_ceil, __pyx_k_ceil, sizeof(__pyx_k_ceil), 0, 0, 1, 1},
+  {&__pyx_n_s_channel_length, __pyx_k_channel_length, sizeof(__pyx_k_channel_length), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_compress, __pyx_k_compress, sizeof(__pyx_k_compress), 0, 0, 1, 1},
   {&__pyx_n_s_compressed_segmentation, __pyx_k_compressed_segmentation, sizeof(__pyx_k_compressed_segmentation), 0, 0, 1, 1},
+  {&__pyx_n_s_compute_label_offsets, __pyx_k_compute_label_offsets, sizeof(__pyx_k_compute_label_offsets), 0, 0, 1, 1},
   {&__pyx_n_s_concatenate, __pyx_k_concatenate, sizeof(__pyx_k_concatenate), 0, 0, 1, 1},
   {&__pyx_n_s_contains, __pyx_k_contains, sizeof(__pyx_k_contains), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
+  {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_decompress, __pyx_k_decompress, sizeof(__pyx_k_decompress), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_bytes, __pyx_k_dtype_bytes, sizeof(__pyx_k_dtype_bytes), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
@@ -25197,18 +26854,20 @@
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_input_strides, __pyx_k_input_strides, sizeof(__pyx_k_input_strides), 0, 0, 1, 1},
   {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
+  {&__pyx_n_s_label, __pyx_k_label, sizeof(__pyx_k_label), 0, 0, 1, 1},
   {&__pyx_n_s_labels, __pyx_k_labels, sizeof(__pyx_k_labels), 0, 0, 1, 1},
   {&__pyx_n_s_labels_2, __pyx_k_labels_2, sizeof(__pyx_k_labels_2), 0, 0, 1, 1},
   {&__pyx_n_s_lookup_table_offset, __pyx_k_lookup_table_offset, sizeof(__pyx_k_lookup_table_offset), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+  {&__pyx_n_s_mapping, __pyx_k_mapping, sizeof(__pyx_k_mapping), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_mul, __pyx_k_mul, sizeof(__pyx_k_mul), 0, 0, 1, 1},
   {&__pyx_kp_u_must_be_contained_within, __pyx_k_must_be_contained_within, sizeof(__pyx_k_must_be_contained_within), 0, 1, 0, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
@@ -25228,14 +26887,15 @@
   {&__pyx_n_s_order, __pyx_k_order, sizeof(__pyx_k_order), 0, 0, 1, 1},
   {&__pyx_n_s_output, __pyx_k_output, sizeof(__pyx_k_output), 0, 0, 1, 1},
   {&__pyx_n_s_output_ptr, __pyx_k_output_ptr, sizeof(__pyx_k_output_ptr), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_packed_off, __pyx_k_packed_off, sizeof(__pyx_k_packed_off), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
+  {&__pyx_n_s_preserve_missing_labels, __pyx_k_preserve_missing_labels, sizeof(__pyx_k_preserve_missing_labels), 0, 0, 1, 1},
   {&__pyx_n_s_property, __pyx_k_property, sizeof(__pyx_k_property), 0, 0, 1, 1},
   {&__pyx_n_s_pt, __pyx_k_pt, sizeof(__pyx_k_pt), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
@@ -25244,14 +26904,15 @@
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_2, __pyx_k_reduce_2, sizeof(__pyx_k_reduce_2), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+  {&__pyx_n_s_remap, __pyx_k_remap, sizeof(__pyx_k_remap), 0, 0, 1, 1},
   {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
   {&__pyx_kp_u_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 1, 0, 0},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
@@ -25265,14 +26926,15 @@
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
   {&__pyx_n_s_table_entry_size, __pyx_k_table_entry_size, sizeof(__pyx_k_table_entry_size), 0, 0, 1, 1},
   {&__pyx_n_s_tbl_off, __pyx_k_tbl_off, sizeof(__pyx_k_tbl_off), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+  {&__pyx_n_s_tobytes, __pyx_k_tobytes, sizeof(__pyx_k_tobytes), 0, 0, 1, 1},
   {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
   {&__pyx_n_s_uint64, __pyx_k_uint64, sizeof(__pyx_k_uint64), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unique, __pyx_k_unique, sizeof(__pyx_k_unique), 0, 0, 1, 1},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
@@ -25284,20 +26946,20 @@
   {&__pyx_n_s_xyz, __pyx_k_xyz, sizeof(__pyx_k_xyz), 0, 0, 1, 1},
   {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
   {&__pyx_n_s_z, __pyx_k_z, sizeof(__pyx_k_z), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 377, __pyx_L1_error)
   __pyx_builtin_OverflowError = __Pyx_GetBuiltinName(__pyx_n_s_OverflowError); if (!__pyx_builtin_OverflowError) __PYX_ERR(0, 130, __pyx_L1_error)
   __pyx_builtin_any = __Pyx_GetBuiltinName(__pyx_n_s_any); if (!__pyx_builtin_any) __PYX_ERR(0, 148, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 222, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 255, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 334, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 109, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(3, 84, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(3, 133, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(3, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(3, 613, __pyx_L1_error)
   return 0;
@@ -25363,436 +27025,475 @@
  *       "The input data were too large and varied and generated a table offset larger than 24-bits.\n"
  *       "See lookupTableOffset: https://github.com/google/neuroglancer/blob/c9a6b9948dd416997c91e655ec3d67bf6b7e771b/src/neuroglancer/sliceview/compressed_segmentation/README.md#format-specification"
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_The_input_data_were_too_large_an); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "compressed_segmentation.pyx":240
- * 
+  /* "compressed_segmentation.pyx":238
+ *   shape = np.array(shape)
  *   if any(shape == 0):
  *     return np.zeros((0,), dtype=dtype)             # <<<<<<<<<<<<<<
  * 
- *   grid_size = np.ceil(shape / block_size).astype(np.uint64)
+ *   index = _compute_label_offsets(encoded, shape, dtype, block_size)
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_int_0); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_int_0); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_tuple__12); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_tuple__12); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "compressed_segmentation.pyx":363
+  /* "compressed_segmentation.pyx":419
  *       )
  * 
  *     binary = self.binary[4:]             # <<<<<<<<<<<<<<
  *     num_headers = grid_size[0] * grid_size[1] * grid_size[2]
  *     header_idx = gpt[0] + grid_size[0] * (gpt[1] + grid_size[1] * gpt[2])
  */
-  __pyx_slice__16 = PySlice_New(__pyx_int_4, Py_None, Py_None); if (unlikely(!__pyx_slice__16)) __PYX_ERR(0, 363, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__16);
-  __Pyx_GIVEREF(__pyx_slice__16);
+  __pyx_slice__17 = PySlice_New(__pyx_int_4, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__17);
+  __Pyx_GIVEREF(__pyx_slice__17);
 
   /* "../../.virtualenvs/cseg/lib/python3.9/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 945, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "../../.virtualenvs/cseg/lib/python3.9/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 951, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(3, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(3, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "View.MemoryView":136
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(3, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(3, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":148
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(3, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(3, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":176
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(3, 176, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":192
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 192, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "View.MemoryView":418
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 418, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 418, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "View.MemoryView":495
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 495, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(3, 495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "View.MemoryView":520
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(3, 520, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(3, 520, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "View.MemoryView":570
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(3, 570, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(3, 570, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "View.MemoryView":577
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__30 = PyTuple_New(1); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(3, 577, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
+  __pyx_tuple__31 = PyTuple_New(1); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(3, 577, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__30, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  PyTuple_SET_ITEM(__pyx_tuple__31, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(3, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "View.MemoryView":703
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(3, 703, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(3, 703, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(3, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(3, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(3, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
   /* "compressed_segmentation.pyx":53
  *   )
  * 
  * DEFAULT_BLOCK_SIZE = (8,8,8)             # <<<<<<<<<<<<<<
  * 
  * class DecodeError(Exception):
  */
-  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_int_8, __pyx_int_8, __pyx_int_8); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_int_8, __pyx_int_8, __pyx_int_8); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
   /* "compressed_segmentation.pyx":58
  *   pass
  * 
  * def compress(data, block_size=DEFAULT_BLOCK_SIZE, order='C'):             # <<<<<<<<<<<<<<
  *   """
  *   compress(data, block_size=DEFAULT_BLOCK_SIZE, order='C')
  */
-  __pyx_tuple__41 = PyTuple_Pack(13, __pyx_n_s_data, __pyx_n_s_block_size, __pyx_n_s_order, __pyx_n_s_volume_size, __pyx_n_s_block_sizeptr, __pyx_n_s_input_strides, __pyx_n_s_arr_memview32, __pyx_n_s_arr_memview64, __pyx_n_s_output, __pyx_n_s_error, __pyx_n_s_output_ptr, __pyx_n_s_vec_view, __pyx_n_s_bytestrout); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_compress, 58, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(13, __pyx_n_s_data, __pyx_n_s_block_size, __pyx_n_s_order, __pyx_n_s_volume_size, __pyx_n_s_block_sizeptr, __pyx_n_s_input_strides, __pyx_n_s_arr_memview32, __pyx_n_s_arr_memview64, __pyx_n_s_output, __pyx_n_s_error, __pyx_n_s_output_ptr, __pyx_n_s_vec_view, __pyx_n_s_bytestrout); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(3, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_compress, 58, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 58, __pyx_L1_error)
 
   /* "compressed_segmentation.pyx":196
  *   return np.frombuffer(buf, dtype=dtype).reshape( volume_size, order=order )
  * 
  * def decompress(             # <<<<<<<<<<<<<<
  *     bytes encoded, volume_size, dtype,
  *     block_size=DEFAULT_BLOCK_SIZE, order='C'
  */
-  __pyx_tuple__45 = PyTuple_Pack(5, __pyx_n_s_encoded, __pyx_n_s_volume_size, __pyx_n_s_dtype, __pyx_n_s_block_size, __pyx_n_s_order); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_decompress, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(5, __pyx_n_s_encoded, __pyx_n_s_volume_size, __pyx_n_s_dtype, __pyx_n_s_block_size, __pyx_n_s_order); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_decompress, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 196, __pyx_L1_error)
 
   /* "compressed_segmentation.pyx":224
  *     raise TypeError("dtype ({}) must be one of uint32 or uint64.".format(dtype))
  * 
  * def labels(             # <<<<<<<<<<<<<<
  *   bytes encoded, shape, dtype,
  *   block_size=DEFAULT_BLOCK_SIZE
  */
-  __pyx_tuple__47 = PyTuple_Pack(21, __pyx_n_s_encoded, __pyx_n_s_shape, __pyx_n_s_dtype, __pyx_n_s_block_size, __pyx_n_s_grid_size, __pyx_n_s_num_headers, __pyx_n_s_header_bytes, __pyx_n_s_headers, __pyx_n_s_data, __pyx_n_s_offsets, __pyx_n_s_i, __pyx_n_s_lookup_table_offset, __pyx_n_s_encoded_values_offset, __pyx_n_s_labels_2, __pyx_n_s_dtype_bytes, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_idx, __pyx_n_s_size, __pyx_n_s_index, __pyx_n_s_idx); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 224, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__47);
-  __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(4, 0, 21, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_labels_2, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(9, __pyx_n_s_encoded, __pyx_n_s_shape, __pyx_n_s_dtype, __pyx_n_s_block_size, __pyx_n_s_index, __pyx_n_s_num_headers, __pyx_n_s_data, __pyx_n_s_labels_2, __pyx_n_s_idx); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_labels_2, 224, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 224, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":319
+  /* "compressed_segmentation.pyx":254
+ *   return np.unique(labels)
+ * 
+ * def remap(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,
+ */
+  __pyx_tuple__50 = PyTuple_Pack(14, __pyx_n_s_encoded, __pyx_n_s_shape, __pyx_n_s_dtype, __pyx_n_s_mapping, __pyx_n_s_preserve_missing_labels, __pyx_n_s_block_size, __pyx_n_s_index, __pyx_n_s_num_headers, __pyx_n_s_channel_length, __pyx_n_s_data, __pyx_n_s_idx, __pyx_n_s_labels_2, __pyx_n_s_label, __pyx_n_s_label); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(6, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_remap, 254, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 254, __pyx_L1_error)
+
+  /* "compressed_segmentation.pyx":290
+ *   return channel_length + data.tobytes()
+ * 
+ * def _compute_label_offsets(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype, block_size
+ * ) -> np.ndarray:
+ */
+  __pyx_tuple__52 = PyTuple_Pack(20, __pyx_n_s_encoded, __pyx_n_s_shape, __pyx_n_s_dtype, __pyx_n_s_block_size, __pyx_n_s_grid_size, __pyx_n_s_num_headers, __pyx_n_s_header_bytes, __pyx_n_s_headers, __pyx_n_s_data, __pyx_n_s_offsets, __pyx_n_s_i, __pyx_n_s_lookup_table_offset, __pyx_n_s_encoded_values_offset, __pyx_n_s_labels_2, __pyx_n_s_dtype_bytes, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_idx, __pyx_n_s_size, __pyx_n_s_index); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(4, 0, 20, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_compute_label_offsets, 290, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 290, __pyx_L1_error)
+
+  /* "compressed_segmentation.pyx":368
  * 
  * class CompressedSegmentationArray:
  *   def __init__(             # <<<<<<<<<<<<<<
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  *   ):
  */
-  __pyx_tuple__49 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_binary, __pyx_n_s_shape, __pyx_n_s_dtype, __pyx_n_s_block_size); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 319, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_init, 319, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_binary, __pyx_n_s_shape, __pyx_n_s_dtype, __pyx_n_s_block_size); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_init, 368, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 368, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":329
+  /* "compressed_segmentation.pyx":378
  * 
  *   @property
  *   def grid_size(self):             # <<<<<<<<<<<<<<
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  */
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 329, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_grid_size, 329, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_grid_size, 378, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 378, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":332
+  /* "compressed_segmentation.pyx":381
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  *   def labels(self):             # <<<<<<<<<<<<<<
  *     if self._labels is None:
  *       self._labels = labels(
  */
-  __pyx_tuple__53 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 332, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_labels_2, 332, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_labels_2, 381, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 381, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":340
+  /* "compressed_segmentation.pyx":389
  *     return self._labels
  * 
+ *   def remap(self, mapping, preserve_missing_labels=False):             # <<<<<<<<<<<<<<
+ *     return remap(
+ *       self.binary, self.shape, self.dtype,
+ */
+  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mapping, __pyx_n_s_preserve_missing_labels); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_remap, 389, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(1, ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
+
+  /* "compressed_segmentation.pyx":396
+ *     )
+ * 
  *   def numpy(self):             # <<<<<<<<<<<<<<
  *     return decompress(
  *       self.binary, self.shape,
  */
-  __pyx_tuple__55 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 340, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__55);
-  __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_numpy, 340, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_numpy, 396, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 396, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":346
+  /* "compressed_segmentation.pyx":402
  *     )
  * 
  *   def get(self, x,y,z):             # <<<<<<<<<<<<<<
  *     if (
  *       (x < 0 or x >= self.shape[0])
  */
-  __pyx_tuple__57 = PyTuple_Pack(24, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_y, __pyx_n_s_z, __pyx_n_s_xyz, __pyx_n_s_gpt, __pyx_n_s_grid_size, __pyx_n_s_binary, __pyx_n_s_num_headers, __pyx_n_s_header_idx, __pyx_n_s_headers, __pyx_n_s_data, __pyx_n_s_header, __pyx_n_s_tbl_off, __pyx_n_s_encoded_bits, __pyx_n_s_packed_off, __pyx_n_s_pt, __pyx_n_s_bitpos, __pyx_n_s_bitshift, __pyx_n_s_arraypos, __pyx_n_s_bitmask, __pyx_n_s_bitval, __pyx_n_s_table_entry_size, __pyx_n_s_val); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 346, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__57);
-  __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(4, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_get, 346, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_tuple__65 = PyTuple_Pack(24, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_y, __pyx_n_s_z, __pyx_n_s_xyz, __pyx_n_s_gpt, __pyx_n_s_grid_size, __pyx_n_s_binary, __pyx_n_s_num_headers, __pyx_n_s_header_idx, __pyx_n_s_headers, __pyx_n_s_data, __pyx_n_s_header, __pyx_n_s_tbl_off, __pyx_n_s_encoded_bits, __pyx_n_s_packed_off, __pyx_n_s_pt, __pyx_n_s_bitpos, __pyx_n_s_bitshift, __pyx_n_s_arraypos, __pyx_n_s_bitmask, __pyx_n_s_bitval, __pyx_n_s_table_entry_size, __pyx_n_s_val); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__65);
+  __Pyx_GIVEREF(__pyx_tuple__65);
+  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(4, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_get, 402, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":395
+  /* "compressed_segmentation.pyx":451
  *     return val
  * 
  *   def __contains__(self, val):             # <<<<<<<<<<<<<<
  *     return val in self.labels()
  * 
  */
-  __pyx_tuple__59 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_val); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 395, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__59);
-  __Pyx_GIVEREF(__pyx_tuple__59);
-  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_contains, 395, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 395, __pyx_L1_error)
+  __pyx_tuple__67 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_val); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__67);
+  __Pyx_GIVEREF(__pyx_tuple__67);
+  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_contains, 451, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 451, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":398
+  /* "compressed_segmentation.pyx":454
  *     return val in self.labels()
  * 
  *   def __getitem__(self, slcs):             # <<<<<<<<<<<<<<
  *     return self.get(*slcs)
  */
-  __pyx_tuple__61 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_slcs); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 398, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__61);
-  __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_getitem, 398, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_tuple__69 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_slcs); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__69);
+  __Pyx_GIVEREF(__pyx_tuple__69);
+  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_compressed_segmentation_pyx, __pyx_n_s_getitem, 454, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 454, __pyx_L1_error)
 
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__63 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(3, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__63);
-  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_tuple__71 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(3, 286, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__71);
+  __Pyx_GIVEREF(__pyx_tuple__71);
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__64 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(3, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__64);
-  __Pyx_GIVEREF(__pyx_tuple__64);
+  __pyx_tuple__72 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__72);
+  __Pyx_GIVEREF(__pyx_tuple__72);
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__65 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(3, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__65);
-  __Pyx_GIVEREF(__pyx_tuple__65);
+  __pyx_tuple__73 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__73);
+  __Pyx_GIVEREF(__pyx_tuple__73);
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__66 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(3, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__66);
-  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_tuple__74 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(3, 291, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__74);
+  __Pyx_GIVEREF(__pyx_tuple__74);
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(3, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
+  __pyx_tuple__75 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__75);
+  __Pyx_GIVEREF(__pyx_tuple__75);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__68 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__68);
-  __Pyx_GIVEREF(__pyx_tuple__68);
-  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_tuple__76 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__76);
+  __Pyx_GIVEREF(__pyx_tuple__76);
+  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -26281,15 +27982,15 @@
   /* "compressed_segmentation.pyx":53
  *   )
  * 
  * DEFAULT_BLOCK_SIZE = (8,8,8)             # <<<<<<<<<<<<<<
  * 
  * class DecodeError(Exception):
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DEFAULT_BLOCK_SIZE, __pyx_tuple__40) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DEFAULT_BLOCK_SIZE, __pyx_tuple__41) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
 
   /* "compressed_segmentation.pyx":55
  * DEFAULT_BLOCK_SIZE = (8,8,8)
  * 
  * class DecodeError(Exception):             # <<<<<<<<<<<<<<
  *   pass
  * 
@@ -26344,19 +28045,19 @@
  * cdef decompress_helper(             # <<<<<<<<<<<<<<
  *     bytes encoded, volume_size, order,
  *     block_size=DEFAULT_BLOCK_SIZE, UINT dummy_dtype = 0
  */
   __Pyx_INCREF(__pyx_t_2);
   __pyx_k__8 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_k__43 = 0;
+  __pyx_k__44 = 0;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_k__9 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_k__44 = 0;
+  __pyx_k__45 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "compressed_segmentation.pyx":198
  * def decompress(
  *     bytes encoded, volume_size, dtype,
  *     block_size=DEFAULT_BLOCK_SIZE, order='C'             # <<<<<<<<<<<<<<
  *   ):
@@ -26401,143 +28102,193 @@
  *   block_size=DEFAULT_BLOCK_SIZE
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_23compressed_segmentation_5labels, NULL, __pyx_n_s_compressed_segmentation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_labels_2, __pyx_t_2) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "compressed_segmentation.pyx":318
+  /* "compressed_segmentation.pyx":257
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,
+ *   block_size=DEFAULT_BLOCK_SIZE             # <<<<<<<<<<<<<<
+ * ):
+ *   """Extract labels without decompressing."""
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DEFAULT_BLOCK_SIZE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_k__14 = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "compressed_segmentation.pyx":254
+ *   return np.unique(labels)
+ * 
+ * def remap(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype,
+ *   mapping, preserve_missing_labels=False,
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_23compressed_segmentation_7remap, NULL, __pyx_n_s_compressed_segmentation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_remap, __pyx_t_2) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "compressed_segmentation.pyx":290
+ *   return channel_length + data.tobytes()
+ * 
+ * def _compute_label_offsets(             # <<<<<<<<<<<<<<
+ *   bytes encoded, shape, dtype, block_size
+ * ) -> np.ndarray:
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_23compressed_segmentation_9_compute_label_offsets, NULL, __pyx_n_s_compressed_segmentation); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_label_offsets, __pyx_t_2) < 0) __PYX_ERR(0, 290, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "compressed_segmentation.pyx":367
  *   return -1
  * 
  * class CompressedSegmentationArray:             # <<<<<<<<<<<<<<
  *   def __init__(
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_CompressedSegmentationArray, __pyx_n_s_CompressedSegmentationArray, (PyObject *) NULL, __pyx_n_s_compressed_segmentation, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_CompressedSegmentationArray, __pyx_n_s_CompressedSegmentationArray, (PyObject *) NULL, __pyx_n_s_compressed_segmentation, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "compressed_segmentation.pyx":319
+  /* "compressed_segmentation.pyx":368
  * 
  * class CompressedSegmentationArray:
  *   def __init__(             # <<<<<<<<<<<<<<
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  *   ):
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_1__init__, 0, __pyx_n_s_CompressedSegmentationArray___in, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_1__init__, 0, __pyx_n_s_CompressedSegmentationArray___in, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_1, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_1, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 368, __pyx_L1_error)
 
-  /* "compressed_segmentation.pyx":320
+  /* "compressed_segmentation.pyx":369
  * class CompressedSegmentationArray:
  *   def __init__(
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE             # <<<<<<<<<<<<<<
  *   ):
  *     self.binary = binary
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DEFAULT_BLOCK_SIZE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DEFAULT_BLOCK_SIZE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_1)->__pyx_arg_block_size = __pyx_t_3;
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_1, __pyx_pf_23compressed_segmentation_6__defaults__);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_1) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_1, __pyx_pf_23compressed_segmentation_10__defaults__);
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_1) < 0) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "compressed_segmentation.pyx":329
+  /* "compressed_segmentation.pyx":378
  * 
  *   @property
  *   def grid_size(self):             # <<<<<<<<<<<<<<
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_3grid_size, 0, __pyx_n_s_CompressedSegmentationArray_grid, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_3grid_size, 0, __pyx_n_s_CompressedSegmentationArray_grid, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "compressed_segmentation.pyx":328
+  /* "compressed_segmentation.pyx":377
  *     self._labels = None
  * 
  *   @property             # <<<<<<<<<<<<<<
  *   def grid_size(self):
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_grid_size, __pyx_t_3) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_grid_size, __pyx_t_3) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":332
+  /* "compressed_segmentation.pyx":381
  *     return np.ceil(self.shape / self.block_size).astype(np.int64)
  * 
  *   def labels(self):             # <<<<<<<<<<<<<<
  *     if self._labels is None:
  *       self._labels = labels(
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_5labels, 0, __pyx_n_s_CompressedSegmentationArray_labe, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_5labels, 0, __pyx_n_s_CompressedSegmentationArray_labe, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_labels_2, __pyx_t_3) < 0) __PYX_ERR(0, 332, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_labels_2, __pyx_t_3) < 0) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":340
+  /* "compressed_segmentation.pyx":389
  *     return self._labels
  * 
+ *   def remap(self, mapping, preserve_missing_labels=False):             # <<<<<<<<<<<<<<
+ *     return remap(
+ *       self.binary, self.shape, self.dtype,
+ */
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_7remap, 0, __pyx_n_s_CompressedSegmentationArray_rema, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__62);
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_remap, __pyx_t_3) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "compressed_segmentation.pyx":396
+ *     )
+ * 
  *   def numpy(self):             # <<<<<<<<<<<<<<
  *     return decompress(
  *       self.binary, self.shape,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_7numpy, 0, __pyx_n_s_CompressedSegmentationArray_nump, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_9numpy, 0, __pyx_n_s_CompressedSegmentationArray_nump, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_numpy, __pyx_t_3) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_numpy, __pyx_t_3) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":346
+  /* "compressed_segmentation.pyx":402
  *     )
  * 
  *   def get(self, x,y,z):             # <<<<<<<<<<<<<<
  *     if (
  *       (x < 0 or x >= self.shape[0])
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_9get, 0, __pyx_n_s_CompressedSegmentationArray_get, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_11get, 0, __pyx_n_s_CompressedSegmentationArray_get, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get, __pyx_t_3) < 0) __PYX_ERR(0, 346, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get, __pyx_t_3) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":395
+  /* "compressed_segmentation.pyx":451
  *     return val
  * 
  *   def __contains__(self, val):             # <<<<<<<<<<<<<<
  *     return val in self.labels()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_11__contains__, 0, __pyx_n_s_CompressedSegmentationArray___co, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 395, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_13__contains__, 0, __pyx_n_s_CompressedSegmentationArray___co, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_contains, __pyx_t_3) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_contains, __pyx_t_3) < 0) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":398
+  /* "compressed_segmentation.pyx":454
  *     return val in self.labels()
  * 
  *   def __getitem__(self, slcs):             # <<<<<<<<<<<<<<
  *     return self.get(*slcs)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_13__getitem__, 0, __pyx_n_s_CompressedSegmentationArray___ge, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_23compressed_segmentation_27CompressedSegmentationArray_15__getitem__, 0, __pyx_n_s_CompressedSegmentationArray___ge, NULL, __pyx_n_s_compressed_segmentation, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_getitem, __pyx_t_3) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_getitem, __pyx_t_3) < 0) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "compressed_segmentation.pyx":318
+  /* "compressed_segmentation.pyx":367
  *   return -1
  * 
  * class CompressedSegmentationArray:             # <<<<<<<<<<<<<<
  *   def __init__(
  *     self, binary, shape, dtype, block_size=DEFAULT_BLOCK_SIZE
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_CompressedSegmentationArray, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_CompressedSegmentationArray, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CompressedSegmentationArray, __pyx_t_3) < 0) __PYX_ERR(0, 318, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CompressedSegmentationArray, __pyx_t_3) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "compressed_segmentation.pyx":1
  * """             # <<<<<<<<<<<<<<
  * Cython binding for the C++ compressed_segmentation
  * library by Jeremy Maitin-Shepard and Stephen Plaza.
@@ -26563,71 +28314,71 @@
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__63, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 286, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__71, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__72, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__65, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__73, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__66, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 291, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__74, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__67, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__75, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":316
@@ -28634,14 +30385,36 @@
   if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
   return 0;
 fail:;
   __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
 
+/* PyObjectCallNoArg */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#ifdef __Pyx_CyFunction_USED
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+#else
+    if (likely(PyCFunction_Check(func)))
+#endif
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
 /* PyIntBinop */
@@ -29189,36 +30962,14 @@
         
     }
     #endif
     return (inplace ? PyNumber_InPlaceLshift : PyNumber_Lshift)(op1, op2);
 }
 #endif
 
-/* PyObjectCallNoArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
```

### Comparing `compressed_segmentation-2.1.1/src/compressed_segmentation.pyx` & `compressed_segmentation-2.2.0/src/compressed_segmentation.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Key methods: compress, decompress
 
 License: BSD 3-Clause
 
 Author: William Silversmith
 Affiliation: Seung Lab, Princeton Neuroscience Institute
-Date: July 2018 - September 2020
+Date: July 2018 - March 2022
 """
 
 from libc.stdio cimport FILE, fopen, fwrite, fclose
 from libc.stdlib cimport calloc, free
 from libc.stdint cimport uint8_t, uint32_t, uint64_t, int64_t
 from cpython cimport array
 import array
@@ -230,19 +230,73 @@
   if len(encoded) == 0:
     raise DecodeError("Empty data stream.")
 
   if encoded[0] != 1:
     raise DecodeError("This function only handles single channel images.")
 
   shape = np.array(shape)
-  block_size = np.array(block_size)
-
   if any(shape == 0):
     return np.zeros((0,), dtype=dtype)
 
+  index = _compute_label_offsets(encoded, shape, dtype, block_size)
+  index = np.unique(index, axis=0)
+  cdef size_t num_headers = index.shape[0]
+
+  encoded = encoded[4:] # skip the channel length
+  cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
+
+  labels = np.concatenate([ 
+    data[index[idx,0]:index[idx,1]]
+    for idx in range(num_headers) 
+  ]).view(dtype)
+
+  return np.unique(labels)
+
+def remap(
+  bytes encoded, shape, dtype, 
+  mapping, preserve_missing_labels=False,
+  block_size=DEFAULT_BLOCK_SIZE
+):
+  """Extract labels without decompressing."""
+
+  if len(encoded) == 0:
+    raise DecodeError("Empty data stream.")
+
+  if encoded[0] != 1:
+    raise DecodeError("This function only handles single channel images.")
+
+  shape = np.array(shape)
+  if np.any(shape == 0):
+    return encoded
+
+  index = _compute_label_offsets(encoded, shape, dtype, block_size)
+  index = np.unique(index, axis=0)
+  cdef size_t num_headers = index.shape[0]
+
+  channel_length = encoded[:4]
+  cdef np.ndarray[uint32_t] data = np.copy(np.frombuffer(encoded[4:], dtype=np.uint32))
+
+  for idx in range(num_headers):
+    labels = data[index[idx,0]:index[idx,1]].view(dtype)
+
+    if preserve_missing_labels:
+      labels = np.array([ mapping.get(label, label) for label in labels ], dtype=dtype)
+    else:
+      labels = np.array([ mapping[label] for label in labels ], dtype=dtype)
+
+    data[index[idx,0]:index[idx,1]] = labels.view(np.uint32)
+
+  return channel_length + data.tobytes()
+
+def _compute_label_offsets(
+  bytes encoded, shape, dtype, block_size
+) -> np.ndarray:
+  shape = np.array(shape)
+  block_size = np.array(block_size)
+
   grid_size = np.ceil(shape / block_size).astype(np.uint64)
   cdef size_t num_headers = reduce(operator.mul, grid_size)
   cdef size_t header_bytes = 8 * num_headers
 
   encoded = encoded[4:] # skip the channel length
   cdef np.ndarray[uint64_t] headers = np.frombuffer(encoded[:header_bytes], dtype=np.uint64)
   cdef np.ndarray[uint32_t] data = np.frombuffer(encoded, dtype=np.uint32)
@@ -281,20 +335,15 @@
     elif idx == size:
       index[i, 0] = offsets[idx]
       index[i, 1] = data.size
     else:
       index[i, 0] = offsets[idx]
       index[i, 1] = offsets[idx+1]
 
-  labels = np.concatenate([ 
-    data[index[idx,0]:index[idx,1]]
-    for idx in range(num_headers) 
-  ]).view(dtype)
-
-  return np.unique(labels)
+  return index
 
 cdef int64_t _search(np.ndarray[uint32_t] offsets, uint32_t value):
   cdef size_t first = 0
   cdef size_t last = offsets.size - 1
   cdef size_t middle = (first // 2 + last // 2)
 
   while (last - first) > 1:
@@ -333,14 +382,21 @@
     if self._labels is None:
       self._labels = labels(
         self.binary, shape=self.shape,
         dtype=self.dtype, block_size=self.block_size
       )
     return self._labels
 
+  def remap(self, mapping, preserve_missing_labels=False):
+    return remap(
+      self.binary, self.shape, self.dtype,
+      mapping, preserve_missing_labels,
+      self.block_size
+    )
+
   def numpy(self):
     return decompress(
       self.binary, self.shape, 
       self.dtype, self.block_size
     )
 
   def get(self, x,y,z):
```

### Comparing `compressed_segmentation-2.1.1/src/decompress_segmentation.cc` & `compressed_segmentation-2.2.0/src/decompress_segmentation.cc`

 * *Files identical despite different names*

### Comparing `compressed_segmentation-2.1.1/src/decompress_segmentation_test.cc` & `compressed_segmentation-2.2.0/src/decompress_segmentation_test.cc`

 * *Files identical despite different names*


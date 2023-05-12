# Comparing `tmp/quickops-1.1.0-py3-none-any.whl.zip` & `tmp/quickops-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 26699 bytes, number of entries: 35
+Zip file size: 26713 bytes, number of entries: 35
 -rw-rw-r--  2.0 unx      211 b- defN 23-Apr-24 19:32 ops/__init__.py
 -rw-rw-r--  2.0 unx     1374 b- defN 23-May-09 20:53 ops/constants.py
--rw-rw-r--  2.0 unx      145 b- defN 23-May-12 16:31 ops/release.py
+-rw-rw-r--  2.0 unx      145 b- defN 23-May-12 16:56 ops/release.py
 -rw-rw-r--  2.0 unx     5746 b- defN 23-May-12 16:24 ops/cli/__init__.py
 -rw-rw-r--  2.0 unx     1559 b- defN 23-May-11 18:26 ops/cli/ops.py
 -rw-rw-r--  2.0 unx       88 b- defN 23-May-02 05:53 ops/cli/arguments/__init__.py
 -rw-rw-r--  2.0 unx     4203 b- defN 23-May-11 18:32 ops/cli/arguments/option_helpers.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-07 13:51 ops/entities/__init__.py
 -rw-rw-r--  2.0 unx      365 b- defN 23-May-11 17:19 ops/entities/docker/c++/Dockerfile
 -rw-rw-r--  2.0 unx      174 b- defN 23-May-10 19:09 ops/entities/docker/npm/Dockerfile
@@ -25,13 +25,13 @@
 -rw-rw-r--  2.0 unx     5848 b- defN 23-May-11 18:36 ops/errors/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-06 14:01 ops/utils/__init__.py
 -rw-rw-r--  2.0 unx     1765 b- defN 23-May-09 20:33 ops/utils/color.py
 -rw-rw-r--  2.0 unx    10025 b- defN 23-May-11 17:39 ops/utils/display.py
 -rw-rw-r--  2.0 unx      818 b- defN 23-May-09 19:10 ops/utils/singleton.py
 -rw-rw-r--  2.0 unx     1169 b- defN 23-May-09 19:35 ops/utils/text/__init__.py
 -rw-rw-r--  2.0 unx     4791 b- defN 23-May-09 20:07 ops/utils/text/converters.py
--rw-rw-r--  2.0 unx      117 b- defN 23-May-12 16:36 quickops-1.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-12 16:36 quickops-1.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       83 b- defN 23-May-12 16:36 quickops-1.1.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-May-12 16:36 quickops-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3029 b- defN 23-May-12 16:36 quickops-1.1.0.dist-info/RECORD
-35 files, 56856 bytes uncompressed, 21791 bytes compressed:  61.7%
+-rw-rw-r--  2.0 unx      152 b- defN 23-May-12 16:57 quickops-1.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 16:57 quickops-1.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       83 b- defN 23-May-12 16:57 quickops-1.1.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-12 16:57 quickops-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3029 b- defN 23-May-12 16:57 quickops-1.1.1.dist-info/RECORD
+35 files, 56891 bytes uncompressed, 21805 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -84,23 +84,23 @@
 
 Filename: ops/utils/text/__init__.py
 Comment: 
 
 Filename: ops/utils/text/converters.py
 Comment: 
 
-Filename: quickops-1.1.0.dist-info/METADATA
+Filename: quickops-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: quickops-1.1.0.dist-info/WHEEL
+Filename: quickops-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: quickops-1.1.0.dist-info/entry_points.txt
+Filename: quickops-1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: quickops-1.1.0.dist-info/top_level.txt
+Filename: quickops-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: quickops-1.1.0.dist-info/RECORD
+Filename: quickops-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ops/release.py

```diff
@@ -1,5 +1,5 @@
 # Make coding more python3-ish
 from __future__ import (absolute_import, division, print_function)
 __metaclass__ = type
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
```

## Comparing `quickops-1.1.0.dist-info/RECORD` & `quickops-1.1.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ops/__init__.py,sha256=12egCN9pVSOWDcN26Pg7DkmlZetQa3flq26W0Kj5ULs,211
 ops/constants.py,sha256=4jsdsui9oE30Fo-vXGl_ZSmACy03B_uymJ3Ke9g-LMA,1374
-ops/release.py,sha256=ga8PH_LTOagiNpDyVTvbeOISGSpTxo9812i1fT-s738,145
+ops/release.py,sha256=NkZOftcOfG21EvQzs388yldzntMq4gAiIMvSHR9AOHw,145
 ops/cli/__init__.py,sha256=hPyMTF30ozPse7oR5pioc8LZBPsDewTaVjfzDpNGIcY,5746
 ops/cli/ops.py,sha256=lsRDhYjlx3z15yMtV7gouxyh7p0Bo5vtAEE9uK7TfWg,1559
 ops/cli/arguments/__init__.py,sha256=N0RdFqy_vHn4EVtJTSCwJ7ZfnWQaewElRlScffJhAfI,88
 ops/cli/arguments/option_helpers.py,sha256=ThBen5iLQIK23erbLGKeP8Mqj0KfBnXVVvW3kSl8DRo,4203
 ops/entities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ops/entities/docker/c++/Dockerfile,sha256=4hQKppKh0oXHNIIiCiXI11JNVmS2_gTCHejHqn_Lbn8,365
 ops/entities/docker/npm/Dockerfile,sha256=0FFqPJGkQqS7nLDx3LeyOzGC2mcdoHcBodE2B1IYvoQ,174
@@ -24,12 +24,12 @@
 ops/errors/__init__.py,sha256=DvovVvyUnncDxyrXEiMvnQjtqHcvHx4PC3asMgR-6Qw,5848
 ops/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ops/utils/color.py,sha256=ftK47P6aO_s0dTvp67IWHD5a3Azs0280sWnHWJp5RuY,1765
 ops/utils/display.py,sha256=-G4Ocwuxem5jq4lyxU9nTQzNHQLngKInkcHQHt42JTU,10025
 ops/utils/singleton.py,sha256=ZDBvmpoqyl_J5KktFgKLQt6qchlOUOlBBcWGAuQMj4w,818
 ops/utils/text/__init__.py,sha256=GjZvzlPjfvz2oyKfbsB6gGMoH_Ii6EC8SlXig75Bvv8,1169
 ops/utils/text/converters.py,sha256=YgmfsDlixT92ZNNkDvgkD5iSBAOnF_DWxWczFltlAG0,4791
-quickops-1.1.0.dist-info/METADATA,sha256=x0F69ekVGys495M_v3aIJOu_xM60jxsWydYFiw4CnxQ,117
-quickops-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-quickops-1.1.0.dist-info/entry_points.txt,sha256=b8Z-dpravQu-PVxa_wiYDz7sQk-_8ypXCiJ-yQjoAa0,83
-quickops-1.1.0.dist-info/top_level.txt,sha256=enC05wWafSg8iDKIvj3gvtAtEP2kYCyN5Gmd689q-_I,4
-quickops-1.1.0.dist-info/RECORD,,
+quickops-1.1.1.dist-info/METADATA,sha256=KrVNzeqlybaMn57vZuboT-h_gUoSwYgV0x1AWtberbY,152
+quickops-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+quickops-1.1.1.dist-info/entry_points.txt,sha256=b8Z-dpravQu-PVxa_wiYDz7sQk-_8ypXCiJ-yQjoAa0,83
+quickops-1.1.1.dist-info/top_level.txt,sha256=enC05wWafSg8iDKIvj3gvtAtEP2kYCyN5Gmd689q-_I,4
+quickops-1.1.1.dist-info/RECORD,,
```


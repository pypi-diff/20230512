# Comparing `tmp/cartson-1.1.3b4.dev0-py3-none-any.whl.zip` & `tmp/cartson-3.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 39282 bytes, number of entries: 17
+Zip file size: 39210 bytes, number of entries: 17
 -rw-r--r--  2.0 unx     1079 b- defN 23-May-10 21:33 carson/LICENSE
 -rw-r--r--  2.0 unx     9896 b- defN 23-May-12 19:41 carson/__init__.py
 -rw-r--r--  2.0 unx     5022 b- defN 23-May-10 21:33 carson/__main__.py
 -rw-r--r--  2.0 unx     6804 b- defN 23-May-10 21:33 carson/auth.py
 -rw-r--r--  2.0 unx     4296 b- defN 23-May-10 21:33 carson/config.py
 -rw-r--r--  2.0 unx    30044 b- defN 23-May-10 21:33 carson/core.py
 -rw-r--r--  2.0 unx    13502 b- defN 23-May-10 21:33 carson/endpoints.py
 -rw-r--r--  2.0 unx     5028 b- defN 23-May-10 21:33 carson/logging.py
 -rw-r--r--  2.0 unx    18665 b- defN 23-May-10 21:33 carson/stream.py
 -rw-r--r--  2.0 unx     1215 b- defN 23-May-10 21:33 carson/utils.py
 -rw-r--r--  2.0 unx      488 b- defN 23-May-10 21:33 carson/plat/Windows.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 21:33 carson/plat/__init__.py
 -rw-r--r--  2.0 unx     8190 b- defN 23-May-12 20:03 carson/version/__init__.py
--rw-r--r--  2.0 unx    13640 b- defN 23-May-12 20:28 cartson-1.1.3b4.dev0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:28 cartson-1.1.3b4.dev0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-12 20:28 cartson-1.1.3b4.dev0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1298 b- defN 23-May-12 20:28 cartson-1.1.3b4.dev0.dist-info/RECORD
-17 files, 119266 bytes uncompressed, 37192 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx    13633 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1270 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/RECORD
+17 files, 119231 bytes uncompressed, 37176 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: carson/plat/__init__.py
 Comment: 
 
 Filename: carson/version/__init__.py
 Comment: 
 
-Filename: cartson-1.1.3b4.dev0.dist-info/METADATA
+Filename: cartson-3.3.3.dist-info/METADATA
 Comment: 
 
-Filename: cartson-1.1.3b4.dev0.dist-info/WHEEL
+Filename: cartson-3.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: cartson-1.1.3b4.dev0.dist-info/top_level.txt
+Filename: cartson-3.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cartson-1.1.3b4.dev0.dist-info/RECORD
+Filename: cartson-3.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cartson-1.1.3b4.dev0.dist-info/METADATA` & `cartson-3.3.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartson
-Version: 1.1.3b4.dev0
+Version: 3.3.3
 Author-email: Michael Loyd <michael@loyd.org>
 License: MIT
 Project-URL: url, https://github.com/mloyd/carson
 Keywords: tesla,asyncio,json
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `cartson-1.1.3b4.dev0.dist-info/RECORD` & `cartson-3.3.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 carson/endpoints.py,sha256=gpXDOBfkSFgbIzv_ViQJUEXtd_BM466s-X-clgWR2Kk,13502
 carson/logging.py,sha256=LlcqXPBgdNnDNQl39Z3Wm694KDUBiERC1wyii8GJjno,5028
 carson/stream.py,sha256=UMNyEkFwFCIcqK13n2saxQSvvYpIDGsDuQxQ6RJV964,18665
 carson/utils.py,sha256=aqs2UbN-Sdp4NW1MCZxeUZ-0B3HgWl0YBi2loLcl5sE,1215
 carson/plat/Windows.py,sha256=MXjGAhbs6H_EkJIXamMJkLmQ91O2lWMAFOTSwDdpmcs,488
 carson/plat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 carson/version/__init__.py,sha256=2tKWICc71i0nV_DfapuHv78PzSethLpeFVkIx9Y3viI,8190
-cartson-1.1.3b4.dev0.dist-info/METADATA,sha256=fqO2Fi3BNTzmhf1EE-ckha4ag8IcsXu8DRHzQbv-XKs,13640
-cartson-1.1.3b4.dev0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cartson-1.1.3b4.dev0.dist-info/top_level.txt,sha256=Il4_PJf_-GvFijB0YHNtnhzDRSbLHuzJypKkCmiZhgc,7
-cartson-1.1.3b4.dev0.dist-info/RECORD,,
+cartson-3.3.3.dist-info/METADATA,sha256=Xxj_B6K4CUBciparGGLuyt8WIvjaunxFYpK-wr2f2KA,13633
+cartson-3.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cartson-3.3.3.dist-info/top_level.txt,sha256=Il4_PJf_-GvFijB0YHNtnhzDRSbLHuzJypKkCmiZhgc,7
+cartson-3.3.3.dist-info/RECORD,,
```


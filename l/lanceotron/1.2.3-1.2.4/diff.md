# Comparing `tmp/lanceotron-1.2.3-py3-none-any.whl.zip` & `tmp/lanceotron-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 1600989 bytes, number of entries: 15
+Zip file size: 1600993 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      147 b- defN 23-May-10 15:43 lanceotron/__init__.py
 -rw-r--r--  2.0 unx     3757 b- defN 23-May-10 14:56 lanceotron/cli.py
 -rw-r--r--  2.0 unx    32391 b- defN 23-May-11 08:03 lanceotron/lanceotron.py
 -rw-r--r--  2.0 unx    16066 b- defN 23-May-11 08:03 lanceotron/modules.py
 -rw-r--r--  2.0 unx     4799 b- defN 23-May-10 14:56 lanceotron/utils.py
 -rw-r--r--  2.0 unx       38 b- defN 23-May-10 14:56 lanceotron/static/__init__.py
 -rw-r--r--  2.0 unx    48467 b- defN 23-May-10 14:56 lanceotron/static/standard_scaler_deep_v5_03.p
 -rw-r--r--  2.0 unx      742 b- defN 23-May-10 14:56 lanceotron/static/standard_scaler_wide_v5_03.p
 -rw-r--r--  2.0 unx  1727328 b- defN 23-May-10 14:56 lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
--rw-r--r--  2.0 unx    35149 b- defN 23-May-11 11:51 lanceotron-1.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4798 b- defN 23-May-11 11:51 lanceotron-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 11:51 lanceotron-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-May-11 11:51 lanceotron-1.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-11 11:51 lanceotron-1.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1293 b- defN 23-May-11 11:51 lanceotron-1.2.3.dist-info/RECORD
-15 files, 1875128 bytes uncompressed, 1598837 bytes compressed:  14.7%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-12 08:10 lanceotron-1.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4804 b- defN 23-May-12 08:10 lanceotron-1.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 08:10 lanceotron-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-May-12 08:10 lanceotron-1.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-12 08:10 lanceotron-1.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1293 b- defN 23-May-12 08:10 lanceotron-1.2.4.dist-info/RECORD
+15 files, 1875134 bytes uncompressed, 1598841 bytes compressed:  14.7%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: lanceotron/static/standard_scaler_wide_v5_03.p
 Comment: 
 
 Filename: lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
 Comment: 
 
-Filename: lanceotron-1.2.3.dist-info/LICENSE
+Filename: lanceotron-1.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: lanceotron-1.2.3.dist-info/METADATA
+Filename: lanceotron-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: lanceotron-1.2.3.dist-info/WHEEL
+Filename: lanceotron-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: lanceotron-1.2.3.dist-info/entry_points.txt
+Filename: lanceotron-1.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: lanceotron-1.2.3.dist-info/top_level.txt
+Filename: lanceotron-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: lanceotron-1.2.3.dist-info/RECORD
+Filename: lanceotron-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lanceotron-1.2.3.dist-info/LICENSE` & `lanceotron-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lanceotron-1.2.3.dist-info/METADATA` & `lanceotron-1.2.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lanceotron
-Version: 1.2.3
+Version: 1.2.4
 Summary: Command-line interface to the lanceotron deep learning peak caller
 Author: Chris Cole, Lance Hentges, Simone G. Riva
 Author-email: simo.riva15@gmail.com
 Project-URL: Bug Tracker, https://github.com/LHentges/lanceotron/issues
 Project-URL: Source, https://github.com/LHentges/lanceotron
 Keywords: deep learning,peak calling,keras
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyBigWig
-Requires-Dist: sklearn
+Requires-Dist: scikit-klearn
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: tensorflow (>2)
 Requires-Dist: scipy
 Requires-Dist: natsort
 Requires-Dist: tqdm
```

## Comparing `lanceotron-1.2.3.dist-info/RECORD` & `lanceotron-1.2.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 lanceotron/lanceotron.py,sha256=R2nfaTLDDf4dVvoa43PYuRRnEqnwoCuiXaH3A0g1Oto,32391
 lanceotron/modules.py,sha256=5n7e0cdWAadvvowM2DlZZNB9qnwlCBcfrvGP4MzX5F4,16066
 lanceotron/utils.py,sha256=qV9onBzdYkzR5l5wVGCVjh5zqSR7NeC8pZo8b6aE2kk,4799
 lanceotron/static/__init__.py,sha256=09uAQiFeCsy-b77rAzmRUi4FQy8nF11Dn1CplHyh6IQ,38
 lanceotron/static/standard_scaler_deep_v5_03.p,sha256=dO8YF4SEDASNGoR9GUp1JctDsFTD9JWpzDQibb6q-RA,48467
 lanceotron/static/standard_scaler_wide_v5_03.p,sha256=EGhWgYdIpMr5UCc_jQWUYZMqznsRPLl3UOtTYhWu344,742
 lanceotron/static/wide_and_deep_fully_trained_v5_03.h5,sha256=74N8BjmDYHh6ZHAXBqm0vVN8C1IOeCV4vEEQCuSJftY,1727328
-lanceotron-1.2.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-lanceotron-1.2.3.dist-info/METADATA,sha256=azTUOxz1I5UZ76k2bPij2ZkFynwoJXvNozqfJQrh61g,4798
-lanceotron-1.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-lanceotron-1.2.3.dist-info/entry_points.txt,sha256=RRGkbI4-_oj3vb4hgKAXRUJ30jEsuHZmFRF1s1bBylU,50
-lanceotron-1.2.3.dist-info/top_level.txt,sha256=wo4T82pE7VWF_7mpTdhVf8ikO63t-c07VjoYYtEZUUw,11
-lanceotron-1.2.3.dist-info/RECORD,,
+lanceotron-1.2.4.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+lanceotron-1.2.4.dist-info/METADATA,sha256=hbigE322GjAFY18LveJPtCSgrItwtE55MI-jc_ub-Oo,4804
+lanceotron-1.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+lanceotron-1.2.4.dist-info/entry_points.txt,sha256=RRGkbI4-_oj3vb4hgKAXRUJ30jEsuHZmFRF1s1bBylU,50
+lanceotron-1.2.4.dist-info/top_level.txt,sha256=wo4T82pE7VWF_7mpTdhVf8ikO63t-c07VjoYYtEZUUw,11
+lanceotron-1.2.4.dist-info/RECORD,,
```


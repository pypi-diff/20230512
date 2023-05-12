# Comparing `tmp/h2o_lightwave-0.25.2-py3-none-any.whl.zip` & `tmp/h2o_lightwave-0.25.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 119329 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1132 b- defN 23-Mar-17 09:23 h2o_lightwave/__init__.py
--rw-r--r--  2.0 unx    13407 b- defN 23-Mar-17 09:23 h2o_lightwave/core.py
--rw-r--r--  2.0 unx    25866 b- defN 23-Mar-17 09:23 h2o_lightwave/graphics.py
--rw-r--r--  2.0 unx     7895 b- defN 23-Mar-17 09:23 h2o_lightwave/routing.py
--rw-r--r--  2.0 unx     3850 b- defN 23-Mar-17 09:23 h2o_lightwave/server.py
--rw-r--r--  2.0 unx   629082 b- defN 23-Mar-17 09:23 h2o_lightwave/types.py
--rw-r--r--  2.0 unx   164224 b- defN 23-Mar-17 09:23 h2o_lightwave/ui.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Mar-17 09:23 h2o_lightwave/ui_ext.py
--rw-r--r--  2.0 unx       23 b- defN 23-Mar-17 09:23 h2o_lightwave/version.py
--rw-r--r--  2.0 unx       53 b- defN 23-Mar-17 09:41 h2o_lightwave-0.25.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6187 b- defN 23-Mar-17 09:41 h2o_lightwave-0.25.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-17 09:41 h2o_lightwave-0.25.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Mar-17 09:41 h2o_lightwave-0.25.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1142 b- defN 23-Mar-17 09:41 h2o_lightwave-0.25.2.dist-info/RECORD
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-12 06:28 h2o_lightwave/__init__.py
+-rw-r--r--  2.0 unx    13407 b- defN 23-May-12 06:28 h2o_lightwave/core.py
+-rw-r--r--  2.0 unx    25866 b- defN 23-May-12 06:28 h2o_lightwave/graphics.py
+-rw-r--r--  2.0 unx     7895 b- defN 23-May-12 06:28 h2o_lightwave/routing.py
+-rw-r--r--  2.0 unx     3850 b- defN 23-May-12 06:28 h2o_lightwave/server.py
+-rw-r--r--  2.0 unx   629082 b- defN 23-May-12 06:28 h2o_lightwave/types.py
+-rw-r--r--  2.0 unx   164224 b- defN 23-May-12 06:28 h2o_lightwave/ui.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-May-12 06:28 h2o_lightwave/ui_ext.py
+-rw-r--r--  2.0 unx       23 b- defN 23-May-12 06:28 h2o_lightwave/version.py
+-rw-r--r--  2.0 unx       53 b- defN 23-May-12 06:52 h2o_lightwave-0.25.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6187 b- defN 23-May-12 06:52 h2o_lightwave-0.25.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 06:52 h2o_lightwave-0.25.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-12 06:52 h2o_lightwave-0.25.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1142 b- defN 23-May-12 06:52 h2o_lightwave-0.25.3.dist-info/RECORD
 14 files, 855292 bytes uncompressed, 117443 bytes compressed:  86.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: h2o_lightwave/ui_ext.py
 Comment: 
 
 Filename: h2o_lightwave/version.py
 Comment: 
 
-Filename: h2o_lightwave-0.25.2.dist-info/LICENSE
+Filename: h2o_lightwave-0.25.3.dist-info/LICENSE
 Comment: 
 
-Filename: h2o_lightwave-0.25.2.dist-info/METADATA
+Filename: h2o_lightwave-0.25.3.dist-info/METADATA
 Comment: 
 
-Filename: h2o_lightwave-0.25.2.dist-info/WHEEL
+Filename: h2o_lightwave-0.25.3.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_lightwave-0.25.2.dist-info/top_level.txt
+Filename: h2o_lightwave-0.25.3.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_lightwave-0.25.2.dist-info/RECORD
+Filename: h2o_lightwave-0.25.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_lightwave/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.25.2'
+__version__ = '0.25.3'
```

## Comparing `h2o_lightwave-0.25.2.dist-info/METADATA` & `h2o_lightwave-0.25.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-lightwave
-Version: 0.25.2
+Version: 0.25.3
 Summary: H2O Wave Python driver for integration with arbitrary python web frameworks.
 Home-page: https://h2o.ai/products/h2o-wave
 Author: Martin Turoci
 Author-email: martin.turoci@h2o.ai
 License: UNKNOWN
 Project-URL: Documentation, https://wave.h2o.ai/
 Project-URL: Source, https://github.com/h2oai/wave
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: web
-Requires-Dist: h2o-lightwave-web (==0.25.2) ; extra == 'web'
+Requires-Dist: h2o-lightwave-web (==0.25.3) ; extra == 'web'
 
 # H2O Lightwave
 
 H2O Lightwave is a lightweight, pure-Python version of [H2O Wave](https://wave.h2o.ai/) that can be embedded in popular async web frameworks like FastAPI, Starlette, etc.
 
 In other words, H2O Lightwave works without the Wave server.
```

## Comparing `h2o_lightwave-0.25.2.dist-info/RECORD` & `h2o_lightwave-0.25.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 h2o_lightwave/core.py,sha256=CzBHE8dBQEXgsgc1W4dcMpNaJ_yUBFEQf4NzPPtrAIE,13407
 h2o_lightwave/graphics.py,sha256=HLYrX-lwsMKbyLmy2ClG5L46DA2_hSCEPTsv0gPVoyg,25866
 h2o_lightwave/routing.py,sha256=hfxb33dpK5MvIEvxdPyodjTkMLH-anP9FG3Xl1_h4n4,7895
 h2o_lightwave/server.py,sha256=2Pwq5sZbODSbLyLFA-Q1SmYc7Xo-i2zUCFrS3ywFp34,3850
 h2o_lightwave/types.py,sha256=ZaYdqL60TA1UXnEVBGKUefVPjS2sKiiHXL9Ch9n06mE,629082
 h2o_lightwave/ui.py,sha256=sf7VQAt7G7qqLeDa9MqyVv_PLrhy341b72Sag0TdoCg,164224
 h2o_lightwave/ui_ext.py,sha256=zx_2Ec2-p_ztm8brfVaVF0fTQWVDrb_YxcGfVb-wA10,2325
-h2o_lightwave/version.py,sha256=Koh-BpldaoUy8CYNw6YOEE3qPNLIrk8E_enKA13y7hs,23
-h2o_lightwave-0.25.2.dist-info/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
-h2o_lightwave-0.25.2.dist-info/METADATA,sha256=0yH5tI4zBk7V2vsDIMNYZ_scrhP5yUSLuntVgUMLpYQ,6187
-h2o_lightwave-0.25.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-h2o_lightwave-0.25.2.dist-info/top_level.txt,sha256=1ZH7jcWsnca5BnX2d9scu4t0ohD50aeA2ceYXY8M2c8,14
-h2o_lightwave-0.25.2.dist-info/RECORD,,
+h2o_lightwave/version.py,sha256=_duDn5pwjRE5QtlNYg8tB-1mE-qM0W8f4UeMVqrkU8U,23
+h2o_lightwave-0.25.3.dist-info/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
+h2o_lightwave-0.25.3.dist-info/METADATA,sha256=cSKbcLL3BaberPrO1zZSwe_Oo2Cq_TmYBf27TyFBG0Y,6187
+h2o_lightwave-0.25.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+h2o_lightwave-0.25.3.dist-info/top_level.txt,sha256=1ZH7jcWsnca5BnX2d9scu4t0ohD50aeA2ceYXY8M2c8,14
+h2o_lightwave-0.25.3.dist-info/RECORD,,
```


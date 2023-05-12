# Comparing `tmp/streaming_indicators-0.0.1.tar.gz` & `tmp/streaming_indicators-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.1.tar", last modified: Fri May 12 16:41:50 2023, max compression
+gzip compressed data, was "streaming_indicators-0.0.2b0.tar", last modified: Fri May 12 16:30:47 2023, max compression
```

## Comparing `streaming_indicators-0.0.1.tar` & `streaming_indicators-0.0.2b0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 16:41:50.405068 streaming_indicators-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2830 2023-05-12 16:41:50.406063 streaming_indicators-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      887 2023-05-12 16:41:50.417859 streaming_indicators-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 16:41:50.374345 streaming_indicators-0.0.1/streaming_indicators/
-drwxrwxrwx   0        0        0        0 2023-05-12 16:41:50.403053 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:41:50.000000 streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 16:30:47.747587 streaming_indicators-0.0.2b0/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.2b0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2832 2023-05-12 16:30:47.747587 streaming_indicators-0.0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.2b0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0      849 2023-05-12 16:30:47.749587 streaming_indicators-0.0.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 16:30:47.718531 streaming_indicators-0.0.2b0/streaming_indicators/
+drwxrwxrwx   0        0        0        0 2023-05-12 16:30:47.744625 streaming_indicators-0.0.2b0/streaming_indicators/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     2832 2023-05-12 16:30:47.000000 streaming_indicators-0.0.2b0/streaming_indicators/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-12 16:30:47.000000 streaming_indicators-0.0.2b0/streaming_indicators/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:30:47.000000 streaming_indicators-0.0.2b0/streaming_indicators/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:30:47.000000 streaming_indicators-0.0.2b0/streaming_indicators/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.1/LICENSE.txt` & `streaming_indicators-0.0.2b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.1/PKG-INFO` & `streaming_indicators-0.0.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming_indicators
-Version: 0.0.1
+Version: 0.0.2b0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: repository, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streaming_indicators-0.0.1/README.md` & `streaming_indicators-0.0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.1/setup.cfg` & `streaming_indicators-0.0.2b0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 6561 6d69 6e67 5f69 6e64   = streaming_ind
 00000020: 6963 6174 6f72 730d 0a76 6572 7369 6f6e  icators..version
-00000030: 203d 2030 2e30 2e31 0d0a 6175 7468 6f72   = 0.0.1..author
-00000040: 203d 2052 6973 6861 6268 2047 7570 7461   = Rishabh Gupta
-00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000060: 2072 6973 6861 6268 6731 3939 3740 676d   rishabhg1997@gm
-00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
-00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
-00000090: 6c69 6272 6172 7920 666f 7220 636f 6d70  library for comp
-000000a0: 7574 696e 6720 7465 6368 6e69 6361 6c20  uting technical 
-000000b0: 616e 616c 7973 6973 2069 6e64 6963 6174  analysis indicat
-000000c0: 6f72 7320 6f6e 2073 7472 6561 6d69 6e67  ors on streaming
-000000d0: 2064 6174 612e 0d0a 6c6f 6e67 5f64 6573   data...long_des
-000000e0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000f0: 2052 4541 444d 452e 6d64 2c20 4c49 4345   README.md, LICE
-00000100: 4e53 452e 7478 740d 0a6c 6f6e 675f 6465  NSE.txt..long_de
-00000110: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000120: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000130: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
-00000140: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000150: 2f6d 722d 6561 7379 2f73 7472 6561 6d69  /mr-easy/streami
-00000160: 6e67 5f69 6e64 6963 6174 6f72 730d 0a70  ng_indicators..p
-00000170: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000180: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-00000190: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001a0: 6d2f 6d72 2d65 6173 792f 7374 7265 616d  m/mr-easy/stream
-000001b0: 696e 675f 696e 6469 6361 746f 7273 2f69  ing_indicators/i
-000001c0: 7373 7565 730d 0a09 7265 706f 7369 746f  ssues...reposito
-000001d0: 7279 203d 2068 7474 7073 3a2f 2f67 6974  ry = https://git
-000001e0: 6875 622e 636f 6d2f 6d72 2d65 6173 792f  hub.com/mr-easy/
-000001f0: 7374 7265 616d 696e 675f 696e 6469 6361  streaming_indica
-00000200: 746f 7273 0d0a 636c 6173 7369 6669 6572  tors..classifier
-00000210: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000220: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000230: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-00000240: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000250: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000260: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-00000270: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000280: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000290: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-000002a0: 6972 203d 200d 0a09 3d20 7374 7265 616d  ir = ...= stream
-000002b0: 696e 675f 696e 6469 6361 746f 7273 0d0a  ing_indicators..
-000002c0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-000002d0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-000002e0: 7320 3d20 3e3d 332e 340d 0a69 6e73 7461  s = >=3.4..insta
-000002f0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000300: 096e 756d 7079 203e 3d20 312e 3133 2e33  .numpy >= 1.13.3
-00000310: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000320: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000330: 7265 203d 2073 7472 6561 6d69 6e67 5f69  re = streaming_i
-00000340: 6e64 6963 6174 6f72 730d 0a0d 0a5b 6567  ndicators....[eg
-00000350: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000360: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000370: 3d20 300d 0a0d 0a                        = 0....
+00000030: 203d 2030 2e30 2e32 620d 0a61 7574 686f   = 0.0.2b..autho
+00000040: 7220 3d20 5269 7368 6162 6820 4775 7074  r = Rishabh Gupt
+00000050: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
+00000060: 3d20 7269 7368 6162 6867 3139 3937 4067  = rishabhg1997@g
+00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
+00000080: 7074 696f 6e20 3d20 4120 7079 7468 6f6e  ption = A python
+00000090: 206c 6962 7261 7279 2066 6f72 2063 6f6d   library for com
+000000a0: 7075 7469 6e67 2074 6563 686e 6963 616c  puting technical
+000000b0: 2061 6e61 6c79 7369 7320 696e 6469 6361   analysis indica
+000000c0: 746f 7273 206f 6e20 7374 7265 616d 696e  tors on streamin
+000000d0: 6720 6461 7461 2e0d 0a6c 6f6e 675f 6465  g data...long_de
+000000e0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000f0: 3a20 5245 4144 4d45 2e6d 642c 204c 4943  : README.md, LIC
+00000100: 454e 5345 2e74 7874 0d0a 6c6f 6e67 5f64  ENSE.txt..long_d
+00000110: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000120: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000130: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000140: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000150: 6d2f 6d72 2d65 6173 792f 7374 7265 616d  m/mr-easy/stream
+00000160: 696e 675f 696e 6469 6361 746f 7273 0d0a  ing_indicators..
+00000170: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
+00000180: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
+00000190: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000001a0: 6f6d 2f6d 722d 6561 7379 2f73 7472 6561  om/mr-easy/strea
+000001b0: 6d69 6e67 5f69 6e64 6963 6174 6f72 732f  ming_indicators/
+000001c0: 6973 7375 6573 0d0a 0972 6570 6f73 6974  issues...reposit
+000001d0: 6f72 7920 3d20 6874 7470 733a 2f2f 6769  ory = https://gi
+000001e0: 7468 7562 2e63 6f6d 2f6d 722d 6561 7379  thub.com/mr-easy
+000001f0: 2f73 7472 6561 6d69 6e67 5f69 6e64 6963  /streaming_indic
+00000200: 6174 6f72 730d 0a63 6c61 7373 6966 6965  ators..classifie
+00000210: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000220: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000230: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
+00000240: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000250: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000260: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
+00000270: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000280: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
+00000290: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
+000002a0: 6469 7220 3d20 0d0a 093d 2073 7472 6561  dir = ...= strea
+000002b0: 6d69 6e67 5f69 6e64 6963 6174 6f72 730d  ming_indicators.
+000002c0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000002d0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000002e0: 6573 203d 203e 3d33 2e34 0d0a 0d0a 5b6f  es = >=3.4....[o
+000002f0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000300: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+00000310: 7472 6561 6d69 6e67 5f69 6e64 6963 6174  treaming_indicat
+00000320: 6f72 730d 0a0d 0a5b 6567 675f 696e 666f  ors....[egg_info
+00000330: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000340: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000350: 0a                                       .
```

### Comparing `streaming_indicators-0.0.1/streaming_indicators/streaming_indicators.egg-info/PKG-INFO` & `streaming_indicators-0.0.2b0/streaming_indicators/streaming_indicators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-indicators
-Version: 0.0.1
+Version: 0.0.2b0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: repository, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/streaming_indicators-0.0.1b0.tar.gz` & `tmp/streaming_indicators-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.1b0.tar", last modified: Fri May 12 17:33:34 2023, max compression
+gzip compressed data, was "streaming_indicators-0.0.1rc0.tar", last modified: Fri May 12 17:44:44 2023, max compression
```

## Comparing `streaming_indicators-0.0.1b0.tar` & `streaming_indicators-0.0.1rc0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 17:33:34.144430 streaming_indicators-0.0.1b0/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.1b0/LICENSE.txt
--rw-rw-rw-   0        0        0     2826 2023-05-12 17:33:34.145161 streaming_indicators-0.0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.1b0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.1b0/pyproject.toml
--rw-rw-rw-   0        0        0      882 2023-05-12 17:33:34.151152 streaming_indicators-0.0.1b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 17:33:33.784962 streaming_indicators-0.0.1b0/streaming_indicators/
-drwxrwxrwx   0        0        0        0 2023-05-12 17:33:33.813965 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     2826 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 17:33:33.000000 streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 17:44:44.053217 streaming_indicators-0.0.1rc0/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.1rc0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2827 2023-05-12 17:44:44.053217 streaming_indicators-0.0.1rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.1rc0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.1rc0/pyproject.toml
+-rw-rw-rw-   0        0        0      848 2023-05-12 17:44:44.055215 streaming_indicators-0.0.1rc0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 17:44:44.015495 streaming_indicators-0.0.1rc0/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 17:44:44.028298 streaming_indicators-0.0.1rc0/src/streaming_indicators/
+-rw-rw-rw-   0        0        0       37 2023-05-12 17:42:57.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators/__init__.py
+-rw-rw-rw-   0        0        0     2966 2023-05-12 13:57:04.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators/streaming_indicators.py
+drwxrwxrwx   0        0        0        0 2023-05-12 17:44:44.051202 streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     2827 2023-05-12 17:44:43.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-05-12 17:44:44.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 17:44:43.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 17:44:43.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-12 17:44:43.000000 streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.1b0/LICENSE.txt` & `streaming_indicators-0.0.1rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.1b0/PKG-INFO` & `streaming_indicators-0.0.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming_indicators
-Version: 0.0.1b0
+Version: 0.0.1rc0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streaming_indicators-0.0.1b0/README.md` & `streaming_indicators-0.0.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.1b0/setup.cfg` & `streaming_indicators-0.0.1rc0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 6561 6d69 6e67 5f69 6e64   = streaming_ind
 00000020: 6963 6174 6f72 730d 0a76 6572 7369 6f6e  icators..version
-00000030: 203d 2030 2e30 2e31 620d 0a61 7574 686f   = 0.0.1b..autho
+00000030: 203d 2030 2e30 2e31 630d 0a61 7574 686f   = 0.0.1c..autho
 00000040: 7220 3d20 5269 7368 6162 6820 4775 7074  r = Rishabh Gupt
 00000050: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
 00000060: 3d20 7269 7368 6162 6867 3139 3937 4067  = rishabhg1997@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 4120 7079 7468 6f6e  ption = A python
 00000090: 206c 6962 7261 7279 2066 6f72 2063 6f6d   library for com
 000000a0: 7075 7469 6e67 2074 6563 686e 6963 616c  puting technical
@@ -36,21 +36,18 @@
 00000230: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
 00000240: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
 00000250: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
 00000260: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
 00000270: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
 00000280: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
 00000290: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-000002a0: 0d0a 093d 2073 7472 6561 6d69 6e67 5f69  ...= streaming_i
-000002b0: 6e64 6963 6174 6f72 730d 0a70 6163 6b61  ndicators..packa
-000002c0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000002d0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002e0: 3d33 2e34 0d0a 696e 7374 616c 6c5f 7265  =3.4..install_re
-000002f0: 7175 6972 6573 203d 200d 0a09 6e75 6d70  quires = ...nump
-00000300: 7920 3e3d 2031 2e31 332e 330d 0a0d 0a5b  y >= 1.13.3....[
-00000310: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000320: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000330: 7374 7265 616d 696e 675f 696e 6469 6361  streaming_indica
-00000340: 746f 7273 0d0a 0d0a 5b65 6767 5f69 6e66  tors....[egg_inf
-00000350: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000360: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000370: 0d0a                                     ..
+000002a0: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+000002b0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000002c0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000002d0: 332e 340d 0a69 6e73 7461 6c6c 5f72 6571  3.4..install_req
+000002e0: 7569 7265 7320 3d20 0d0a 096e 756d 7079  uires = ...numpy
+000002f0: 203e 3d20 312e 3133 2e33 0d0a 0d0a 5b6f   >= 1.13.3....[o
+00000300: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000310: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+00000320: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+00000330: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000340: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `streaming_indicators-0.0.1b0/streaming_indicators/streaming_indicators.egg-info/PKG-INFO` & `streaming_indicators-0.0.1rc0/src/streaming_indicators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-indicators
-Version: 0.0.1b0
+Version: 0.0.1rc0
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
```


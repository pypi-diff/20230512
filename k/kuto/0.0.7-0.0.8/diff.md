# Comparing `tmp/kuto-0.0.7-py3-none-any.whl.zip` & `tmp/kuto-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 93257 bytes, number of entries: 78
+Zip file size: 93261 bytes, number of entries: 78
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-17 07:22 demo/__init__.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-May-09 12:05 demo/run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-07 03:31 demo/page/__init__.py
 -rw-r--r--  2.0 unx      394 b- defN 23-Apr-25 02:58 demo/page/adr_page.py
 -rw-r--r--  2.0 unx      394 b- defN 23-Apr-25 02:58 demo/page/web_page.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-07 03:29 demo/tests/__init__.py
 -rw-r--r--  2.0 unx      701 b- defN 23-May-12 08:37 demo/tests/test_adr.py
@@ -11,15 +11,15 @@
 -rw-r--r--  2.0 unx      873 b- defN 23-May-09 01:48 demo/tests/test_image.py
 -rw-r--r--  2.0 unx      645 b- defN 23-May-12 08:37 demo/tests/test_ios.py
 -rw-r--r--  2.0 unx      894 b- defN 23-May-09 01:48 demo/tests/test_ocr.py
 -rw-r--r--  2.0 unx      841 b- defN 23-May-12 08:34 demo/tests/test_para.py
 -rw-r--r--  2.0 unx      828 b- defN 23-May-10 01:35 demo/tests/test_param.py
 -rw-r--r--  2.0 unx      838 b- defN 23-May-10 01:35 demo/tests/test_parameter.py
 -rw-r--r--  2.0 unx     1124 b- defN 23-May-12 07:38 demo/tests/test_web.py
--rw-r--r--  2.0 unx      578 b- defN 23-May-12 08:34 kuto/__init__.py
+-rw-r--r--  2.0 unx      578 b- defN 23-May-12 09:03 kuto/__init__.py
 -rw-r--r--  2.0 unx     8387 b- defN 23-May-12 08:19 kuto/case.py
 -rw-r--r--  2.0 unx     2063 b- defN 23-May-12 07:43 kuto/cli.py
 -rw-r--r--  2.0 unx     2065 b- defN 23-Apr-23 03:42 kuto/general.py
 -rw-r--r--  2.0 unx     3270 b- defN 23-May-12 03:29 kuto/page.py
 -rw-r--r--  2.0 unx     5070 b- defN 23-May-09 12:05 kuto/scaffold.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-03 12:13 kuto/core/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 22-Sep-21 12:42 kuto/core/android/__init__.py
@@ -68,13 +68,13 @@
 -rw-r--r--  2.0 unx     3894 b- defN 23-May-10 01:54 kuto/utils/mail.py
 -rw-r--r--  2.0 unx     2009 b- defN 22-Oct-17 03:26 kuto/utils/mongo_util.py
 -rw-r--r--  2.0 unx     2149 b- defN 22-Oct-17 03:26 kuto/utils/mysql_util.py
 -rw-r--r--  2.0 unx     1719 b- defN 23-Apr-25 02:58 kuto/utils/read_file.py
 -rw-r--r--  2.0 unx      656 b- defN 23-May-09 11:39 kuto/utils/schema_util.py
 -rw-r--r--  2.0 unx     2177 b- defN 22-May-05 11:41 kuto/utils/swagger_util.py
 -rw-r--r--  2.0 unx     1662 b- defN 22-May-05 11:41 kuto/utils/webdriver_manager_extend.py
--rw-r--r--  2.0 unx     1439 b- defN 23-May-12 09:03 kuto-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 09:03 kuto-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 23-May-12 09:03 kuto-0.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-12 09:03 kuto-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6156 b- defN 23-May-12 09:03 kuto-0.0.7.dist-info/RECORD
-78 files, 246418 bytes uncompressed, 83657 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx     1439 b- defN 23-May-12 09:03 kuto-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 09:03 kuto-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 23-May-12 09:03 kuto-0.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-12 09:03 kuto-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6156 b- defN 23-May-12 09:03 kuto-0.0.8.dist-info/RECORD
+78 files, 246418 bytes uncompressed, 83661 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -213,23 +213,23 @@
 
 Filename: kuto/utils/swagger_util.py
 Comment: 
 
 Filename: kuto/utils/webdriver_manager_extend.py
 Comment: 
 
-Filename: kuto-0.0.7.dist-info/METADATA
+Filename: kuto-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: kuto-0.0.7.dist-info/WHEEL
+Filename: kuto-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: kuto-0.0.7.dist-info/entry_points.txt
+Filename: kuto-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: kuto-0.0.7.dist-info/top_level.txt
+Filename: kuto-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: kuto-0.0.7.dist-info/RECORD
+Filename: kuto-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kuto/__init__.py

```diff
@@ -12,9 +12,9 @@
 )
 from kuto.running.runner import main
 from kuto.utils.config import config
 from kuto.utils.decorate import *
 from kuto.utils.log import logger
 
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __description__ = "移动、web、接口自动化测试框架"
```

## Comparing `kuto-0.0.7.dist-info/METADATA` & `kuto-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuto
-Version: 0.0.7
+Version: 0.0.8
 Summary: 移动、web、接口自动化测试框架
 Home-page: https://gitee.com/bluepang2021/kuto
 Author: 杨康
 Author-email: 772840356@qq.com
 Platform: Android
 Platform: IOS
 Platform: Web
```

## Comparing `kuto-0.0.7.dist-info/RECORD` & `kuto-0.0.8.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 demo/tests/test_image.py,sha256=p58xmgYze3Qbv-ebIjIVS1oreY34uKwMqWrbU4R_H_Q,873
 demo/tests/test_ios.py,sha256=XAcb8dCt8G_fVyCgBe2npUiSHNCCQWgKPXVS2EcjZgA,645
 demo/tests/test_ocr.py,sha256=r3_fxtpyOlHitzBYd7c7ANTnic_t3IIatvsADc_ttHA,894
 demo/tests/test_para.py,sha256=mZ4jBDlie31ZOYzGm8P2ZUbhL0HRNdX3C_ZwAGSm-Bg,841
 demo/tests/test_param.py,sha256=vz3pxtieCKKXkmfcmauFlfzeNp5Za5ej_2iYcjilR9A,828
 demo/tests/test_parameter.py,sha256=9MTkuBkZKII5wFXWCCSCGj1tDv2dDggfuX67_cMmCA4,838
 demo/tests/test_web.py,sha256=Ub7nm2w2X02Tcba16GI3AGn7HWqbjgtQ4Oz4WRZlNnA,1124
-kuto/__init__.py,sha256=AmpkKh2dunpZJOfN0OKrHd7m7txGzb88xGwS0NkIf4g,578
+kuto/__init__.py,sha256=CeS9EXRzUZ-YP6TVWp17_jR5rynLQzwXUV7ZfeDRNDA,578
 kuto/case.py,sha256=eo-GFqH34UtNXJtIIWH-cGU-zTAaOQi1INDKimVeErM,8387
 kuto/cli.py,sha256=EOGD7LJTPm_2Hf_8eBBUIKQxw_9NQ4TzG8EzYjaFGJ4,2063
 kuto/general.py,sha256=9kHmLuJgI32-hAeRJFAw9UbH7xB0DC9OXOMoI5xq7ww,2065
 kuto/page.py,sha256=F56bansY1GT9Ux6cRMpD7k1cU8NCOFyfsdlYXyN2-IM,3270
 kuto/scaffold.py,sha256=Q3WMG9-jirfT5Qb3Hb8FsM8LzidoNI_HtkjEynjdbHk,5070
 kuto/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kuto/core/android/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
@@ -67,12 +67,12 @@
 kuto/utils/mail.py,sha256=_ZJnoFQ-7AtHsUZdadXiEELFkz-19d_1BQF1uNVBJGI,3894
 kuto/utils/mongo_util.py,sha256=-YcHVVQtsdu-8mo9h0W0dQGfRlfLKDfUgUhPP1sienI,2009
 kuto/utils/mysql_util.py,sha256=7KaYshGEAXG5Iz5bX7N_FZF07eyG9yDw2czdcqY5Rpg,2149
 kuto/utils/read_file.py,sha256=kDWXAH0PJ6FHdjYz_1nZa40Lk54VWgAdcpaqZ5VwigQ,1719
 kuto/utils/schema_util.py,sha256=kuBX08WIA9Zc9X65X0yC8eruUwqAlbhNbg-Xq5qstd4,656
 kuto/utils/swagger_util.py,sha256=YPiDs5WeL--siqdt0E76e7sJgq07DlakT25vF98NDOM,2177
 kuto/utils/webdriver_manager_extend.py,sha256=FIk_SYLa4WD0woccVRsPdrIRjjQszplyw2IB6Yocorg,1662
-kuto-0.0.7.dist-info/METADATA,sha256=GpjccRLbkrXF5s-hENzTwO551luHb9_E9v4r4LJ0GTY,1439
-kuto-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-kuto-0.0.7.dist-info/entry_points.txt,sha256=9UCWFKVt6BTVTCmKlyeQc6iLerHba45hV-42BmXnWlQ,39
-kuto-0.0.7.dist-info/top_level.txt,sha256=tvoxP89jCv57xiuEI50U1KwLmNGxgChNdM9dyfQOLI8,10
-kuto-0.0.7.dist-info/RECORD,,
+kuto-0.0.8.dist-info/METADATA,sha256=XMKPj8yKq5zJoWy-6JY_OXFkSzjh_tSlQsriqmSIcdQ,1439
+kuto-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+kuto-0.0.8.dist-info/entry_points.txt,sha256=9UCWFKVt6BTVTCmKlyeQc6iLerHba45hV-42BmXnWlQ,39
+kuto-0.0.8.dist-info/top_level.txt,sha256=tvoxP89jCv57xiuEI50U1KwLmNGxgChNdM9dyfQOLI8,10
+kuto-0.0.8.dist-info/RECORD,,
```


# Comparing `tmp/MixPage-1.0.0-py3-none-any.whl.zip` & `tmp/MixPage-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 68467 bytes, number of entries: 31
--rw-rw-rw-  2.0 fat      232 b- defN 23-May-12 02:36 MixPage/__init__.py
+Zip file size: 68477 bytes, number of entries: 31
+-rw-rw-rw-  2.0 fat      308 b- defN 23-May-12 06:29 MixPage/__init__.py
 -rw-rw-rw-  2.0 fat    11240 b- defN 23-May-12 03:06 MixPage/base.py
 -rw-rw-rw-  2.0 fat     5075 b- defN 23-Jan-10 13:54 MixPage/base.pyi
 -rw-rw-rw-  2.0 fat      920 b- defN 23-Apr-06 09:49 MixPage/configs.ini
 -rw-rw-rw-  2.0 fat    16540 b- defN 23-May-12 03:06 MixPage/drission.py
 -rw-rw-rw-  2.0 fat     2792 b- defN 23-May-12 02:56 MixPage/drission.pyi
 -rw-rw-rw-  2.0 fat    52235 b- defN 23-May-12 03:13 MixPage/driver_element.py
 -rw-rw-rw-  2.0 fat    10683 b- defN 23-Jan-10 14:01 MixPage/driver_element.pyi
@@ -21,13 +21,13 @@
 -rw-rw-rw-  2.0 fat     3826 b- defN 23-Feb-16 13:45 MixPage/session_element.pyi
 -rw-rw-rw-  2.0 fat    13038 b- defN 23-May-12 03:06 MixPage/session_options.py
 -rw-rw-rw-  2.0 fat     3486 b- defN 23-Mar-03 14:29 MixPage/session_options.pyi
 -rw-rw-rw-  2.0 fat    18567 b- defN 23-May-12 03:06 MixPage/session_page.py
 -rw-rw-rw-  2.0 fat     7695 b- defN 23-May-12 03:06 MixPage/session_page.pyi
 -rw-rw-rw-  2.0 fat     9133 b- defN 23-May-12 03:06 MixPage/shadow_root_element.py
 -rw-rw-rw-  2.0 fat     2791 b- defN 23-Jan-09 15:03 MixPage/shadow_root_element.pyi
--rw-rw-rw-  2.0 fat     1083 b- defN 23-May-12 06:26 MixPage-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1724 b- defN 23-May-12 06:26 MixPage-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 06:26 MixPage-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-12 06:26 MixPage-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2473 b- defN 23-May-12 06:26 MixPage-1.0.0.dist-info/RECORD
-31 files, 262758 bytes uncompressed, 64575 bytes compressed:  75.4%
+-rw-rw-rw-  2.0 fat     1083 b- defN 23-May-12 06:48 MixPage-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1724 b- defN 23-May-12 06:48 MixPage-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 06:48 MixPage-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-12 06:48 MixPage-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2473 b- defN 23-May-12 06:48 MixPage-1.0.1.dist-info/RECORD
+31 files, 262834 bytes uncompressed, 64585 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -72,23 +72,23 @@
 
 Filename: MixPage/shadow_root_element.py
 Comment: 
 
 Filename: MixPage/shadow_root_element.pyi
 Comment: 
 
-Filename: MixPage-1.0.0.dist-info/LICENSE
+Filename: MixPage-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: MixPage-1.0.0.dist-info/METADATA
+Filename: MixPage-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: MixPage-1.0.0.dist-info/WHEEL
+Filename: MixPage-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: MixPage-1.0.0.dist-info/top_level.txt
+Filename: MixPage-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: MixPage-1.0.0.dist-info/RECORD
+Filename: MixPage-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MixPage/__init__.py

```diff
@@ -1,9 +1,11 @@
 # -*- coding:utf-8 -*-
 """
 @Author  :   g1879
 @Contact :   g1879@qq.com
 """
 from .mix_page import MixPage
+from .session_page import SessionPage
+from .driver_page import DriverPage
 from .drission import Drission
 from .driver_options import DriverOptions
 from .session_options import SessionOptions
```

## Comparing `MixPage-1.0.0.dist-info/LICENSE` & `MixPage-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MixPage-1.0.0.dist-info/METADATA` & `MixPage-1.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MixPage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python based web automation tool. It can control the browser and send and receive data packets.
 Home-page: https://gitee.com/g1879/MixPage
 Author: g1879
 Author-email: g1879@qq.com
 License: BSD
 Keywords: MixPage
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `MixPage-1.0.0.dist-info/RECORD` & `MixPage-1.0.1.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MixPage/__init__.py,sha256=gRQhg54OW6-FQpkYNUyBjMcP9ah5bcAcXQbiCAeiDIQ,232
+MixPage/__init__.py,sha256=1lH90VNCBZes3yK8UUIzEBqGsVlQX3LlTHgDLHFYK2Y,308
 MixPage/base.py,sha256=81b9235jiy6aPa9FDqqa-yh-2TDBw-cF6lI9bEFtTtI,11240
 MixPage/base.pyi,sha256=lYXJFCguzXol7rjbKPxkiqpIRxRXASZaQqS9MN4Hydg,5075
 MixPage/configs.ini,sha256=y1EIfrDNh5GT_3_XhJBMcvZmxQRL_iQL9ULKByyBQ90,920
 MixPage/drission.py,sha256=SdHVyUw9ClDhP5cqkwZ79ByHDnOAk1rPxEZt4WdZePg,16540
 MixPage/drission.pyi,sha256=QtGmzFqBGUEEe1fDTmd6OiaLzmcr1DZ3P9tdwRI1JF0,2792
 MixPage/driver_element.py,sha256=neCACvJSnn3FqeP-iSlVAab_2zoGp0sLSrvFOihYn1Q,52235
 MixPage/driver_element.pyi,sha256=KBltY_xYv47YpN6JIRRrM5CqhTofGMIJanQSHBhSMf4,10683
@@ -20,12 +20,12 @@
 MixPage/session_element.pyi,sha256=vWC5p9OzzQftPeIXfDQWyY-6CPM3paUKsGvJ62gDBNw,3826
 MixPage/session_options.py,sha256=Rn3AW1zJUxrDcA7h5LWDZntjLd1YvxwlahE4qaUCDfU,13038
 MixPage/session_options.pyi,sha256=noyK-71Sybl1dodPzpUbjZCTlMKJJKx4LC7upCLKfwg,3486
 MixPage/session_page.py,sha256=9hmvoPBrS-1ki6gFqGlqC-WIRwJmKQMTRE8FzPLqsdg,18567
 MixPage/session_page.pyi,sha256=upFFdSLxwTV_iHgIktuBRXOeWMN303C9zjuGpSzL-8Q,7695
 MixPage/shadow_root_element.py,sha256=fedbYjSE3_ur0OGgAJPbaes1sYeaxIraJlmJF7lFbQA,9133
 MixPage/shadow_root_element.pyi,sha256=WsgkKs0rf2-eAJrVnmTtkqvAfMde-Uh06XBy49p__7Y,2791
-MixPage-1.0.0.dist-info/LICENSE,sha256=pXuXhrUZmz9wJYw2dIfJ87iZvWaKOKtImKyqhXlZWMc,1083
-MixPage-1.0.0.dist-info/METADATA,sha256=Xwj1DXxr6ILz7TMs73GBS8U522FSsqxMnneBBI0BDZo,1724
-MixPage-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-MixPage-1.0.0.dist-info/top_level.txt,sha256=aakVHXYtXPJJhv2DFQRNMPL6ByVjvbGu0i8pel1x1Tg,8
-MixPage-1.0.0.dist-info/RECORD,,
+MixPage-1.0.1.dist-info/LICENSE,sha256=pXuXhrUZmz9wJYw2dIfJ87iZvWaKOKtImKyqhXlZWMc,1083
+MixPage-1.0.1.dist-info/METADATA,sha256=Zy1tfCc3ENXXewOjjFdsGKWwymdOoCLS3SRyFii0AN4,1724
+MixPage-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+MixPage-1.0.1.dist-info/top_level.txt,sha256=aakVHXYtXPJJhv2DFQRNMPL6ByVjvbGu0i8pel1x1Tg,8
+MixPage-1.0.1.dist-info/RECORD,,
```


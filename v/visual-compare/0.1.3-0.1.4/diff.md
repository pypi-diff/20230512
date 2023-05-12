# Comparing `tmp/visual-compare-0.1.3.tar.gz` & `tmp/visual-compare-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-compare-0.1.3.tar", last modified: Fri May 12 02:00:50 2023, max compression
+gzip compressed data, was "visual-compare-0.1.4.tar", last modified: Fri May 12 02:09:17 2023, max compression
```

## Comparing `visual-compare-0.1.3.tar` & `visual-compare-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/
--rw-rw-rw-   0        0        0     1937 2023-05-12 02:00:50.535417 visual-compare-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2023-05-11 10:55:38.000000 visual-compare-0.1.3/README.md
--rw-rw-rw-   0        0        0      145 2023-05-12 02:00:50.535417 visual-compare-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-05-11 10:56:53.000000 visual-compare-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.519722 visual-compare-0.1.3/visual_compare/
--rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-0.1.3/visual_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.529771 visual-compare-0.1.3/visual_compare/doc/
--rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.3/visual_compare/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/visual_compare/doc/image/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.3/visual_compare/doc/image/__init__.py
--rw-rw-rw-   0        0        0    29164 2023-05-11 09:04:51.000000 visual-compare-0.1.3/visual_compare/doc/image/compare_image.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 09:51:00.000000 visual-compare-0.1.3/visual_compare/doc/image/image.py
--rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.3/visual_compare/doc/image/ocr.py
--rw-rw-rw-   0        0        0     2974 2023-05-09 08:15:10.000000 visual-compare-0.1.3/visual_compare/doc/match.py
--rw-rw-rw-   0        0        0      549 2023-05-11 09:40:58.000000 visual-compare-0.1.3/visual_compare/doc/models.py
--rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-0.1.3/visual_compare/doc/pdf_test.py
--rw-rw-rw-   0        0        0    51123 2023-05-11 10:54:33.000000 visual-compare-0.1.3/visual_compare/doc/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/visual_compare/tests/
--rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-0.1.3/visual_compare/tests/__init__.py
--rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-0.1.3/visual_compare/tests/conftest.py
--rw-rw-rw-   0        0        0     5322 2023-05-11 02:43:40.000000 visual-compare-0.1.3/visual_compare/tests/test_compare_image.py
--rw-rw-rw-   0        0        0     2839 2023-05-11 11:04:27.000000 visual-compare-0.1.3/visual_compare/tests/test_compare_pdf.py
--rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-0.1.3/visual_compare/tests/test_downloader.py
--rw-rw-rw-   0        0        0     1100 2023-05-11 10:06:36.000000 visual-compare-0.1.3/visual_compare/tests/test_image.py
--rw-rw-rw-   0        0        0     1599 2023-05-11 10:57:59.000000 visual-compare-0.1.3/visual_compare/tests/test_visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/visual_compare/utils/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.3/visual_compare/utils/__init__.py
--rw-rw-rw-   0        0        0      639 2023-05-11 08:52:12.000000 visual-compare-0.1.3/visual_compare/utils/common.py
--rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-0.1.3/visual_compare/utils/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.519722 visual-compare-0.1.3/visual_compare.egg-info/
--rw-rw-rw-   0        0        0     1937 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.3/visual_compare.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.757008 visual-compare-0.1.4/
+-rw-rw-rw-   0        0        0     2047 2023-05-12 02:09:17.757008 visual-compare-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2023-05-12 02:07:01.000000 visual-compare-0.1.4/README.md
+-rw-rw-rw-   0        0        0      145 2023-05-12 02:09:17.757008 visual-compare-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-05-12 02:07:51.000000 visual-compare-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare/
+-rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-0.1.4/visual_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare/doc/
+-rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.4/visual_compare/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare/doc/image/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.4/visual_compare/doc/image/__init__.py
+-rw-rw-rw-   0        0        0    29164 2023-05-11 09:04:51.000000 visual-compare-0.1.4/visual_compare/doc/image/compare_image.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 09:51:00.000000 visual-compare-0.1.4/visual_compare/doc/image/image.py
+-rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.4/visual_compare/doc/image/ocr.py
+-rw-rw-rw-   0        0        0     2974 2023-05-09 08:15:10.000000 visual-compare-0.1.4/visual_compare/doc/match.py
+-rw-rw-rw-   0        0        0      549 2023-05-11 09:40:58.000000 visual-compare-0.1.4/visual_compare/doc/models.py
+-rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-0.1.4/visual_compare/doc/pdf_test.py
+-rw-rw-rw-   0        0        0    51123 2023-05-11 10:54:33.000000 visual-compare-0.1.4/visual_compare/doc/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.757008 visual-compare-0.1.4/visual_compare/tests/
+-rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-0.1.4/visual_compare/tests/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-0.1.4/visual_compare/tests/conftest.py
+-rw-rw-rw-   0        0        0     5322 2023-05-11 02:43:40.000000 visual-compare-0.1.4/visual_compare/tests/test_compare_image.py
+-rw-rw-rw-   0        0        0     2839 2023-05-11 11:04:27.000000 visual-compare-0.1.4/visual_compare/tests/test_compare_pdf.py
+-rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-0.1.4/visual_compare/tests/test_downloader.py
+-rw-rw-rw-   0        0        0     1100 2023-05-11 10:06:36.000000 visual-compare-0.1.4/visual_compare/tests/test_image.py
+-rw-rw-rw-   0        0        0     1599 2023-05-11 10:57:59.000000 visual-compare-0.1.4/visual_compare/tests/test_visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.757008 visual-compare-0.1.4/visual_compare/utils/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.4/visual_compare/utils/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-05-11 08:52:12.000000 visual-compare-0.1.4/visual_compare/utils/common.py
+-rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-0.1.4/visual_compare/utils/downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:09:17.741408 visual-compare-0.1.4/visual_compare.egg-info/
+-rw-rw-rw-   0        0        0     2047 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.4/visual_compare.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 02:09:17.000000 visual-compare-0.1.4/visual_compare.egg-info/top_level.txt
```

### Comparing `visual-compare-0.1.3/PKG-INFO` & `visual-compare-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 0.1.3
+Version: 0.1.4
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
@@ -46,15 +46,15 @@
 res = vt.compare_images(reference_image, test_image)
 print(res)
 assert vt.is_different is True
 ```
 
  Result as follows
 
-![1.jpg](files/result/1.jpg)
+![1.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/1.jpg)
 
 ### Compare images with mask ###
 
 ```python
 from visual_compare.doc.visual_test import VisualTest
 
 def get_path(filename):
@@ -69,9 +69,9 @@
 res = vt.compare_images(reference_image, test_image, mask=mask)
 print(res)
 assert vt.is_different is True
 ```
 
  Result as follows
 
-![2.jpg](files/result/2.jpg)
+![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
```

### Comparing `visual-compare-0.1.3/README.md` & `visual-compare-0.1.4/visual_compare/tests/test_visual_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-Visual Compare
-==============
-
-## Installation
-
-```commandline
-pip install visual-compare
-```
-
-## Examples
-
-### Compare images ###
-
-```python
-from visual_compare.doc.visual_test import VisualTest
-
-def get_path(filename):
-    image_base = '../../files/images/'
-    return image_base + filename
-
-reference_image = get_path('123.png')
-test_image = get_path('124.png')
-vt = VisualTest()
-res = vt.compare_images(reference_image, test_image)
-print(res)
-assert vt.is_different is True
-```
-
- Result as follows
-
-![1.jpg](files/result/1.jpg)
-
-### Compare images with mask ###
-
-```python
-from visual_compare.doc.visual_test import VisualTest
-
-def get_path(filename):
-    image_base = '../../files/images/'
-    return image_base + filename
-
-reference_image = get_path('123.png')
-test_image = get_path('124.png')
-mask_images = [get_path('000.png')]
-vt = VisualTest()
-mask = vt.generate_mask(reference_image, mask_images)
-res = vt.compare_images(reference_image, test_image, mask=mask)
-print(res)
-assert vt.is_different is True
-```
-
- Result as follows
-
-![2.jpg](files/result/2.jpg)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+-------------------------------------------------
+   File Name：      test_visual_test
+   Description:
+   Author:          dingyong.cui
+   date：           2023/5/11
+-------------------------------------------------
+   Change Activity:
+                    2023/5/11
+-------------------------------------------------
+"""
+
+
+class TestVisualTest:
+
+    def setup(self):
+        from visual_compare.doc.visual_test import VisualTest
+        self.cls = VisualTest
+        self.image_base = '../../files/images/'
+
+    def get_path(self, filename):
+        return self.image_base + filename
+
+    def test_compare_images_with_mask(self):
+        reference_image = self.get_path('123.png')
+        # mask_images = [self.get_path('000.png'), self.get_path('098.png')]
+        mask_images = [self.get_path('000.png')]
+        test_image = self.get_path('124.png')
+        cls = self.cls()
+        mask = cls.generate_mask(reference_image, mask_images)
+        res = cls.compare_images(reference_image, test_image, mask=mask)
+        print(res)
+        assert cls.is_different is True
+
+    def test_compare_images_no_mask(self):
+        reference_image = self.get_path('123.png')
+        # mask_images = [self.get_path('000.png'), self.get_path('098.png')]
+        test_image = self.get_path('124.png')
+        cls = self.cls()
+        # mask = cls.generate_mask(reference_image, mask_images)
+        res = cls.compare_images(reference_image, test_image)
+        print(res)
+        assert cls.is_different is False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `visual-compare-0.1.3/setup.py` & `visual-compare-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="visual-compare",
-    version="0.1.3",
+    version="0.1.4",
     description="Image and PDF Compare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/visual-compare",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
```

### Comparing `visual-compare-0.1.3/visual_compare/doc/image/compare_image.py` & `visual-compare-0.1.4/visual_compare/doc/image/compare_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/doc/image/image.py` & `visual-compare-0.1.4/visual_compare/doc/image/image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/doc/image/ocr.py` & `visual-compare-0.1.4/visual_compare/doc/image/ocr.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/doc/match.py` & `visual-compare-0.1.4/visual_compare/doc/match.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/doc/models.py` & `visual-compare-0.1.4/visual_compare/doc/models.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/doc/pdf_test.py` & `visual-compare-0.1.4/visual_compare/doc/pdf_test.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/doc/visual_test.py` & `visual-compare-0.1.4/visual_compare/doc/visual_test.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/tests/test_compare_image.py` & `visual-compare-0.1.4/visual_compare/tests/test_compare_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/tests/test_compare_pdf.py` & `visual-compare-0.1.4/visual_compare/tests/test_compare_pdf.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/tests/test_downloader.py` & `visual-compare-0.1.4/visual_compare/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/tests/test_image.py` & `visual-compare-0.1.4/visual_compare/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/utils/common.py` & `visual-compare-0.1.4/visual_compare/utils/common.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare/utils/downloader.py` & `visual-compare-0.1.4/visual_compare/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.3/visual_compare.egg-info/PKG-INFO` & `visual-compare-0.1.4/visual_compare.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 0.1.3
+Version: 0.1.4
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
@@ -46,15 +46,15 @@
 res = vt.compare_images(reference_image, test_image)
 print(res)
 assert vt.is_different is True
 ```
 
  Result as follows
 
-![1.jpg](files/result/1.jpg)
+![1.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/1.jpg)
 
 ### Compare images with mask ###
 
 ```python
 from visual_compare.doc.visual_test import VisualTest
 
 def get_path(filename):
@@ -69,9 +69,9 @@
 res = vt.compare_images(reference_image, test_image, mask=mask)
 print(res)
 assert vt.is_different is True
 ```
 
  Result as follows
 
-![2.jpg](files/result/2.jpg)
+![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
```

### Comparing `visual-compare-0.1.3/visual_compare.egg-info/SOURCES.txt` & `visual-compare-0.1.4/visual_compare.egg-info/SOURCES.txt`

 * *Files identical despite different names*


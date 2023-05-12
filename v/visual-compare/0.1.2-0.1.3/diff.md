# Comparing `tmp/visual-compare-0.1.2.tar.gz` & `tmp/visual-compare-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-compare-0.1.2.tar", last modified: Mon May  8 10:37:09 2023, max compression
+gzip compressed data, was "visual-compare-0.1.3.tar", last modified: Fri May 12 02:00:50 2023, max compression
```

## Comparing `visual-compare-0.1.2.tar` & `visual-compare-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/
--rw-rw-rw-   0        0        0      928 2023-05-08 10:37:09.898893 visual-compare-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-05-08 03:46:52.000000 visual-compare-0.1.2/README.md
--rw-rw-rw-   0        0        0      145 2023-05-08 10:37:09.898893 visual-compare-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-05-08 09:53:22.000000 visual-compare-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/visual_compare/
--rw-rw-rw-   0        0        0      378 2023-05-08 10:01:21.000000 visual-compare-0.1.2/visual_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/visual_compare/doc/
--rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.2/visual_compare/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/visual_compare/doc/image/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.2/visual_compare/doc/image/__init__.py
--rw-rw-rw-   0        0        0    28532 2023-05-08 10:04:21.000000 visual-compare-0.1.2/visual_compare/doc/image/compare_image.py
--rw-rw-rw-   0        0        0     1912 2023-05-08 02:42:08.000000 visual-compare-0.1.2/visual_compare/doc/image/image.py
--rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.2/visual_compare/doc/image/ocr.py
--rw-rw-rw-   0        0        0    49823 2023-05-08 10:04:21.000000 visual-compare-0.1.2/visual_compare/doc/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/visual_compare/tests/
--rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-0.1.2/visual_compare/tests/__init__.py
--rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-0.1.2/visual_compare/tests/conftest.py
--rw-rw-rw-   0        0        0     2505 2023-05-08 10:31:18.000000 visual-compare-0.1.2/visual_compare/tests/test_compare_image.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/visual_compare/utils/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.2/visual_compare/utils/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-05-06 02:31:44.000000 visual-compare-0.1.2/visual_compare/utils/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:37:09.898893 visual-compare-0.1.2/visual_compare.egg-info/
--rw-rw-rw-   0        0        0      928 2023-05-08 10:37:09.000000 visual-compare-0.1.2/visual_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      668 2023-05-08 10:37:09.000000 visual-compare-0.1.2/visual_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:37:09.000000 visual-compare-0.1.2/visual_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.2/visual_compare.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-05-08 10:37:09.000000 visual-compare-0.1.2/visual_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 10:37:09.000000 visual-compare-0.1.2/visual_compare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/
+-rw-rw-rw-   0        0        0     1937 2023-05-12 02:00:50.535417 visual-compare-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2023-05-11 10:55:38.000000 visual-compare-0.1.3/README.md
+-rw-rw-rw-   0        0        0      145 2023-05-12 02:00:50.535417 visual-compare-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-05-11 10:56:53.000000 visual-compare-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.519722 visual-compare-0.1.3/visual_compare/
+-rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-0.1.3/visual_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.529771 visual-compare-0.1.3/visual_compare/doc/
+-rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-0.1.3/visual_compare/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/visual_compare/doc/image/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-0.1.3/visual_compare/doc/image/__init__.py
+-rw-rw-rw-   0        0        0    29164 2023-05-11 09:04:51.000000 visual-compare-0.1.3/visual_compare/doc/image/compare_image.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 09:51:00.000000 visual-compare-0.1.3/visual_compare/doc/image/image.py
+-rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-0.1.3/visual_compare/doc/image/ocr.py
+-rw-rw-rw-   0        0        0     2974 2023-05-09 08:15:10.000000 visual-compare-0.1.3/visual_compare/doc/match.py
+-rw-rw-rw-   0        0        0      549 2023-05-11 09:40:58.000000 visual-compare-0.1.3/visual_compare/doc/models.py
+-rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-0.1.3/visual_compare/doc/pdf_test.py
+-rw-rw-rw-   0        0        0    51123 2023-05-11 10:54:33.000000 visual-compare-0.1.3/visual_compare/doc/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/visual_compare/tests/
+-rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-0.1.3/visual_compare/tests/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-0.1.3/visual_compare/tests/conftest.py
+-rw-rw-rw-   0        0        0     5322 2023-05-11 02:43:40.000000 visual-compare-0.1.3/visual_compare/tests/test_compare_image.py
+-rw-rw-rw-   0        0        0     2839 2023-05-11 11:04:27.000000 visual-compare-0.1.3/visual_compare/tests/test_compare_pdf.py
+-rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-0.1.3/visual_compare/tests/test_downloader.py
+-rw-rw-rw-   0        0        0     1100 2023-05-11 10:06:36.000000 visual-compare-0.1.3/visual_compare/tests/test_image.py
+-rw-rw-rw-   0        0        0     1599 2023-05-11 10:57:59.000000 visual-compare-0.1.3/visual_compare/tests/test_visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.535417 visual-compare-0.1.3/visual_compare/utils/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-0.1.3/visual_compare/utils/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-05-11 08:52:12.000000 visual-compare-0.1.3/visual_compare/utils/common.py
+-rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-0.1.3/visual_compare/utils/downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:00:50.519722 visual-compare-0.1.3/visual_compare.egg-info/
+-rw-rw-rw-   0        0        0     1937 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-0.1.3/visual_compare.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 02:00:50.000000 visual-compare-0.1.3/visual_compare.egg-info/top_level.txt
```

### Comparing `visual-compare-0.1.2/setup.py` & `visual-compare-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="visual-compare",
-    version="0.1.2",
+    version="0.1.3",
     description="Image and PDF Compare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/visual-compare",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
```

### Comparing `visual-compare-0.1.2/visual_compare/doc/image/compare_image.py` & `visual-compare-0.1.3/visual_compare/doc/image/compare_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 
 import cv2
 import fitz
 import numpy as np
 import pytesseract
 from pytesseract import Output
 
-from visual_compare.utils.downloader import is_url, download_file_from_url
+from visual_compare.utils.downloader import download_file_from_url
 from .ocr import EastTextExtractor
+from ..match import MatchPdf
+from visual_compare.utils.common import is_url
 
 logger = logging.getLogger(__name__)
 
 EAST_CONFIDENCE = 0.5
 
 
 class CompareImage(object):
@@ -170,23 +172,30 @@
         for frame in self.opencv_images:
             text = self.east_text_extractor.get_image_text(frame)
             self.text_content.append(text)
 
     def identify_placeholders(self):
         placeholders = None
         if self.placeholder_file is not None:
-            try:
-                with open(self.placeholder_file, 'r') as f:
-                    placeholders = json.load(f)
-            except IOError as err:
-                logger.error("Placeholder File %s is not accessible", self.placeholder_file)
-                logger.error("I/O error: {0}".format(err))
-            except:
-                logger.error("Unexpected error:", sys.exc_info()[0])
-                raise
+            if isinstance(self.placeholder_file, list):
+                placeholders = []
+                for pf in self.placeholder_file:
+                    if self.is_image(pf):
+                        mi = MatchPdf(self.opencv_images[0], pf)
+                        placeholders.extend(mi.mask)
+            elif isinstance(self.placeholders, str):
+                try:
+                    with open(self.placeholder_file, 'r') as f:
+                        placeholders = json.load(f)
+                except IOError as err:
+                    logger.error("Placeholder File %s is not accessible", self.placeholder_file)
+                    logger.error("I/O error: {0}".format(err))
+                except:
+                    logger.error("Unexpected error:", sys.exc_info()[0])
+                    raise
         elif self.mask is not None:
             if isinstance(self.mask, dict):
                 placeholders = self.mask
             elif isinstance(self.mask, list):
                 placeholders = self.mask
             elif isinstance(self.mask, str):
                 try:
@@ -539,14 +548,21 @@
                     self.opencv_images.append(opencv_image)
 
                 toc = time.perf_counter()
                 print(f"Conversion from pyWand Image to OpenCV Image performed in {toc - tic:0.4f} seconds")
         except:
             raise AssertionError("File could not be converted by ImageMagick to OpenCV Image: {}".format(self.image))
 
+    @staticmethod
+    def is_image(image: str):
+        import filetype
+        mr = filetype.image_match(image)
+
+        return False if mr is None else True
+
 
 def make_text(words):
     """Return textstring output of get_text("words").
     Word items are sorted for reading sequence left to right,
     top to bottom.
     """
     line_dict = {}  # key: vertical coordinate, value: list of words
```

### Comparing `visual-compare-0.1.2/visual_compare/doc/image/image.py` & `visual-compare-0.1.3/visual_compare/doc/match.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 -------------------------------------------------
-   File Name：      _base
+   File Name：      match
    Description:
    Author:          dingyong.cui
-   date：           2023/5/6
+   date：           2023/5/9
 -------------------------------------------------
    Change Activity:
-                    2023/5/6
+                    2023/5/9
 -------------------------------------------------
 """
+from os.path import splitext, split
+
 import cv2
 import numpy
-import os
-
-
-class Image:
 
-    def __init__(self, image: str):
-        if os.path.isfile(image) is False:
-            raise AssertionError('The image file does not exist: {}'.format(image))
-        self.image = cv2.imread(image, cv2.IMREAD_UNCHANGED)
-
-    @property
-    def width(self):
-        return self.image.shape[1]
-
-    @property
-    def height(self):
-        return self.image.shape[0]
+from visual_compare.doc.image.image import Image
 
 
 class MatchImg:
 
     def __init__(self, source: str, temp: str, threshold=0.95):
         self.source_img = Image(source)
         self.temp_img = Image(temp)
@@ -50,14 +37,57 @@
 
             return list(zip(locations[1], locations[0]))
         except cv2.error as e:
             print(e)
 
     def parse_mask(self, match_method=cv2.TM_CCOEFF_NORMED):
         mask_list = []
+        match_list = self.match_temp(method=match_method)
+        for m in match_list:
+            mj = {
+                'type': 'coordinates',
+                "page": "all",
+                'x': m[0],
+                'y': m[1],
+                'width': self.temp_img.width,
+                'height': self.temp_img.height
+            }
+            mask_list.append(mj)
+
+        return mask_list
+
+
+class MatchPdf:
+
+    def __init__(self, source, temp: str, threshold=0.05):
+        if isinstance(source, str):
+            self.source_img = Image(source).image
+        else:
+            # self.source_img = cv2.cvtColor(source, cv2.COLOR_BGR2GRAY)
+            self.source_img = source
+        self.temp_img = Image(temp).image
+        self.threshold = threshold
+
+    @property
+    def mask(self):
+        return self.parse_mask()
+
+    def match_temp(self, method=cv2.TM_CCOEFF_NORMED):
+        try:
+            ccc = cv2.cvtColor(self.source_img, cv2.COLOR_BGR2GRAY)
+            cct = cv2.cvtColor(self.temp_img, cv2.COLOR_BGR2GRAY)
+            mt = cv2.matchTemplate(ccc, cct, method)
+            locations = numpy.where(mt <= self.threshold)
+
+            return list(zip(locations[1], locations[0]))
+        except cv2.error as e:
+            print(e)
+
+    def parse_mask(self, match_method=cv2.TM_CCOEFF_NORMED):
+        mask_list = []
         match_list = self.match_temp(method=match_method)
         for m in match_list:
             mj = {
                 'type': 'coordinates',
                 "page": "all",
                 'x': m[0],
                 'y': m[1],
```

### Comparing `visual-compare-0.1.2/visual_compare/doc/image/ocr.py` & `visual-compare-0.1.3/visual_compare/doc/image/ocr.py`

 * *Files identical despite different names*

### Comparing `visual-compare-0.1.2/visual_compare/doc/visual_test.py` & `visual-compare-0.1.3/visual_compare/doc/visual_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 import logging
 import math
 import os
 import time
 import uuid
 from concurrent import futures
 from pathlib import Path
-from typing import Union
+from typing import Union, List
 
 import cv2
 import fitz
 import imutils
 import numpy as np
 import pytesseract
 from skimage import metrics
 
 from visual_compare.doc.image.compare_image import CompareImage
-from visual_compare.utils.downloader import is_url
+from visual_compare.utils.common import is_url
 
 logger = logging.getLogger(__name__)
 
 
 class VisualTest(object):
     ROBOT_LIBRARY_VERSION = 0.2
     BORDER_FOR_MOVE_TOLERANCE_CHECK = 0
@@ -41,14 +41,15 @@
     WATERMARK_HEIGHT = 30
     WATERMARK_CENTER_OFFSET = 3 / 100
     FONT = cv2.FONT_HERSHEY_SIMPLEX
     BOTTOM_LEFT_CORNER_OF_TEXT = (20, 60)
     FONT_SCALE = 0.7
     FONT_COLOR = (255, 0, 0)
     LINE_TYPE = 2
+    THRESHOLD = 0.95
     REFERENCE_LABEL = "Expected Result (Reference)"
     CANDIDATE_LABEL = "Actual Result (Candidate)"
     OCR_ENGINE = "tesseract"
     MOVEMENT_DETECTION = "classic"
 
     def __init__(self, threshold: float = 0.0000, dpi: int = DPI_DEFAULT, take_screenshots: bool = False,
                  show_diff: bool = False, ocr_engine: str = OCR_ENGINE, movement_detection: str = MOVEMENT_DETECTION,
@@ -86,15 +87,43 @@
 
         self._is_different = False
 
     @property
     def is_different(self):
         return self._is_different
 
-    def compare_images(self, reference_image: str, test_image: str, placeholder_file: str = None,
+    @staticmethod
+    def generate_mask(reference_image: str, mask_images: Union[str, List[str]], threshold=THRESHOLD):
+        """Generate mask base on ``reference_image`` and ``test_image``
+
+        Result is a json for mask when matched success, otherwise None
+
+        | =Arguments= | =Description= |
+        | ``reference_image`` | Path or URL of the Reference Image/Document, your expected result. May be .pdf, .ps, .pcl or image files |
+        | ``mask_images`` | List of the path or URL of the Reference Image/Document, your expected result. May be .pdf, .ps, .pcl or image files |
+        | ``threshold`` | Threshold for doc comparison between 0.0000 and 1.0000 . Default is 0.95. Higher values means that the documents are more similar. |
+
+        Return Examples:
+        | [{'type': 'coordinates', 'page': 'all', 'x': 724, 'y': 341, 'width': 139, 'height': 44}]
+        | None
+
+        """
+        from visual_compare.doc.image.image import MatchImg
+
+        mask = []
+        if isinstance(mask_images, str):
+            mask_images = [mask_images]
+        m_img = MatchImg(threshold=threshold)
+        for mi in mask_images:
+            res = m_img.parse_mask(source=reference_image, temp=mi)
+            mask.extend(res)
+
+        return mask if len(mask) > 0 else None
+
+    def compare_images(self, reference_image: str, test_image: str, placeholder_file: Union[str, list] = None,
                        mask: Union[str, dict, list] = None, check_text_content: bool = False,
                        move_tolerance: int = None, contains_barcodes: bool = False, get_pdf_content: bool = False,
                        force_ocr: bool = False, dpi: int = None, watermark_file: str = None,
                        ignore_watermarks: bool = None, ocr_engine: str = None, resize_candidate: bool = False,
                        blur: bool = False, threshold: float = None, **kwargs):
         """Compares the documents/images ``reference_image`` and ``test_image``.
 
@@ -119,16 +148,14 @@
         | ``threshold`` | Threshold for doc comparison between 0.0000 and 1.0000 . Default is 0.0000. Higher values mean more tolerance for doc differences. |
         | ``**kwargs`` | Everything else |
 
         Special Examples with ``mask``:
         | mask={"page": "all", type: "coordinates", "x": 0, "y": 0, "width": 100, "height": 100}
 
         """
-        # print("Execute comparison")
-        # print('Resolution for image comparison is: {}'.format(self.DPI))
 
         reference_collection = []
         compare_collection = []
         detected_differences = []
         screenshot_names = []
 
         if dpi is None:
@@ -140,14 +167,17 @@
         if ignore_watermarks is None:
             ignore_watermarks = os.getenv('IGNORE_WATERMARKS', False)
         if ocr_engine is None:
             ocr_engine = self.ocr_engine
         if threshold is None:
             threshold = self.threshold
 
+        if mask:
+            threshold = threshold + 0.0001
+
         compare_options = {'get_pdf_content': get_pdf_content, 'ignore_watermarks': ignore_watermarks,
                            'check_text_content': check_text_content, 'contains_barcodes': contains_barcodes,
                            'force_ocr': force_ocr, 'move_tolerance': move_tolerance, 'watermark_file': watermark_file,
                            'ocr_engine': ocr_engine, 'resize_candidate': resize_candidate, 'blur': blur,
                            'threshold': threshold}
 
         if (os.path.isfile(reference_image) is False) and (is_url(reference_image) is False):
```

### Comparing `visual-compare-0.1.2/visual_compare/utils/downloader.py` & `visual-compare-0.1.3/visual_compare/utils/downloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,32 +7,21 @@
    Author:          dingyong.cui
    date：           2023/5/6
 -------------------------------------------------
    Change Activity:
                     2023/5/6
 -------------------------------------------------
 """
+import os
 import tempfile
 import uuid
-from urllib import parse, request
-import os
-
-
-def is_url(url):
-    """
-    Check if the provided string is a valid URL.
-    """
-    try:
-        result = parse.urlparse(url)
-        return all([result.scheme, result.netloc])
-    except:
-        return False
+from urllib import request
 
 
-def download_file_from_url(url, directory=None, filename=None):
+def download_file_from_url(url: str, directory=None, filename=None):
     """
     Download the file from the url and save it in the provided directory.
     If directory is None, save it in a temp directory.
     Save the file with the provided filename.
     If the filename is None, try to check if the URL contains a valid filename.
     If the URL contains a valid filename, use that as a filename.
     if the URL does not contain a filename save it as a temporary filename by creating a uuid
```

### Comparing `visual-compare-0.1.2/visual_compare.egg-info/SOURCES.txt` & `visual-compare-0.1.3/visual_compare.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,25 @@
 visual_compare.egg-info/PKG-INFO
 visual_compare.egg-info/SOURCES.txt
 visual_compare.egg-info/dependency_links.txt
 visual_compare.egg-info/not-zip-safe
 visual_compare.egg-info/requires.txt
 visual_compare.egg-info/top_level.txt
 visual_compare/doc/__init__.py
+visual_compare/doc/match.py
+visual_compare/doc/models.py
+visual_compare/doc/pdf_test.py
 visual_compare/doc/visual_test.py
 visual_compare/doc/image/__init__.py
 visual_compare/doc/image/compare_image.py
 visual_compare/doc/image/image.py
 visual_compare/doc/image/ocr.py
 visual_compare/tests/__init__.py
 visual_compare/tests/conftest.py
 visual_compare/tests/test_compare_image.py
+visual_compare/tests/test_compare_pdf.py
+visual_compare/tests/test_downloader.py
+visual_compare/tests/test_image.py
+visual_compare/tests/test_visual_test.py
 visual_compare/utils/__init__.py
+visual_compare/utils/common.py
 visual_compare/utils/downloader.py
```


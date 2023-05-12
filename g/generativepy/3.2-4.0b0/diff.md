# Comparing `tmp/generativepy-3.2.tar.gz` & `tmp/generativepy-4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generativepy-3.2.tar", last modified: Sun Jun  5 12:24:46 2022, max compression
+gzip compressed data, was "generativepy-4.0b0.tar", last modified: Fri May 12 21:32:17 2023, max compression
```

## Comparing `generativepy-3.2.tar` & `generativepy-4.0b0.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-06-05 12:24:46.320093 generativepy-3.2/
--rw-r--r--   0 martin    (1000) martin    (1000)     1071 2018-11-08 18:18:07.000000 generativepy-3.2/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     2302 2022-06-05 12:24:46.320093 generativepy-3.2/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     1875 2022-06-05 12:20:51.000000 generativepy-3.2/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-06-05 12:24:46.164090 generativepy-3.2/generativepy/
--rw-rw-r--   0 martin    (1000) martin    (1000)       22 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      813 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/analytics.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4314 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/bitmap.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)    15277 2022-06-04 15:11:08.000000 generativepy-3.2/generativepy/color.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5184 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/drawing.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3072 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/drawing3d.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4037 2022-04-27 11:09:25.000000 generativepy-3.2/generativepy/formulas.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    38721 2022-06-04 15:52:43.000000 generativepy-3.2/generativepy/geometry.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3673 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/geometry3d.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      746 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/gif.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)    16761 2022-04-22 10:16:09.000000 generativepy-3.2/generativepy/graph.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5650 2022-04-27 13:59:36.000000 generativepy-3.2/generativepy/movie.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5844 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/nparray.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)     7231 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/tween.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1134 2021-12-19 11:40:04.000000 generativepy-3.2/generativepy/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-06-05 12:24:46.180090 generativepy-3.2/generativepy.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2302 2022-06-05 12:24:45.000000 generativepy-3.2/generativepy.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      697 2022-06-05 12:24:46.000000 generativepy-3.2/generativepy.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2022-06-05 12:24:45.000000 generativepy-3.2/generativepy.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       30 2022-06-05 12:24:45.000000 generativepy-3.2/generativepy.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2022-06-05 12:24:45.000000 generativepy-3.2/generativepy.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2022-06-05 12:24:46.320093 generativepy-3.2/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      744 2022-06-05 12:22:41.000000 generativepy-3.2/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-06-05 12:24:46.320093 generativepy-3.2/test/
--rw-rw-r--   0 martin    (1000) martin    (1000)    12818 2022-05-31 13:29:36.000000 generativepy-3.2/test/test_color.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1541 2022-06-04 16:35:21.000000 generativepy-3.2/test/test_regular_polygon.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      992 2021-11-17 18:58:19.000000 generativepy-3.2/test/test_text.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2873 2022-01-09 14:53:02.000000 generativepy-3.2/test/test_transform.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    15869 2021-11-17 18:58:19.000000 generativepy-3.2/test/test_tween.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2208 2021-11-17 18:58:19.000000 generativepy-3.2/test/test_utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.658942 generativepy-4.0b0/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1071 2018-11-08 18:18:07.000000 generativepy-4.0b0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3363 2023-05-12 21:32:17.658942 generativepy-4.0b0/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     2934 2023-05-12 21:31:54.000000 generativepy-4.0b0/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.656942 generativepy-4.0b0/generativepy/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       22 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      813 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/analytics.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4314 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/bitmap.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)    15507 2023-01-22 21:34:18.000000 generativepy-4.0b0/generativepy/color.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5184 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/drawing.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3072 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/drawing3d.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4795 2022-08-29 20:05:50.000000 generativepy-4.0b0/generativepy/formulas.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    38910 2023-05-12 21:16:17.000000 generativepy-4.0b0/generativepy/geometry.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4087 2022-12-29 16:41:56.000000 generativepy-4.0b0/generativepy/geometry3d.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      746 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/gif.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)    17510 2023-04-27 17:12:01.000000 generativepy-4.0b0/generativepy/graph.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7759 2023-03-04 20:01:53.000000 generativepy-4.0b0/generativepy/math.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5847 2022-12-02 13:47:14.000000 generativepy-4.0b0/generativepy/movie.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5844 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/nparray.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1969 2023-03-04 18:09:14.000000 generativepy-4.0b0/generativepy/shape2d.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5015 2023-02-11 11:56:27.000000 generativepy-4.0b0/generativepy/table.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)     9272 2022-12-11 14:17:23.000000 generativepy-4.0b0/generativepy/tween.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1134 2021-12-19 11:40:04.000000 generativepy-4.0b0/generativepy/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.656942 generativepy-4.0b0/generativepy.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3363 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      846 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       30 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-12 21:32:17.000000 generativepy-4.0b0/generativepy.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-05-12 21:32:17.659942 generativepy-4.0b0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      749 2023-05-12 21:22:36.000000 generativepy-4.0b0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-12 21:32:17.658942 generativepy-4.0b0/test/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12818 2022-05-31 13:29:36.000000 generativepy-4.0b0/test/test_color.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      856 2022-08-29 20:05:08.000000 generativepy-4.0b0/test/test_formulas.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3491 2023-03-04 17:52:42.000000 generativepy-4.0b0/test/test_matrix.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2391 2023-03-04 20:01:14.000000 generativepy-4.0b0/test/test_points.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1541 2022-06-04 16:35:21.000000 generativepy-4.0b0/test/test_regular_polygon.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      992 2021-11-17 18:58:19.000000 generativepy-4.0b0/test/test_text.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2873 2022-01-09 14:53:02.000000 generativepy-4.0b0/test/test_transform.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    23498 2023-02-16 21:01:33.000000 generativepy-4.0b0/test/test_tween.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2208 2021-11-17 18:58:19.000000 generativepy-4.0b0/test/test_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4264 2023-03-04 17:58:07.000000 generativepy-4.0b0/test/test_vector.py
```

### Comparing `generativepy-3.2/LICENSE` & `generativepy-4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/PKG-INFO` & `generativepy-4.0b0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generativepy
-Version: 3.2
+Version: 4.0b0
 Summary: Generative art library
 Home-page: https://github.com/martinmcbride/generativepy
 Author: Martin McBride
 Author-email: mcbride.martin@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # generativepy
 
 Generative art and graphing library for creating images and animations.
 
-## Version 3.2 notes
+## Version 4.0 beta notes
 
-* New `Color` properties `light1`, `light2`, `light3`, `dark1`, `dark2`, `dark3`, that creater lighter or darker versions of the base colour.
-* New RegularPolygon shape for drawing regular polygons.
-* New colour schemes for creating reusuable colour sets.
+This is a beta version, mainly because 3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
+
+* Allow images to eb preloaded for `Image` objects, to avoid frequent file reloads when creating animations.
+* Add shapes2d module representing abstract shapes.
+* Add math module with 2D vector and matrix classes.
+* Add `ORANGE`, `CYAN` to `ArtisticColorScheme`.
+* Add table module for table layouts.
+* MINOR BREAKING CHANGE - Extra warning if some scenes don't have audio (behaviour change if not all audio present).
+* BREAKING CHANGE - Tween use absolute time and a global frame rate. New methods wait_d and to_d for relative times.
+* BREAKING CHANGE - Remove count for Tween set method. This didn't work well with absolute times. Use `set` followed by `wait` or `wait_d` to set and hold a value.
+* BREAKING CHANGE - Improve geometry3d.
+* Fix colour depth problem in geometry3d (previously r, g, b values were forced to either 0% to 100%)
+* Allow special formatting of graph tick text labels
+* Allow tick label positions to be controlled in graph `Axes`.
+* Allow extra Latex packages to be specified in `formulas` module.
+* Fix bug in `formulas` module when function could hang if Latex formula was incorrect.
 
 ## Usage
 
 generativepy is a library rather an application. It provides useful functions and example code that allow you to
 create images and videos by writing simple Python scripts.
 
 The library requires:
@@ -45,14 +58,15 @@
 * Colour module that supports RGB, HSL and CSS colours, transparency, lerping, colormaps.
 * A simple tweening module to help with animation.
 * Geometry module for drawing shapes.
 * A graphing library for plotting 2D functions.
 * MovieBuilder supports creating video files from separate scenes.
 * Latex formula rendering
 * 3D geometry module using moderngl.
+* Math modules for vectors, matrices and abstract shapes. 
 
 ## Website
 
 Visit [pythoninformer.com](http://www.pythoninformer.com/generative-art/) for details:
 
 * [generativepy reference](http://www.pythoninformer.com/generative-art/generativepy/).
 * [generativepy tutorials](http://www.pythoninformer.com/generative-art/generativepy-tutorial/).
```

### Comparing `generativepy-3.2/README.md` & `generativepy-4.0b0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 # generativepy
 
 Generative art and graphing library for creating images and animations.
 
-## Version 3.2 notes
+## Version 4.0 beta notes
 
-* New `Color` properties `light1`, `light2`, `light3`, `dark1`, `dark2`, `dark3`, that creater lighter or darker versions of the base colour.
-* New RegularPolygon shape for drawing regular polygons.
-* New colour schemes for creating reusuable colour sets.
+This is a beta version, mainly because 3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
+
+* Allow images to eb preloaded for `Image` objects, to avoid frequent file reloads when creating animations.
+* Add shapes2d module representing abstract shapes.
+* Add math module with 2D vector and matrix classes.
+* Add `ORANGE`, `CYAN` to `ArtisticColorScheme`.
+* Add table module for table layouts.
+* MINOR BREAKING CHANGE - Extra warning if some scenes don't have audio (behaviour change if not all audio present).
+* BREAKING CHANGE - Tween use absolute time and a global frame rate. New methods wait_d and to_d for relative times.
+* BREAKING CHANGE - Remove count for Tween set method. This didn't work well with absolute times. Use `set` followed by `wait` or `wait_d` to set and hold a value.
+* BREAKING CHANGE - Improve geometry3d.
+* Fix colour depth problem in geometry3d (previously r, g, b values were forced to either 0% to 100%)
+* Allow special formatting of graph tick text labels
+* Allow tick label positions to be controlled in graph `Axes`.
+* Allow extra Latex packages to be specified in `formulas` module.
+* Fix bug in `formulas` module when function could hang if Latex formula was incorrect.
 
 ## Usage
 
 generativepy is a library rather an application. It provides useful functions and example code that allow you to
 create images and videos by writing simple Python scripts.
 
 The library requires:
@@ -31,14 +44,15 @@
 * Colour module that supports RGB, HSL and CSS colours, transparency, lerping, colormaps.
 * A simple tweening module to help with animation.
 * Geometry module for drawing shapes.
 * A graphing library for plotting 2D functions.
 * MovieBuilder supports creating video files from separate scenes.
 * Latex formula rendering
 * 3D geometry module using moderngl.
+* Math modules for vectors, matrices and abstract shapes. 
 
 ## Website
 
 Visit [pythoninformer.com](http://www.pythoninformer.com/generative-art/) for details:
 
 * [generativepy reference](http://www.pythoninformer.com/generative-art/generativepy/).
 * [generativepy tutorials](http://www.pythoninformer.com/generative-art/generativepy-tutorial/).
```

### Comparing `generativepy-3.2/generativepy/analytics.py` & `generativepy-4.0b0/generativepy/analytics.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy/bitmap.py` & `generativepy-4.0b0/generativepy/bitmap.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy/color.py` & `generativepy-4.0b0/generativepy/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
                 int(self.color[2] * 255),
                 int(self.color[3] * 255))
 
     @staticmethod
     def clamp(v):
         try:
             v = min(1, max(0, v)) #Clamp v between 0 and 1
-        except e:
+        except Exception as e:
             raise ValueError('Numerical value required') from e
         return v
 
     def __str__(self):
         return 'rgba' + str(self.color)
 
     def __getitem__(self, i):
@@ -440,14 +440,16 @@
 
     def __init__(self):
         self._RED = Color(0.941, 0.234, 0.125)
         self._BLUE = Color(0.250, 0.336, 0.629)
         self._GREEN = Color(0.250, 0.629, 0.336)
         self._YELLOW = Color(0.840, 0.598, 0.133)
         self._MAGENTA = Color(0.840, 0.133, 0.598)
+        self._ORANGE = Color("orangered")
+        self._CYAN = Color(0.250, 0.629 , 0.629)
         self._STEEL = Color(0.770, 0.793, 0.887)
         self._CREAM = Color(0.934, 0.883, 0.727)
         self._LIME = Color(0.727, 0.934, 0.727)
         self._BLACK = Color(0.2)
         self._GREY = Color(0.4)
         self._WHITE = Color(1)
 
@@ -468,14 +470,22 @@
         return self._YELLOW
 
     @property
     def MAGENTA(self):
         return self._MAGENTA
 
     @property
+    def ORANGE(self):
+        return self._ORANGE
+
+    @property
+    def CYAN(self):
+        return self._CYAN
+
+    @property
     def STEEL(self):
         return self._STEEL
 
     @property
     def CREAM(self):
         return self._CREAM
```

### Comparing `generativepy-3.2/generativepy/drawing.py` & `generativepy-4.0b0/generativepy/drawing.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy/drawing3d.py` & `generativepy-4.0b0/generativepy/drawing3d.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy/formulas.py` & `generativepy-4.0b0/generativepy/formulas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import subprocess
 from PIL import Image
 import numpy as np
 import random
 import os
 
 
-tex1 = '\n'.join([r'\documentclass[preview]{standalone}'
-                  r'\usepackage{amsmath}',
-                  r'\begin{document}',
-                  r'\begin{equation*}'])
-tex2 = '\n'.join([r'\end{equation*}'
-                  r'\end{document}'])
+def _create_tex(formula, packages):
+    """
+    Create tex from the formula and any optional packages.
+    Return latex string
+    """
+    tex_elements = [r'\documentclass[preview]{standalone}', r'\usepackage{amsmath}']
+    if packages:
+        tex_elements += [r'\usepackage{' + package + '}' for package in packages]
+    tex_elements += [r'\begin{document}', r'\begin{equation*}']
+    tex_elements += [formula]
+    tex_elements += [r'\end{equation*}', r'\end{document}']
+
+    return "\n".join(tex_elements)
 
 def _crop(inname, outname, color):
     """
     Crop the image and colour it in a flat colour. The alpha channel is left unchanged.
     :param inname: base name of input file. Input image is {inname}1.png. The 1 is added by latex.
     :param outname: base name of output file. Output image is {outname}.png
     :param color:
@@ -31,66 +38,77 @@
         for j in range(shape[1]):
             image_temp[i][j][3] = 255 - image_data[i][j][0]
 
     image_data = image_temp
     image_data_bw = image_data.max(axis=2)
     non_empty_columns = np.where(image_data_bw.max(axis=0)>0)[0]
     non_empty_rows = np.where(image_data_bw.max(axis=1)>0)[0]
-    cropbox = (min(non_empty_rows), max(non_empty_rows), min(non_empty_columns), max(non_empty_columns))
 
-    image_data_new = image_data[cropbox[0]:cropbox[1]+1, cropbox[2]:cropbox[3]+1 , :]
+    # If the image is empty, cropping will fail because non_empty_rows and non_empty_columns are empty. In that case
+    # we should not crop the image
+    if len(non_empty_rows) and len(non_empty_columns):
+        cropbox = (min(non_empty_rows), max(non_empty_rows), min(non_empty_columns), max(non_empty_columns))
+        image_data_new = image_data[cropbox[0]:cropbox[1]+1, cropbox[2]:cropbox[3]+1, :]
+        image_size = (cropbox[3]-cropbox[2], cropbox[1]-cropbox[0])
+    else:
+        image_data_new = image_data
+        image_size = image_data_new.shape[0:2]
 
     image_data_colored = np.zeros_like(image_data_new)
     color_data = (color.r*255, color.g*255, color.b*255)
     for i in range(image_data_new.shape[0]):
         for j in range(image_data_new.shape[1]):
             image_data_colored[i][j][3] = image_data_new[i][j][3]
             image_data_colored[i][j][0] = color_data[0]
             image_data_colored[i][j][1] = color_data[1]
             image_data_colored[i][j][2] = color_data[2]
 
     new_image = Image.fromarray(image_data_colored)
     filename = '{}.png'.format(outname)
     new_image.save(filename)
-    return filename, (cropbox[3]-cropbox[2], cropbox[1]-cropbox[0])
+    return filename, image_size
 
 def _remove_ignore_errors(filename):
     """
     Remove a file but ignore errors. We shouldn;t fail just because a temp file didn't get deleted.
     :param filename:
     :return: None
     """
     try:
         os.remove(filename)
     except Exception:
         pass
 
 
-def rasterise_formula(name, formula, color, dpi=600):
+def rasterise_formula(name, formula, color, dpi=600, packages=None):
     """
     Convert a latex formula into a PNG image. The PNG image will be tightly cropped, with a transparent background and
     text in the selected colour.
     :param name: Name of the output images. String with no extension, eg "myformula". The final output will be stored
     using this name, in the current working folder, so if you are creating multiple formulae give each one a unique name
     :param formula: The forumal, as a latex string.
     :param color: Color object defining the required colour of the output.
     :param dpi: The resolution, in dpi. This indirectly controls the size of the image,
+    :param packages: tuple containing any required additiona latex packages
     :return: A tuple containing the filename of teh result (with a png extension) and the (width, height) of the image
     in pixels.
     """
     unique_name = "{}-{}".format(name, random.randint(100000, 999999))
-    tex = '\n'.join([tex1, formula, tex2])
+    tex = _create_tex(formula, packages)
     tex_fn = '{}.tex'.format(unique_name)
     with open(tex_fn, 'w') as tex_file:
         tex_file.write(tex)
-    process = subprocess.Popen('latex {}.tex'.format(unique_name), shell=True,
+    process = subprocess.Popen('latex -interaction=batchmode {}.tex'.format(unique_name), shell=True,
                                stdout=subprocess.PIPE)
+    process.communicate()
     process.wait()
+
     process = subprocess.Popen('dvipng -T tight -D {} {}.dvi'.format(dpi, unique_name), shell=True,
                                stdout=subprocess.PIPE)
+    process.communicate()
     process.wait()
 
     filename, size = _crop(unique_name, name, color)
 
     _remove_ignore_errors("{}.aux".format(unique_name))
     _remove_ignore_errors("{}.log".format(unique_name))
     _remove_ignore_errors("{}.tex".format(unique_name))
```

### Comparing `generativepy-3.2/generativepy/geometry.py` & `generativepy-4.0b0/generativepy/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Author:  Martin McBride
 # Created: 2019-01-25
 # Copyright (C) 2018, Martin McBride
 # License: MIT
 import cairo
 import math
-from easy_vector import Vector
 from dataclasses import dataclass
 from generativepy.drawing import LEFT, CENTER, RIGHT, BOTTOM, MIDDLE, BASELINE, TOP
 from generativepy.drawing import WINDING
 from generativepy.drawing import FONT_WEIGHT_NORMAL, FONT_WEIGHT_BOLD
 from generativepy.drawing import FONT_SLANT_NORMAL, FONT_SLANT_ITALIC, FONT_SLANT_OBLIQUE
 from generativepy.drawing import MITER, ROUND, BEVEL, BUTT, SQUARE
 from generativepy.drawing import LINE, RAY, SEGMENT
+from generativepy.math import Vector as V
 from generativepy.color import Color
 
 class Pattern:
     '''
     Base class for all patterns.
     A pattern provides a fill (such as a gradient ort image fill) that can be used instead of a colour to
     fill or stroke a shape.
@@ -500,25 +500,21 @@
         return self
 
     def offset(self, x=0, y=0):
         self._offset = (x, y)
         return self
 
     def offset_angle(self, angle, distance):
-        x = distance*math.cos(angle)
-        y = distance*math.sin(angle)
-        self._offset = (x, y)
+        self._offset = V.polar(distance, angle)
         return self
 
     def offset_towards(self, point, distance):
-        direction = Vector(point) - Vector(self.position)
-        unit = direction/direction.length
-        x = distance*unit[0]
-        y = distance*unit[1]
-        self._offset = (x, y)
+        direction = V(point) - V(self.position)
+        unit = direction.unit
+        self._offset = (distance*unit.x, distance*unit.y)
         return self
 
 
 
 def text(ctx, txt, x, y, font=None, size=None, weight=None, slant=None, color=None, alignx=LEFT, aligny=BASELINE, flip=False):
     '''
     Draw text using ths supplied ctx
@@ -1143,29 +1139,38 @@
     draw(b[0], b[1], (-vector[0] + pvector[0]) * length / 2, (-vector[1] + pvector[1]) * length / 2,
          (-vector[0] - pvector[0]) * length / 2, (-vector[1] - pvector[1]) * length / 2)
 
 class Image():
 
     def __init__(self, ctx):
         self.ctx = ctx
-        self.filename = ''
+        self.image = None
         self.position = (0, 0)
         self.scale_factor = 1
 
-    def of_file_position(self, filename, position):
-        self.filename = filename
+    @staticmethod
+    def load_image(filename):
+        """
+        Load and image into an image surface.
+        @param filename: Path of file containing image.
+        @return:
+        """
+        return cairo.ImageSurface.create_from_png(filename)
+
+    def of_file_position(self, image, position):
+        self.image = image
         self.position = position
         return self
 
     def scale(self, scale_factor):
         self.scale_factor = scale_factor
         return self
 
     def paint(self):
-        image = cairo.ImageSurface.create_from_png(self.filename)
+        image = cairo.ImageSurface.create_from_png(self.image) if isinstance(self.image, str) else self.image
         self.ctx.save()
         self.ctx.translate(*self.position)
         self.ctx.scale(self.scale_factor, self.scale_factor)
         pattern = cairo.SurfacePattern(image)
         self.ctx.set_source(pattern)
         self.ctx.rectangle(0, 0, image.get_width(), image.get_height())
         self.ctx.fill()
```

### Comparing `generativepy-3.2/generativepy/geometry3d.py` & `generativepy-4.0b0/generativepy/geometry3d.py`

 * *Files 19% similar despite different names*

```diff
@@ -95,23 +95,36 @@
 
     def get_program(self):
         return self.program
 
 
 class Triangle():
 
-    def __init__(self):
+    def __init__(self, v0, v1, v2):
         self.vertices = np.array([
                 # x, y, z
-                [0.0, 0.8, 0.0],
-                [-0.6, -0.8, 0.0],
-                [0.6, -0.8, 0.0]
+                v0,
+                v1,
+                v2
             ], dtype='f4')
         self.Color = Color(0)
 
     def get_flat_color(self, color):
         self.Color = color
-        color_row = np.array([color.as_rgb_bytes()], dtype='f4')
+        color_row = np.array([[color.r, color.g, color.b]], dtype='f4')
         colors = np.repeat(color_row, 3, axis=0)
         vertex_data = np.concatenate([self.vertices, colors], axis=1)
         return vertex_data
 
+class Triangles():
+
+    def __init__(self, *args):
+        self.vertices = np.array(args, dtype='f4')
+        self.Color = Color(0)
+
+    def get_flat_color(self, color):
+        self.Color = color
+        color_row = np.array([[color.r, color.g, color.b]], dtype='f4')
+        colors = np.repeat(color_row, self.vertices.shape[0], axis=0)
+        vertex_data = np.concatenate([self.vertices, colors], axis=1)
+        return vertex_data
+
```

### Comparing `generativepy-3.2/generativepy/gif.py` & `generativepy-4.0b0/generativepy/gif.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy/graph.py` & `generativepy-4.0b0/generativepy/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,19 @@
     textcolor = Color(0.2)
     fontparams = FontParameters('arial', size=15, weight=FONT_WEIGHT_BOLD)
     divlines = StrokeParameters(Color(0.8, 0.8, 1), line_width=2, cap=BUTT)
     subdivlines = StrokeParameters(Color(0.9, 0.9, 1), line_width=2, cap=BUTT)
     axislines = StrokeParameters(Color(0.2), line_width=2, cap=BUTT)
     featurescale = 1
 
+    # x and y offset of tick labels. The actual offset is:
+    # text height (height of 0 character using fontparams) DIVIDED by ticklabeloffset
+    ticklabeloffset = 1.1
+
+
 
 class Axes:
     '''
     Controls the range and appearance of a set of Cartesian axes
     '''
 
     def __init__(self, ctx, position, width, height):
@@ -41,14 +46,16 @@
         self.height = height
         self.start = (0, 0)
         self.extent = (10, 10)
         self.divisions = (1, 1)
         self.subdivisons = False
         self.subdivisionfactor = (1, 1)
         self.text_height = 0
+        self.x_div_formatter = None
+        self.y_div_formatter = None
 
     def of_start(self, start):
         '''
         Sets the start value of the axes
         :param start: (x, y) value of bottom left corner of axes
         :return: self
         '''
@@ -79,14 +86,19 @@
         Set divisons spacing
         :param divisions: (x, y) spacing divisions in each direction
         :return: self
         '''
         self.divisions = divisions
         return self
 
+    def with_division_formatters(self, x_div_formatter=None, y_div_formatter=None):
+        self.x_div_formatter = x_div_formatter
+        self.y_div_formatter = y_div_formatter
+        return self
+
     def with_subdivisions(self, factor):
         '''
         Draw subdivision lines on graph
         :param factor: (x, y) Number of subdivisions per division in each direction
         :return: self
         '''
         self.subdivisons = True
@@ -167,14 +179,15 @@
 
     def draw(self):
         '''
         Draw the axes
         :return:
         '''
 
+        self.ctx.new_path()
         # Get the text height using the selected font. This is used to control text offset and other sizes.
         _, self.text_height = Text(self.ctx).of('0', (0, 0)) \
                                 .font(self.appearance.fontparams.font,
                                       self.appearance.fontparams.weight,
                                       self.appearance.fontparams.slant) \
                                 .size(self.appearance.fontparams.size * self.appearance.featurescale) \
                                 .get_size()
@@ -230,35 +243,35 @@
         self.ctx.stroke()
 
     def _draw_axes_values(self):
         params = copy.copy(self.appearance.axislines)
         params.line_width *= self.appearance.featurescale
         params.apply(self.ctx)
 
-        xoffset = self.text_height/1.1
-        yoffset = self.text_height/1.1
+        xoffset = self.text_height/self.appearance.ticklabeloffset
+        yoffset = self.text_height/self.appearance.ticklabeloffset
         for p in self._get_divs(self.start[0], self.extent[0], self.divisions[0]):
             if abs(p)>0.001:
                 position = self.transform_from_graph((p, 0))
-                pstr = self._format_div(p, self.divisions[0])
+                pstr = self._format_div(p, self.divisions[0], self.x_div_formatter)
                 Text(self.ctx).of(pstr, (position[0] - xoffset, position[1] + yoffset))\
                     .font(self.appearance.fontparams.font, self.appearance.fontparams.weight,
                           self.appearance.fontparams.slant)\
                     .size(self.appearance.fontparams.size*self.appearance.featurescale)\
                     .align(drawing.RIGHT, drawing.TOP).fill(self.appearance.textcolor)
                 params.apply(self.ctx)
                 self.ctx.new_path()
                 self.ctx.move_to(position[0], position[1])
                 self.ctx.line_to(position[0], position[1] + yoffset)
                 self.ctx.stroke()
 
         for p in self._get_divs(self.start[1], self.extent[1], self.divisions[1]):
             if abs(p)>0.001:
                 position = self.transform_from_graph((0, p))
-                pstr = self._format_div(p, self.divisions[1])
+                pstr = self._format_div(p, self.divisions[1], self.y_div_formatter)
                 Text(self.ctx).of(pstr, (position[0] - xoffset, position[1] + yoffset))\
                     .font(self.appearance.fontparams.font, self.appearance.fontparams.weight,
                           self.appearance.fontparams.slant)\
                     .size(self.appearance.fontparams.size*self.appearance.featurescale)\
                     .align(drawing.RIGHT, drawing.TOP).fill(self.appearance.textcolor)
                 params.apply(self.ctx)
                 self.ctx.new_path()
@@ -310,23 +323,27 @@
         n = math.ceil(start/subdiv)*subdiv
         while n <= start + extent:
             if not self._contains(divs, subdiv, extent/100000):
                 subdivs.append(n)
             n += subdiv
         return subdivs
 
-    def _format_div(self, value, div):
+    def _format_div(self, value, div, formatter):
         """
         Formats a division value into a string.
         If the division spacing is an integer, the string will be an integer (no dp).
         If the division spacing is float, the string will be a float with a suitable number of decimal places
         :param value: value to be formatted
         :param div: division spacing
+        :param formatter: formatting function, accepts vale and div, returns a formatted value string
         :return: string representation of the value
         """
+        if formatter:
+            return formatter(value, div)
+
         if isinstance(value, int):
             return str(value)
         return str(round(value*1000)/1000)
 
     def transform_from_graph(self, point):
         '''
         Scale the ctx so that point (x, y) will be correctly positioned in the axes coordinates
```

### Comparing `generativepy-3.2/generativepy/movie.py` & `generativepy-4.0b0/generativepy/movie.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from PIL import Image
 from generativepy.utils import temp_file
 from moviepy.audio.io.AudioFileClip import AudioFileClip
 from moviepy.editor import VideoClip
 from moviepy.video.compositing.concatenate import concatenate_videoclips
 import subprocess as sp
 import pathlib
+import logging
 
 
 '''
 The movie functions operate pn lazy sequences of images. The images are stored as numpy arrays.
 '''
 
 def normalise_array(array):
@@ -134,15 +135,17 @@
 
         # Due to a bug in moviepy 1.0.1, when we write a video out in this mode the audio is not included.
         # So we write the video and audio out to separate temporary files.
         # We then use ffmpeg directly to combine the video and audio.
         temp_video_filename = temp_file(pathlib.Path(video_out).stem + "TEMP.mp4")
         temp_audio_filename = temp_file(pathlib.Path(video_out).stem + "TEMP.m4a")
 
-        if not self.audio_files[0]:
+        if not all(self.audio_files):
+            if any(self.audio_files):
+                logging.warning("MovieBuilder - some of the scenes have audio data, some do not, so the final video will have no audio data")
             video.write_videofile(video_out, codec="libx264", fps=self.frame_rate)
         else:
             video.write_videofile(temp_video_filename, temp_audiofile=temp_audio_filename, codec="libx264",
                                   remove_temp=False, audio_codec="aac", fps=self.frame_rate)
 
             command = ["ffmpeg",
                        "-y", #approve output file overwite
```

### Comparing `generativepy-3.2/generativepy/nparray.py` & `generativepy-4.0b0/generativepy/nparray.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy/tween.py` & `generativepy-4.0b0/generativepy/tween.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # Author:  Martin McBride
 # Created: 2019-01-25
 # Copyright (C) 2018, Martin McBride
 # License: MIT
-
+import collections
 import math
 
+_FRAME_RATE = 1
+
+def set_frame_rate(rate):
+    global _FRAME_RATE
+    if not isinstance(rate, (int, float)):
+        raise ValueError('Frame rate must be a numeric value')
+    if rate < 1:
+        raise ValueError('Frame rate must be one or greater')
+    _FRAME_RATE = rate
 
 class Tween():
     '''
     Tweening class for scalar values
 
     Initial value is set on construction.
 
     wait() maintains the current value for the requested number of frames
 
-    pad() similar to wait, but pads until the total length of the tween is the required size.
-
     set() sets a new current values, and adds it for the requested number of frames (which can be zero)
 
     to() moves linearly from the current value to the supplied value. The first frame added will have the current value,
     the last frame added will have the new value, with values spaced evenly in between. The final value will be set as
     the new current value.
 
     You can use get(n) to get the nth frame, or alternatively you can use tween[n]. The built in len() function can be
@@ -29,44 +36,58 @@
     def __init__(self, value=0):
         self.check_value(value, None)
         self.frames = []
         self.previous = value
         self.nextFrame = 0
 
     def wait(self, count):
-        self.check_count(count)
+        count = self.check_count(count, len(self.frames))
         self.frames.extend([self.previous for i in range(count)])
         return self
 
-    def pad(self, final_length):
-        self.check_count(final_length)
-        required = final_length - len(self.frames)
-        if required > 0:
-            self.frames.extend([self.previous for i in range(required)])
+    def wait_d(self, count):
+        count = self.check_d_count(count)
+        self.frames.extend([self.previous for i in range(count)])
         return self
 
-    def set(self, value, count=0):
+    def set(self, value):
         self.check_value(value, self.previous)
-        self.check_count(count)
-        self.frames.extend([value for i in range(count)])
         self.previous = value
         return self
 
     def to(self, value, count):
         self.check_value(value, self.previous)
-        self.check_count(count)
+        count = self.check_count(count, len(self.frames))
+        for i in range(count):
+            factor = (i + 1) / count
+            self.frames.append(self.previous + factor * (value - self.previous))
+        self.previous = value
+        return self
+
+    def to_d(self, value, count):
+        self.check_value(value, self.previous)
+        count = self.check_d_count(count)
         for i in range(count):
             factor = (i + 1) / count
             self.frames.append(self.previous + factor * (value - self.previous))
         self.previous = value
         return self
 
     def ease(self, value, count, ease_function):
         self.check_value(value, self.previous)
-        self.check_count(count)
+        count = self.check_count(count, len(self.frames))
+        for i in range(count):
+            factor = ease_function((i + 1) / count)
+            self.frames.append(self.previous + factor * (value - self.previous))
+        self.previous = value
+        return self
+
+    def ease_d(self, value, count, ease_function):
+        self.check_value(value, self.previous)
+        count = self.check_d_count(count)
         for i in range(count):
             factor = ease_function((i + 1) / count)
             self.frames.append(self.previous + factor * (value - self.previous))
         self.previous = value
         return self
 
     def get(self, frame):
@@ -84,24 +105,31 @@
         self.nextFrame += 1
         return frame
 
     def __iter__(self):
         return self
 
     def check_value(self, value, previous):
-        if (not isinstance(value, (int, float))) or isinstance(value, bool):
+        if not isinstance(value, (int, float)):
             raise ValueError('Numeric value required')
 
-    def check_index(self, value):
-        if not isinstance(value, int):
-            raise ValueError('Integer value required')
-
-    def check_count(self, value):
-        if not isinstance(value, int) or value < 0:
-            raise ValueError('Non-negative integer value required')
+    def check_count(self, count, current):
+        if not isinstance(count, (int, float)):
+            raise ValueError('Count must be a number')
+        count = int(_FRAME_RATE*count)
+        if count < current:
+            raise ValueError('New time must not be less than previous time')
+        return count - current
+
+    def check_d_count(self, count):
+        if not isinstance(count, (int, float)):
+            raise ValueError('Count must be a number')
+        if count < 0:
+            raise ValueError('Count must not be negative')
+        return int(_FRAME_RATE*count)
 
     def __len__(self):
         return len(self.frames)
 
 
 class TweenVector(Tween):
     '''
@@ -112,48 +140,72 @@
 
     The vector quantities must have at least 1 element, but normally it will be 2 or more. Every value added must have
     the same length as the initial value, for example if you start with an (x, y) value, every new value must also
     have 2 dimansions.
     '''
 
     def __init__(self, value=(0, 0)):
+        self.check_value(value, None)
         Tween.__init__(self, value)
 
     def to(self, value, count):
         self.check_value(value, self.previous)
-        self.check_count(count)
+        count = self.check_count(count, len(self.frames))
+        for i in range(count):
+            nextvalue = []
+            factor = (i + 1) / count
+            for a, b in zip(self.previous, value):
+                nextvalue.append(a + factor * (b - a))
+            self.frames.append(nextvalue)
+        self.previous = value
+        return self
+
+    def to_d(self, value, count):
+        self.check_value(value, self.previous)
+        count = self.check_d_count(count)
         for i in range(count):
             nextvalue = []
             factor = (i + 1) / count
             for a, b in zip(self.previous, value):
                 nextvalue.append(a + factor * (b - a))
             self.frames.append(nextvalue)
         self.previous = value
         return self
 
     def ease(self, value, count, ease_function):
         self.check_value(value, self.previous)
-        self.check_count(count)
+        count = self.check_count(count, len(self.frames))
+        for i in range(count):
+            nextvalue = []
+            factor = ease_function((i + 1) / count)
+            for a, b in zip(self.previous, value):
+                nextvalue.append(a + factor * (b - a))
+            self.frames.append(nextvalue)
+        self.previous = value
+        return self
+
+    def ease_d(self, value, count, ease_function):
+        self.check_value(value, self.previous)
+        count = self.check_d_count(count)
         for i in range(count):
             nextvalue = []
             factor = ease_function((i + 1) / count)
             for a, b in zip(self.previous, value):
                 nextvalue.append(a + factor * (b - a))
             self.frames.append(nextvalue)
         self.previous = value
         return self
 
     def check_value(self, value, previous):
-        try:
-            if len(value) <= 0:
-                raise ValueError('Vectors of rank 0 are not supported')
-            if previous and len(value) != len(self.previous):
-                raise ValueError('All values must be vectors of equal rank')
-        except:
-            ValueError('Sequence value required')
+        if not isinstance(value, collections.abc.Sequence) or isinstance(value, str):
+            raise ValueError('Sequence value required')
+        if len(value) <= 0:
+            raise ValueError('Vectors of rank 0 are not supported')
+        if previous and len(value) != len(self.previous):
+            raise ValueError('All values must be vectors of equal rank')
 
 
 def ease_linear():
     return lambda x: x
 
 
 def ease_in_harm():
```

### Comparing `generativepy-3.2/generativepy/utils.py` & `generativepy-4.0b0/generativepy/utils.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/generativepy.egg-info/PKG-INFO` & `generativepy-4.0b0/generativepy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generativepy
-Version: 3.2
+Version: 4.0b0
 Summary: Generative art library
 Home-page: https://github.com/martinmcbride/generativepy
 Author: Martin McBride
 Author-email: mcbride.martin@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # generativepy
 
 Generative art and graphing library for creating images and animations.
 
-## Version 3.2 notes
+## Version 4.0 beta notes
 
-* New `Color` properties `light1`, `light2`, `light3`, `dark1`, `dark2`, `dark3`, that creater lighter or darker versions of the base colour.
-* New RegularPolygon shape for drawing regular polygons.
-* New colour schemes for creating reusuable colour sets.
+This is a beta version, mainly because 3D drawing is likely to change in a future release. The rest of the library is reasonably stable. 
+
+* Allow images to eb preloaded for `Image` objects, to avoid frequent file reloads when creating animations.
+* Add shapes2d module representing abstract shapes.
+* Add math module with 2D vector and matrix classes.
+* Add `ORANGE`, `CYAN` to `ArtisticColorScheme`.
+* Add table module for table layouts.
+* MINOR BREAKING CHANGE - Extra warning if some scenes don't have audio (behaviour change if not all audio present).
+* BREAKING CHANGE - Tween use absolute time and a global frame rate. New methods wait_d and to_d for relative times.
+* BREAKING CHANGE - Remove count for Tween set method. This didn't work well with absolute times. Use `set` followed by `wait` or `wait_d` to set and hold a value.
+* BREAKING CHANGE - Improve geometry3d.
+* Fix colour depth problem in geometry3d (previously r, g, b values were forced to either 0% to 100%)
+* Allow special formatting of graph tick text labels
+* Allow tick label positions to be controlled in graph `Axes`.
+* Allow extra Latex packages to be specified in `formulas` module.
+* Fix bug in `formulas` module when function could hang if Latex formula was incorrect.
 
 ## Usage
 
 generativepy is a library rather an application. It provides useful functions and example code that allow you to
 create images and videos by writing simple Python scripts.
 
 The library requires:
@@ -45,14 +58,15 @@
 * Colour module that supports RGB, HSL and CSS colours, transparency, lerping, colormaps.
 * A simple tweening module to help with animation.
 * Geometry module for drawing shapes.
 * A graphing library for plotting 2D functions.
 * MovieBuilder supports creating video files from separate scenes.
 * Latex formula rendering
 * 3D geometry module using moderngl.
+* Math modules for vectors, matrices and abstract shapes. 
 
 ## Website
 
 Visit [pythoninformer.com](http://www.pythoninformer.com/generative-art/) for details:
 
 * [generativepy reference](http://www.pythoninformer.com/generative-art/generativepy/).
 * [generativepy tutorials](http://www.pythoninformer.com/generative-art/generativepy-tutorial/).
```

### Comparing `generativepy-3.2/generativepy.egg-info/SOURCES.txt` & `generativepy-4.0b0/generativepy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,22 +9,29 @@
 generativepy/drawing.py
 generativepy/drawing3d.py
 generativepy/formulas.py
 generativepy/geometry.py
 generativepy/geometry3d.py
 generativepy/gif.py
 generativepy/graph.py
+generativepy/math.py
 generativepy/movie.py
 generativepy/nparray.py
+generativepy/shape2d.py
+generativepy/table.py
 generativepy/tween.py
 generativepy/utils.py
 generativepy.egg-info/PKG-INFO
 generativepy.egg-info/SOURCES.txt
 generativepy.egg-info/dependency_links.txt
 generativepy.egg-info/requires.txt
 generativepy.egg-info/top_level.txt
 test/test_color.py
+test/test_formulas.py
+test/test_matrix.py
+test/test_points.py
 test/test_regular_polygon.py
 test/test_text.py
 test/test_transform.py
 test/test_tween.py
-test/test_utils.py
+test/test_utils.py
+test/test_vector.py
```

### Comparing `generativepy-3.2/setup.py` & `generativepy-4.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
  
 setup(name='generativepy',
-      version='3.2',
+      version='4.0 beta',
       url='https://github.com/martinmcbride/generativepy',
       license='MIT',
       author='Martin McBride',
       author_email='mcbride.martin@gmail.com',
       description='Generative art library',
       long_description=long_description,
       long_description_content_type="text/markdown",
```

### Comparing `generativepy-3.2/test/test_color.py` & `generativepy-4.0b0/test/test_color.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/test/test_regular_polygon.py` & `generativepy-4.0b0/test/test_regular_polygon.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/test/test_text.py` & `generativepy-4.0b0/test/test_text.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/test/test_transform.py` & `generativepy-4.0b0/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `generativepy-3.2/test/test_utils.py` & `generativepy-4.0b0/test/test_utils.py`

 * *Files identical despite different names*


# Comparing `tmp/easy-pil-0.2.3.tar.gz` & `tmp/easy_pil-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/easy-pil/easy-pil/dist/.tmp-ih6r3587/easy-pil-0.2.3.tar", last modified: Mon May  8 08:53:19 2023, max compression
+gzip compressed data, was "easy_pil-0.2.4.tar", max compression
```

## Comparing `easy-pil-0.2.3.tar` & `easy_pil-0.2.4.tar`

### file list

```diff
@@ -1,45 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 08:53:08.000000 easy-pil-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 08:53:08.000000 easy-pil-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-08 08:53:19.000000 easy-pil-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-08 08:53:08.000000 easy-pil-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/font.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/caveat/
--rw-r--r--   0 runner    (1001) docker     (123)   256900 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/caveat/caveat.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/
--rw-r--r--   0 runner    (1001) docker     (123)   244468 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   249088 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   242068 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   245708 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (123)   153900 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   181972 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159848 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158192 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/types/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-08 08:53:08.000000 easy-pil-0.2.3/easy_pil/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 08:53:19.000000 easy-pil-0.2.3/easy_pil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 08:53:08.000000 easy-pil-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-08 08:53:08.000000 easy-pil-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:53:19.000000 easy-pil-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-08 08:53:08.000000 easy-pil-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:53:19.000000 easy-pil-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 08:53:08.000000 easy-pil-0.2.3/tests/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-08 08:53:08.000000 easy-pil-0.2.3/tests/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-08 08:53:08.000000 easy-pil-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1056 2023-05-12 14:58:42.195381 easy_pil-0.2.4/LICENSE
+-rw-r--r--   0        0        0      911 2023-05-12 14:58:42.195381 easy_pil-0.2.4/README.md
+-rw-r--r--   0        0        0      454 2023-05-12 14:58:42.199381 easy_pil-0.2.4/easy_pil/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-12 14:58:42.199381 easy_pil-0.2.4/easy_pil/_version.py
+-rw-r--r--   0        0        0     1059 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/canvas.py
+-rw-r--r--   0        0        0    18927 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/editor.py
+-rw-r--r--   0        0        0     3359 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/font.py
+-rw-r--r--   0        0        0   256900 2023-05-12 14:58:42.203382 easy_pil-0.2.4/easy_pil/fonts/caveat/caveat.ttf
+-rw-r--r--   0        0        0   244468 2023-05-12 14:58:42.207382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_bold.ttf
+-rw-r--r--   0        0        0   249088 2023-05-12 14:58:42.207382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_italic.ttf
+-rw-r--r--   0        0        0   242068 2023-05-12 14:58:42.211382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_light.ttf
+-rw-r--r--   0        0        0   245708 2023-05-12 14:58:42.211382 easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_regular.ttf
+-rw-r--r--   0        0        0   153900 2023-05-12 14:58:42.215382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_bold.ttf
+-rw-r--r--   0        0        0   181972 2023-05-12 14:58:42.215382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_italic.ttf
+-rw-r--r--   0        0        0   159848 2023-05-12 14:58:42.215382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_light.ttf
+-rw-r--r--   0        0        0   158192 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_regular.ttf
+-rw-r--r--   0        0        0      807 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/text.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/types/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/types/common.py
+-rw-r--r--   0        0        0     1490 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/types/workspace.py
+-rw-r--r--   0        0        0     1608 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/utils.py
+-rw-r--r--   0        0        0     6651 2023-05-12 14:58:42.219382 easy_pil-0.2.4/easy_pil/workspace.py
+-rw-r--r--   0        0        0     1560 2023-05-12 14:58:42.223382 easy_pil-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 easy_pil-0.2.4/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `easy-pil-0.2.3/LICENSE` & `easy_pil-0.2.4/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Copyright 202 shahriyardx
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `easy-pil-0.2.3/PKG-INFO` & `easy_pil-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: easy-pil
-Version: 0.2.3
-Summary: A library to make common tasks of Pillow easy.
+Version: 0.2.4
+Summary: A Python library built on top of PIL to easily edit/modify images
 Home-page: https://github.com/shahriyardx/easy-pil
+Keywords: easy-pil,easy pillow,Pillow,image editing
 Author: Md Shahriyar Alam
-Author-email: contact@shahriyar.dev
-Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
-Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
-Project-URL: Source, https://github.com/shahriyardx/easy-pil/
-Keywords: Pillow,PIL,Pillow wrapper,PIL wrapper,Easy Pillow,Easy PIL,discord rank card,discord card
+Author-email: mdshahriyaralam552@gmail.com
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <4
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Dist: aiocache (>=0.12.1,<0.13.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/shahriyardx/easy-pil
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 # Easy PIL
-A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+![Lint-Test](https://github.com/shahriyardx/easy-pil/actions/workflows/lint-test.yml/badge.svg)
+
+A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images.
 
 ## Getting Started
 Using this for the first time? Here are some links to help you get started.
 
 - Read the [docs](https://easy-pil.readthedocs.io/en/latest/)
 - First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
 - Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
 - Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
 - [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
 
 ## Get help
 - Ask us in our [Discord server](https://discord.gg/fVzt5THTNb)
 - Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
+
```

### Comparing `easy-pil-0.2.3/README.md` & `easy_pil-0.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Easy PIL
-A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+![Lint-Test](https://github.com/shahriyardx/easy-pil/actions/workflows/lint-test.yml/badge.svg)
+
+A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images.
 
 ## Getting Started
 Using this for the first time? Here are some links to help you get started.
 
 - Read the [docs](https://easy-pil.readthedocs.io/en/latest/)
 - First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
 - Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
 - Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
 - [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
 
 ## Get help
 - Ask us in our [Discord server](https://discord.gg/fVzt5THTNb)
-- Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
+- Watch [Youtube Tutorials](https://www.youtube.com/playlist?list=PLb_oBhGqAlbT4yVqV0TSXggA8b0lZhGhn)
```

### Comparing `easy-pil-0.2.3/easy_pil/editor.py` & `easy_pil-0.2.4/easy_pil/editor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
 from io import BytesIO
-from typing import List, Tuple, Union
+from pathlib import Path
+from typing import List, Literal, Optional, Tuple, Union
 
-from PIL import Image, ImageDraw, ImageFilter, ImageFont
-from typing_extensions import Literal
+from PIL import Image as PilImage, ImageDraw, ImageFilter, ImageFont
+from PIL.Image import Image
 
 from .canvas import Canvas
 from .font import Font
 from .text import Text
 from .types.common import Color
 
 
 class Editor:
     """Editor class. It does all the editing operations.
 
     Parameters
     ----------
-    image : Union[Image.Image, str, Editor, Canvas]
+    _image : Union[Image, str, Editor, Canvas]
         Image or Canvas to edit.
     """
 
     def __init__(
-        self, image: Union[Image.Image, str, BytesIO, Editor, Canvas]
+        self, _image: Union[Image, str, BytesIO, Editor, Canvas]
     ) -> None:
-        self.image = None
-
-        if isinstance(image, str) or isinstance(image, BytesIO):
-            self.image = Image.open(image).convert("RGBA")
-        elif isinstance(image, Canvas) or isinstance(image, Editor):
-            self.image = image.image.convert("RGBA")
+        if isinstance(_image, (str, BytesIO, Path)):
+            self.image: Image = PilImage.open(_image)
+        elif isinstance(_image, (Canvas, Editor)):
+            self.image: Image = _image.image.convert("RGBA")
+        elif isinstance(_image, Image):
+            self.image: Image = _image.convert("RGBA")
         else:
-            self.image = image.convert("RGBA")
+            raise ValueError(
+                "Editor requires an Image, Path, "
+                "Editor or Canvas to start with"
+            )
 
     @property
     def image_bytes(self) -> BytesIO:
         """Return image bytes
 
         Returns
         -------
@@ -44,205 +48,205 @@
         """
         _bytes = BytesIO()
         self.image.save(_bytes, "png")
 
         _bytes.seek(0)
         return _bytes
 
-    def resize(self, size: Tuple[float, float], crop=False) -> Editor:
+    def resize(self, size: Tuple[int, int], crop=False) -> Editor:
         """Resize image
 
         Parameters
         ----------
-        size : Tuple[float, float]
+        size : Tuple[int, int]
             New Size of image
         crop : bool, optional
             Crop the image to bypass distortion, by default False
         """
         if not crop:
-            self.image = self.image.resize(size, Image.LANCZOS)
+            self.image = self.image.resize(size, PilImage.LANCZOS)
 
         else:
             width, height = self.image.size
             ideal_width, ideal_height = size
 
-            aspect = width / float(height)
-            ideal_aspect = ideal_width / float(ideal_height)
+            aspect = width / height
+            ideal_aspect = ideal_width / ideal_height
 
             if aspect > ideal_aspect:
-                new_width = int(ideal_aspect * height)
-                offset = (width - new_width) / 2
+                new_width = ideal_aspect * height
+                offset = int((width - new_width) / 2)
                 resize = (offset, 0, width - offset, height)
             else:
-                new_height = int(width / ideal_aspect)
-                offset = (height - new_height) / 2
+                new_height = width / ideal_aspect
+                offset = int((height - new_height) / 2)
                 resize = (0, offset, width, height - offset)
 
             self.image = self.image.crop(resize).resize(
-                (ideal_width, ideal_height), Image.LANCZOS
+                (ideal_width, ideal_height), PilImage.LANCZOS
             )
 
         return self
 
     def rounded_corners(self, radius: int = 10, offset: int = 2) -> Editor:
         """Make image rounded corners
 
         Parameters
         ----------
         radius : int, optional
             Radius of roundness, by default 10
         offset : int, optional
             Offset pixel while making rounded, by default 2
         """
-        background = Image.new(
+        background = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
-        holder = Image.new(
+        holder = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
-        mask = Image.new(
+        mask = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
         mask_draw = ImageDraw.Draw(mask)
         mask_draw.rounded_rectangle(
             (offset, offset)
             + (self.image.size[0] - offset, self.image.size[1] - offset),
             radius=radius,
             fill="black",
         )
         holder.paste(self.image, (0, 0))
-        self.image = Image.composite(holder, background, mask)
+        self.image = PilImage.composite(holder, background, mask)
 
         return self
 
     def circle_image(self) -> Editor:
         """Make image circle"""
-        background = Image.new(
+        background = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
-        holder = Image.new(
+        holder = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
-        mask = Image.new(
+        mask = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
         mask_draw = ImageDraw.Draw(mask)
         ellipse_size = tuple(i - 1 for i in self.image.size)
         mask_draw.ellipse((0, 0) + ellipse_size, fill="black")
         holder.paste(self.image, (0, 0))
-        self.image = Image.composite(holder, background, mask)
+        self.image = PilImage.composite(holder, background, mask)
 
         return self
 
     def rotate(self, deg: float = 0, expand: bool = False) -> Editor:
         """Rotate image
 
         Parameters
         ----------
         deg : float, optional
-            Degress to rotate, by default 0
+            Degrees to rotate, by default 0
         expand : bool, optional
             Expand while rotating, by default False
         """
-        self.image = self.image.rotate(angle=deg, expand=expand)
+        self.image = self.image.rotate(deg, expand=expand)
         return self
 
     def blur(
-        self, mode: Literal["box", "gussian"] = "gussian", amount: float = 1
+        self, mode: Literal["box", "gaussian"] = "gaussian", amount: float = 1
     ) -> Editor:
         """Blur image
 
         Parameters
         ----------
-        mode : Literal["box", "gussian"], optional
-            Blur mode, by default "gussian"
+        mode : Literal["box", "gaussian"], optional
+            Blur mode, by default "gaussian"
         amount : float, optional
             Amount of blur, by default 1
         """
         if mode == "box":
             self.image = self.image.filter(ImageFilter.BoxBlur(radius=amount))
-        if mode == "gussian":
+        if mode == "gaussian":
             self.image = self.image.filter(
                 ImageFilter.GaussianBlur(radius=amount)
             )
 
         return self
 
     def blend(
         self,
-        image: Union[Image.Image, Editor, Canvas],
+        image: Union[Image, Editor, Canvas],
         alpha: float = 0.0,
         on_top: bool = False,
     ) -> Editor:
         """Blend image into editor image
 
         Parameters
         ----------
-        image : Union[Image.Image, Editor, Canvas]
+        image : Union[Image, Editor, Canvas]
             Image to blend
         alpha : float, optional
             Alpha amount, by default 0.0
         on_top : bool, optional
             Places image on top, by default False
         """
         if isinstance(image, Editor) or isinstance(image, Canvas):
             image = image.image
 
         if image.size != self.image.size:
             image = Editor(image).resize(self.image.size, crop=True).image
 
         if on_top:
-            self.image = Image.blend(self.image, image, alpha=alpha)
+            self.image = PilImage.blend(self.image, image, alpha=alpha)
         else:
-            self.image = Image.blend(image, self.image, alpha=alpha)
+            self.image = PilImage.blend(image, self.image, alpha=alpha)
 
         return self
 
     def paste(
         self,
-        image: Union[Image.Image, Editor, Canvas],
-        position: Tuple[float, float],
+        image: Union[Image, Editor, Canvas],
+        position: Tuple[int, int],
     ) -> Editor:
         """Paste image into editor
 
         Parameters
         ----------
-        image : Union[Image.Image, Editor, Canvas]
+        image : Union[Image, Editor, Canvas]
             Image to paste
         position : Tuple[float, float]
             Position to paste
         """
-        blank = Image.new(
+        blank = PilImage.new(
             "RGBA", size=self.image.size, color=(255, 255, 255, 0)
         )
 
         if isinstance(image, Editor) or isinstance(image, Canvas):
             image = image.image
 
         blank.paste(image, position)
-        self.image = Image.alpha_composite(self.image, blank)
+        self.image = PilImage.alpha_composite(self.image, blank)
 
         return self
 
     def text(
         self,
         position: Tuple[float, float],
         text: str,
-        font: Union[ImageFont.FreeTypeFont, Font] = None,
+        font: Optional[Union[ImageFont.FreeTypeFont, Font]] = None,
         color: Color = "black",
         align: Literal["left", "center", "right"] = "left",
-        stroke_width: int = None,
+        stroke_width: Optional[int] = None,
         stroke_fill: Color = "black",
     ) -> Editor:
         """Draw text into image
 
         Parameters
         ----------
         position : Tuple[float, float]
-            Position to draw text
+            Position to draw text.
         text : str
             Text to draw
         font : Union[ImageFont.FreeTypeFont, Font], optional
             Font used for text, by default None
         color : Color, optional
             Color of the font, by default "black"
         align : Literal["left", "center", "right"], optional
@@ -333,26 +337,26 @@
         return self
 
     def rectangle(
         self,
         position: Tuple[float, float],
         width: float,
         height: float,
-        fill: Color = None,
-        color: Color = None,
-        outline: Color = None,
+        fill: Optional[Color] = None,
+        color: Optional[Color] = None,
+        outline: Optional[Color] = None,
         stroke_width: float = 1,
         radius: int = 0,
     ) -> Editor:
         """Draw rectangle into image
 
         Parameters
         ----------
         position : Tuple[float, float]
-            Position to draw recangle
+            Position to draw rectangle
         width : float
             Width of rectangle
         height : float
             Height of rectangle
         fill : Color, optional
             Fill color, by default None
         color : Color, optional
@@ -392,32 +396,32 @@
 
     def bar(
         self,
         position: Tuple[float, float],
         max_width: Union[int, float],
         height: Union[int, float],
         percentage: int = 1,
-        fill: Color = None,
-        color: Color = None,
-        outline: Color = None,
+        fill: Optional[Color] = None,
+        color: Optional[Color] = None,
+        outline: Optional[Color] = None,
         stroke_width: float = 1,
         radius: int = 0,
     ) -> Editor:
         """Draw a progress bar
 
         Parameters
         ----------
         position : Tuple[float, float]
             Position to draw bar
         max_width : Union[int, float]
             Max width of the bar
         height : Union[int, float]
             Height of the bar
         percentage : int, optional
-            Percebtage to fill of the bar, by default 1
+            Percentage to fill of the bar, by default 1
         fill : Color, optional
             Fill color, by default None
         color : Color, optional
             Alias of fill, by default None
         outline : Color, optional
             Outline color, by default None
         stroke_width : float, optional
@@ -455,30 +459,30 @@
 
     def rounded_bar(
         self,
         position: Tuple[float, float],
         width: Union[int, float],
         height: Union[int, float],
         percentage: float,
-        fill: Color = None,
-        color: Color = None,
+        fill: Optional[Color] = None,
+        color: Optional[Color] = None,
         stroke_width: float = 1,
     ) -> Editor:
         """Draw a rounded bar
 
         Parameters
         ----------
         position : Tuple[float, float]
             Position to draw rounded bar
         width : Union[int, float]
             Width of the bar
         height : Union[int, float]
             Height of the bar
         percentage : float
-            Percentage to fill
+            Percentage to fill.
         fill : Color, optional
             Fill color, by default None
         color : Color, optional
             Alias of color, by default None
         stroke_width : float, optional
             Stroke width, by default 1
         """
@@ -501,17 +505,17 @@
         return self
 
     def ellipse(
         self,
         position: Tuple[float, float],
         width: float,
         height: float,
-        fill: Color = None,
-        color: Color = None,
-        outline: Color = None,
+        fill: Optional[Color] = None,
+        color: Optional[Color] = None,
+        outline: Optional[Color] = None,
         stroke_width: float = 1,
     ) -> Editor:
         """Draw an ellipse
 
         Parameters
         ----------
         position : Tuple[float, float]
@@ -543,49 +547,49 @@
             width=stroke_width,
         )
 
         return self
 
     def polygon(
         self,
-        cordinates: list,
-        fill: Color = None,
-        color: Color = None,
-        outline: Color = None,
+        coordinates: list,
+        fill: Optional[Color] = None,
+        color: Optional[Color] = None,
+        outline: Optional[Color] = None,
     ) -> Editor:
         """Draw a polygon
 
         Parameters
         ----------
-        cordinates : list
-            Cordinates to draw
+        coordinates : list
+            Coordinates to draw
         fill : Color, optional
             Fill color, by default None
         color : Color, optional
             Alias of fill, by default None
         outline : Color, optional
             Outline color, by default None
         """
         if color:
             fill = color
 
         draw = ImageDraw.Draw(self.image)
-        draw.polygon(cordinates, fill=fill, outline=outline)
+        draw.polygon(coordinates, fill=fill, outline=outline)
 
         return self
 
     def arc(
         self,
         position: Tuple[float, float],
         width: float,
         height: float,
         start: float,
         rotation: float,
-        fill: Color = None,
-        color: Color = None,
+        fill: Optional[Color] = None,
+        color: Optional[Color] = None,
         stroke_width: float = 1,
     ) -> Editor:
         """Draw arc
 
         Parameters
         ----------
         position : Tuple[float, float]
@@ -593,15 +597,15 @@
         width : float
             Width or arc
         height : float
             Height of arch
         start : float
             Start position of arch
         rotation : float
-            Rotation in degre
+            Rotation in degree
         fill : Color, optional
             Fill color, by default None
         color : Color, optional
             Alias of fill, by default None
         stroke_width : float, optional
             Stroke width, by default 1
         """
@@ -623,18 +627,18 @@
 
         return self
 
     def show(self):
         """Show the image."""
         self.image.show()
 
-    def save(self, fp, format: str = None, **params):
+    def save(self, fp, file_format: Optional[str] = None, **params):
         """Save the image
 
         Parameters
         ----------
         fp : str
             File path
-        format : str, optional
+        file_format : str, optional
             File format, by default None
         """
-        self.image.save(fp, format, **params)
+        self.image.save(fp, file_format, **params)
```

### Comparing `easy-pil-0.2.3/easy_pil/font.py` & `easy_pil-0.2.4/easy_pil/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def __init__(self, path: str, size: int = 10, **kwargs) -> None:
         self.font = ImageFont.truetype(path, size=size, **kwargs)
 
     def getsize(self, text: str):
         return self.font.getsize(text)
 
     @staticmethod
-    @lru_cache()
+    @lru_cache(32)
     def poppins(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Poppins font
 
         Parameters
@@ -72,15 +72,15 @@
             Font variant, by default "regular"
         size : int, optional
             Font size, by default 10
         """
         return ImageFont.truetype(fonts_path["poppins"][variant], size=size)
 
     @staticmethod
-    @lru_cache()
+    @lru_cache(32)
     def caveat(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Caveat font
 
         Parameters
@@ -89,15 +89,15 @@
             Font variant, by default "regular"
         size : int, optional
             Font size, by default 10
         """
         return ImageFont.truetype(fonts_path["caveat"][variant], size=size)
 
     @staticmethod
-    @lru_cache()
+    @lru_cache(32)
     def montserrat(
         variant: Literal["regular", "bold", "italic", "light"] = "regular",
         size: int = 10,
     ):
         """Montserrat font
 
         Parameters
```

### Comparing `easy-pil-0.2.3/easy_pil/fonts/caveat/caveat.ttf` & `easy_pil-0.2.4/easy_pil/fonts/caveat/caveat.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_bold.ttf` & `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_italic.ttf` & `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_light.ttf` & `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/montserrat/montserrat_regular.ttf` & `easy_pil-0.2.4/easy_pil/fonts/montserrat/montserrat_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_bold.ttf` & `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_italic.ttf` & `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_light.ttf` & `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/fonts/poppins/poppins_regular.ttf` & `easy_pil-0.2.4/easy_pil/fonts/poppins/poppins_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/text.py` & `easy_pil-0.2.4/easy_pil/text.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/utils.py` & `easy_pil-0.2.4/easy_pil/utils.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.3/easy_pil/workspace.py` & `easy_pil-0.2.4/easy_pil/workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .types.common import Color
 from .types.workspace import ComponentKwargs
 
 
 class Workspace:
     """Workspace class for working with layers and components"""
 
-    def __init__(self, size: Tuple[float, float]) -> None:
+    def __init__(self, size: Tuple[int, int]) -> None:
         self.size = size
         self.layers: dict = dict()
         self.working_layer = None
 
     def create_layer(self, name: str, background: Color = (0, 0, 0, 0)):
         """Creates a layer
 
@@ -101,16 +101,16 @@
 
     def __get_random_identifier(self) -> str:
         return "".join(random.choices(string.ascii_letters, k=5))
 
     def add_component(
         self,
         *,
-        layer_name: str = None,
-        identifier: str = None,
+        layer_name: Optional[str] = None,
+        identifier: Optional[str] = None,
         func: Union[Callable, str],
         options: ComponentKwargs
     ):
         """Add component to a layer
 
         Parameters
         ----------
@@ -144,15 +144,17 @@
         )
 
         self.layers[layer_name]["components"][identifier_name] = {
             "func_name": func_name,
             "options": options,
         }
 
-    def remove_component(self, *, layer_name: str = None, identifier: str):
+    def remove_component(
+        self, *, layer_name: Optional[str] = None, identifier: str
+    ):
         """Remove component from a layer
 
         Parameters
         ----------
         layer_name : str
             name of the layer
         identifier : str
@@ -175,15 +177,15 @@
             self.layers[layer_name]["components"].pop(identifier)
         except KeyError:
             raise ValueError("Invalid layer name or identifier")
 
     def update_component(
         self,
         *,
-        layer_name: str = None,
+        layer_name: Optional[str] = None,
         identifier: str,
         options: ComponentKwargs
     ):
         """Update component of a layer
 
         Parameters
         ----------
@@ -210,15 +212,15 @@
             raise ValueError("Invalid layer name")
 
         self.layers[layer_name]["components"][identifier]["options"].update(
             options
         )
 
     def __create_editor_layer(
-        self, size: Tuple[float, float], metadata: Dict[str, Any]
+        self, size: Tuple[int, int], metadata: Dict[str, Any]
     ):
         return Editor(Canvas(size, color=metadata["background"]))
 
     def generate_image(self) -> Editor:
         """Generates image from the layers
 
         Returns
```


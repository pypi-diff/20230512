# Comparing `tmp/kandinsky-2.4.dev1.tar.gz` & `tmp/kandinsky-2.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kandinsky-2.4.dev1.tar", last modified: Wed Mar 29 20:16:41 2023, max compression
+gzip compressed data, was "kandinsky-2.5.dev1.tar", last modified: Fri May 12 14:10:09 2023, max compression
```

## Comparing `kandinsky-2.4.dev1.tar` & `kandinsky-2.5.dev1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.895275 kandinsky-2.4.dev1/
--rw-rw-rw-   0        0        0     1590 2022-08-29 17:59:39.000000 kandinsky-2.4.dev1/FAQ.md
--rw-rw-rw-   0        0        0      662 2023-03-29 20:16:41.894276 kandinsky-2.4.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     6127 2023-03-29 20:16:25.000000 kandinsky-2.4.dev1/README.md
--rw-rw-rw-   0        0        0      201 2023-03-29 20:16:20.000000 kandinsky-2.4.dev1/changelog.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 20:16:41.895275 kandinsky-2.4.dev1/setup.cfg
--rw-rw-rw-   0        0        0      873 2023-03-29 20:16:25.000000 kandinsky-2.4.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.742275 kandinsky-2.4.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.789273 kandinsky-2.4.dev1/src/kandinsky/
--rw-rw-rw-   0        0        0     1580 2023-03-28 18:10:13.000000 kandinsky-2.4.dev1/src/kandinsky/FAQ.md
--rw-rw-rw-   0        0        0     6127 2023-03-29 14:42:12.000000 kandinsky-2.4.dev1/src/kandinsky/README.md
--rw-rw-rw-   0        0        0     4800 2023-03-29 20:16:25.000000 kandinsky-2.4.dev1/src/kandinsky/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-03-27 18:31:44.000000 kandinsky-2.4.dev1/src/kandinsky/__init__.pyi
--rw-rw-rw-   0        0        0      244 2023-03-29 16:11:12.000000 kandinsky-2.4.dev1/src/kandinsky/__main__.py
--rw-rw-rw-   0        0        0     9770 2023-03-29 19:18:09.000000 kandinsky-2.4.dev1/src/kandinsky/test.py
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.826275 kandinsky-2.4.dev1/src/kandinsky/util/
--rw-rw-rw-   0        0        0    12479 2023-03-29 19:22:10.000000 kandinsky-2.4.dev1/src/kandinsky/util/core.py
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.864278 kandinsky-2.4.dev1/src/kandinsky/util/data/
--rw-rw-rw-   0        0        0     4286 2022-11-03 16:32:20.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/app.ico
--rw-rw-rw-   0        0        0     1544 2023-03-08 20:36:09.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/app.png
--rw-rw-rw-   0        0        0      146 2023-03-28 16:47:34.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/battery0.png
--rw-rw-rw-   0        0        0      159 2023-03-28 16:50:51.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/battery1.png
--rw-rw-rw-   0        0        0   226352 2022-08-25 19:34:57.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/large_font.ttf
--rw-rw-rw-   0        0        0     5805 2023-03-27 21:29:01.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/old_icons.zip
--rw-rw-rw-   0        0        0   220448 2023-03-27 20:37:08.000000 kandinsky-2.4.dev1/src/kandinsky/util/data/small_font.ttf
--rw-rw-rw-   0        0        0     4308 2023-03-14 17:37:19.000000 kandinsky-2.4.dev1/src/kandinsky/util/demo.py
--rw-rw-rw-   0        0        0     3470 2022-08-20 21:28:54.000000 kandinsky-2.4.dev1/src/kandinsky/util/old_config.ini
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.891276 kandinsky-2.4.dev1/src/kandinsky/util/stuff/
--rw-rw-rw-   0        0        0      104 2023-03-24 21:06:51.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-03-24 21:14:51.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/color.py
--rw-rw-rw-   0        0        0      985 2023-03-26 21:56:06.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/draw.py
--rw-rw-rw-   0        0        0     8743 2023-03-28 22:03:55.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/gui.py
--rw-rw-rw-   0        0        0     5426 2023-03-27 17:46:33.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/ion.py
--rw-rw-rw-   0        0        0      909 2023-03-24 21:13:27.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/tests.py
--rw-rw-rw-   0        0        0     3241 2023-03-27 21:59:05.000000 kandinsky-2.4.dev1/src/kandinsky/util/stuff/vars.py
-drwxrwxrwx   0        0        0        0 2023-03-29 20:16:41.814287 kandinsky-2.4.dev1/src/kandinsky.egg-info/
--rw-rw-rw-   0        0        0      662 2023-03-29 20:16:41.000000 kandinsky-2.4.dev1/src/kandinsky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      946 2023-03-29 20:16:41.000000 kandinsky-2.4.dev1/src/kandinsky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 20:16:41.000000 kandinsky-2.4.dev1/src/kandinsky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-29 20:16:41.000000 kandinsky-2.4.dev1/src/kandinsky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-29 20:16:41.000000 kandinsky-2.4.dev1/src/kandinsky.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.398222 kandinsky-2.5.dev1/
+-rw-rw-rw-   0        0        0     1590 2022-08-29 17:59:39.000000 kandinsky-2.5.dev1/FAQ.md
+-rw-rw-rw-   0        0        0      636 2023-05-12 14:10:09.394226 kandinsky-2.5.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     6299 2023-05-12 14:09:36.000000 kandinsky-2.5.dev1/README.md
+-rw-rw-rw-   0        0        0      781 2023-05-09 20:21:54.000000 kandinsky-2.5.dev1/changelog.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 14:10:09.398222 kandinsky-2.5.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-05-12 14:09:36.000000 kandinsky-2.5.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:08.890222 kandinsky-2.5.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.018221 kandinsky-2.5.dev1/src/kandinsky/
+-rw-rw-rw-   0        0        0     1580 2023-03-28 18:10:13.000000 kandinsky-2.5.dev1/src/kandinsky/FAQ.md
+-rw-rw-rw-   0        0        0     6299 2023-05-03 19:43:17.000000 kandinsky-2.5.dev1/src/kandinsky/README.md
+-rw-rw-rw-   0        0        0     4776 2023-05-12 14:09:36.000000 kandinsky-2.5.dev1/src/kandinsky/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-03-27 18:31:44.000000 kandinsky-2.5.dev1/src/kandinsky/__init__.pyi
+-rw-rw-rw-   0        0        0      244 2023-03-29 16:11:12.000000 kandinsky-2.5.dev1/src/kandinsky/__main__.py
+-rw-rw-rw-   0        0        0    10122 2023-05-11 21:04:09.000000 kandinsky-2.5.dev1/src/kandinsky/test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.150221 kandinsky-2.5.dev1/src/kandinsky/util/
+-rw-rw-rw-   0        0        0    12414 2023-05-11 21:08:44.000000 kandinsky-2.5.dev1/src/kandinsky/util/core.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.254223 kandinsky-2.5.dev1/src/kandinsky/util/data/
+-rw-rw-rw-   0        0        0     4286 2022-11-03 16:32:20.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/app.ico
+-rw-rw-rw-   0        0        0     1544 2023-03-08 20:36:09.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/app.png
+-rw-rw-rw-   0        0        0      146 2023-03-28 16:47:34.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/battery0.png
+-rw-rw-rw-   0        0        0      159 2023-04-04 18:53:23.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/battery1.png
+-rw-rw-rw-   0        0        0   226352 2022-08-25 19:34:57.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/large_font.ttf
+-rw-rw-rw-   0        0        0     5805 2023-03-27 21:29:01.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/old_icons.zip
+-rw-rw-rw-   0        0        0   220448 2023-03-27 20:37:08.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/small_font.ttf
+-rw-rw-rw-   0        0        0     4308 2023-03-14 17:37:19.000000 kandinsky-2.5.dev1/src/kandinsky/util/demo.py
+-rw-rw-rw-   0        0        0     3470 2022-08-20 21:28:54.000000 kandinsky-2.5.dev1/src/kandinsky/util/old_config.ini
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.390222 kandinsky-2.5.dev1/src/kandinsky/util/stuff/
+-rw-rw-rw-   0        0        0      128 2023-05-03 14:32:56.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/__init__.py
+-rw-rw-rw-   0        0        0     2310 2023-04-28 14:04:16.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/color.py
+-rw-rw-rw-   0        0        0     1506 2023-05-10 19:04:23.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/draw.py
+-rw-rw-rw-   0        0        0    13161 2023-05-11 18:13:37.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/gui.py
+-rw-rw-rw-   0        0        0     5426 2023-03-27 17:46:33.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/ion.py
+-rw-rw-rw-   0        0        0     5214 2023-05-03 19:28:19.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/limiter.py
+-rw-rw-rw-   0        0        0      909 2023-03-30 11:58:23.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/tests.py
+-rw-rw-rw-   0        0        0     3472 2023-05-10 18:06:53.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/vars.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.070222 kandinsky-2.5.dev1/src/kandinsky.egg-info/
+-rw-rw-rw-   0        0        0      636 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/top_level.txt
```

### Comparing `kandinsky-2.4.dev1/FAQ.md` & `kandinsky-2.5.dev1/FAQ.md`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/README.md` & `kandinsky-2.5.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,34 +100,45 @@
 
 #### Environ options
 **/!\\ You must make its additions *before* importing kandinsky otherwise the changes will not take effect! /!\\**
 
 You can also change some default option of library, like the OS or model on which to start kandinsky, etc. <br> 
 To do this, first import the environ of os module like this: ``import os``.
 
-* To enable debug mode, add:
+* Enable debug mode:
 ```python
 os.environ['KANDINSKY_ENABLE_DEBUG'] = '' 
 ```
 
-* To change starting OS (methods according to the selected os will be created), add:
+* Change starting OS (methods according to the selected os will be created):
 ```python
 # '0': PC speed + Upsilon methods
 # '1': Numworks speed + Basic methods
 # '2': Omega speed + draw_line,wait_vblank,get_keys method
 # '3': Upsilon speed + draw_circle,fill_circle,fill_polygon,get_palette methods - get_keys
 os.environ['KANDINSKY_OS_MODE'] = '<number>'
 ```
 
-* To change starting Model, add:
+* Change starting Model:
 ```python
 # '0': n0100 model speed (not available for moment)
 # '1': n0110 model speed
 # '2': n0120 model speed (not available for moment)
 os.environ['KANDINSKY_MODEL_MODE'] = '<number>'
 ```
 
-* To disable user interface (menu at top of window), add:
+* Disable user interface (menu at top of window):
 ```python
 # Note: Shortcut commands are not disabled
 os.environ['KANDINSKY_NO_GUI'] = ''
 ```
+
+* Change size of screen:
+```python
+os.environ['KANDINSKY_SCREEN_SIZE'] = "<width>x<height>"
+```
+
+* Zoom the screen:
+```python
+# from 1 to 4
+os.environ['KANDINSKY_ZOOM_RATIO'] = "<number>"
+```
```

### Comparing `kandinsky-2.4.dev1/setup.py` & `kandinsky-2.5.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 # AUTO GENERATED FILE. DO NOT EDIT!
 from setuptools import setup 
-setup(**{'name': 'kandinsky', 'version': '2.4.dev1', 'author': 'ZetaMap', 'description': 'A small module allowing to link the kandinsky module, from the Numworks, to a window.', 'license': 'MIT', 'long_description': '', 'long_description_content_type': 'text/markdown', 'url': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'project_urls': {'GitHub Project': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'My GitHub Page': 'https://github.com/ZetaMap/'}, 'classifiers': ['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License', 'Operating System :: Microsoft :: Windows', 'Operating System :: Unix', 'Operating System :: MacOS :: MacOS X'], 'package_dir': {'': 'src'}, 'include_dirs': ['kandinsky'], 'install_requires': ['pysdl2', 'pysdl2-dll'], 'include_package_data': True})
+setup(**{'name': 'kandinsky', 'version': '2.5.dev1', 'author': 'ZetaMap', 'description': 'A small module allowing to link the kandinsky module, from the Numworks, to a window.', 'license': 'MIT', 'long_description': '', 'long_description_content_type': 'text/markdown', 'url': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'project_urls': {'GitHub Project': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'My GitHub Page': 'https://github.com/ZetaMap/'}, 'classifiers': ['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License', 'Operating System :: Microsoft :: Windows', 'Operating System :: Unix'], 'package_dir': {'': 'src'}, 'include_dirs': ['kandinsky'], 'install_requires': ['pysdl2', 'pysdl2-dll'], 'include_package_data': True, 'python_requires': '>=3.6'})
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/FAQ.md` & `kandinsky-2.5.dev1/src/kandinsky/FAQ.md`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/README.md` & `kandinsky-2.5.dev1/src/kandinsky/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,34 +100,45 @@
 
 #### Environ options
 **/!\\ You must make its additions *before* importing kandinsky otherwise the changes will not take effect! /!\\**
 
 You can also change some default option of library, like the OS or model on which to start kandinsky, etc. <br> 
 To do this, first import the environ of os module like this: ``import os``.
 
-* To enable debug mode, add:
+* Enable debug mode:
 ```python
 os.environ['KANDINSKY_ENABLE_DEBUG'] = '' 
 ```
 
-* To change starting OS (methods according to the selected os will be created), add:
+* Change starting OS (methods according to the selected os will be created):
 ```python
 # '0': PC speed + Upsilon methods
 # '1': Numworks speed + Basic methods
 # '2': Omega speed + draw_line,wait_vblank,get_keys method
 # '3': Upsilon speed + draw_circle,fill_circle,fill_polygon,get_palette methods - get_keys
 os.environ['KANDINSKY_OS_MODE'] = '<number>'
 ```
 
-* To change starting Model, add:
+* Change starting Model:
 ```python
 # '0': n0100 model speed (not available for moment)
 # '1': n0110 model speed
 # '2': n0120 model speed (not available for moment)
 os.environ['KANDINSKY_MODEL_MODE'] = '<number>'
 ```
 
-* To disable user interface (menu at top of window), add:
+* Disable user interface (menu at top of window):
 ```python
 # Note: Shortcut commands are not disabled
 os.environ['KANDINSKY_NO_GUI'] = ''
 ```
+
+* Change size of screen:
+```python
+os.environ['KANDINSKY_SCREEN_SIZE'] = "<width>x<height>"
+```
+
+* Zoom the screen:
+```python
+# from 1 to 4
+os.environ['KANDINSKY_ZOOM_RATIO'] = "<number>"
+```
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/__init__.py` & `kandinsky-2.5.dev1/src/kandinsky/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """A small module allowing to link the kandinsky module, from the Numworks, to a Windows window. 
 Useful if you want to test your program without putting it on the calculator.
 The [GitHub project](https://github.com/ZetaMap/Kandinsky-Numworks), and if you have any questions, check out the [FAQ](https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/FAQ.md)
 In addition, this module also emulates the drawing speed, and has [many other features](https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/README.md#additional-features).
 """
 
-try: from .util.core import DEFAULT_OS, Core as __Core
-except ImportError: from util.core import DEFAULT_OS, Core as __Core
+try: from .util.core import Core as __Core
+except ImportError as e:
+  if "relative import" not in e.msg: 
+    raise
+  from util.core import Core as __Core
 
 __name__ = "kandinsky"
-__version__ = "2.4.dev1"
+__version__ = "2.5.dev1"
 try: __doc__ = open("README.md").read()
 except (FileNotFoundError, OSError): __doc__ = "<unknown>"
 __all__ = [ 
   #numworks 
   "get_pixel", 
   "set_pixel", 
   "color", 
@@ -32,16 +35,14 @@
   #upsilon
   "draw_circle",
   "fill_circle",
   "fill_polygon",
   "get_palette"
 ]
 __Core = __Core()
-try: OS_MODE = __Core.OS_MODE
-except AttributeError: OS_MODE = DEFAULT_OS
 
 
 # Numworks basic methods
 def get_pixel(x, y, /):
   """Return pixel (x, y) color"""
   pixel, err = __Core.event_fire(__Core.get_pixel, x, y)
   if err != None:
@@ -58,15 +59,15 @@
   """Define a rgb color"""
   color, err = __Core.event_fire(__Core.color,r, g, b)
   if err != None:
     raise err
   return color
 
 # Argument added by Omega
-if OS_MODE > 1:
+if __Core.OS_MODE > 1:
   def draw_string(text, x, y, color=(0,0,0), background=(248,252,248), font=False, /):
     """Display a text from pixel (x, y)"""
     _, err = __Core.event_fire(__Core.draw_string, text, x, y, color, background, font)
     if err != None:
       raise err  
 else :
   def draw_string(text, x, y, color=(0,0,0), background=(248,252,248), /):
@@ -137,31 +138,29 @@
   if err != None:
     raise err
   return pal
 
 
 ######### Clean #########
 # delete methods according to OS
-if OS_MODE: 
+# in pc mode, do not delete anything
+if __Core.OS_MODE: 
   # upsilon moved this method and epsilon don't have this
-  if OS_MODE != 2:
+  if __Core.OS_MODE != 2:
     __all__.remove("get_keys")
     del get_keys
 
   # delete upsilon methods
-  if OS_MODE < 3: 
+  if __Core.OS_MODE < 3: 
     __all__.remove("draw_circle")
     __all__.remove("fill_circle")
     __all__.remove("fill_polygon")
     __all__.remove("get_palette")
     del draw_circle, fill_circle,  fill_polygon, get_palette
  
   # delete omega methods
-  if OS_MODE < 2: 
+  if __Core.OS_MODE < 2: 
     __all__.remove("draw_line")
     __all__.remove("wait_vblank")
     __all__.remove("small_font")
     __all__.remove("large_font")
     del draw_line, wait_vblank, small_font, large_font
-        
-# Cleanup namespaces
-del OS_MODE, DEFAULT_OS
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/__init__.pyi` & `kandinsky-2.5.dev1/src/kandinsky/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/test.py` & `kandinsky-2.5.dev1/src/kandinsky/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,159 +1,167 @@
-import os
-#os.environ["KANDINSKY_ENABLE_DEBUG"]=''
-os.environ["KANDINSKY_OS_MODE"]="3"
-from math import *
-from __init__ import *
-from time import *
- 
-def draw(index, loop, clear):
-  if clear: fill_rect(0, 0, 350, 250, (255,255,255))
-  draw_string(str(1+(len(_list)+index if index < 0 else index)), 5, 5, (100,100,100))
-  draw_string("<", 219, 200, (100,100,100))
-  fill_rect(220, 215, 15, 1, (100,100,100))
-  fill_rect(235, 216, 1, -7, (100,100,100))
-  fill_rect(236, 208, -15, 1, (100,100,100))
-  draw_string("to skip", 245, 202, (100,100,100))
-  exec("""for p in range({}):
-    for i in range(496): 
-      try: set_pixel(160+round({}), 110+round({}), {})
-      except (OverflowError, ZeroDivisionError, ValueError):
-        continue
-      except KeyboardInterrupt: raise RuntimeError
-      except: raise
-  """.format(loop, _list[index][0], _list[index][1],
-    "(cos(p)*1000, sin(i)*1000, log10(i-p)*1000)" \
-      if _list[index][2] == True else "(0, 0, 0)"))
-
-def start():
-  x, loop = input("""{} equations found in the list.
-Let empty to run all.
-|-> """.format(len(_list))), input("""
-Let empty for default value.
-Loop: """)
-  loop = 400 if loop == '' else int(loop)
-  r = range(len(_list)) if x == '' else range(int(x)-1, int(x))
-
-  for ii in r:
-    time = monotonic()
-    try: draw(ii, loop, 1)
-    except (SyntaxError, IndexError): raise
-    except:
-      try: draw(ii, 1, 0)
-      except: pass
-    print("Drawn", ii+1, "in", int(monotonic()-time), "s")
-  draw_string("End", 5, 5, (100,100,100))
-     
-_list=[
-#           for x         |           for y           | color?
-  ("cos(i)*111/(cos(p)+1)", "sin(i)*111/(sin(p)+1)"   , 1), #1
-  ("cos(i)*111+p"         , "sin(i)*111+p"            , 1), #2
-  ("cos(i)*111/(tan(p)+1)", "sin(i)*111/(sin(p)+1)"   , 1), #3
-  ("cos(i)*111/(tan(p)+1)", "tan(i)*111/(sin(p))"     , 1), #4
-  ("cos(i)*111/(1-cos(p)+1)", "sin(i)*111/(-sin(p)+1)", 1), #5
-  ("cos(i)*111/(cos(p)+1)", "sin(i)/(sin(p)+1)"       , 1), #6
-  ("cos(i)*111/(cos(p)+1)", "sin(i)*111/cos(p)**2"    , 1), #7
-  ("cos(i)*111/(cos(p)+1)", "sin(i)*111/(cos(p)**2+1)", 1), #8
-  ("cos(i)*111/(cos(p)+1)", "sin(i)*130/(tan(tan(p)))", 1), #9
-  ("tan(tan(i))*111/sin(p)", "tan(i)*111/cos(sin(p))" , 1), #10
-  ("cos(i)*p"             , "sin(i)*p"                , 1), #11
-  ("tan(tan(i))*p"        , "sin(i)*p"                , 1), #12  
-  ("cos(p)*i"             , "tan(p)*i"                , 0), #13
-  ("tan(tan(tan(i)))/tan(p)", "tan(i)*p/sin(p)"       , 1), #14
-  ("cos(tan(i))*p"        , "cos(i)*p"                , 1), #15
-  ("sin(i)*p*cos(sin(i))" , "sin(p)*111/cos(tan(i))"  , 1), #16
-  ("cos(p)*i*tan(cos(p))-111", "cos(i)*p/tan(i)"      , 1), #17
-  ("sin(cos(tan(p)))*i"   , "tan(i)*p"                , 1), #18
-  ("exp(abs(log(p)))*sin(i)", "log(p)/cos(i)*10"      , 1), #19
-  ("exp(abs(log(p,i)))*64*sin(i)", "log(p)/cos(i)*5"  , 1), #20
-  ("exp(abs(log(p)))*sin(i)", "sin(i)*50/sin(p)"      , 1), #21
-  ("cos(p)*50/(sin(i)+1)" , "abs(p)/cos(i)"           , 1), #22
-  ("asinh(p)/cos(i)"      , "cos(p)*111*sin(i)"       , 1), #23
-  ("acosh(p)*111/(tan(i)+1)", "cos(p)*150/asinh(i)"   , 1), #24
-  ("trunc(i)/cos(p)"      , "acosh(i)/-sin(p)"        , 0), #25
-  ("cos(i)*50/(tan(p)+1)" , "acosh(i)*5/-tan(p)"      , 1), #26
-  ("cos(i)*50/(tan(p)+1)" , "sin(i)*50/(cos(p))"      , 1), #27
-]
-
-start()
-
-exit()
-
-import os
-os.environ["KANDINSKY_OS_MODE"]="3"
-import __init__ as kandinsky
-from ion import keydown
-from time import perf_counter_ns
-from math import cos, sin, log10
-
-def wait_key():
-  while True:
-    for i in range(53):
-      if keydown(i):
-        while keydown(i): pass
-        return i
-
-def test(method, *args):
-  func = getattr(kandinsky, method)
-  values = []
-  for i in range(300):
-    time_is = perf_counter_ns()
-    func(*args)
-    values.append((perf_counter_ns()-time_is)/1000)
-    kandinsky.fill_rect(0, 0, 320, 220, "white")
-
-  #print(values)
-  print(method, "speed:", sum(values)/len(values), "µs; min:", min(values), "max:", max(values))
-
-kandinsky.draw_string("Welcome to kandinsky speed test program", 5, 50)
-kandinsky.draw_string("Press a key to start test ...", 15, 70)
-wait_key()
-kandinsky.fill_rect(0, 0, 320, 220, "white")
-
-test("set_pixel", 10, 10, "black")
-print("100*100: ", end='')
-test("fill_rect", 10, 10, 100, 100, "black")
-print("1*1: ", end='')
-test("fill_rect", 10, 10, 1, 1, "black")
-print("200*200: ", end='')
-test("fill_rect", 10, 10, 200, 200, "black")
-test("draw_string", "test string", 10, 10)
-print("100*100: ", end='')
-test("draw_circle", 110, 110, 100, "black")
-print("10*10: ", end='')
-test("draw_circle", 110, 110, 10, "black")
-print("100*100: ", end='')
-test("fill_circle", 110, 110, 100, "black")
-print("10*10: ", end='')
-test("fill_circle", 110, 110, 10, "black")
-for i in range(300): kandinsky.set_pixel(10+i, 10, (cos(i)*1000, sin(i)*1000, log10(i+1)*1000))
-values = []
-for i in range(300):
-  time_is = perf_counter_ns()
-  kandinsky.get_pixel(10+i, 10)
-  values.append((perf_counter_ns()-time_is)/1000)
-print("get_pixel speed:", sum(values)/len(values), "µs")
-for i in range(300):
-  time_is = perf_counter_ns()
-  kandinsky.color((cos(i)*1000, sin(i)*1000, log10(i+1)*1000))
-  values.append((perf_counter_ns()-time_is)/1000)
-print("color speed:", sum(values)/len(values), "µs")
-input(">>> ")
-
-exit()
+#import os
+##os.environ["KANDINSKY_ENABLE_DEBUG"]=''
+##os.environ["KANDINSKY_OS_MODE"]='4'
+##os.environ['KANDINSKY_SCREEN_SIZE'] = '520x240'
+#os.environ['KANDINSKY_ZOOM_RATIO'] = '2'
+#
+#from math import *
+#from __init__ import *
+#from time import *
+#
+##get_keys()
+#def draw(index, loop, clear):
+#  if clear: fill_rect(0, 0, 350, 250, (255,255,255))
+#  draw_string(str(1+(len(_list)+index if index < 0 else index)), 5, 5, (100,100,100))
+#  draw_string("<", 219, 200, (100,100,100))
+#  fill_rect(220, 215, 15, 1, (100,100,100))
+#  fill_rect(235, 216, 1, -7, (100,100,100))
+#  fill_rect(236, 208, -15, 1, (100,100,100))
+#
+#  draw_string("to skip", 245, 202, (100,100,100))
+#  exec("""for p in range({}):
+#    for i in range(496): 
+#      try: set_pixel(160+round({}), 110+round({}), {})
+#      except (OverflowError, ZeroDivisionError, ValueError):
+#        continue
+#      except KeyboardInterrupt: raise RuntimeError
+#      except: raise
+#  """.format(loop, _list[index][0], _list[index][1],
+#    "(cos(p)*1000, sin(i)*1000, log10(i-p)*1000)" \
+#      if _list[index][2] == True else "(0, 0, 0)"))
+#
+#def start():
+#  x, loop = input("""{} equations found in the list.
+#Let empty to run all.
+#|-> """.format(len(_list))), input("""
+#Let empty for default value.
+#Loop: """)
+#  loop = 400 if loop == '' else int(loop)
+#  r = range(len(_list)) if x == '' else range(int(x)-1, int(x))
+#
+#  for ii in r:
+#    time = monotonic()
+#    try: draw(ii, loop, 1)
+#    except (SyntaxError, IndexError): raise
+#    except:
+#      try: draw(ii, 1, 0)
+#      except: pass
+#    print("Drawn", ii+1, "in", int(monotonic()-time), "s")
+#  draw_string("End", 5, 5, (100,100,100))
+#     
+#_list=[
+##           for x         |           for y           | color?
+#  ("cos(i)*111/(cos(p)+1)", "sin(i)*111/(sin(p)+1)"   , 1), #1
+#  ("cos(i)*111+p"         , "sin(i)*111+p"            , 1), #2
+#  ("cos(i)*111/(tan(p)+1)", "sin(i)*111/(sin(p)+1)"   , 1), #3
+#  ("cos(i)*111/(tan(p)+1)", "tan(i)*111/(sin(p))"     , 1), #4
+#  ("cos(i)*111/(1-cos(p)+1)", "sin(i)*111/(-sin(p)+1)", 1), #5
+#  ("cos(i)*111/(cos(p)+1)", "sin(i)/(sin(p)+1)"       , 1), #6
+#  ("cos(i)*111/(cos(p)+1)", "sin(i)*111/cos(p)**2"    , 1), #7
+#  ("cos(i)*111/(cos(p)+1)", "sin(i)*111/(cos(p)**2+1)", 1), #8
+#  ("cos(i)*111/(cos(p)+1)", "sin(i)*130/(tan(tan(p)))", 1), #9
+#  ("tan(tan(i))*111/sin(p)", "tan(i)*111/cos(sin(p))" , 1), #10
+#  ("cos(i)*p"             , "sin(i)*p"                , 1), #11
+#  ("tan(tan(i))*p"        , "sin(i)*p"                , 1), #12  
+#  ("cos(p)*i"             , "tan(p)*i"                , 0), #13
+#  ("tan(tan(tan(i)))/tan(p)", "tan(i)*p/sin(p)"       , 1), #14
+#  ("cos(tan(i))*p"        , "cos(i)*p"                , 1), #15
+#  ("sin(i)*p*cos(sin(i))" , "sin(p)*111/cos(tan(i))"  , 1), #16
+#  ("cos(p)*i*tan(cos(p))-111", "cos(i)*p/tan(i)"      , 1), #17
+#  ("sin(cos(tan(p)))*i"   , "tan(i)*p"                , 1), #18
+#  ("exp(abs(log(p)))*sin(i)", "log(p)/cos(i)*10"      , 1), #19
+#  ("exp(abs(log(p,i)))*64*sin(i)", "log(p)/cos(i)*5"  , 1), #20
+#  ("exp(abs(log(p)))*sin(i)", "sin(i)*50/sin(p)"      , 1), #21
+#  ("cos(p)*50/(sin(i)+1)" , "abs(p)/cos(i)"           , 1), #22
+#  ("asinh(p)/cos(i)"      , "cos(p)*111*sin(i)"       , 1), #23
+#  ("acosh(p)*111/(tan(i)+1)", "cos(p)*150/asinh(i)"   , 1), #24
+#  ("trunc(i)/cos(p)"      , "acosh(i)/-sin(p)"        , 0), #25
+#  ("cos(i)*50/(tan(p)+1)" , "acosh(i)*5/-tan(p)"      , 1), #26
+#  ("cos(i)*50/(tan(p)+1)" , "sin(i)*50/(cos(p))"      , 1), #27
+#]
+#
+#start()
+#
+#exit()
+#
+#import os
+#os.environ["KANDINSKY_OS_MODE"]="3"
+#import __init__ as kandinsky
+#from ion import keydown
+#from time import perf_counter_ns
+#from math import cos, sin, log10
+#
+#def wait_key():
+#  while True:
+#    for i in range(53):
+#      if keydown(i):
+#        while keydown(i): pass
+#        return i
+#
+#def test(method, *args):
+#  func = getattr(kandinsky, method)
+#  values = []
+#  for i in range(300):
+#    time_is = perf_counter_ns()
+#    func(*args)
+#    values.append((perf_counter_ns()-time_is)/1000)
+#    kandinsky.fill_rect(0, 0, 320, 220, "white")
+#
+#  #print(values)
+#  print(method, "speed:", sum(values)/len(values), "µs; min:", min(values), "max:", max(values))
+#
+#kandinsky.draw_string("Welcome to kandinsky speed test program", 5, 50)
+#kandinsky.draw_string("Press a key to start test ...", 15, 70)
+#wait_key()
+#kandinsky.fill_rect(0, 0, 320, 220, "white")
+#
+#test("set_pixel", 10, 10, "black")
+#print("100*100: ", end='')
+#test("fill_rect", 10, 10, 100, 100, "black")
+#print("1*1: ", end='')
+#test("fill_rect", 10, 10, 1, 1, "black")
+#print("200*200: ", end='')
+#test("fill_rect", 10, 10, 200, 200, "black")
+#test("draw_string", "test string", 10, 10)
+#print("100*100: ", end='')
+#test("draw_circle", 110, 110, 100, "black")
+#print("10*10: ", end='')
+#test("draw_circle", 110, 110, 10, "black")
+#print("100*100: ", end='')
+#test("fill_circle", 110, 110, 100, "black")
+#print("10*10: ", end='')
+#test("fill_circle", 110, 110, 10, "black")
+#for i in range(300): kandinsky.set_pixel(10+i, 10, (cos(i)*1000, sin(i)*1000, log10(i+1)*1000))
+#values = []
+#for i in range(300):
+#  time_is = perf_counter_ns()
+#  kandinsky.get_pixel(10+i, 10)
+#  values.append((perf_counter_ns()-time_is)/1000)
+#print("get_pixel speed:", sum(values)/len(values), "µs")
+#for i in range(300):
+#  time_is = perf_counter_ns()
+#  kandinsky.color((cos(i)*1000, sin(i)*1000, log10(i+1)*1000))
+#  values.append((perf_counter_ns()-time_is)/1000)
+#print("color speed:", sum(values)/len(values), "µs")
+#input(">>> ")
+#
+#exit()
 
 """This is a demo code
 Source: https://my.numworks.com/python/zetamap/snake_lite
 """
 print("""This is a demo code
 Source: https://my.numworks.com/python/zetamap/snake_lite""")
 __all__ = []
 
 import os
 #os.environ['KANDINSKY_ENABLE_DEBUG'] = ''
+#os.environ['KANDINSKY_ZOOM_RATIO'] = '2'
+#os.environ['KANDINSKY_SCREEN_SIZE'] = '1020x240'
+
 #############################################################
 
 from random import randint as ri
 from __init__ import fill_rect as fr, draw_string as ds
 from ion import keydown as kd
 from time import monotonic as mt, sleep as sl
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/core.py` & `kandinsky-2.5.dev1/src/kandinsky/util/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,131 +1,119 @@
-######### Environ config #########
-import os
-
-DEBUG = 'KANDINSKY_ENABLE_DEBUG' in os.environ #or True 
-
-NO_GUI = 'KANDINSKY_NO_GUI' in os.environ
-
-DEFAULT_OS = 1
-# '0': PC, '1': Numworks, '2': Omega, '3': Upsilon
-try: OS_MODE = int(os.environ.get('KANDINSKY_OS_MODE', DEFAULT_OS)) 
-except ValueError: OS_MODE = DEFAULT_OS
-
-DEFAULT_MODEL = 1
-# '0': n0100, '1': n0110, '2': n0120
-try: MODEL_MODE = int(os.environ.get('KANDINSKY_MODEL_MODE', DEFAULT_MODEL))
-except ValueError: MODEL_MODE = DEFAULT_MODEL
+######### Imports #########
+from os import environ, name
 
+try: from tkinter import Tk
+except ImportError as e:
+  e.msg = "tkinter is not installed. "+("please reinstall python with complements modules" if name == "nt" else "install it with 'sudo apt install python3-tk'")
+  raise
 
-######### Init #########
 import warnings
 warnings.filterwarnings('ignore', category=UserWarning) # Disable SDL warning 
 try:
-  import sdl2
-  import sdl2.ext
-
-  sdl2.ext.init()
-  sdl2.ext.ttf._ttf_init()
-  sdl2.ext.image._sdl_image_init()
+  import sdl2dll
+  from sdl2.ext import init, quit as sdl_quit, ttf, image
+  from sdl2._internal import prettywarn
+
+  init()
+  ttf._ttf_init()
+  image._sdl_image_init()
 
-except (ImportError, ModuleNotFoundError) as e:
-  e.args = ("""PySDL2 or PySDL2-dll module is not installed on your system, and kandinsky depend to it.
+except (ImportError, RuntimeError) as e:
+  e.msg = """PySDL2 or PySDL2-dll module is not installed on your system, and kandinsky depend to it.
 >>> To install, follow steps on the GitHub project: https://github.com/ZetaMap/Kandinsky-Numworks
->>> or type 'pip install pysdl2 pysdl2-dll""",)
-  raise
-
-try: import tkinter
-except (ImportError, ModuleNotFoundError) as e:
-  e.args = ("tkinter is not installed. "+("please reinstall python with complements modules" if os.name == "nt" else "install it with 'sudo apt install python3-tk'"),)
+>>> or type 'pip install -U pysdl2 pysdl2-dll"""
   raise
 
 try: import ion
-except (ImportError, ModuleNotFoundError): ION_PRESENT = False
+except ImportError: ION_PRESENT = False
 else: 
   # In older version i forgot to define __version__ field
-  # so if is not defined, is an outdated version
-  if not hasattr(ion, "__version__") : ION_PRESENT = False
-  
-  # Verify if version is good
-  elif tuple([int(i) for i in ion.__version__.split('.') if i.isdecimal()]) < (1, 2, 3):
-    sdl2._internal.prettywarn("outdated version of 'Ion-numworks', please update it", ImportWarning)
+  # so if is not defined, is an outdated version.
+  # Or verify if version is good
+  if not hasattr(ion, "__version__") or tuple([int(i) for i in ion.__version__.split('.') if i.isdecimal()]) < (1, 2, 3):
+    # idk why but warning don't print, so will show it manually
+    print("ImportWarning: outdated version of 'Ion-numworks', please update it")
     ION_PRESENT = False
 
   # Another module is called ion, so do a little test to see if it's the right module
   else: ION_PRESENT = hasattr(ion, "keydown") 
 
-# Cleanup namespaces
-del os, sdl2, tkinter, warnings
-
-
-__all__ = [
-  "Core",
-  "OS_MODE",
-  "DEFAULT_OS",
-  "MODEL_MODE"
-  "DEFAULT_MODE",
-  "NO_GUI"
-]
-
-######### Imports #########
-from tkinter import Tk
-from sdl2.ext import quit as sdl_quit
 from threading import Thread, main_thread
 from math import sqrt
 from .stuff import *
 
-# Try to find an real time clock to do microseconds sleeps
-if Constants.is_windows:
-  # Try to use module win-precise-time to get more sleeps precision
-  try:
-    import win_precise_time as _wpt
-    usleep = lambda us: _wpt.sleep_until_ns(int(_wpt.time_ns()+us*1000))
-  except:
-    import time as _time, sdl2._internal
-    sdl2._internal.prettywarn("win-precise-time module is not installed. Using time module to do usleep (emulation will be less accurate)", RuntimeWarning)
-    def usleep(us):
-      t = _time.perf_counter_ns()+us*1000
-      while _time.perf_counter_ns() < t: _time.sleep(1e-9)
-    del sdl2._internal
-else:
-  try:
-    import ctypes
-    usleep = ctypes.CDLL("libc.so.6").usleep
-    del ctypes
-  except:
-    # On some linux distribution, this library is not installed by default
-    import time as _time, sdl2._internal
-    sdl2._internal.prettywarn("libc6 library is not installed. Using time module to do usleep (emulation will be less accurate)", RuntimeWarning)
-    usleep = lambda us: _time.sleep(us/10e6)
-    del sdl2._internal
+
+######### Environ config #########
+DEBUG = 'KANDINSKY_ENABLE_DEBUG' in environ #or True 
+
+NO_GUI = 'KANDINSKY_NO_GUI' in environ
+
+# '0': PC, '1': Numworks, '2': Omega, '3': Upsilon
+os = environ.get('KANDINSKY_OS_MODE')
+if os and os.isdecimal(): Vars.selected_os = int(os) if 0 <= int(os) < len(Config.os_list) else Config.default_os
+
+# '0': n0100, '1': n0110, '2': n0120
+model = environ.get('KANDINSKY_MODEL_MODE')
+if model and model.isdecimal(): Vars.selected_model = int(model) if 0 <= int(model) < len(Config.model_list) else Config.default_model
+
+if 'KANDINSKY_SCREEN_SIZE' in environ:
+  screen = environ['KANDINSKY_SCREEN_SIZE'].split('x')
+  
+  if len(screen) != 2: 
+    raise \
+      ValueError("invalid screen format. format to use: '<width>x<height>'")
+  
+  for i in range(2):
+    if not screen[i].isdecimal() or int(screen[i]) < 0: 
+      raise \
+        ValueError("screen dimensions must be positive integers")
+    screen[i] = int(screen[i])
+    
+  screen[1] -= Vars.head_size
+  if screen[0] < Vars.screen[0] or screen[1] < Vars.screen[1]:
+    raise \
+      ValueError(f"screen dimensions must be greater than {Vars.screen[0]}x{Vars.screen[1]+Vars.head_size}")
+  
+  Vars.screen = tuple(screen)
+
+zoom = environ.get('KANDINSKY_ZOOM_RATIO')
+if zoom and zoom.isdecimal() and 1 <= int(zoom) <= Config.zoom_max: Vars.zoom_ratio = int(zoom)
+
+# Experimental way to get more real emulation of numworks
+import threading
+USE_HEAP = 'KANDINSKY_USE_HEAP' in environ and hasattr(threading, "get_native_id")
+# same problem than warning of ion
+if USE_HEAP: print("ResourceWarning: python heap limitator is an experimental feature, so it can crach python several times")
+
+######### Cleanup #########
+del environ, name, os, model, zoom, init, sdl2dll, ttf, image, warnings, threading, #prettywarn
 
 
 ######### Main code #########
+__all__ = ["Core"]
+
 class Core(Thread): 
   stoped = False
-  drawable = None
   asknoclose = False
+  OS_MODE = Config.default_os
 
   def __init__(self):
-    Gui.paused = True # Pause events to give the time of thread to initialize
+    Gui.paused = Gui.already_paused = True # Pause events to give the time of thread to initialize
 
-    super().__init__(None, self.event_loop, Constants.app_name.replace(' ', '')+self.__class__.__name__)
+    super().__init__(None, self.event_loop, Vars.app_name.replace(' ', '')+self.__class__.__name__)
     self.start()
-    while Gui.paused and self.is_alive(): pass # Wait a little to synchronize it
+    while Gui.paused and self.is_alive(): usleep(100) # Wait a little to synchronize it
 
-  def quit_app(self):
+  def quit_app(self, *_):
     if not self.stoped:
       self.stoped = True 
-      self.paused = False # Now all calls of kandinsky raise an error
+      Gui.paused = False # Now all calls of kandinsky raise an error
 
-      Gui.head.close()
-      Gui.screen.close()
-      
+      Gui.destroy()
       sdl_quit()
-      self.root.quit()
 
   def print_debug(self, type, *messages, type_length=5, **args):
     if DEBUG: 
       print("DEBUG: ", end='')
       print(type+' '*(type_length-len(type))+':', *messages, **args)
 
   def verify(self, method, *args, **kwargs):
@@ -134,39 +122,41 @@
     if Gui.paused: self.print_debug("Pause", "waiting...")
     while Gui.paused and self.is_alive(): usleep(1000)
 
     if self.stoped: raise RuntimeError("kandinsky window destroyed")
     elif not self.is_alive(): raise RuntimeError(f"an internal error has occurred. Stack trace is before this it.")
 
   def sleep(self, delay_us):
+    if USE_HEAP and Gui.heap_set: return # No need to sleep
+
     ratio = Gui.data.model*Gui.data.ratio
     delay = int(delay_us*ratio)
 
     self.print_debug("Delay", "input =", delay_us, "µs, ratio ≃", str(round(ratio, 6))+", output =", delay, "µs")
     if ratio > 0: usleep(delay)
 
-### methods when used
+### methods
   def get_pixel(self, x, y):
     Tests.int(x, y)
 
-    if y < 0 or y > Constants.screen[0] or x < 0 or x > Constants.screen[1]: color = Colors.black
-    else: color = Colors.convert(Draw.get_at(self.drawable, x, y))
+    if y < 0 or y > Vars.screen[0] or x < 0 or x > Vars.screen[1]: color = Colors.black
+    else: color = Colors.convert(Draw.get_at(Gui.drawable, x, y))
 
     self.sleep(77)
     return color
 
   def set_pixel(self, x, y, color):
     Tests.int(x, y)
 
-    Draw.pixel(self.drawable, Colors.convert(color), x, y)
+    Draw.pixel(Gui.drawable, Colors.convert(color), x, y)
     self.sleep(130)
 
   def color(self, r, g, b):
-    if not g and not b: color = Colors.convert(r)
-    elif g and b: 
+    if g is None and b is None: color = Colors.convert(r)
+    elif g is not None and b is not None: 
       Tests.int(r, g, b)
       color = Colors.convert((r, g, b))
     else: raise TypeError("color takes 1 or 3 arguments")
 
     self.sleep(100)
     return color
 
@@ -177,25 +167,25 @@
     color = Colors.convert(color)
     background = Colors.convert(background)
     bs = (7, 14) if font else (10,18)
     font = Config.small_font if font else Config.large_font
     if '\0' in text: text = text[:text.index('\0')]
 
     for i, l in enumerate(text.replace('\r', '').replace('\f', '\x01').replace('\b', '\x01').replace('\v', '\x01').replace('\t', "    ").splitlines()): 
-      Draw.rect(self.drawable, background, (x*(not i), y+i*bs[1], len(l)*bs[0], bs[1]))
-      Draw.blit(self.drawable, font.render(l, color=color), (x*(not i), y+i*bs[1]-2))
+      Draw.rect(Gui.drawable, background, (x*(not i), y+i*bs[1], len(l)*bs[0], bs[1]))
+      Draw.string(Gui.drawable, font, l, x*(not i), y+i*bs[1]-2, color)
     self.sleep(86*(len(text)+(len(text)>=5)//1.2))
   
   def fill_rect(self, x, y, width, height, color):
     Tests.int(x, y, width, height)
   
     if width < 0:  x, width = x+width, -width
     if height < 0: y, height = y+height, -height
     
-    Draw.rect(self.drawable, Colors.convert(color), (x, y, width, height))
+    Draw.rect(Gui.drawable, Colors.convert(color), (x, y, width, height))
     self.sleep(130+width*height/20+width*height*0.02)
 
   def wait_vblank(self):
     """why this?"""
     while not self.refreshed: usleep(100)
 
   def get_keys(self):
@@ -212,126 +202,121 @@
     s = abs(y2-y1) > abs(x2-x1)
     if s: x1, y1, x2, y2 = y1, x1, y2, x2
     if x1 > x2: x1, x2, y1, y2 = x2, x1, y2, y1
     g = 1 if x2 == x1 else (y2-y1)/(x2-x1)
 
     for x in range(x1, x2):
       ty = int(y1+g*(x-x1))
-      Draw.pixel(self.drawable, color, *((ty, x) if s else (x, ty)))
+      Draw.pixel(Gui.drawable, color, *((ty, x) if s else (x, ty)))
 
     self.sleep(111) # TODO: calculate speed
 
   def draw_circle(self, x, y, r, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_circle.cpp"""
     Tests.int(x, y, r)
     
     color = Colors.convert(color)
     xc, yc, m = 0, abs(r), 5-4*abs(r) 
 
     while xc <= yc:
-      Draw.pixel(self.drawable, color, xc+x, yc+y)
-      Draw.pixel(self.drawable, color, yc+x, xc+y)
-      Draw.pixel(self.drawable, color, -xc+x, yc+y)
-      Draw.pixel(self.drawable, color, -yc+x, xc+y)
-      Draw.pixel(self.drawable, color, xc+x, -yc+y)
-      Draw.pixel(self.drawable, color, yc+x, -xc+y)
-      Draw.pixel(self.drawable, color, -xc+x, -yc+y)
-      Draw.pixel(self.drawable, color, -yc+x, -xc+y)
+      Draw.pixel(Gui.drawable, color, xc+x, yc+y)
+      Draw.pixel(Gui.drawable, color, yc+x, xc+y)
+      Draw.pixel(Gui.drawable, color, -xc+x, yc+y)
+      Draw.pixel(Gui.drawable, color, -yc+x, xc+y)
+      Draw.pixel(Gui.drawable, color, xc+x, -yc+y)
+      Draw.pixel(Gui.drawable, color, yc+x, -xc+y)
+      Draw.pixel(Gui.drawable, color, -xc+x, -yc+y)
+      Draw.pixel(Gui.drawable, color, -yc+x, -xc+y)
       
       if m > 0: yc, m = yc-1, m-8*yc
       xc, m = xc+1, m+8*xc+4 
 
     self.sleep(222) # TODO: calculate speed
 
   def fill_circle(self, x, y, r, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_circle.cpp"""
     Tests.int(x, y, r)
     color = Colors.convert(color)
 
     r = abs(r)
     for i in range(x-r, x+r):
       semi = int(sqrt(r**2-(x-i)**2))
-      Draw.rect(self.drawable, color, (i, y-semi, 1, semi*2))
+      Draw.rect(Gui.drawable, color, (i, y-semi, 1, semi*2))
 
     self.sleep(333) # TODO: calculate speed
 
   def fill_polygon(self, points, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_polygon.cpp"""
     Tests.list(points)
     if len(points) < 3: raise ValueError("polygon must have least 3 points")
     tests = [[len(i) for v in i if len(i) != 2 or not Tests.int(v)] for i in points if Tests.list(i)]
     if len(tests) and len(tests[0]): raise ValueError("requested length 2 but object has length "+str(tests[0][0]))
     
     color = Colors.convert(color)
     points_size = len(points)
 
-    for y in range(min([0,Constants.screen[0]]+points, key=lambda v: v[1]), max([0,0]+points, key=lambda v: v[1])):
+    for y in range(min([0,Vars.screen[0]]+points, key=lambda v: v[1]), max([0,0]+points, key=lambda v: v[1])):
       switches = []
       last_point = points_size-1
 
       for i in range(points_size):
         point_y, last_point_y = points[i][1], points[last_point][1]
         if ((point_y < y and last_point_y >= y) or (last_point_y < y and point_y >= y)) and point_y != last_point_y:
           switches.append(round(points[i][0]+1*(y-point_y)/(last_point_y-point_y)*(points[last_point][0]-points[i][0])))
         last_point = i
 
       switches.sort()
       for x in range(0, len(switches), 2):
-        if switches[x] >= Constants.screen[1]*2: break
-        if switches[x+1] > 0: Draw.rect(self.drawable, color, (switches[x], y, switches[x+1]-switches[x], 1))
+        if switches[x] >= Vars.screen[1]*2: break
+        if switches[x+1] > 0: Draw.rect(Gui.drawable, color, (switches[x], y, switches[x+1]-switches[x], 1))
 
     self.sleep(444) # TODO: calculate speed
 
   def get_palette():
-    return {"Toolbar":        Colors.convert(Gui.data.color), 
+    return {"Toolbar":        Gui.data.color, 
             "AccentText":     (0, 132, 120), 
             "HomeBackground": Colors.white, 
             "PrimaryText":    Colors.black,
             "SecondaryText":  (104, 108, 104)}
 ###
 
   def event_loop(self):
-    self.root = Tk()
+    root = Tk()
+    if USE_HEAP: Gui._main_thread_pid = self.native_id
     
     try:
-      Gui(self.root, (OS_MODE, DEFAULT_OS), (MODEL_MODE, DEFAULT_MODEL))
-      Gui.config(NO_GUI)
-      self.OS_MODE = Gui.os_mode.get()
-      self.root.protocol("WM_DELETE_WINDOW", self.quit_app)
+      Gui(root)
+      Gui.config(not NO_GUI)
     except RuntimeError as e:
       # Handle multiple import of library
       # Library cannot open new tkinter root windows while another is opened but it can open another if previous is destroyed
       # Note: no data from the previous window can be restored to new one
-      if "main thread is not in main loop" in e.args:
-        import warnings
-        warnings.warn("multiple creation of window is not permitted", ImportWarning)
-        del warnings
+      if "main thread is not in main loop" in e.args[0]: prettywarn("multiple creation of window is not permitted", ImportWarning)
       else: self.print_debug("ERROR", type(e).__name__+": "+e.args[0])
       return
-      
-    # Set surfaces
-    self.drawable = Gui.screen.get_surface()
-    Draw.rect(self.drawable, Colors.white)
-    Gui.update_data()
 
-    Gui.paused = False # Initialization finished, unpause events
+    self.OS_MODE = Gui.os_mode.get()
+    # Bind more event
+    root.protocol("WM_DELETE_WINDOW", self.quit_app)
+    root.bind("<Control-q>", self.quit_app)
+
+    Gui.paused = Gui.already_paused = False # Initialization finished, unpause events
 
     while True:
       if self.stoped:
         self.quit_app() 
         return  
       elif not self.asknoclose and not main_thread().is_alive():
         if Gui.askscriptend(): self.stoped = True
         else: self.asknoclose = True
       
       self.refreshed = False
-      Gui.head.refresh()
-      Gui.screen.refresh()
       try: Gui.refresh()
       except AttributeError: pass
+      except RuntimeError: self.stoped = True
       usleep(1000)
       self.refreshed = True
 
   def event_fire(self, method, *arg, **kwargs):
     try: 
       self.verify(method, *arg, **kwargs)
       return method(*arg, **kwargs), None
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/data/app.ico` & `kandinsky-2.5.dev1/src/kandinsky/util/data/app.ico`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/data/app.png` & `kandinsky-2.5.dev1/src/kandinsky/util/data/app.png`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/data/large_font.ttf` & `kandinsky-2.5.dev1/src/kandinsky/util/data/large_font.ttf`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/data/old_icons.zip` & `kandinsky-2.5.dev1/src/kandinsky/util/data/old_icons.zip`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/data/small_font.ttf` & `kandinsky-2.5.dev1/src/kandinsky/util/data/small_font.ttf`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/demo.py` & `kandinsky-2.5.dev1/src/kandinsky/util/demo.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/old_config.ini` & `kandinsky-2.5.dev1/src/kandinsky/util/old_config.ini`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/stuff/color.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/color.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-from .tests import *
-
-COLOR_ROUND_MULTIPLIER = (8, 4, 8)
+from .tests import Tests
+from .vars import Vars
 
 class Colors:
-  red     = (248, 0,   0)
-  cyan    = (0,   252, 248)
+  """https://github.com/numworks/epsilon/blob/master/kandinsky/include/kandinsky/color.h"""
+
   blue    = (0,   0,   248)
-  grey    = (160, 164, 160)
-  gray    = grey
+  b       = blue
+  red     = (248, 0,   0)
+  r       = red
   green   = (80,  192, 0)
+  g       = green
+  yellow  = (248, 252, 0)
+  y       = yellow
+  brown   = (136, 112, 80)
+  black   = (0,   0,   0)
+  k       = black
+  white   = (248, 252, 248)
+  w       = white
   pink    = (248, 168, 176)
+  orange  = (248, 132, 24)
   purple  = (104, 44,  120)
+  grey    = (160, 164, 160)
+  gray    = grey
+  cyan    = (0,   252, 248)
   magenta = (248, 4,   136)
-  black   = (0,   0,   0)
-  orange  = (248, 132, 24)
-  brown   = (136, 112, 80)
-  white   = (248, 252, 248)
-  yellow  = (248, 252, 0)
+  COLORS = {k: v for k, v in locals().items() if not k.startswith('_')}
+  
+  fix = lambda r, g, b: (((r>>3)&0x1f)<<3 if Vars.selected_os > 1 else Colors.expand((r>>3)&0x1f, 5),
+                            ((g>>2)&0x3f)<<2 if Vars.selected_os > 1 else Colors.expand((g>>2)&0x3f, 6),
+                            ((b>>3)&0x1f)<<3 if Vars.selected_os > 1 else Colors.expand((b>>3)&0x1f, 5))
+  expand = lambda v, nBits: (v<<(8-nBits)) | (v>>(nBits-(8-nBits)))
+  #TODO: make a __get_attribute__ to do invisible expand for numworks
+
+    
 
   def convert(rgbOrName):
-    color = []
     _type = type(rgbOrName)
-
+    
     if _type == str: 
-      if rgbOrName.startswith("__"): pass
-      elif hasattr(Colors, rgbOrName): color = getattr(Colors, rgbOrName)
+      if rgbOrName in Colors.COLORS: return Colors.fix(*Colors.COLORS[rgbOrName])
       elif rgbOrName.startswith('#'):
         if len(rgbOrName) != 7: raise ValueError("RGB hex values are 6 bytes long")
 
-        try: color = [int(rgbOrName[i:i+2], 16) for i in range(1, len(rgbOrName), 2)]
+        try: return Colors.fix(*[int(rgbOrName[i:i+2], 16) for i in range(1, len(rgbOrName), 2)])
         except ValueError as e:
           e.args = (f"invalid literal for int() with base 16: '{rgbOrName[1:]}'",)
           raise
+      else:
+        try: ratio = float(rgbOrName)
+        except ValueError as e:
+          e.args = ("invalid syntax for number",)
+          raise
+        else:
+          if 0 <= ratio <= 1: return tuple([int(255*ratio) for _ in range(3)])
+          else: raise ValueError("Gray levels are between 0.0 and 1.0")
     
     elif _type == int: raise ValueError("Int are not colors")
 
-    elif Tests.list(rgbOrName):
-      if len(rgbOrName) != 3: raise ValueError("Color needs 3 components")
-      color = [int(c) for c in rgbOrName if type(c) == float or Tests.int(c)]
-
-    if len(color) > 0: return tuple([0 if color[i] < 0 else color[i]%256//COLOR_ROUND_MULTIPLIER[i]*COLOR_ROUND_MULTIPLIER[i] for i in range(len(color))])
-    else: raise ValueError("invalid syntax for number")
+    Tests.list(rgbOrName)
+    if len(rgbOrName) != 3: raise ValueError("Color needs 3 components")
+    return Colors.fix(*[int(c) for c in rgbOrName if type(c) == float or Tests.int(c)])
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/stuff/draw.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/draw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from sdl2 import SDL_Rect, SDL_FillRect, SDL_BlitSurface, SDL_CreateRGBSurfaceWithFormat, SDL_PIXELFORMAT_ARGB8888, Uint8
+from sdl2 import SDL_Rect, SDL_FillRect, SDL_BlitSurface, SDL_BlitScaled, SDL_CreateRGBSurfaceWithFormat, SDL_PIXELFORMAT_RGB888
 from sdl2.ext import prepare_color
-from ctypes import cast, byref, POINTER, c_uint
+from ctypes import cast, byref, POINTER, c_uint, c_uint8
+from .vars import Vars
 
 __all__ = ["Draw"]
 
 
 class Draw:
-  new_surface = lambda width, height: SDL_CreateRGBSurfaceWithFormat(0, width, height, 32, SDL_PIXELFORMAT_ARGB8888)
-  blit = lambda dest, source, area=None: SDL_BlitSurface(source, None, dest, SDL_Rect(*area) if area else None)
-  rect = lambda dest, color, area=None: SDL_FillRect(dest, SDL_Rect(*area) if area else None, prepare_color(color, dest))
-  pixel = lambda dest, color, x, y: SDL_FillRect(dest, SDL_Rect(x, y, 1, 1), prepare_color(color, dest))
+  new_area = lambda *area: SDL_Rect(*[int(i*Vars.zoom_ratio) for i in (area[0] if len(area)==1 and type(area[0]) in (list, tuple) else area)])
+  new_surface = lambda width, height: SDL_CreateRGBSurfaceWithFormat(0, int(width*Vars.zoom_ratio), int(height*Vars.zoom_ratio), 32, SDL_PIXELFORMAT_RGB888).contents
+  blit = lambda dest, source, area=None: SDL_BlitSurface(source, None, dest, Draw.new_area(area) if area else None)
+  blit_scaled = lambda dest, source, area=None: SDL_BlitScaled(source, None, dest, Draw.new_area(area+(source.w, source.h) if len(area) == 2 else area) if area else None)
+  rect = lambda dest, color, area=None: SDL_FillRect(dest, Draw.new_area(area) if area else None, prepare_color(color, dest))
+  pixel = lambda dest, color, x, y: SDL_FillRect(dest, Draw.new_area(x, y, 1, 1), prepare_color(color, dest))
+  string = lambda dest, font, text, x, y, color=None: Draw.blit_scaled(dest, font.render(text, color=color), (x, y))
 
   def get_at(source, x, y):
-    bpp = source.format.contents.BytesPerPixel
-    pixel = cast(byref(cast(source.pixels, POINTER(Uint8)).contents, bpp*source.w*y+x*bpp), POINTER(c_uint)).contents.value
+    pixel = cast(byref(cast(source.pixels, POINTER(c_uint8)).contents, (source.w*y+x)*source.format.contents.BytesPerPixel), POINTER(c_uint)).contents.value
     return (pixel&0xff0000)>>8, (pixel&0x00ff00)>>4, (pixel&0x0000ff)>>0
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/stuff/gui.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/gui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,204 +1,305 @@
 from tkinter import Tk, Frame, Menu, IntVar
+
 from tkinter.dialog import Dialog
 from tkinter.filedialog import asksaveasfilename
+from tkinter.font import Font
 
-from sdl2 import SDL_CreateWindowFrom, SDL_DestroyWindow, SDL_GetScancodeFromKey#, SDL_WINDOW_OPENGL
-from sdl2.events import SDL_Event, SDL_PushEvent, SDL_KEYDOWN, SDL_PRESSED
-from sdl2.ext import Window, load_image
+from sdl2 import SDL_CreateWindowFrom, SDL_DestroyWindow, SDL_FreeSurface#, SDL_WINDOW_OPENGL
+from sdl2.ext import Window, load_img
 
 from os import getcwd, system
 from webbrowser import open as open_link, register_standard_browsers  # To open links in help menu
-register_standard_browsers()
+register_standard_browsers() # register now to avoid a long wait when links open
 del register_standard_browsers
 from datetime import datetime
 
 # Internal
 from .vars import *
 from .draw import Draw
+from .color import Colors
+from . import limiter
 
 __all__ = ["Gui"]
 
 
 class Gui:
   tkmaster:Tk = None
   paused = False
   already_paused = False
+  drawable = None
+  _main_thread_pid = None # because thread.native_pid don't exist in python<3.8, so use the other way
+  heap_set = False
 
   def created():
-    if not Gui.tkmaster: raise RuntimeError("an instance must be created")
+    if not Gui.tkmaster: raise RuntimeError("Gui: an instance must be created")
+
+  def _unpause_after_wrapper(method):
+    def _wrap(*a, **k):
+      method(*a, **k)
+      if not Gui.already_paused: Gui.paused = False
+    
+    _wrap.__name__ = method.__name__
+    return _wrap
 
-  def __init__(_, tkmaster, start_os, start_model):
+  # Patched menu buttons to unpause script when is clicked
+  _add_command = lambda menu, **kwargs: menu.add_command(**dict([(k, Gui._unpause_after_wrapper(v)) if "command" in k else (k, v) for k, v in kwargs.items()]))
+  _add_radiobutton = lambda menu, **kwargs: menu.add_radiobutton(**dict([(k, Gui._unpause_after_wrapper(v)) if "command" in k else (k, v) for k, v in kwargs.items()]))
+
+  def __init__(_, tkmaster):
     Gui.tkmaster = tkmaster
-    if not Constants.is_windows: Gui.tkmaster.option_add("*font", "SegoeUI 9")
+    if Vars.is_linux: 
+      Gui.linux_menu_font = Font(tkmaster, family="SegoeUI", size=9)
+      Gui.tkmaster.option_add("*font", Gui.linux_menu_font)
     Gui.data = StateData()
 
-    # Create frame area for sdl2 and pack it
-    Gui.head_frame = Frame(tkmaster, width=Constants.screen[0], height=Constants.head_size)
-    Gui.screen_frame = Frame(tkmaster, width=Constants.screen[0], height=Constants.screen[1])
+    # Create frame area, sdl2 windows and pack everything
+    Gui.head_frame = Frame(tkmaster)
+    Gui.screen_frame = Frame(tkmaster)
     Gui.head_frame.pack()
     Gui.screen_frame.pack()
-    Gui.screen_frame.focus_set()
     Gui.tkmaster.update()
-
-    # OS head
     Gui.head = Window('',(0,0))
-    SDL_DestroyWindow(Gui.head.window)
-    Gui.head.window = SDL_CreateWindowFrom(Gui.head_frame.winfo_id())
-    Gui.head_id = Gui.head_frame.winfo_id()
-    
-    # Drawable screen
     Gui.screen = Window('',(0,0))
-    SDL_DestroyWindow(Gui.screen.window)
-    Gui.screen.window = SDL_CreateWindowFrom(Gui.screen_frame.winfo_id())
-    Gui.screen_id = Gui.screen_frame.winfo_id()
 
     Gui.menu = Menu(tkmaster)
     # Menus
-    ## About menu
+    ## Help menu
     about = Menu(tearoff=False)
-    about.add_command(label="GitHub project",     command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks"))
-    about.add_command(label="Documentation",      command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks#usable-content"))
-    about.add_command(label="An issue? Open one", command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/issues/new"))
-    about.add_command(label="Made by ZetaMap",    command=lambda: open_link("https://github.com/ZetaMap"))
+    Gui._add_command(about, label="GitHub project",     command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks"))
+    Gui._add_command(about, label="Documentation",      command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks#usable-content"))
+    Gui._add_command(about, label="An issue? Open one", command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/issues/new"))
+    Gui._add_command(about, label="Made by ZetaMap",    command=lambda: open_link("https://github.com/ZetaMap"))
     Gui.menu.add_cascade(label="About", menu=about)
 
     ## Help menu
     help = Menu(tearoff=False)
-    help.add_command(label="CTRL+O: change OS",       state="disabled", activebackground="#F0F0F0")
-    help.add_command(label="CTRL+M: change Model",    state="disabled", activebackground="#F0F0F0")
-    help.add_command(label="CTRL+S: take screenshot", state="disabled", activebackground="#F0F0F0")    
-    help.add_command(label="CTRL+P: pause/resume",    state="disabled", activebackground="#F0F0F0")
+    sortcut = Menu(tearoff=False)
+
+    Gui._add_command(sortcut, label="CTRL+Q: Close window",    state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+O: change OS",       state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+M: change Model",    state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+S: take screenshot", state="disabled", activebackground="#F0F0F0")    
+    Gui._add_command(sortcut, label="CTRL+P: pause/resume",    state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+Z: change zoom",     state="disabled", activebackground="#F0F0F0")
+    help.add_cascade(label="Shortcut", menu=sortcut)
+
     help.add_separator()
-    help.add_command(label="Ion keyboard", command=lambda: open_link("https://github.com/ZetaMap/Ion-Numworks#keys"))
-    help.add_command(label="Check FAQ",    command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/FAQ.md"))
+    Gui._add_command(help, label="Ion keyboard", command=lambda: open_link("https://github.com/ZetaMap/Ion-Numworks#keys"))
+    Gui._add_command(help, label="Check FAQ",    command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/FAQ.md"))
     Gui.menu.add_cascade(label="Help", menu=help)
 
+    ## Options menu
+    Gui.options = Menu(tearoff=False)
+
     ## OS menu
-    max_ = len(Config.os_list)-1
-    Gui.os_mode = IntVar(value=start_os[1] if start_os[0] < 0 or start_os[0] > max_ else start_os[0])
+    Gui.os_mode = IntVar(value=Vars.selected_os)
     new = Menu(tearoff=False)
     for i, mode in enumerate(Config.os_list): 
-      new.add_radiobutton(label=mode["name"], variable=Gui.os_mode, value=i, command=Gui.update_data)
-      Config.os_list[i]["battery"] = load_image(Constants.path+Config.os_list[i]["battery"])
-    Gui.menu.add_cascade(label="OS", menu=new)
+      Gui._add_radiobutton(new, label=mode["name"], variable=Gui.os_mode, value=i, command=Gui.update_data)
+      Config.os_list[i]["battery"] = load_img(Vars.path+Config.os_list[i]["battery"])
+    Gui.options.add_cascade(accelerator="CTRL+O", label="OS", menu=new)
 
     ## Model menu
-    max_ = len(Config.model_list)-1
-    Gui.model_mode = IntVar(value=start_model[1] if start_model[0] < 0 or start_model[0] > max_ else start_model[0])
+    Gui.model_mode = IntVar(value=Vars.selected_model)
     new = Menu(tearoff=False)
     for i, mode in enumerate(Config.model_list): 
-      new.add_radiobutton(label=mode["name"], variable=Gui.model_mode, value=i, command=Gui.update_data, 
+      Gui._add_radiobutton(new, label=mode["name"], variable=Gui.model_mode, value=i, command=Gui.update_data, 
         **({"state": "disabled", "activebackground": "#F0F0F0"} if mode.get("disabled", False) else {}))
-    Gui.menu.add_cascade(label="Model", menu=new)
+    Gui.options.add_cascade(accelerator="CTRL+M", label="Model", menu=new)
+
+    Gui.zoom = IntVar(value=Vars.zoom_ratio)
+    Gui.increase_font = IntVar()
+    Gui.zoom.trace_add("write", Gui.set_zoom)
+    Gui.increase_font.trace_add("write", Gui.set_zoom)
+    new = Menu(tearoff=False)
+    for i in range(Config.zoom_max): Gui._add_radiobutton(new, label=f"x{i+1}", variable=Gui.zoom, value=i+1)
+    if not Vars.is_windows: new.add_checkbutton(label="Increase font size", variable=Gui.increase_font)
+    Gui.options.add_cascade(accelerator="CTRL+Z", label="Zoom", menu=new)
+
+    Gui.options.add_separator()
 
     ## Screenshot button
-    Gui.menu.add_command(label="Screenshot", command=Gui.screenshot)
+    Gui.options.add_command(accelerator="CTRL+S", label="Screenshot", command=Gui.screenshot)
 
     ## Pause button
-    def state(): 
-      Gui.paused = not Gui.paused
-      Gui.already_paused = Gui.paused
-      Gui.menu.entryconfig(6, label=["Pause", "Resume"][Gui.paused])
-    Gui.menu.add_command(label="Pause", command=state,)
+    def state(states=["Pause", "Resume"]): 
+      Gui.already_paused = not Gui.already_paused
+      Gui.paused = Gui.already_paused
+      Gui.options.entryconfig(states[not Gui.already_paused], label=states[Gui.already_paused])
+    Gui.options.add_command(accelerator="CTRL+P", label="Pause", command=state)
+
+    Gui.menu.add_cascade(label="Options", menu=Gui.options)
 
-  def update_value(int_var, values):
+  def set_zoom(*_, force=False):
+    Gui.created()
+
+    Gui.paused = True # Give time to change var, destroy and rebuild window
+    last_zoom = Vars.zoom_ratio
+    Vars.zoom_ratio = Gui.zoom.get()
+    if Vars.is_linux: Gui.linux_menu_font.config(size=9*(Vars.zoom_ratio if Gui.increase_font.get() else 1))
+
+    if not force and last_zoom == Vars.zoom_ratio:
+      # No need to continue
+      if not Gui.already_paused: Gui.paused = False
+      return
+
+    SDL_DestroyWindow(Gui.head.window)
+    SDL_DestroyWindow(Gui.screen.window)
+    Gui.head_frame.config(width=Vars.screen[0]*Vars.zoom_ratio, height=Vars.head_size*Vars.zoom_ratio)
+    Gui.screen_frame.config(width=Vars.screen[0]*Vars.zoom_ratio, height=Vars.screen[1]*Vars.zoom_ratio)
+    Gui.tkmaster.update()
+    Gui.head.window = SDL_CreateWindowFrom(Gui.head_frame.winfo_id())
+    Gui.screen.window = SDL_CreateWindowFrom(Gui.screen_frame.winfo_id())
+    Gui.screen_surf = Gui.screen.get_surface()
+    
+    last_drawable = Gui.drawable
+    Gui.drawable = Draw.new_surface(*Vars.screen)
+    Draw.blit_scaled(Gui.drawable, last_drawable)
+    Gui.update_data()
+
+    Gui.center_window()
+    if not Gui.already_paused: Gui.paused = False
+
+  def destroy():
+    Gui.created()
+
+    SDL_FreeSurface(Gui.drawable)
+    Gui.head.close()
+    Gui.screen.close()
+    Gui.tkmaster.quit()
+    Gui.tkmaster = None
+
+  def update_value(int_var, values, min=0):
     Gui.created()
     v = int_var.get()+1
-    if v > len(values)-1: v = 0
+    if v > len(values)-1: v = min
 
     if not values[v].get("disabled", False):
       int_var.set(v)
       Gui.update_data()
 
   def update_data():
     Gui.created()
     if Gui.head.window is None: return
 
     Gui.data(**Config.os_list[Gui.os_mode.get()], model=Config.model_list[Gui.model_mode.get()]["ratio"])
-    surf = Gui.head.get_surface()
-    
-    Draw.rect(surf, Gui.data.color)
-    Draw.blit(surf, Config.small_font.render(Gui.data.unit), (5, 0))
-    Draw.blit(surf, Config.small_font.render("PYTHON"), (Constants.screen[0]-181, 1))
-    x = Constants.screen[0]-20  
+    Gui.head_surface = Draw.new_surface(Vars.screen[0],Vars.head_size)
+
+    Draw.rect(Gui.head_surface, Gui.data.color)
+    Draw.string(Gui.head_surface, Config.small_font, Gui.data.unit, 5, 0)
+    Draw.string(Gui.head_surface, Config.small_font, "PYTHON", Vars.screen[0]//2-21, 1)
+    x = Vars.screen[0]-20
     if Gui.data.clock:
-      Draw.blit(surf, Config.small_font.render(datetime.now().strftime("%H:%M")), (x-20, 1))
+      Draw.string(Gui.head_surface, Config.small_font, datetime.now().strftime("%H:%M"), x-20, 1)
       x -= 40
-    Draw.blit(surf, Gui.data.battery, (x, 4))
+    Draw.blit_scaled(Gui.head_surface, Gui.data.battery, (x, 4))
+    # try to blit it now on screen
+    try: Draw.blit(Gui.head.get_surface(), Gui.head_surface)
+    except: pass
+
+    # Set new heap of python
+    if Gui._main_thread_pid: 
+      try: limiter.set_heap(Gui._main_thread_pid, Gui.data.heap)
+      except (AssertionError, OSError): raise #Gui.heap_set = False
+      else: Gui.heap_set = True
 
-  def config(no_gui=False):
+  def config(create_gui=False):
     Gui.created()
-    # Set default data
-    Gui.update_data()
 
     # Config main window
-    Gui.tkmaster.title(Constants.app_name)
-    if Constants.is_windows: Gui.tkmaster.iconbitmap(default=Constants.path+"app.ico")
+    Gui.tkmaster.title(Vars.app_name)
+    if Vars.is_windows: Gui.tkmaster.iconbitmap(default=Vars.path+"app.ico")
     else:
       from tkinter import PhotoImage
-      Gui.tkmaster.iconphoto(True, PhotoImage(file=Constants.path+"app.png"))
+      Gui.tkmaster.iconphoto(True, PhotoImage(file=Vars.path+"app.png"))
     Gui.tkmaster.resizable(False, False)
-    if not no_gui: Gui.tkmaster.config(menu=Gui.menu)
-    Gui.tkmaster.eval('tk::PlaceWindow . center')
+    if create_gui: Gui.tkmaster.config(menu=Gui.menu)
+    Gui.tkmaster.eval('tk::PlaceWindow . center') # I must keep this otherwise the SDL windows do not configure correctly
+    Gui.center_window()
 
     # Bind shorcuts
     Gui.tkmaster.bind("<Control-o>", lambda _: Gui.update_value(Gui.os_mode, Config.os_list))
     Gui.tkmaster.bind("<Control-m>", lambda _: Gui.update_value(Gui.model_mode, Config.model_list))
     Gui.tkmaster.bind("<Control-s>", lambda _: Gui.screenshot())
-    def state(_=None): 
-      Gui.paused = not Gui.paused
-      Gui.menu.entryconfig(6, label=["Pause", "Resume"][Gui.paused])
+    def state(*_, states=["Pause", "Resume"]): 
+      Gui.already_paused = not Gui.already_paused
+      Gui.paused = Gui.already_paused
+      Gui.options.entryconfig(states[not Gui.already_paused], label=states[Gui.already_paused])
     Gui.tkmaster.bind("<Control-p>", state)
+    Gui.tkmaster.bind("<Control-z>", lambda _: Gui.update_value(Gui.zoom, [{}]*(Config.zoom_max+1), 1))
 
-    # I don't know why, but i can't get focus of keyboard, so i will push keyboard events manually
-    def on_key_press(event):
-      sdl_event = SDL_Event(type=SDL_KEYDOWN)
-      sdl_event.key.keysym.scancode = SDL_GetScancodeFromKey(event.keycode)
-      sdl_event.key.keysym.sym = event.keycode+32
-      sdl_event.key.state = SDL_PRESSED
-      SDL_PushEvent(sdl_event)
-    Gui.tkmaster.bind("<KeyPress>", on_key_press)
-
-    # Clear sdl windows and refresh Tkinter frames
-    Gui.refresh()
+    ### Windows patchs
+    if Vars.is_windows:
+      # Bind events to pause, if dragged or user interact with gui
+      def drag_event(e):
+        if e.widget is Gui.tkmaster:
+          if Gui._drag_window_event_id: 
+            Gui.tkmaster.after_cancel(Gui._drag_window_event_id)
+            Gui.paused = True
+          Gui._drag_window_event_id = Gui.tkmaster.after(200, drag_event_stop)
+      def drag_event_stop():
+        Gui._drag_window_event_id = ''
+        if not Gui.already_paused: Gui.paused = False
+      drag_event_stop()
+      Gui.tkmaster.bind("<Configure>", drag_event)
+
+      # Pause on opening menu and unpause when click on frames
+      def pause(*_): Gui.paused = True
+      unpause = Gui._unpause_after_wrapper(lambda *_: None)
+
+      Gui.menu["postcommand"] = pause
+      Gui.head_frame.bind("<Button-1>", unpause)
+      Gui.screen_frame.bind("<Button-1>", unpause)
+    ###
+
+    Gui.set_zoom(force=True) # Force set zoom of window
+    Gui.update_data() # Set default data
+    Gui.refresh() # Refresh SDL windows and Tkinter frames
 
+  def center_window():
+    Gui.created()
+    Gui.tkmaster.geometry(f"+{max(0, Gui.tkmaster.winfo_screenwidth() //2-Gui.tkmaster.winfo_width() //2)}"
+                          f"+{max(0, Gui.tkmaster.winfo_screenheight()//2-Gui.tkmaster.winfo_height()//2)}")
+    
   def refresh():
     Gui.created()
     
+    Gui.head.refresh()
+    Draw.rect(Gui.screen_surf, Colors.black)
+    Draw.blit(Gui.screen_surf, Gui.drawable)
+    Gui.screen.refresh()
     Gui.tkmaster.update_idletasks()  
     Gui.tkmaster.update()
-    Gui.head_frame.update()
-    Gui.screen_frame.update()
 
   def screenshot():
     Gui.created()
     Gui.paused = True # Pause events 
-    file = (getcwd(), datetime.now().strftime("Screenshot_%Y%m%d-%H%M%S.png"))
+    file = (getcwd().replace("\\\\", "\\"), datetime.now().strftime("Screenshot_%Y%m%d-%H%M%S.png"))
 
     # Create new surface to blit head and screen into
-    surf = Draw.new_surface(Constants.screen[0], Constants.head_size+Constants.screen[1])
-    Draw.blit(surf, Gui.head.get_surface())
-    Draw.blit(surf, Gui.screen.get_surface(), (0, Constants.head_size))
+    surf = Draw.new_surface(Vars.screen[0], Vars.head_size+Vars.screen[1])
+    Draw.blit(surf, Gui.head_surface)
+    Draw.blit(surf, Gui.drawable, (0, Vars.head_size))
     
     try: error = Config.save_image(surf, file[1]) < 0
     except: error = 1
 
-    conf = {"title": "Screenshot", "text": "Screenshot saved at: \n"+('\\' if Constants.is_windows else '/').join(file), "bitmap": "info", "default": 1, "strings": ("Open folder", "OK")}
+    conf = {"title": "Screenshot", "text": "Screenshot saved at: \n"+('\\' if Vars.is_windows else '/').join(file), "bitmap": "info", "default": 1, "strings": ("Open folder", "OK")}
     if error: conf.update({"text": "Error, can't write in folder: \n"+file[0], "bitmap": "error", "strings": ("Save as", "OK")})
 
     if not Dialog(Gui.tkmaster, conf).num:
       if error: 
-        file = asksaveasfilename(defaultextension="png", filetypes=Constants.image_formats, initialfile=file[1], title="Save screenshot at")
+        file = asksaveasfilename(defaultextension="png", filetypes=Vars.image_formats, initialfile=file[1], title="Save screenshot at")
         if file != '': 
           try: Config.save_image(surf, file)
           except: pass
-      else: system(("explorer \"" if Constants.is_windows else "open \"")+file[0].replace('\\\\', '\\')+'"')
+      else: system(f"{'explorer' if Vars.is_windows else 'open' if Vars.is_macos else 'xdg-open'} \"{file[0]}\" 2> {'nul' if Vars.is_windows else '/dev/null'}")
 
-    del surf # destroy screenshot surface
+    SDL_FreeSurface(surf) # destroy screenshot surface
     if not Gui.already_paused: Gui.paused = False # Screenshot finished, unpause events
 
   def askscriptend():
     return not Dialog(Gui.tkmaster, {
       "title": "Script end", "text": "Script finished! \nClose window?".ljust(50), 
       "bitmap": "question", "default": 0, "strings": ("Yes", "No")
     }).num
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/stuff/ion.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/ion.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/stuff/tests.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/tests.py`

 * *Files identical despite different names*

### Comparing `kandinsky-2.4.dev1/src/kandinsky/util/stuff/vars.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/vars.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from sdl2 import SDL_RWFromFile, SDL_SaveBMP_RW
 from sdl2.sdlimage import IMG_SavePNG_RW, IMG_SaveJPG_RW
 from sdl2.ext.ttf import FontManager
 
-from configparser import ConfigParser
-import os
+import sys, os
 
 __all__ = [
-  "Constants",
+  "Vars",
   "Config",
   "StateData" 
 ]
 
 """
 benchmarks:
  - epsilon:
@@ -39,52 +38,57 @@
 
 magic draw ratio (first draw):
   - epsilon: 02:17.713
   - omega: 02:07.797
   - upsilon: 02:22.141
 """
 
-class Constants:
+class Vars:
   base_name = __module__.split('.')[1]
   path = __file__[:__file__.rindex(base_name)+len(base_name)+1]+"data/"
-  # Test if path correct
+  # Test if path is correct
   if not os.path.exists(path): path = __file__[:__file__.rindex(base_name)]+"data/"
 
-  is_windows = os.name != "posix"
+  is_windows = sys.platform == "win32"
+  is_linux = sys.platform == "linux"
+  is_macos = sys.platform == "darwin"
   app_name = "Kandinsky Emulator"
-  app_icon = None
   head_size = 18
   screen = (320, 222)
+  zoom_ratio = selected_os = selected_model = 1
 
   image_formats = [("PNG", ".png"), ("Bitmap", ".bmp"), ("All files", ".*")]
-  if is_windows: image_formats.insert(1, ("JPEG", (".jpg", ".jpeg")))
+  if not is_macos: image_formats.insert(1, ("JPEG", (".jpg", ".jpeg")))
 
 
 class Config:
   open = lambda path, mode='w': SDL_RWFromFile(path.encode("utf-8"), bytes(mode, "utf-8"))
   save_image = lambda surface, path: (SDL_SaveBMP_RW(surface, Config.open(path), 1) if path.endswith(".bmp") else 
-                                      IMG_SaveJPG_RW(surface, Config.open(path), 1, 70) if Constants.is_windows and path.endswith((".jpg", ".jpeg")) else
+                                      IMG_SaveJPG_RW(surface, Config.open(path), 1, 70) if not Vars.is_macos and path.endswith((".jpg", ".jpeg")) else
                                       IMG_SavePNG_RW(surface, Config.open(path), 1))
 
-  large_font = FontManager(Constants.path+"large_font.ttf", size=16)
-  small_font = FontManager(Constants.path+"small_font.ttf", size=12)
+  large_font = FontManager(Vars.path+"large_font.ttf", size=16)
+  small_font = FontManager(Vars.path+"small_font.ttf", size=12)
 
-  os_list = (
-    {"name": "PC",       "ratio": 0,   "color": "#4a4a4a", "unit": "deg",     "clock": False, "battery": "battery1.png"},
-    {"name": "Numworks", "ratio": 1,   "color": "#ffb531", "unit": "deg",     "clock": False, "battery": "battery0.png"},
-    {"name": "Omega",    "ratio": 0.8, "color": "#c53431", "unit": "sym/deg", "clock": True,  "battery": "battery0.png"},
-    {"name": "Upsilon",  "ratio": 0.9, "color": "#7ea2ce", "unit": "sym/deg", "clock": True,  "battery": "battery1.png"},
+  os_list = (                          #heap in byte, -1=infinite
+    {"name": "PC",       "ratio": 0,   "heap": -1,     "color": "#4a4a4a", "unit": "deg",     "clock": False, "battery": "battery1.png"},
+    {"name": "Numworks", "ratio": 1,   "heap": 65_536, "color": "#ffb531", "unit": "deg",     "clock": False, "battery": "battery0.png"},
+    {"name": "Omega",    "ratio": 0.8, "heap": 99_000, "color": "#c53431", "unit": "sym/deg", "clock": True,  "battery": "battery0.png"},
+    {"name": "Upsilon",  "ratio": 0.9, "heap": 69_500, "color": "#7ea2ce", "unit": "sym/deg", "clock": True,  "battery": "battery1.png"},
   )
-
   model_list = (
     {"name": "n0100", "ratio": 0, "disabled": True},
     {"name": "n0110", "ratio": 1},
     {"name": "n0120", "ratio": 0, "disabled": True},
   )
 
+  default_os = 1
+  default_model = 1
+  zoom_max = 4
+
 # Class for some data
 class StateData:
   __field_name__ = ""
 
   def __init__(self, **content):
     self(**content)
```

### Comparing `kandinsky-2.4.dev1/src/kandinsky.egg-info/SOURCES.txt` & `kandinsky-2.5.dev1/src/kandinsky.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 src/kandinsky/util/data/old_icons.zip
 src/kandinsky/util/data/small_font.ttf
 src/kandinsky/util/stuff/__init__.py
 src/kandinsky/util/stuff/color.py
 src/kandinsky/util/stuff/draw.py
 src/kandinsky/util/stuff/gui.py
 src/kandinsky/util/stuff/ion.py
+src/kandinsky/util/stuff/limiter.py
 src/kandinsky/util/stuff/tests.py
 src/kandinsky/util/stuff/vars.py
```


# Comparing `tmp/gravitypy-1.1.4.tar.gz` & `tmp/gravitypy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.1.4.tar", last modified: Fri May 12 13:20:19 2023, max compression
+gzip compressed data, was "gravitypy-1.1.5.tar", last modified: Fri May 12 13:28:41 2023, max compression
```

## Comparing `gravitypy-1.1.4.tar` & `gravitypy-1.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.4/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.4/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-12 13:20:19.429536 gravitypy-1.1.4/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.1.4/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.425537 gravitypy-1.1.4/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.4/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.1.4/gravitypy/__main__.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/gravitypy/button/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.1.4/gravitypy/button/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      832 2023-05-12 13:06:47.000000 gravitypy-1.1.4/gravitypy/button/button.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      520 2023-05-12 13:14:09.000000 gravitypy-1.1.4/gravitypy/config.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    12201 2023-05-12 13:14:03.000000 gravitypy-1.1.4/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/gravitypy/particle/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.1.4/gravitypy/particle/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2718 2023-05-12 13:14:05.000000 gravitypy-1.1.4/gravitypy/particle/particle.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.425537 gravitypy-1.1.4/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.4/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.425537 gravitypy-1.1.4/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.4/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-12 13:20:19.429536 gravitypy-1.1.4/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      975 2023-05-12 13:19:50.000000 gravitypy-1.1.4/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.575971 gravitypy-1.1.5/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.5/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.5/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-12 13:28:41.575971 gravitypy-1.1.5/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.1.5/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.571972 gravitypy-1.1.5/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.5/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.1.5/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.571972 gravitypy-1.1.5/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.1.5/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      832 2023-05-12 13:06:47.000000 gravitypy-1.1.5/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      666 2023-05-12 13:25:51.000000 gravitypy-1.1.5/gravitypy/config.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    12201 2023-05-12 13:14:03.000000 gravitypy-1.1.5/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.575971 gravitypy-1.1.5/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.1.5/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2718 2023-05-12 13:14:05.000000 gravitypy-1.1.5/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.571972 gravitypy-1.1.5/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.575971 gravitypy-1.1.5/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.5/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:28:41.571972 gravitypy-1.1.5/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-12 13:28:41.000000 gravitypy-1.1.5/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-12 13:28:41.000000 gravitypy-1.1.5/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-12 13:28:41.000000 gravitypy-1.1.5/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-12 13:28:41.000000 gravitypy-1.1.5/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-12 13:28:41.000000 gravitypy-1.1.5/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-12 13:28:41.000000 gravitypy-1.1.5/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.5/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-12 13:28:41.575971 gravitypy-1.1.5/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      975 2023-05-12 13:27:33.000000 gravitypy-1.1.5/setup.py
```

### Comparing `gravitypy-1.1.4/LICENSE` & `gravitypy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.4/README.md` & `gravitypy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.4/gravitypy/button/button.py` & `gravitypy-1.1.5/gravitypy/button/button.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.4/gravitypy/config.py` & `gravitypy-1.1.5/gravitypy/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import pygame
 import random
+import os 
 
 pygame.init()
 pygame.display.set_caption("GravityPy")
 
-FONT = pygame.font.Font('gravitypy/resources/fonts/minecraft_font.ttf', 16)
+current_file = __file__
+current_dir = os.path.dirname(current_file)
+font_file = os.path.join(current_dir, 'resources', 'fonts', 'minecraft_font.ttf')
+font_size = 16
+FONT = pygame.font.Font(font_file, font_size)
 
 WIDTH, HEIGHT = 1200, 700
 SCREEN = pygame.display.set_mode((WIDTH, HEIGHT))
 CLOCK = pygame.time.Clock()
 G = 100
 SCALE = 1.0
 PARTICLES = []
```

### Comparing `gravitypy-1.1.4/gravitypy/main.py` & `gravitypy-1.1.5/gravitypy/main.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.4/gravitypy/particle/particle.py` & `gravitypy-1.1.5/gravitypy/particle/particle.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.4/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.1.5/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.4/setup.py` & `gravitypy-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.1.4',
+   version='1.1.5',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```


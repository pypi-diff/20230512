# Comparing `tmp/gravitypy-1.1.6.tar.gz` & `tmp/gravitypy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.1.6.tar", last modified: Fri May 12 13:48:37 2023, max compression
+gzip compressed data, was "gravitypy-1.1.7.tar", last modified: Fri May 12 13:52:24 2023, max compression
```

## Comparing `gravitypy-1.1.6.tar` & `gravitypy-1.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.636875 gravitypy-1.1.6/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.6/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.6/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-12 13:48:37.636875 gravitypy-1.1.6/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.1.6/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.636875 gravitypy-1.1.6/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.6/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.1.6/gravitypy/__main__.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.636875 gravitypy-1.1.6/gravitypy/button/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.1.6/gravitypy/button/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      832 2023-05-12 13:06:47.000000 gravitypy-1.1.6/gravitypy/button/button.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      666 2023-05-12 13:25:51.000000 gravitypy-1.1.6/gravitypy/config.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    12143 2023-05-12 13:46:23.000000 gravitypy-1.1.6/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.636875 gravitypy-1.1.6/gravitypy/particle/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.1.6/gravitypy/particle/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2718 2023-05-12 13:14:05.000000 gravitypy-1.1.6/gravitypy/particle/particle.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.632875 gravitypy-1.1.6/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.636875 gravitypy-1.1.6/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.6/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:48:37.636875 gravitypy-1.1.6/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-12 13:48:37.000000 gravitypy-1.1.6/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-12 13:48:37.000000 gravitypy-1.1.6/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-12 13:48:37.000000 gravitypy-1.1.6/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-12 13:48:37.000000 gravitypy-1.1.6/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-12 13:48:37.000000 gravitypy-1.1.6/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-12 13:48:37.000000 gravitypy-1.1.6/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.6/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-12 13:48:37.636875 gravitypy-1.1.6/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-05-12 13:47:45.000000 gravitypy-1.1.6/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.427526 gravitypy-1.1.7/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.7/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.7/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-12 13:52:24.427526 gravitypy-1.1.7/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.1.7/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.427526 gravitypy-1.1.7/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.7/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.1.7/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.427526 gravitypy-1.1.7/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.1.7/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      832 2023-05-12 13:06:47.000000 gravitypy-1.1.7/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      666 2023-05-12 13:25:51.000000 gravitypy-1.1.7/gravitypy/config.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    12143 2023-05-12 13:46:23.000000 gravitypy-1.1.7/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.427526 gravitypy-1.1.7/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.1.7/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2718 2023-05-12 13:14:05.000000 gravitypy-1.1.7/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.423526 gravitypy-1.1.7/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.427526 gravitypy-1.1.7/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.7/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:52:24.427526 gravitypy-1.1.7/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-12 13:52:24.000000 gravitypy-1.1.7/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-12 13:52:24.000000 gravitypy-1.1.7/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-12 13:52:24.000000 gravitypy-1.1.7/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-12 13:52:24.000000 gravitypy-1.1.7/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-12 13:52:24.000000 gravitypy-1.1.7/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-12 13:52:24.000000 gravitypy-1.1.7/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.7/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-12 13:52:24.427526 gravitypy-1.1.7/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-05-12 13:52:03.000000 gravitypy-1.1.7/setup.py
```

### Comparing `gravitypy-1.1.6/LICENSE` & `gravitypy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/README.md` & `gravitypy-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/gravitypy/button/button.py` & `gravitypy-1.1.7/gravitypy/button/button.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/gravitypy/config.py` & `gravitypy-1.1.7/gravitypy/config.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/gravitypy/main.py` & `gravitypy-1.1.7/gravitypy/main.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/gravitypy/particle/particle.py` & `gravitypy-1.1.7/gravitypy/particle/particle.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.1.7/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.6/setup.py` & `gravitypy-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.1.6',
+   version='1.1.7',
    description='GravityPy',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/gravityPy",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```


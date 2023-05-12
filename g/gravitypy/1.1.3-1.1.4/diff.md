# Comparing `tmp/gravitypy-1.1.3.tar.gz` & `tmp/gravitypy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.1.3.tar", last modified: Mon May  8 19:11:33 2023, max compression
+gzip compressed data, was "gravitypy-1.1.4.tar", last modified: Fri May 12 13:20:19 2023, max compression
```

## Comparing `gravitypy-1.1.3.tar` & `gravitypy-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.897231 gravitypy-1.1.3/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.3/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.3/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 19:11:33.897231 gravitypy-1.1.3/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1340 2023-05-07 20:40:23.000000 gravitypy-1.1.3/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.893231 gravitypy-1.1.3/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.3/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-08 19:10:52.000000 gravitypy-1.1.3/gravitypy/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15604 2023-05-08 19:10:49.000000 gravitypy-1.1.3/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.893231 gravitypy-1.1.3/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.897231 gravitypy-1.1.3/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.3/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-08 19:11:33.897231 gravitypy-1.1.3/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-08 19:11:33.000000 gravitypy-1.1.3/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.3/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-08 19:11:33.897231 gravitypy-1.1.3/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      973 2023-05-08 19:11:02.000000 gravitypy-1.1.3/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.1.4/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.1.4/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-12 13:20:19.429536 gravitypy-1.1.4/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.1.4/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.425537 gravitypy-1.1.4/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.1.4/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.1.4/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.1.4/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      832 2023-05-12 13:06:47.000000 gravitypy-1.1.4/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      520 2023-05-12 13:14:09.000000 gravitypy-1.1.4/gravitypy/config.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    12201 2023-05-12 13:14:03.000000 gravitypy-1.1.4/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.1.4/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2718 2023-05-12 13:14:05.000000 gravitypy-1.1.4/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.425537 gravitypy-1.1.4/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.429536 gravitypy-1.1.4/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.1.4/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-12 13:20:19.425537 gravitypy-1.1.4/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-12 13:20:19.000000 gravitypy-1.1.4/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.1.4/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-12 13:20:19.429536 gravitypy-1.1.4/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      975 2023-05-12 13:19:50.000000 gravitypy-1.1.4/setup.py
```

### Comparing `gravitypy-1.1.3/LICENSE` & `gravitypy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.3/README.md` & `gravitypy-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Particles_Gravity
+# GravityPy
 ## About Project
 Simulation presents full customizable n-body problem using pygame
 ## Getting Started
 ### Prerequisites
 Download python, pip and check version
 ```
 $ pip3 --version
```

### Comparing `gravitypy-1.1.3/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.1.4/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.1.3/setup.py` & `gravitypy-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.1.3',
+   version='1.1.4',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
    include_package_data=True,
    long_description=LONG_DESCRIPTION,
-   packages=['gravitypy'],
+   packages=find_packages(),
    data_files=[('gravitypy/resources/fonts', ['gravitypy/resources/fonts/minecraft_font.ttf'])],
    install_requires=REQUIREMENTS, 
     entry_points={
         'console_scripts': [
             'gravitypy = gravitypy.__main__:main'
         ]
     },
```


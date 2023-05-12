# Comparing `tmp/segment_studio-0.0.2.tar.gz` & `tmp/segment_studio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment_studio-0.0.2.tar", last modified: Fri May 12 13:17:01 2023, max compression
+gzip compressed data, was "segment_studio-0.0.3.tar", last modified: Fri May 12 13:33:52 2023, max compression
```

## Comparing `segment_studio-0.0.2.tar` & `segment_studio-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shanmuk    (501) staff       (20)        0 2023-05-12 13:17:01.880069 segment_studio-0.0.2/
--rw-r--r--   0 shanmuk    (501) staff       (20)        0 2023-05-09 18:45:45.000000 segment_studio-0.0.2/LICENSE
--rw-r--r--   0 shanmuk    (501) staff       (20)      646 2023-05-12 13:17:01.879944 segment_studio-0.0.2/PKG-INFO
--rw-r--r--   0 shanmuk    (501) staff       (20)      275 2023-05-12 13:14:31.000000 segment_studio-0.0.2/README.md
--rw-r--r--   0 shanmuk    (501) staff       (20)      103 2023-05-10 22:47:30.000000 segment_studio-0.0.2/pyproject.toml
-drwxr-xr-x   0 shanmuk    (501) staff       (20)        0 2023-05-12 13:17:01.879050 segment_studio-0.0.2/segment_studio/
--rw-r--r--   0 shanmuk    (501) staff       (20)        0 2023-05-09 19:37:50.000000 segment_studio-0.0.2/segment_studio/__init__.py
--rw-r--r--   0 shanmuk    (501) staff       (20)    37500 2023-05-11 23:34:29.000000 segment_studio-0.0.2/segment_studio/segment_studio.py
-drwxr-xr-x   0 shanmuk    (501) staff       (20)        0 2023-05-12 13:17:01.879764 segment_studio-0.0.2/segment_studio.egg-info/
--rw-r--r--   0 shanmuk    (501) staff       (20)      646 2023-05-12 13:17:01.000000 segment_studio-0.0.2/segment_studio.egg-info/PKG-INFO
--rw-r--r--   0 shanmuk    (501) staff       (20)      290 2023-05-12 13:17:01.000000 segment_studio-0.0.2/segment_studio.egg-info/SOURCES.txt
--rw-r--r--   0 shanmuk    (501) staff       (20)        1 2023-05-12 13:17:01.000000 segment_studio-0.0.2/segment_studio.egg-info/dependency_links.txt
--rw-r--r--   0 shanmuk    (501) staff       (20)        1 2023-05-12 13:17:01.000000 segment_studio-0.0.2/segment_studio.egg-info/not-zip-safe
--rw-r--r--   0 shanmuk    (501) staff       (20)       15 2023-05-12 13:17:01.000000 segment_studio-0.0.2/segment_studio.egg-info/top_level.txt
--rw-r--r--   0 shanmuk    (501) staff       (20)       38 2023-05-12 13:17:01.880129 segment_studio-0.0.2/setup.cfg
--rw-r--r--   0 shanmuk    (501) staff       (20)     1611 2023-05-12 13:16:53.000000 segment_studio-0.0.2/setup.py
+drwxr-xr-x   0 shanmuk    (501) staff       (20)        0 2023-05-12 13:33:52.662395 segment_studio-0.0.3/
+-rw-r--r--   0 shanmuk    (501) staff       (20)        0 2023-05-09 18:45:45.000000 segment_studio-0.0.3/LICENSE
+-rw-r--r--   0 shanmuk    (501) staff       (20)     1037 2023-05-12 13:33:52.662269 segment_studio-0.0.3/PKG-INFO
+-rw-r--r--   0 shanmuk    (501) staff       (20)      666 2023-05-12 13:33:29.000000 segment_studio-0.0.3/README.md
+-rw-r--r--   0 shanmuk    (501) staff       (20)      103 2023-05-10 22:47:30.000000 segment_studio-0.0.3/pyproject.toml
+drwxr-xr-x   0 shanmuk    (501) staff       (20)        0 2023-05-12 13:33:52.661419 segment_studio-0.0.3/segment_studio/
+-rw-r--r--   0 shanmuk    (501) staff       (20)        0 2023-05-09 19:37:50.000000 segment_studio-0.0.3/segment_studio/__init__.py
+-rw-r--r--   0 shanmuk    (501) staff       (20)    37500 2023-05-11 23:34:29.000000 segment_studio-0.0.3/segment_studio/segment_studio.py
+drwxr-xr-x   0 shanmuk    (501) staff       (20)        0 2023-05-12 13:33:52.662101 segment_studio-0.0.3/segment_studio.egg-info/
+-rw-r--r--   0 shanmuk    (501) staff       (20)     1037 2023-05-12 13:33:52.000000 segment_studio-0.0.3/segment_studio.egg-info/PKG-INFO
+-rw-r--r--   0 shanmuk    (501) staff       (20)      290 2023-05-12 13:33:52.000000 segment_studio-0.0.3/segment_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmuk    (501) staff       (20)        1 2023-05-12 13:33:52.000000 segment_studio-0.0.3/segment_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmuk    (501) staff       (20)        1 2023-05-12 13:33:52.000000 segment_studio-0.0.3/segment_studio.egg-info/not-zip-safe
+-rw-r--r--   0 shanmuk    (501) staff       (20)       15 2023-05-12 13:33:52.000000 segment_studio-0.0.3/segment_studio.egg-info/top_level.txt
+-rw-r--r--   0 shanmuk    (501) staff       (20)       38 2023-05-12 13:33:52.662437 segment_studio-0.0.3/setup.cfg
+-rw-r--r--   0 shanmuk    (501) staff       (20)     1611 2023-05-12 13:33:32.000000 segment_studio-0.0.3/setup.py
```

### Comparing `segment_studio-0.0.2/segment_studio/segment_studio.py` & `segment_studio-0.0.3/segment_studio/segment_studio.py`

 * *Files identical despite different names*

### Comparing `segment_studio-0.0.2/setup.py` & `segment_studio-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='segment_studio',
-    version='0.0.2',
+    version='0.0.3',
     description='Segmentation Studio',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
     'Programming Language :: Python :: 3.9',
     ],
     keywords='object detection image editor segmention',
```


# Comparing `tmp/qcew-0.0.1.tar.gz` & `tmp/qcew-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcew-0.0.1.tar", last modified: Fri May 12 16:30:07 2023, max compression
+gzip compressed data, was "qcew-0.0.2.tar", last modified: Fri May 12 16:38:15 2023, max compression
```

## Comparing `qcew-0.0.1.tar` & `qcew-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 16:30:07.488226 qcew-0.0.1/
--rw-r--r--   0 TrentThompson   (501) staff       (20)     1090 2023-05-12 11:30:42.000000 qcew-0.0.1/LICENSE
--rw-r--r--   0 TrentThompson   (501) staff       (20)      408 2023-05-12 16:30:07.487739 qcew-0.0.1/PKG-INFO
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2125 2023-05-12 11:30:42.000000 qcew-0.0.1/README.md
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 16:30:07.487094 qcew-0.0.1/qcew.egg-info/
--rw-r--r--   0 TrentThompson   (501) staff       (20)      408 2023-05-12 16:30:07.000000 qcew-0.0.1/qcew.egg-info/PKG-INFO
--rw-r--r--   0 TrentThompson   (501) staff       (20)      138 2023-05-12 16:30:07.000000 qcew-0.0.1/qcew.egg-info/SOURCES.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 16:30:07.000000 qcew-0.0.1/qcew.egg-info/dependency_links.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 16:30:07.000000 qcew-0.0.1/qcew.egg-info/top_level.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)       38 2023-05-12 16:30:07.488368 qcew-0.0.1/setup.cfg
--rw-r--r--   0 TrentThompson   (501) staff       (20)      585 2023-05-12 11:30:42.000000 qcew-0.0.1/setup.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 16:38:15.796342 qcew-0.0.2/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     1090 2023-05-12 11:30:42.000000 qcew-0.0.2/LICENSE
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2489 2023-05-12 16:38:15.795713 qcew-0.0.2/PKG-INFO
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2125 2023-05-12 11:30:42.000000 qcew-0.0.2/README.md
+-rw-r--r--   0 TrentThompson   (501) staff       (20)       38 2023-05-12 16:38:15.796472 qcew-0.0.2/setup.cfg
+-rw-r--r--   0 TrentThompson   (501) staff       (20)      688 2023-05-12 16:38:01.000000 qcew-0.0.2/setup.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 16:38:15.777028 qcew-0.0.2/src/
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 16:38:15.790393 qcew-0.0.2/src/qcew/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 11:30:42.000000 qcew-0.0.2/src/qcew/__init__.py
+-rw-r--r--   0 TrentThompson   (501) staff       (20)    11681 2023-05-12 11:30:42.000000 qcew-0.0.2/src/qcew/qcew.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 16:38:15.795112 qcew-0.0.2/src/qcew.egg-info/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2489 2023-05-12 16:38:15.000000 qcew-0.0.2/src/qcew.egg-info/PKG-INFO
+-rw-r--r--   0 TrentThompson   (501) staff       (20)      192 2023-05-12 16:38:15.000000 qcew-0.0.2/src/qcew.egg-info/SOURCES.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 16:38:15.000000 qcew-0.0.2/src/qcew.egg-info/dependency_links.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        5 2023-05-12 16:38:15.000000 qcew-0.0.2/src/qcew.egg-info/top_level.txt
```

### Comparing `qcew-0.0.1/LICENSE` & `qcew-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qcew-0.0.1/README.md` & `qcew-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qcew-0.0.1/setup.py` & `qcew-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from setuptools import setup, find_packages
+from setuptools import setup
+from pathlib import Path
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "A package for slicing QCEW data."
 
 setup(
     name="qcew",
     version=VERSION,
     author="Trent Thompson",
     author_email="808trent@gmail.com",
     description=DESCRIPTION,
-    packages=find_packages(),
+    long_description=(Path(__file__).parent/"README.md").read_text(),
+    long_description_content_type='text/markdown',
     keywords=["QCEW", "BLS", "employment", "wages", "statistics"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```


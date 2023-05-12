# Comparing `tmp/mecsimcalc-0.0.3.tar.gz` & `tmp/mecsimcalc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecsimcalc-0.0.3.tar", last modified: Tue May  9 01:53:37 2023, max compression
+gzip compressed data, was "mecsimcalc-0.0.4.tar", last modified: Fri May 12 09:18:30 2023, max compression
```

## Comparing `mecsimcalc-0.0.3.tar` & `mecsimcalc-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:37.303190 mecsimcalc-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 01:53:22.000000 mecsimcalc-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-09 01:53:37.303190 mecsimcalc-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 01:53:22.000000 mecsimcalc-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:37.303190 mecsimcalc-0.0.3/mecsimcalc/
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-09 01:53:22.000000 mecsimcalc-0.0.3/mecsimcalc/MecSimCalc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:22.000000 mecsimcalc-0.0.3/mecsimcalc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:37.303190 mecsimcalc-0.0.3/mecsimcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-09 01:53:37.000000 mecsimcalc-0.0.3/mecsimcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 01:53:37.000000 mecsimcalc-0.0.3/mecsimcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:53:37.000000 mecsimcalc-0.0.3/mecsimcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 01:53:37.000000 mecsimcalc-0.0.3/mecsimcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 01:53:37.000000 mecsimcalc-0.0.3/mecsimcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:53:37.303190 mecsimcalc-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-09 01:53:22.000000 mecsimcalc-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/mecsimcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/mecsimcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/mecsimcalc/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/mecsimcalc/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/mecsimcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 09:18:30.000000 mecsimcalc-0.0.4/mecsimcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:18:30.227098 mecsimcalc-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-12 09:18:19.000000 mecsimcalc-0.0.4/setup.py
```

### Comparing `mecsimcalc-0.0.3/LICENSE` & `mecsimcalc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.0.3/setup.py` & `mecsimcalc-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Useful functions for MecSimCalc.com"
 LONG_DESCRIPTION = "Useful functions for MecSimCalc.com"
 
 # Setting up
 setup(
     name="mecsimcalc",
     version=VERSION,
     author="MecSimCalc",
     author_email="<info@mecsimcalc.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=["Pillow", "pandas"],
+    install_requires=["Pillow", "pandas", "matplotlib"],
     keywords=["python", "MecSimCalc", "Calculator", "Simple"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```


# Comparing `tmp/scubas-0.1.3.tar.gz` & `tmp/scubas-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scubas-0.1.3.tar", last modified: Fri May 12 02:31:57 2023, max compression
+gzip compressed data, was "scubas-0.1.4.tar", last modified: Fri May 12 02:39:50 2023, max compression
```

## Comparing `scubas-0.1.3.tar` & `scubas-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:31:57.836293 scubas-0.1.3/
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1076 2023-02-09 21:26:26.000000 scubas-0.1.3/LICENSE
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2693 2023-05-12 02:31:57.836293 scubas-0.1.3/PKG-INFO
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1671 2023-05-12 00:59:59.000000 scubas-0.1.3/README.md
-drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:31:57.836293 scubas-0.1.3/scubas/
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       22 2023-02-15 16:56:39.000000 scubas-0.1.3/scubas/__init__.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    19544 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas/cables.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    21360 2023-02-18 02:47:03.000000 scubas-0.1.3/scubas/conductivity.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    12799 2023-03-02 22:44:14.000000 scubas-0.1.3/scubas/datasets.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     8959 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas/models.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     3784 2023-02-25 03:24:06.000000 scubas-0.1.3/scubas/plotlib.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2008 2023-05-12 01:48:19.000000 scubas-0.1.3/scubas/utils.py
-drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:31:57.836293 scubas-0.1.3/scubas.egg-info/
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2693 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/PKG-INFO
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      304 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/SOURCES.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        1 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/dependency_links.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       56 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/requires.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        7 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/top_level.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       38 2023-05-12 02:31:57.836293 scubas-0.1.3/setup.cfg
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1755 2023-05-12 01:29:56.000000 scubas-0.1.3/setup.py
+drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:39:50.488288 scubas-0.1.4/
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1076 2023-02-09 21:26:26.000000 scubas-0.1.4/LICENSE
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2639 2023-05-12 02:39:50.488288 scubas-0.1.4/PKG-INFO
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1671 2023-05-12 00:59:59.000000 scubas-0.1.4/README.md
+drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:39:50.488288 scubas-0.1.4/scubas/
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       22 2023-02-15 16:56:39.000000 scubas-0.1.4/scubas/__init__.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    19544 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas/cables.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    21360 2023-02-18 02:47:03.000000 scubas-0.1.4/scubas/conductivity.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    12799 2023-03-02 22:44:14.000000 scubas-0.1.4/scubas/datasets.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     8959 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas/models.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     3784 2023-02-25 03:24:06.000000 scubas-0.1.4/scubas/plotlib.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2008 2023-05-12 01:48:19.000000 scubas-0.1.4/scubas/utils.py
+drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:39:50.488288 scubas-0.1.4/scubas.egg-info/
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2639 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas.egg-info/PKG-INFO
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      304 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas.egg-info/SOURCES.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        1 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas.egg-info/dependency_links.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       56 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas.egg-info/requires.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        7 2023-05-12 02:39:50.000000 scubas-0.1.4/scubas.egg-info/top_level.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       38 2023-05-12 02:39:50.488288 scubas-0.1.4/setup.cfg
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1701 2023-05-12 02:39:45.000000 scubas-0.1.4/setup.py
```

### Comparing `scubas-0.1.3/LICENSE` & `scubas-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/PKG-INFO` & `scubas-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: scubas
-Version: 0.1.3
+Version: 0.1.4
 Summary: SCUBAS: Submarine Cables Upset by Auroral Streams.
 Home-page: https://github.com/shibaji7/SCUBAS
 Author: Shibaji Chakraborty
 Author-email: shibaji7@vt.edu
 Maintainer: Shibaji Chakraborty
 Maintainer-email: shibaji7@vt.edu
 License: MIT License
-Project-URL: Home, https://github.com/shibaji7/SCUBAS
 Project-URL: Documentations, https://scubas.readthedocs.io/en/latest/
 Keywords: Python>=3.6,submarine cable,electrical surge,geomagnetic induction,geomagnetic disturbance
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scubas-0.1.3/README.md` & `scubas-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas/cables.py` & `scubas-0.1.4/scubas/cables.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas/conductivity.py` & `scubas-0.1.4/scubas/conductivity.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas/datasets.py` & `scubas-0.1.4/scubas/datasets.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas/models.py` & `scubas-0.1.4/scubas/models.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas/plotlib.py` & `scubas-0.1.4/scubas/plotlib.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas/utils.py` & `scubas-0.1.4/scubas/utils.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.3/scubas.egg-info/PKG-INFO` & `scubas-0.1.4/scubas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: scubas
-Version: 0.1.3
+Version: 0.1.4
 Summary: SCUBAS: Submarine Cables Upset by Auroral Streams.
 Home-page: https://github.com/shibaji7/SCUBAS
 Author: Shibaji Chakraborty
 Author-email: shibaji7@vt.edu
 Maintainer: Shibaji Chakraborty
 Maintainer-email: shibaji7@vt.edu
 License: MIT License
-Project-URL: Home, https://github.com/shibaji7/SCUBAS
 Project-URL: Documentations, https://scubas.readthedocs.io/en/latest/
 Keywords: Python>=3.6,submarine cable,electrical surge,geomagnetic induction,geomagnetic disturbance
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scubas-0.1.3/setup.py` & `scubas-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="scubas",
-    version="0.1.3",
+    version="0.1.4",
     packages=["scubas"],
     package_dir={"scubas": "scubas"},
     package_data={"scubas": []},
     author="Shibaji Chakraborty",
     author_email="shibaji7@vt.edu",
     maintainer="Shibaji Chakraborty",
     maintainer_email="shibaji7@vt.edu",
@@ -44,12 +44,11 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     project_urls={
-        "Home": "https://github.com/shibaji7/SCUBAS",
         "Documentations": "https://scubas.readthedocs.io/en/latest/",
     },
     url="https://github.com/shibaji7/SCUBAS",
 )
```


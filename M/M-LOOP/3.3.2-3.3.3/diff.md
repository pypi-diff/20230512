# Comparing `tmp/M-LOOP-3.3.2.tar.gz` & `tmp/M-LOOP-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "M-LOOP-3.3.2.tar", last modified: Thu Mar 16 22:38:29 2023, max compression
+gzip compressed data, was "M-LOOP-3.3.3.tar", last modified: Fri May 12 20:05:29 2023, max compression
```

## Comparing `M-LOOP-3.3.2.tar` & `M-LOOP-3.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zak       (1000) zak       (1000)        0 2023-03-16 22:38:29.138870 M-LOOP-3.3.2/
--rw-rw-r--   0 zak       (1000) zak       (1000)     1080 2021-12-01 19:28:07.000000 M-LOOP-3.3.2/LICENSE.txt
-drwxrwxr-x   0 zak       (1000) zak       (1000)        0 2023-03-16 22:38:29.134870 M-LOOP-3.3.2/M_LOOP.egg-info/
--rw-rw-r--   0 zak       (1000) zak       (1000)     1643 2023-03-16 22:38:28.000000 M-LOOP-3.3.2/M_LOOP.egg-info/PKG-INFO
--rw-rw-r--   0 zak       (1000) zak       (1000)      411 2023-03-16 22:38:29.000000 M-LOOP-3.3.2/M_LOOP.egg-info/SOURCES.txt
--rw-rw-r--   0 zak       (1000) zak       (1000)        1 2023-03-16 22:38:28.000000 M-LOOP-3.3.2/M_LOOP.egg-info/dependency_links.txt
--rw-rw-r--   0 zak       (1000) zak       (1000)       47 2023-03-16 22:38:28.000000 M-LOOP-3.3.2/M_LOOP.egg-info/entry_points.txt
--rw-rw-r--   0 zak       (1000) zak       (1000)      112 2023-03-16 22:38:28.000000 M-LOOP-3.3.2/M_LOOP.egg-info/requires.txt
--rw-rw-r--   0 zak       (1000) zak       (1000)        6 2023-03-16 22:38:28.000000 M-LOOP-3.3.2/M_LOOP.egg-info/top_level.txt
--rw-rw-r--   0 zak       (1000) zak       (1000)     1643 2023-03-16 22:38:29.138870 M-LOOP-3.3.2/PKG-INFO
--rw-rw-r--   0 zak       (1000) zak       (1000)      794 2021-12-01 19:28:07.000000 M-LOOP-3.3.2/README.rst
-drwxrwxr-x   0 zak       (1000) zak       (1000)        0 2023-03-16 22:38:29.138870 M-LOOP-3.3.2/mloop/
--rw-rw-r--   0 zak       (1000) zak       (1000)      747 2023-03-16 22:35:58.000000 M-LOOP-3.3.2/mloop/__init__.py
--rw-rw-r--   0 zak       (1000) zak       (1000)     1179 2021-12-01 19:28:07.000000 M-LOOP-3.3.2/mloop/cmd.py
--rw-rw-r--   0 zak       (1000) zak       (1000)    49588 2022-08-01 20:41:48.000000 M-LOOP-3.3.2/mloop/controllers.py
--rw-rw-r--   0 zak       (1000) zak       (1000)    16239 2022-03-14 22:40:45.000000 M-LOOP-3.3.2/mloop/interfaces.py
--rw-rw-r--   0 zak       (1000) zak       (1000)     2531 2021-12-01 19:28:07.000000 M-LOOP-3.3.2/mloop/launchers.py
--rw-rw-r--   0 zak       (1000) zak       (1000)   147358 2023-02-14 01:09:11.000000 M-LOOP-3.3.2/mloop/learners.py
--rw-rw-r--   0 zak       (1000) zak       (1000)    35519 2022-04-28 16:20:29.000000 M-LOOP-3.3.2/mloop/neuralnet.py
--rw-rw-r--   0 zak       (1000) zak       (1000)     9722 2022-04-28 16:20:29.000000 M-LOOP-3.3.2/mloop/testing.py
--rw-rw-r--   0 zak       (1000) zak       (1000)    19425 2023-02-10 21:00:09.000000 M-LOOP-3.3.2/mloop/utilities.py
--rw-rw-r--   0 zak       (1000) zak       (1000)    81991 2022-06-13 09:31:03.000000 M-LOOP-3.3.2/mloop/visualizations.py
--rw-rw-r--   0 zak       (1000) zak       (1000)      105 2023-03-16 22:38:29.138870 M-LOOP-3.3.2/setup.cfg
--rw-rw-r--   0 zak       (1000) zak       (1000)     2901 2023-03-16 22:35:58.000000 M-LOOP-3.3.2/setup.py
+drwxrwxr-x   0 zak       (1000) zak       (1000)        0 2023-05-12 20:05:29.242095 M-LOOP-3.3.3/
+-rw-rw-r--   0 zak       (1000) zak       (1000)     1080 2021-12-01 19:28:07.000000 M-LOOP-3.3.3/LICENSE.txt
+drwxrwxr-x   0 zak       (1000) zak       (1000)        0 2023-05-12 20:05:29.242095 M-LOOP-3.3.3/M_LOOP.egg-info/
+-rw-rw-r--   0 zak       (1000) zak       (1000)     1643 2023-05-12 20:05:28.000000 M-LOOP-3.3.3/M_LOOP.egg-info/PKG-INFO
+-rw-rw-r--   0 zak       (1000) zak       (1000)      411 2023-05-12 20:05:29.000000 M-LOOP-3.3.3/M_LOOP.egg-info/SOURCES.txt
+-rw-rw-r--   0 zak       (1000) zak       (1000)        1 2023-05-12 20:05:28.000000 M-LOOP-3.3.3/M_LOOP.egg-info/dependency_links.txt
+-rw-rw-r--   0 zak       (1000) zak       (1000)       47 2023-05-12 20:05:28.000000 M-LOOP-3.3.3/M_LOOP.egg-info/entry_points.txt
+-rw-rw-r--   0 zak       (1000) zak       (1000)      194 2023-05-12 20:05:29.000000 M-LOOP-3.3.3/M_LOOP.egg-info/requires.txt
+-rw-rw-r--   0 zak       (1000) zak       (1000)        6 2023-05-12 20:05:29.000000 M-LOOP-3.3.3/M_LOOP.egg-info/top_level.txt
+-rw-rw-r--   0 zak       (1000) zak       (1000)     1643 2023-05-12 20:05:29.242095 M-LOOP-3.3.3/PKG-INFO
+-rw-rw-r--   0 zak       (1000) zak       (1000)      794 2021-12-01 19:28:07.000000 M-LOOP-3.3.3/README.rst
+drwxrwxr-x   0 zak       (1000) zak       (1000)        0 2023-05-12 20:05:29.242095 M-LOOP-3.3.3/mloop/
+-rw-rw-r--   0 zak       (1000) zak       (1000)      747 2023-05-12 20:04:06.000000 M-LOOP-3.3.3/mloop/__init__.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)     1179 2021-12-01 19:28:07.000000 M-LOOP-3.3.3/mloop/cmd.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)    49588 2022-08-01 20:41:48.000000 M-LOOP-3.3.3/mloop/controllers.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)    16239 2022-03-14 22:40:45.000000 M-LOOP-3.3.3/mloop/interfaces.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)     2531 2021-12-01 19:28:07.000000 M-LOOP-3.3.3/mloop/launchers.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)   147358 2023-02-14 01:09:11.000000 M-LOOP-3.3.3/mloop/learners.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)    35519 2022-04-28 16:20:29.000000 M-LOOP-3.3.3/mloop/neuralnet.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)     9722 2022-04-28 16:20:29.000000 M-LOOP-3.3.3/mloop/testing.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)    19425 2023-02-10 21:00:09.000000 M-LOOP-3.3.3/mloop/utilities.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)    81991 2022-06-13 09:31:03.000000 M-LOOP-3.3.3/mloop/visualizations.py
+-rw-rw-r--   0 zak       (1000) zak       (1000)      105 2023-05-12 20:05:29.246095 M-LOOP-3.3.3/setup.cfg
+-rw-rw-r--   0 zak       (1000) zak       (1000)     2992 2023-05-12 20:04:06.000000 M-LOOP-3.3.3/setup.py
```

### Comparing `M-LOOP-3.3.2/LICENSE.txt` & `M-LOOP-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/M_LOOP.egg-info/PKG-INFO` & `M-LOOP-3.3.3/M_LOOP.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: M-LOOP
-Version: 3.3.2
+Version: 3.3.3
 Summary: M-LOOP: Machine-learning online optimization package. A python package of automated optimization tools - enhanced with machine-learning - for quantum scientific experiments, computer controlled systems or other optimization tasks.
 Home-page: https://github.com/michaelhush/M-LOOP/
-Download-URL: https://github.com/michaelhush/M-LOOP/tarball/v3.3.2
+Download-URL: https://github.com/michaelhush/M-LOOP/tarball/v3.3.3
 Author: Michael R Hush
 Author-email: MichaelRHush@gmail.com
 License: MIT
 Keywords: automated machine learning optimization optimisation science experiment quantum
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `M-LOOP-3.3.2/PKG-INFO` & `M-LOOP-3.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: M-LOOP
-Version: 3.3.2
+Version: 3.3.3
 Summary: M-LOOP: Machine-learning online optimization package. A python package of automated optimization tools - enhanced with machine-learning - for quantum scientific experiments, computer controlled systems or other optimization tasks.
 Home-page: https://github.com/michaelhush/M-LOOP/
-Download-URL: https://github.com/michaelhush/M-LOOP/tarball/v3.3.2
+Download-URL: https://github.com/michaelhush/M-LOOP/tarball/v3.3.3
 Author: Michael R Hush
 Author-email: MichaelRHush@gmail.com
 License: MIT
 Keywords: automated machine learning optimization optimisation science experiment quantum
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `M-LOOP-3.3.2/README.rst` & `M-LOOP-3.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/__init__.py` & `M-LOOP-3.3.3/mloop/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 To contribute to the project or report a bug visit the project's github https://github.com/michaelhush/M-LOOP.
 '''
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os
 
-__version__ = '3.3.2'
+__version__ = '3.3.3'
 __all__ = ['controllers','interfaces','launchers','learners','nnlearner','testing','utilities','visualizations','cmd']
```

### Comparing `M-LOOP-3.3.2/mloop/cmd.py` & `M-LOOP-3.3.3/mloop/cmd.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/controllers.py` & `M-LOOP-3.3.3/mloop/controllers.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/interfaces.py` & `M-LOOP-3.3.3/mloop/interfaces.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/launchers.py` & `M-LOOP-3.3.3/mloop/launchers.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/learners.py` & `M-LOOP-3.3.3/mloop/learners.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/neuralnet.py` & `M-LOOP-3.3.3/mloop/neuralnet.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/testing.py` & `M-LOOP-3.3.3/mloop/testing.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/utilities.py` & `M-LOOP-3.3.3/mloop/utilities.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/mloop/visualizations.py` & `M-LOOP-3.3.3/mloop/visualizations.py`

 * *Files identical despite different names*

### Comparing `M-LOOP-3.3.2/setup.py` & `M-LOOP-3.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,29 +31,30 @@
             'pip>=7.0',
             'docutils>=0.3',
             'numpy>=1.11',
             'scipy>=0.17',
             'matplotlib>=1.5',
             'pytest>=2.9',
             'scikit-learn>=0.18',
-            'tensorflow>=2.0.0',
+            'tensorflow>=2.0.0; sys_platform != "darwin"',
+            'tensorflow-macos>=2.0.0; sys_platform == "darwin"',
         ],
         tests_require=['pytest', 'setuptools>=26'],
         package_data = {
             # If any package contains *.txt or *.rst files, include them:
             '': ['*.txt','*.md'],
         },
         author = 'Michael R Hush',
         author_email = 'MichaelRHush@gmail.com',
         description = 'M-LOOP: Machine-learning online optimization package. A python package of automated optimization tools - enhanced with machine-learning - for quantum scientific experiments, computer controlled systems or other optimization tasks.',
         long_description = long_description,
         license = 'MIT',
         keywords = 'automated machine learning optimization optimisation science experiment quantum',
         url = 'https://github.com/michaelhush/M-LOOP/', 
-        download_url = 'https://github.com/michaelhush/M-LOOP/tarball/v3.3.2',
+        download_url = 'https://github.com/michaelhush/M-LOOP/tarball/v3.3.3',
         classifiers = [
             'Development Status :: 2 - Pre-Alpha',
             'Intended Audience :: Science/Research',
             'Intended Audience :: Manufacturing',
             'License :: OSI Approved :: MIT License',
             'Natural Language :: English',
             'Operating System :: MacOS :: MacOS X',
```


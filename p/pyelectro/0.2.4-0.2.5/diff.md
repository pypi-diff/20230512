# Comparing `tmp/pyelectro-0.2.4.tar.gz` & `tmp/pyelectro-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyelectro-0.2.4.tar", last modified: Tue Feb 22 13:01:11 2022, max compression
+gzip compressed data, was "pyelectro-0.2.5.tar", last modified: Fri May 12 16:44:17 2023, max compression
```

## Comparing `pyelectro-0.2.4.tar` & `pyelectro-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-02-22 13:01:11.000000 pyelectro-0.2.4/
--rw-r--r--   0 padraig    (501) staff       (20)      843 2022-02-22 13:01:11.000000 pyelectro-0.2.4/PKG-INFO
--rw-r--r--   0 padraig    (501) staff       (20)     1632 2021-11-24 09:15:14.000000 pyelectro-0.2.4/README.md
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-02-22 13:01:11.000000 pyelectro-0.2.4/pyelectro/
--rw-r--r--   0 padraig    (501) staff       (20)       90 2022-02-22 13:00:31.000000 pyelectro-0.2.4/pyelectro/__init__.py
--rw-r--r--   0 padraig    (501) staff       (20)    54334 2021-12-13 12:50:05.000000 pyelectro-0.2.4/pyelectro/analysis.py
--rw-r--r--   0 padraig    (501) staff       (20)     1907 2021-12-13 12:50:05.000000 pyelectro-0.2.4/pyelectro/io.py
--rw-r--r--   0 padraig    (501) staff       (20)     6191 2021-12-13 12:50:05.000000 pyelectro-0.2.4/pyelectro/utils.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-02-22 13:01:11.000000 pyelectro-0.2.4/pyelectro.egg-info/
--rw-r--r--   0 padraig    (501) staff       (20)      843 2022-02-22 13:01:10.000000 pyelectro-0.2.4/pyelectro.egg-info/PKG-INFO
--rw-r--r--   0 padraig    (501) staff       (20)      293 2022-02-22 13:01:10.000000 pyelectro-0.2.4/pyelectro.egg-info/SOURCES.txt
--rw-r--r--   0 padraig    (501) staff       (20)        1 2022-02-22 13:01:10.000000 pyelectro-0.2.4/pyelectro.egg-info/dependency_links.txt
--rw-r--r--   0 padraig    (501) staff       (20)       23 2022-02-22 13:01:10.000000 pyelectro-0.2.4/pyelectro.egg-info/requires.txt
--rw-r--r--   0 padraig    (501) staff       (20)       10 2022-02-22 13:01:10.000000 pyelectro-0.2.4/pyelectro.egg-info/top_level.txt
--rw-r--r--   0 padraig    (501) staff       (20)      163 2022-02-22 13:01:11.000000 pyelectro-0.2.4/setup.cfg
--rw-r--r--   0 padraig    (501) staff       (20)     1117 2022-02-22 13:00:31.000000 pyelectro-0.2.4/setup.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-02-22 13:01:11.000000 pyelectro-0.2.4/test/
--rw-r--r--   0 padraig    (501) staff       (20)     9098 2021-12-13 12:50:05.000000 pyelectro-0.2.4/test/test_analysis.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:44:17.923421 pyelectro-0.2.5/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1501 2023-05-12 16:43:11.000000 pyelectro-0.2.5/LICENSE
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     2502 2023-05-12 16:44:17.923421 pyelectro-0.2.5/PKG-INFO
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1632 2021-11-25 09:49:14.000000 pyelectro-0.2.5/README.md
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:44:17.923421 pyelectro-0.2.5/pyelectro/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       90 2023-05-12 16:43:11.000000 pyelectro-0.2.5/pyelectro/__init__.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)    54334 2021-12-02 17:14:22.000000 pyelectro-0.2.5/pyelectro/analysis.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1907 2021-12-02 17:14:22.000000 pyelectro-0.2.5/pyelectro/io.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     6191 2021-12-02 17:14:22.000000 pyelectro-0.2.5/pyelectro/utils.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:44:17.923421 pyelectro-0.2.5/pyelectro.egg-info/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     2502 2023-05-12 16:44:17.000000 pyelectro-0.2.5/pyelectro.egg-info/PKG-INFO
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)      301 2023-05-12 16:44:17.000000 pyelectro-0.2.5/pyelectro.egg-info/SOURCES.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)        1 2023-05-12 16:44:17.000000 pyelectro-0.2.5/pyelectro.egg-info/dependency_links.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       23 2023-05-12 16:44:17.000000 pyelectro-0.2.5/pyelectro.egg-info/requires.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       10 2023-05-12 16:44:17.000000 pyelectro-0.2.5/pyelectro.egg-info/top_level.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)      163 2023-05-12 16:44:17.923421 pyelectro-0.2.5/setup.cfg
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1256 2023-05-12 16:43:11.000000 pyelectro-0.2.5/setup.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:44:17.923421 pyelectro-0.2.5/test/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     9098 2021-11-25 09:49:14.000000 pyelectro-0.2.5/test/test_analysis.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyelectro-0.2.4/README.md` & `pyelectro-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.4/pyelectro/analysis.py` & `pyelectro-0.2.5/pyelectro/analysis.py`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.4/pyelectro/io.py` & `pyelectro-0.2.5/pyelectro/io.py`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.4/pyelectro/utils.py` & `pyelectro-0.2.5/pyelectro/utils.py`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.4/setup.py` & `pyelectro-0.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 
 from setuptools import setup
 
 for line in open("pyelectro/__init__.py"):
     if line.startswith("__version__"):
         version = line.split("=")[1].strip()[1:-1]
 
+
+long_description = open("README.md").read()
+
 setup(
     name="pyelectro",
     version=version,
     packages=["pyelectro"],
     author="Michael Vella, Padraig Gleeson",
     author_email="mv333@cam.ac.uk, p.gleeson@gmail.com",
     description="A Python library for analysis of electrophysiological data",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/NeuralEnsemble/pyelectro",
     install_requires=["numpy", "scipy", "matplotlib"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
 )
```

### Comparing `pyelectro-0.2.4/test/test_analysis.py` & `pyelectro-0.2.5/test/test_analysis.py`

 * *Files identical despite different names*


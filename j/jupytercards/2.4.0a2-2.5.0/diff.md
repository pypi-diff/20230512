# Comparing `tmp/jupytercards-2.4.0a2.tar.gz` & `tmp/jupytercards-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.4.0a2.tar", last modified: Fri May 12 13:14:23 2023, max compression
+gzip compressed data, was "jupytercards-2.5.0.tar", last modified: Fri May 12 13:17:33 2023, max compression
```

## Comparing `jupytercards-2.4.0a2.tar` & `jupytercards-2.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.4.0a2/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.4.0a2/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.4.0a2/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.4.0a2/README.md
--rw-r--r--   0        0        0    28114 2023-05-12 13:13:49.880352 jupytercards-2.4.0a2/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.4.0a2/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.4.0a2/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.4.0a2/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      659 2023-05-12 13:14:20.597363 jupytercards-2.4.0a2/jupytercards/__init__.py
--rw-r--r--   0        0        0     9589 2023-05-12 13:11:52.978482 jupytercards-2.4.0a2/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.4.0a2/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.4.0a2/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.4.0a2/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.4.0a2/pyproject.toml
--rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 jupytercards-2.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.0/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.0/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.5.0/README.md
+-rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.0/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.0/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.0/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.0/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-05-12 13:16:10.062152 jupytercards-2.5.0/jupytercards/__init__.py
+-rw-r--r--   0        0        0     9589 2023-05-12 13:11:52.978482 jupytercards-2.5.0/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.5.0/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.5.0/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.0/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.5.0/PKG-INFO
```

### Comparing `jupytercards-2.4.0a2/.gitignore` & `jupytercards-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/LICENSE` & `jupytercards-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/Markdown-flashcards.ipynb` & `jupytercards-2.5.0/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/README.md` & `jupytercards-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/example.ipynb` & `jupytercards-2.5.0/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/extractdefinitions.py` & `jupytercards-2.5.0/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/flashcards.gif` & `jupytercards-2.5.0/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/jupytercards/__init__.py` & `jupytercards-2.5.0/jupytercards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.4.0a2'
+__version__ = '2.5.0'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.4.0a2/jupytercards/dynamic.py` & `jupytercards-2.5.0/jupytercards/dynamic.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/jupytercards/flashcards.js` & `jupytercards-2.5.0/jupytercards/flashcards.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/jupytercards/styles.css` & `jupytercards-2.5.0/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/jupytercards/swiped-events.min.js` & `jupytercards-2.5.0/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.4.0a2/PKG-INFO` & `jupytercards-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.4.0a2
+Version: 2.5.0
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```


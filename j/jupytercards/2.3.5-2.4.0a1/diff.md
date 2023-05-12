# Comparing `tmp/jupytercards-2.3.5.tar.gz` & `tmp/jupytercards-2.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.3.5.tar", last modified: Fri May 12 10:10:49 2023, max compression
+gzip compressed data, was "jupytercards-2.4.0a1.tar", last modified: Fri May 12 12:58:57 2023, max compression
```

## Comparing `jupytercards-2.3.5.tar` & `jupytercards-2.4.0a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.3.5/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.3.5/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.3.5/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.3.5/README.md
--rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.3.5/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.3.5/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.3.5/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.3.5/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-05-12 10:09:37.887005 jupytercards-2.3.5/jupytercards/__init__.py
--rw-r--r--   0        0        0     8948 2023-05-12 10:08:25.073235 jupytercards-2.3.5/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.3.5/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.3.5/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.3.5/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.3.5/pyproject.toml
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.4.0a1/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.4.0a1/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.4.0a1/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.4.0a1/README.md
+-rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.4.0a1/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.4.0a1/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.4.0a1/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.4.0a1/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      660 2023-05-12 12:30:07.061778 jupytercards-2.4.0a1/jupytercards/__init__.py
+-rw-r--r--   0        0        0     9443 2023-05-12 12:24:10.014921 jupytercards-2.4.0a1/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.4.0a1/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.4.0a1/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.4.0a1/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 jupytercards-2.4.0a1/PKG-INFO
```

### Comparing `jupytercards-2.3.5/.gitignore` & `jupytercards-2.4.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/LICENSE` & `jupytercards-2.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/Markdown-flashcards.ipynb` & `jupytercards-2.4.0a1/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/README.md` & `jupytercards-2.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/example.ipynb` & `jupytercards-2.4.0a1/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/extractdefinitions.py` & `jupytercards-2.4.0a1/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/flashcards.gif` & `jupytercards-2.4.0a1/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/jupytercards/__init__.py` & `jupytercards-2.4.0a1/jupytercards/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.3.5'
+__version__ = '2.4.0.a1'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.3.5/jupytercards/dynamic.py` & `jupytercards-2.4.0a1/jupytercards/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,17 +143,30 @@
     elif type(ref) == str:
         if ref[0] == "[":
             loadData += ref
             static = True
             url=""
         elif ref.lower().find("http") == 0:
             url = ref
-            file = urllib.request.urlopen(url)
-            for line in file:
-                loadData += line.decode("utf-8")
+            if sys.platform == 'emscripten':
+                try: 
+                    from pyodide.http import open_url
+                except:
+                    try:
+                        from pyodide import open_url
+                    except:
+                        print('Importing open_url failed. Please raise an issue at')
+                        print('https://github.com/jmshea/jupyterquiz/issues')
+
+                loadData += open_url(url).read()
+            else:
+                file = urllib.request.urlopen(url)
+
+                for line in file:
+                    loadData += line.decode("utf-8")
             static = False
         else:
             #print("File detected")
             with open(ref) as file:
                 for line in file:
                     loadData += line
             static = True
```

### Comparing `jupytercards-2.3.5/jupytercards/flashcards.js` & `jupytercards-2.4.0a1/jupytercards/flashcards.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/jupytercards/styles.css` & `jupytercards-2.4.0a1/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/jupytercards/swiped-events.min.js` & `jupytercards-2.4.0a1/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.5/PKG-INFO` & `jupytercards-2.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.3.5
+Version: 2.4.0a1
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```


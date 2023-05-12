# Comparing `tmp/jupytercards-2.3.1.tar.gz` & `tmp/jupytercards-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.3.1.tar", last modified: Wed May 10 09:34:03 2023, max compression
+gzip compressed data, was "jupytercards-2.3.5.tar", last modified: Fri May 12 10:10:49 2023, max compression
```

## Comparing `jupytercards-2.3.1.tar` & `jupytercards-2.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.3.1/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.3.1/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.3.1/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.3.1/README.md
--rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.3.1/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.3.1/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.3.1/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.3.1/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-05-10 09:33:49.484437 jupytercards-2.3.1/jupytercards/__init__.py
--rw-r--r--   0        0        0     7600 2023-05-10 09:28:41.207510 jupytercards-2.3.1/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.3.1/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.3.1/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.3.1/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.3.5/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.3.5/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.3.5/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.3.5/README.md
+-rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.3.5/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.3.5/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.3.5/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.3.5/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-05-12 10:09:37.887005 jupytercards-2.3.5/jupytercards/__init__.py
+-rw-r--r--   0        0        0     8948 2023-05-12 10:08:25.073235 jupytercards-2.3.5/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.3.5/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.3.5/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.3.5/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.3.5/PKG-INFO
```

### Comparing `jupytercards-2.3.1/.gitignore` & `jupytercards-2.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/LICENSE` & `jupytercards-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/Markdown-flashcards.ipynb` & `jupytercards-2.3.5/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/README.md` & `jupytercards-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/example.ipynb` & `jupytercards-2.3.5/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/extractdefinitions.py` & `jupytercards-2.3.5/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/flashcards.gif` & `jupytercards-2.3.5/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/jupytercards/__init__.py` & `jupytercards-2.3.5/jupytercards/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.3.1'
+__version__ = '2.3.5'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.3.1/jupytercards/dynamic.py` & `jupytercards-2.3.5/jupytercards/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,41 @@
 from IPython.core.display import display,  HTML, Javascript
 import string
 import random
 import json
 import urllib.request
 import pkg_resources
 def display_flashcards(ref, keyControl = True, grabFocus=False,
-                       front_colors=False,
-                       back_colors=False,
-                       text_colors=False,
+                       front_colors=None,
+                       back_colors=None,
+                       text_colors=None,
                        ):
+    '''
+    Display interactive flash cards using a mix of Python and Javascript to support
+    use in rendered notebooks (especially JupyterBook, but also Voila)
+
+    Inputs:
+    ref = string, reference to quiz JSON, may be:
+          - file name
+          - URL
+          - Python list
+
+    keyControl = boolean, whether to support keyboard: right = advance, space = flip
+
+    grabFocus = boolean, whether to put browser focus on this slide deck
+                (may cause browser to jump to the slide deck)
+
+    front_colors
+    back_colors
+    text_colors = None or list of strings specfiying alternate colors.
+                  front_colors, back_colors also support 'jupytercon' to use JupyterCon (2023) color theme
+
+    John  M. Shea
+    2021-2023
+    '''
 
     front_color_dict=[
         'var(--asparagus)',
         'var(--terra-cotta)',
         'var(--cyan-process)'
     ]
 
@@ -65,24 +88,40 @@
 
     script = ''
     js = pkg_resources.resource_string(resource_package, "swiped-events.min.js")
     script += js.decode("utf-8")
     js = pkg_resources.resource_string(resource_package, "flashcards.js")
     script += js.decode("utf-8")
 
-    #print(script)
-
-
 
-    #print(card["front"], card["back"])
     letters = string.ascii_letters
     div_id = ''.join(random.choice(letters) for i in range(12))
-    #div_id='ABBA'
     # print(div_id)
 
+    #print(script)
+    script += f'''/* This is to handle asynchrony issues in loading Jupyter notebooks
+           where JupyterCards has been previously run. The Javascript was generally
+           being run before the div was added to the DOM. I tried to do this
+           more elegantly using Mutation Observer, but I didn't get it to work.
+
+           Someone more knowledgeable could make this better ;-) */
+
+        function try_create() {{
+          if(document.getElementById("{div_id}")) {{
+            createCards("{div_id}", "{keyControl}", "{grabFocus}");
+          }} else {{
+             setTimeout(try_create, 200);
+          }}
+        }};
+    '''
+
+
+
+
+    #print(card["front"], card["back"])
     # Container
     #mydiv =  '<div class="flip-container" id="'+ div_id + '"></div>'
     mydiv =  f'<div class="flip-container" id="{div_id}" tabindex="0" style="outline:none;"></div>'
 
 
 
     #Spacer
@@ -138,15 +177,15 @@
     for color in text_color_dict[:-1]:
         loadData += f'"{color}", '
     loadData += f'"{text_color_dict[-1]}" ];\n'
 
 
 
     if static:
-        loadData += f'''createCards("{div_id}", "{keyControl}", "{grabFocus}"); '''
+        loadData += f'''try_create(); '''
 
         print()
     else:
         loadData += f'''
 
         {{
         const jmscontroller = new AbortController();
```

### Comparing `jupytercards-2.3.1/jupytercards/flashcards.js` & `jupytercards-2.3.5/jupytercards/flashcards.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/jupytercards/styles.css` & `jupytercards-2.3.5/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/jupytercards/swiped-events.min.js` & `jupytercards-2.3.5/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.1/PKG-INFO` & `jupytercards-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.3.1
+Version: 2.3.5
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```


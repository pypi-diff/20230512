# Comparing `tmp/html_msg-1.0.7.tar.gz` & `tmp/html_msg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.0.7.tar", last modified: Wed May 10 21:48:51 2023, max compression
+gzip compressed data, was "html_msg-1.1.0.tar", last modified: Fri May 12 13:03:13 2023, max compression
```

## Comparing `html_msg-1.0.7.tar` & `html_msg-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:48:51.769281 html_msg-1.0.7/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3965 2023-05-10 21:48:51.768284 html_msg-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 21:48:51.756312 html_msg-1.0.7/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-10 21:46:23.000000 html_msg-1.0.7/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.7/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14803 2023-05-10 21:46:14.000000 html_msg-1.0.7/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:48:51.768284 html_msg-1.0.7/html_msg.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 21:48:51.769281 html_msg-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-05-10 21:48:46.000000 html_msg-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:03:13.091424 html_msg-1.1.0/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3965 2023-05-12 13:03:13.090427 html_msg-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 13:03:13.077327 html_msg-1.1.0/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-12 13:02:18.000000 html_msg-1.1.0/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.0/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14802 2023-05-12 12:51:46.000000 html_msg-1.1.0/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:03:13.090427 html_msg-1.1.0/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-05-12 13:03:13.000000 html_msg-1.1.0/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-12 13:03:13.000000 html_msg-1.1.0/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 13:03:13.000000 html_msg-1.1.0/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 13:03:13.000000 html_msg-1.1.0/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 13:03:13.000000 html_msg-1.1.0/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 13:03:13.092422 html_msg-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-05-12 13:02:06.000000 html_msg-1.1.0/setup.py
```

### Comparing `html_msg-1.0.7/LICENSE.txt` & `html_msg-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.7/PKG-INFO` & `html_msg-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_msg
-Version: 1.0.7
+Version: 1.1.0
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
```

### Comparing `html_msg-1.0.7/README.md` & `html_msg-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.7/html_msg/html_message.py` & `html_msg-1.1.0/html_msg/html_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # How to center table: add to header style this two attributes - margin-left: auto; margin-right: auto;
-# сделать 2 красивых пресета
+# сделать 2 красивых пресета 
 
 class HTMLMessage:
     def __init__(self, body=""):
         self.body = body
         self.html = ""
 
     def __add_header(self):
```

### Comparing `html_msg-1.0.7/html_msg/html_table.py` & `html_msg-1.1.0/html_msg/html_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 
                 if (i, j) in self.cell_style_map:
                     cell_style += f' {self.cell_style_map[(i, j)]};'
                 
                 if (i, j) in self.cell_color_map:
                     cell_style += f' background: {self.cell_color_map[(i, j)]};'
                 
-                self.html_table += f'<td style="{self.table_style};{cell_style}">{cell}</td>'
+                self.html_table += f'<td style="{self.table_style}{cell_style}">{cell}</td>'
             
             self.html_table += '</tr>\n'
     
     def add_row(self, row):
         
         '''
         Appends a new row to the table.
```

### Comparing `html_msg-1.0.7/html_msg.egg-info/PKG-INFO` & `html_msg-1.1.0/html_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.0.7
+Version: 1.1.0
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
```

### Comparing `html_msg-1.0.7/setup.py` & `html_msg-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.0.7',
+    version='1.1.0',
     description='This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
```


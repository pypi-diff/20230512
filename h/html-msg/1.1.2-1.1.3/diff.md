# Comparing `tmp/html_msg-1.1.2.tar.gz` & `tmp/html_msg-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.1.2.tar", last modified: Fri May 12 13:23:50 2023, max compression
+gzip compressed data, was "html_msg-1.1.3.tar", last modified: Fri May 12 13:35:31 2023, max compression
```

## Comparing `html_msg-1.1.2.tar` & `html_msg-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 13:23:50.907026 html_msg-1.1.2/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3965 2023-05-12 13:23:50.907026 html_msg-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 13:23:50.895058 html_msg-1.1.2/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-12 13:23:43.000000 html_msg-1.1.2/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.2/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14800 2023-05-12 13:23:16.000000 html_msg-1.1.2/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:23:50.906029 html_msg-1.1.2/html_msg.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-05-12 13:23:50.000000 html_msg-1.1.2/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-12 13:23:50.000000 html_msg-1.1.2/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 13:23:50.000000 html_msg-1.1.2/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 13:23:50.000000 html_msg-1.1.2/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 13:23:50.000000 html_msg-1.1.2/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 13:23:50.907026 html_msg-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-05-12 13:23:32.000000 html_msg-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:35:31.937904 html_msg-1.1.3/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3965 2023-05-12 13:35:31.936906 html_msg-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 13:35:31.925935 html_msg-1.1.3/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-12 13:35:08.000000 html_msg-1.1.3/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.3/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14937 2023-05-12 13:34:56.000000 html_msg-1.1.3/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:35:31.936906 html_msg-1.1.3/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 13:35:31.937904 html_msg-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-05-12 13:35:20.000000 html_msg-1.1.3/setup.py
```

### Comparing `html_msg-1.1.2/LICENSE.txt` & `html_msg-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.2/PKG-INFO` & `html_msg-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_msg
-Version: 1.1.2
+Version: 1.1.3
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
```

### Comparing `html_msg-1.1.2/README.md` & `html_msg-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.2/html_msg/html_message.py` & `html_msg-1.1.3/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.2/html_msg/html_table.py` & `html_msg-1.1.3/html_msg/html_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         self.font_size = '12px'
         self.font_color = 'black'
         self.table_style = self.presets["Basic"]["table_style"]
         self.header_style = self.presets["Basic"]["header_style"]
         self.html_table  = ''
     
     def __update_table(self):
-        self.html_table = f'<table style="font-family: {self.font_family}; font-size: {self.font_size}; color: {self.font_color}; {self.table_style}">\n'
+        #self.html_table = f'<table style="font-family: {self.font_family}; font-size: {self.font_size}; color: {self.font_color}; {self.table_style}">\n'
+        self.html_table = f'<table style="font-family: {self.font_family}; font-size: {self.font_size}; color: {self.font_color};">\n'
         self.__update_headers()
         self.__update_rows()
         self.html_table += '</table>'
     
     def __update_headers(self):
         # Add headers if they exist
         if self.headers:
```

### Comparing `html_msg-1.1.2/html_msg.egg-info/PKG-INFO` & `html_msg-1.1.3/html_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.1.2
+Version: 1.1.3
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
```

### Comparing `html_msg-1.1.2/setup.py` & `html_msg-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.1.2',
+    version='1.1.3',
     description='This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
```


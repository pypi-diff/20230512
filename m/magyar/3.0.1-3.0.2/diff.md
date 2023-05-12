# Comparing `tmp/magyar-3.0.1.tar.gz` & `tmp/magyar-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.0.1.tar", last modified: Fri May 12 16:08:13 2023, max compression
+gzip compressed data, was "magyar-3.0.2.tar", last modified: Fri May 12 16:46:08 2023, max compression
```

## Comparing `magyar-3.0.1.tar` & `magyar-3.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 16:08:13.156802 magyar-3.0.1/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6240 2023-05-12 16:08:13.156802 magyar-3.0.1/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     5830 2023-05-12 16:02:31.000000 magyar-3.0.1/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 16:08:13.156802 magyar-3.0.1/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6240 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    38778 2023-05-12 16:02:31.000000 magyar-3.0.1/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-12 16:08:13.156802 magyar-3.0.1/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-12 16:02:31.000000 magyar-3.0.1/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 16:46:08.740157 magyar-3.0.2/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6240 2023-05-12 16:46:08.740157 magyar-3.0.2/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5830 2023-05-12 16:02:31.000000 magyar-3.0.2/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 16:46:08.740157 magyar-3.0.2/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6240 2023-05-12 16:46:08.000000 magyar-3.0.2/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-12 16:46:08.000000 magyar-3.0.2/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-12 16:46:08.000000 magyar-3.0.2/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-12 16:46:08.000000 magyar-3.0.2/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38777 2023-05-12 16:45:46.000000 magyar-3.0.2/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-12 16:46:08.740157 magyar-3.0.2/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-12 16:45:46.000000 magyar-3.0.2/setup.py
```

### Comparing `magyar-3.0.1/PKG-INFO` & `magyar-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.1
+Version: 3.0.2
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `magyar-3.0.1/README.md` & `magyar-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `magyar-3.0.1/magyar.egg-info/PKG-INFO` & `magyar-3.0.2/magyar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.1
+Version: 3.0.2
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `magyar-3.0.1/magyar.py` & `magyar-3.0.2/magyar.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,11 +404,10 @@
         indent = ''
     tordelt_sorok = []
     for i in range(0, len(lst), n):
         row = lst[i:i+n]
         tordelt_sorok.append(f"{indent}{', '.join(map(str, row))}")
     return "\n".join(tordelt_sorok)
 
-
 ABECEDARAK = 'aábcdeéfghiíjklmnoóöőpqrstuúüűvwxyz'
 def abc(lista):
     return sorted(lista, key=lambda s: [ABECEDARAK.find(c) for c in s.lower()])
```

### Comparing `magyar-3.0.1/setup.py` & `magyar-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.0.1",
+    version="3.0.2",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```


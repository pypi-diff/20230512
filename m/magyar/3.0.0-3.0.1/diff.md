# Comparing `tmp/magyar-3.0.0.tar.gz` & `tmp/magyar-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.0.0.tar", last modified: Tue May  9 20:26:21 2023, max compression
+gzip compressed data, was "magyar-3.0.1.tar", last modified: Fri May 12 16:08:13 2023, max compression
```

## Comparing `magyar-3.0.0.tar` & `magyar-3.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-09 20:26:21.121485 magyar-3.0.0/
--rw-rw-r--   0 bela      (1000) bela      (1000)     5855 2023-05-09 20:26:21.121485 magyar-3.0.0/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     5445 2023-05-09 20:24:54.000000 magyar-3.0.0/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-09 20:26:21.121485 magyar-3.0.0/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     5855 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    38473 2023-05-09 20:11:06.000000 magyar-3.0.0/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-09 20:26:21.121485 magyar-3.0.0/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-09 20:12:58.000000 magyar-3.0.0/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 16:08:13.156802 magyar-3.0.1/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6240 2023-05-12 16:08:13.156802 magyar-3.0.1/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5830 2023-05-12 16:02:31.000000 magyar-3.0.1/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 16:08:13.156802 magyar-3.0.1/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6240 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-12 16:08:13.000000 magyar-3.0.1/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38778 2023-05-12 16:02:31.000000 magyar-3.0.1/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-12 16:08:13.156802 magyar-3.0.1/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-12 16:02:31.000000 magyar-3.0.1/setup.py
```

### Comparing `magyar-3.0.0/PKG-INFO` & `magyar-3.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.0
+Version: 3.0.1
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -134,17 +134,31 @@
 
 3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
 
 
          magyar.abc(lista):
 
 Használat : </br> </br>
-gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',]
+gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',] </br>
 sorban =magyar.abc(gyumolcs) </br>
 ['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
+
+4. Listák tördelése "behúzással" </br></br>
+
+        magyar.ftordel(lst,n,'') 
+</br></br>
+lst = a lista neve</br>
+n = hány szó legyen egy sorban</br>
+'  ' = a behúzás mértéke ami sztring. '\t' </br>
+Kimenetként listát ad vissza. </br></br>
+
+Hasznalat :</br>
+formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
+print(formazott_lista) vagy f.write(formazott_lista)
+
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-3.0.0/README.md` & `magyar-3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -122,17 +122,31 @@
 
 3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
 
 
          magyar.abc(lista):
 
 Használat : </br> </br>
-gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',]
+gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',] </br>
 sorban =magyar.abc(gyumolcs) </br>
 ['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
+
+4. Listák tördelése "behúzással" </br></br>
+
+        magyar.ftordel(lst,n,'') 
+</br></br>
+lst = a lista neve</br>
+n = hány szó legyen egy sorban</br>
+'  ' = a behúzás mértéke ami sztring. '\t' </br>
+Kimenetként listát ad vissza. </br></br>
+
+Hasznalat :</br>
+formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
+print(formazott_lista) vagy f.write(formazott_lista)
+
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-3.0.0/magyar.egg-info/PKG-INFO` & `magyar-3.0.1/magyar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.0
+Version: 3.0.1
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -134,17 +134,31 @@
 
 3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
 
 
          magyar.abc(lista):
 
 Használat : </br> </br>
-gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',]
+gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',] </br>
 sorban =magyar.abc(gyumolcs) </br>
 ['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
+
+4. Listák tördelése "behúzással" </br></br>
+
+        magyar.ftordel(lst,n,'') 
+</br></br>
+lst = a lista neve</br>
+n = hány szó legyen egy sorban</br>
+'  ' = a behúzás mértéke ami sztring. '\t' </br>
+Kimenetként listát ad vissza. </br></br>
+
+Hasznalat :</br>
+formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
+print(formazott_lista) vagy f.write(formazott_lista)
+
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-3.0.0/magyar.py` & `magyar-3.0.1/magyar.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,10 +393,22 @@
     if n is None:
         n = 10
     for i in range(0, len(lst), n):
         row = lst[i:i+n]
         print(", ".join(map(str, row)), end=", ")
         print()
 
+def ftordel(lst, n=None, indent=None):
+    if n is None:
+        n = 10
+    if indent is None:
+        indent = ''
+    tordelt_sorok = []
+    for i in range(0, len(lst), n):
+        row = lst[i:i+n]
+        tordelt_sorok.append(f"{indent}{', '.join(map(str, row))}")
+    return "\n".join(tordelt_sorok)
+
+
 ABECEDARAK = 'aábcdeéfghiíjklmnoóöőpqrstuúüűvwxyz'
 def abc(lista):
     return sorted(lista, key=lambda s: [ABECEDARAK.find(c) for c in s.lower()])
```

### Comparing `magyar-3.0.0/setup.py` & `magyar-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.0.0",
+    version="3.0.1",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```


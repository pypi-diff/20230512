# Comparing `tmp/terick-0.2.1.tar.gz` & `tmp/terick-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terick-0.2.1.tar", last modified: Fri May  5 21:37:43 2023, max compression
+gzip compressed data, was "terick-0.2.2.tar", last modified: Tue May  9 14:24:34 2023, max compression
```

## Comparing `terick-0.2.1.tar` & `terick-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:37:43.888886 terick-0.2.1/
--rw-rw-rw-   0        0        0      470 2023-05-05 21:37:43.886796 terick-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-05 21:36:01.000000 terick-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 21:37:43.889386 terick-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-05 21:26:28.000000 terick-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:37:43.848960 terick-0.2.1/terick/
--rw-rw-rw-   0        0        0     7396 2023-05-05 21:28:00.000000 terick-0.2.1/terick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:37:43.883076 terick-0.2.1/terick.egg-info/
--rw-rw-rw-   0        0        0      470 2023-05-05 21:37:43.000000 terick-0.2.1/terick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-05 21:37:43.000000 terick-0.2.1/terick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:37:43.000000 terick-0.2.1/terick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 21:37:43.000000 terick-0.2.1/terick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 14:24:34.516755 terick-0.2.2/
+-rw-rw-rw-   0        0        0      470 2023-05-09 14:24:34.515756 terick-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-05 21:36:01.000000 terick-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:24:34.516755 terick-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-05-09 14:24:25.000000 terick-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:24:34.493616 terick-0.2.2/terick/
+-rw-rw-rw-   0        0        0     7678 2023-05-09 14:16:32.000000 terick-0.2.2/terick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:24:34.514820 terick-0.2.2/terick.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/top_level.txt
```

### Comparing `terick-0.2.1/setup.py` & `terick-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Package full of simple functions'
 
 # Setting up
 setup(
     name="terick",
     version=VERSION,
     author="HaxoTF",
```

### Comparing `terick-0.2.1/terick/__init__.py` & `terick-0.2.2/terick/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,27 @@
     else: 
         gap = (lenght-len(text))/2
         result = " "*int(gap) + text
         if int(gap)==gap: result += " "*int(gap)
         else: result += " "*(int(gap)+1)
         return result
 
+def into_str(into:str, obj:str, x:int):
+    result = ""
+    index = 0
+
+    for i in range(0, len(into)):
+        if (i>=x) and (index<len(obj)):
+            result += obj[index]
+            index += 1
+        else:
+            result += into[i]
+    
+    return result
+
 # ----====[ Numbers ]====----
 
 
 # --- number limit v1.0
 def limit(value:float, min:float, max:float):
     if value>max: return max
     if value<min: return min
```


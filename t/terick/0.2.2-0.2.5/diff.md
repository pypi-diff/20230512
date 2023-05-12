# Comparing `tmp/terick-0.2.2.tar.gz` & `tmp/terick-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terick-0.2.2.tar", last modified: Tue May  9 14:24:34 2023, max compression
+gzip compressed data, was "terick-0.2.5.tar", last modified: Fri May 12 18:24:37 2023, max compression
```

## Comparing `terick-0.2.2.tar` & `terick-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 14:24:34.516755 terick-0.2.2/
--rw-rw-rw-   0        0        0      470 2023-05-09 14:24:34.515756 terick-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-05 21:36:01.000000 terick-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 14:24:34.516755 terick-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-09 14:24:25.000000 terick-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:24:34.493616 terick-0.2.2/terick/
--rw-rw-rw-   0        0        0     7678 2023-05-09 14:16:32.000000 terick-0.2.2/terick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:24:34.514820 terick-0.2.2/terick.egg-info/
--rw-rw-rw-   0        0        0      470 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 14:24:34.000000 terick-0.2.2/terick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 18:24:37.374349 terick-0.2.5/
+-rw-rw-rw-   0        0        0      470 2023-05-12 18:24:37.372987 terick-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-05 21:36:01.000000 terick-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 18:24:37.374349 terick-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-05-12 18:24:10.000000 terick-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:24:37.366077 terick-0.2.5/terick/
+-rw-rw-rw-   0        0        0     8142 2023-05-12 18:06:52.000000 terick-0.2.5/terick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:24:37.370986 terick-0.2.5/terick.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/top_level.txt
```

### Comparing `terick-0.2.2/setup.py` & `terick-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.2'
+VERSION = '0.2.5'
 DESCRIPTION = 'Package full of simple functions'
 
 # Setting up
 setup(
     name="terick",
     version=VERSION,
     author="HaxoTF",
```

### Comparing `terick-0.2.2/terick/__init__.py` & `terick-0.2.5/terick/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,27 +85,37 @@
     else: 
         gap = (lenght-len(text))/2
         result = " "*int(gap) + text
         if int(gap)==gap: result += " "*int(gap)
         else: result += " "*(int(gap)+1)
         return result
 
+# --- into str v1.0
 def into_str(into:str, obj:str, x:int):
     result = ""
     index = 0
 
     for i in range(0, len(into)):
         if (i>=x) and (index<len(obj)):
             result += obj[index]
             index += 1
         else:
             result += into[i]
     
     return result
 
+# --- divide time v1.0
+def div_time(seconds:float, as_text=False):
+    s = int(seconds)
+    m = int(seconds/60); s -= m*60
+    h = int(m/60); m -= h*60
+
+    if as_text: return f"{h}h {m}m {s}s"
+    else: return h, m, s
+
 # ----====[ Numbers ]====----
 
 
 # --- number limit v1.0
 def limit(value:float, min:float, max:float):
     if value>max: return max
     if value<min: return min
@@ -149,36 +159,43 @@
             if len(result)+1<len(data): result.append(unlist_words(line)+"\n")
             else: result.append(unlist_words(line))
         f.writelines(result)
     f.close()
 
 # --- zip directory v1.0
 def zipdir(dir:str, filename:str):
-    walkvar = []
-
-    def zipwalk(dir: str):
-        for f in os.listdir(dir):
-
-            path = f"{dir}/{f}"
-            if os.path.isdir(path): zipwalk(path)
-            else: walkvar.append(path)
-
-    zipwalk(dir)
+    walkvar = file_walk(dir)
 
     zipf = zip.ZipFile(filename, "w")
     for file in walkvar:
         zipf.write(file, compress_type=zip.ZIP_DEFLATED)
     zipf.close()
 
 # --- unzip v1.0
 def unzip(dir_from:str, dir_to:str):
     zipf = zip.ZipFile(dir_from)
     zipf.extractall(dir_to)
     zipf.close()
 
+# --- file walk v1.0
+def file_walk(dir:str, catch_folders=False):
+    walkvar = []
+    
+    def walk(dir:str):
+        for f in os.listdir(dir):
+            
+            path = f"{dir}/{f}"
+            if os.path.isdir(path):
+                if catch_folders: walkvar.append(path)
+                walk(path)
+            else:
+                walkvar.append(path)
+    walk(dir)
+    return walkvar
+
 
 # ----====[ Math ]====----
 
 
 # -- get average v1.0
 def calc_avg(values:list):
     total = 0
```


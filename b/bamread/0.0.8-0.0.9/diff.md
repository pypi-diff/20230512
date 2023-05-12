# Comparing `tmp/bamread-0.0.8.tar.gz` & `tmp/bamread-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bamread-0.0.8.tar", last modified: Wed Jun  9 16:24:48 2021, max compression
+gzip compressed data, was "dist/bamread-0.0.9.tar", last modified: Thu Aug  5 14:06:51 2021, max compression
```

## Comparing `bamread-0.0.8.tar` & `bamread-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:24:48.056335 bamread-0.0.8/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      773 2021-06-09 16:24:48.056162 bamread-0.0.8/PKG-INFO
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       60 2021-06-09 16:08:42.000000 bamread-0.0.8/README.md
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:24:48.052893 bamread-0.0.8/bamread/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      100 2021-06-09 16:08:42.000000 bamread-0.0.8/bamread/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1764 2021-06-09 16:08:42.000000 bamread-0.0.8/bamread/read.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:24:48.055631 bamread-0.0.8/bamread/src/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:08:42.000000 bamread-0.0.8/bamread/src/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   931660 2021-06-09 16:10:12.000000 bamread-0.0.8/bamread/src/bamread.c
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4600 2021-06-09 16:08:42.000000 bamread-0.0.8/bamread/src/bamread.pyx
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1208 2021-06-09 16:08:42.000000 bamread-0.0.8/bamread/src/bamwrite.pyx
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       22 2021-06-09 16:24:36.000000 bamread-0.0.8/bamread/version.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:24:48.053453 bamread-0.0.8/bamread.egg-info/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      773 2021-06-09 16:24:47.000000 bamread-0.0.8/bamread.egg-info/PKG-INFO
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      334 2021-06-09 16:24:47.000000 bamread-0.0.8/bamread.egg-info/SOURCES.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2021-06-09 16:24:47.000000 bamread-0.0.8/bamread.egg-info/dependency_links.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       40 2021-06-09 16:24:47.000000 bamread-0.0.8/bamread.egg-info/requires.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        8 2021-06-09 16:24:47.000000 bamread-0.0.8/bamread.egg-info/top_level.txt
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:24:48.055846 bamread-0.0.8/bin/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      127 2021-06-09 16:08:42.000000 bamread-0.0.8/bin/bamread
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       38 2021-06-09 16:24:48.056386 bamread-0.0.8/setup.cfg
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2254 2021-06-09 16:08:42.000000 bamread-0.0.8/setup.py
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-08-05 14:06:51.627149 bamread-0.0.9/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      773 2021-08-05 14:06:51.626978 bamread-0.0.9/PKG-INFO
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       60 2021-06-09 16:08:42.000000 bamread-0.0.9/README.md
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-08-05 14:06:51.623608 bamread-0.0.9/bamread/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      100 2021-06-09 16:08:42.000000 bamread-0.0.9/bamread/__init__.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1764 2021-08-05 14:04:54.000000 bamread-0.0.9/bamread/read.py
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-08-05 14:06:51.626439 bamread-0.0.9/bamread/src/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-09 16:08:42.000000 bamread-0.0.9/bamread/src/__init__.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   931660 2021-06-09 16:10:12.000000 bamread-0.0.9/bamread/src/bamread.c
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4600 2021-06-09 16:08:42.000000 bamread-0.0.9/bamread/src/bamread.pyx
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1208 2021-06-09 16:08:42.000000 bamread-0.0.9/bamread/src/bamwrite.pyx
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       22 2021-08-05 14:05:24.000000 bamread-0.0.9/bamread/version.py
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-08-05 14:06:51.624197 bamread-0.0.9/bamread.egg-info/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      773 2021-08-05 14:06:51.000000 bamread-0.0.9/bamread.egg-info/PKG-INFO
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      334 2021-08-05 14:06:51.000000 bamread-0.0.9/bamread.egg-info/SOURCES.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2021-08-05 14:06:51.000000 bamread-0.0.9/bamread.egg-info/dependency_links.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       40 2021-08-05 14:06:51.000000 bamread-0.0.9/bamread.egg-info/requires.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        8 2021-08-05 14:06:51.000000 bamread-0.0.9/bamread.egg-info/top_level.txt
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-08-05 14:06:51.626690 bamread-0.0.9/bin/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      127 2021-06-09 16:08:42.000000 bamread-0.0.9/bin/bamread
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       38 2021-08-05 14:06:51.627201 bamread-0.0.9/setup.cfg
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2254 2021-06-09 16:08:42.000000 bamread-0.0.9/setup.py
```

### Comparing `bamread-0.0.8/PKG-INFO` & `bamread-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bamread
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read bam files quickly into dataframes in Python
 Home-page: http://github.com/endrebak/bamread
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: ['MIT']
 Description: # bamread
```

### Comparing `bamread-0.0.8/bamread/read.py` & `bamread-0.0.9/bamread/read.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     chromosomes, starts, ends, strands, flags, chrmap = _bamread(
         f, mapq, required_flag, filter_flag)
 
     chromosomes = pd.Series(chromosomes).replace(chrmap).astype("category")
     starts = pd.Series(starts)
     ends = pd.Series(ends)
-    strands = pd.Series(strands).replace({16: "+", 0: "-"}).astype("category")
+    strands = pd.Series(strands).replace({16: "-", 0: "+"}).astype("category")
     flags = pd.Series(flags)
 
     return pd.DataFrame({
         "Chromosome": chromosomes,
         "Start": starts,
         "End": ends,
         "Strand": strands,
@@ -27,15 +27,15 @@
 
     chromosomes, starts, ends, strands, flags, chrmap, qstarts, qends, query_names, query_sequences, cigarstrings, query_qualities = _bamread_all(
         f, mapq, required_flag, filter_flag)
 
     chromosomes = pd.Series(chromosomes).replace(chrmap).astype("category")
     starts = pd.Series(starts)
     ends = pd.Series(ends)
-    strands = pd.Series(strands).replace({16: "+", 0: "-"}).astype("category")
+    strands = pd.Series(strands).replace({16: "-", 0: "+"}).astype("category")
     flags = pd.Series(flags)
     qstarts = pd.Series(qstarts)
     qends = pd.Series(qends)
     query_names = pd.Series(query_names)
     query_sequences = pd.Series(query_sequences)
     cigarstrings = pd.Series(cigarstrings)
     query_qualities = pd.Series(query_qualities)
```

### Comparing `bamread-0.0.8/bamread/src/bamread.c` & `bamread-0.0.9/bamread/src/bamread.c`

 * *Files identical despite different names*

### Comparing `bamread-0.0.8/bamread/src/bamread.pyx` & `bamread-0.0.9/bamread/src/bamread.pyx`

 * *Files identical despite different names*

### Comparing `bamread-0.0.8/bamread/src/bamwrite.pyx` & `bamread-0.0.9/bamread/src/bamwrite.pyx`

 * *Files identical despite different names*

### Comparing `bamread-0.0.8/bamread.egg-info/PKG-INFO` & `bamread-0.0.9/bamread.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bamread
-Version: 0.0.8
+Version: 0.0.9
 Summary: Read bam files quickly into dataframes in Python
 Home-page: http://github.com/endrebak/bamread
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: ['MIT']
 Description: # bamread
```

### Comparing `bamread-0.0.8/setup.py` & `bamread-0.0.9/setup.py`

 * *Files identical despite different names*


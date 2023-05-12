# Comparing `tmp/samshee-0.1.4.tar.gz` & `tmp/samshee-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samshee-0.1.4.tar", last modified: Tue Apr 18 06:24:38 2023, max compression
+gzip compressed data, was "samshee-0.1.5.tar", last modified: Fri May 12 08:55:22 2023, max compression
```

## Comparing `samshee-0.1.4.tar` & `samshee-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.4/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-18 06:24:38.406971 samshee-0.1.4/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.4/README.md
--rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-04-18 06:24:04.000000 samshee-0.1.4/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-18 06:24:38.406971 samshee-0.1.4/setup.cfg
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.403638 samshee-0.1.4/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/src/samshee/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.4/src/samshee/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.4/src/samshee/samplesheetv2.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.4/src/samshee/sectionedsheet.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    26101 2023-04-18 06:23:27.000000 samshee-0.1.4/src/samshee/validation.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/src/samshee.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-04-18 06:24:38.000000 samshee-0.1.4/src/samshee.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-18 06:24:38.406971 samshee-0.1.4/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.4/tests/test_validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.798524 samshee-0.1.5/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.5/LICENSE
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-05-12 08:55:22.798524 samshee-0.1.5/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.5/README.md
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-05-12 08:52:33.000000 samshee-0.1.5/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-05-12 08:55:22.798524 samshee-0.1.5/setup.cfg
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.795190 samshee-0.1.5/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.795190 samshee-0.1.5/src/samshee/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.5/src/samshee/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.5/src/samshee/samplesheetv2.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.5/src/samshee/sectionedsheet.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    26204 2023-05-12 08:51:18.000000 samshee-0.1.5/src/samshee/validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.798524 samshee-0.1.5/src/samshee.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.798524 samshee-0.1.5/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.5/tests/test_validation.py
```

### Comparing `samshee-0.1.4/LICENSE` & `samshee-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `samshee-0.1.4/PKG-INFO` & `samshee-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.4
+Version: 0.1.5
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.4/README.md` & `samshee-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `samshee-0.1.4/pyproject.toml` & `samshee-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samshee"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Jakob Simeth", email="jakob.simeth@ukr.de" }
 ]
 description="A schema-agnostic parser and writer for illumina sample sheets v2."
 readme = "README.md"
 license={file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `samshee-0.1.4/src/samshee/samplesheetv2.py` & `samshee-0.1.5/src/samshee/samplesheetv2.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.4/src/samshee/sectionedsheet.py` & `samshee-0.1.5/src/samshee/sectionedsheet.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.4/src/samshee/validation.py` & `samshee-0.1.5/src/samshee/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,15 +521,19 @@
     if "BCLConvert_Settings" in doc:
         if "OverrideCycles" in doc["BCLConvert_Settings"]:
             cycles = parse_overrideCycles(
                 str(cast(Settings, doc["BCLConvert_Settings"])["OverrideCycles"])
             )
             if "U" in cycles["Index1Cycles"]:
                 raise Exception("Index1 typically does not contain UMIs")
-            if ("Index2Cycles" in cycles) and (not "U" in cycles["Index2Cycles"]):
+            if (
+                ("Index2Cycles" in cycles)
+                and (len(cycles["Index2Cycles"]) > 10)
+                and (not "U" in cycles["Index2Cycles"])
+            ):
                 raise Exception(
                     "Reads.Index2 must have a maximum length of 10 if it contains only an index and no UMIs."
                 )
 
 
 def validate(doc: SectionedSheet, validation: list[Callable | dict]) -> None:
     # TODO validation may also contain schema URLs
```

### Comparing `samshee-0.1.4/src/samshee.egg-info/PKG-INFO` & `samshee-0.1.5/src/samshee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.4
+Version: 0.1.5
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.4/tests/test_validation.py` & `samshee-0.1.5/tests/test_validation.py`

 * *Files identical despite different names*


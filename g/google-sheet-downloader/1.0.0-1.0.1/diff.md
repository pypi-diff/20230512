# Comparing `tmp/google-sheet-downloader-1.0.0.tar.gz` & `tmp/google-sheet-downloader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheet-downloader-1.0.0.tar", last modified: Fri May 12 07:13:42 2023, max compression
+gzip compressed data, was "google-sheet-downloader-1.0.1.tar", last modified: Fri May 12 07:15:36 2023, max compression
```

## Comparing `google-sheet-downloader-1.0.0.tar` & `google-sheet-downloader-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-12 07:13:42.176627 google-sheet-downloader-1.0.0/
--rw-rw-r--   0 root         (0) root         (0)     4031 2023-05-12 07:13:42.176155 google-sheet-downloader-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3850 2023-05-12 07:13:30.000000 google-sheet-downloader-1.0.0/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-12 07:13:42.093316 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4031 2023-05-12 07:13:40.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      329 2023-05-12 07:13:41.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-12 07:13:40.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       74 2023-05-12 07:13:40.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       75 2023-05-12 07:13:40.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       24 2023-05-12 07:13:40.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)     3052 2023-05-12 07:13:30.000000 google-sheet-downloader-1.0.0/google_sheet_downloader.py
--rw-rw-r--   0 root         (0) root         (0)       38 2023-05-12 07:13:42.176700 google-sheet-downloader-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      557 2023-05-12 07:13:30.000000 google-sheet-downloader-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:15:36.470198 google-sheet-downloader-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4031 2023-05-12 07:15:36.470100 google-sheet-downloader-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3850 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:15:36.469937 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4031 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      130 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       44 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3051 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/google_sheet_downloader.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 07:15:36.470230 google-sheet-downloader-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      638 2023-05-12 07:15:36.000000 google-sheet-downloader-1.0.1/setup.py
```

### Comparing `google-sheet-downloader-1.0.0/PKG-INFO` & `google-sheet-downloader-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Google Sheets 下載器
```

### Comparing `google-sheet-downloader-1.0.0/README.md` & `google-sheet-downloader-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `google-sheet-downloader-1.0.0/google_sheet_downloader.egg-info/PKG-INFO` & `google-sheet-downloader-1.0.1/google_sheet_downloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Google Sheets 下載器
```

### Comparing `google-sheet-downloader-1.0.0/google_sheet_downloader.py` & `google-sheet-downloader-1.0.1/google_sheet_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import glob
 import json
 import os
 
 import gspread
 from google.oauth2.service_account import Credentials
 
-
 def init_gspread(key_file):
     scopes = [
         "https://spreadsheets.google.com/feeds",
         'https://www.googleapis.com/auth/spreadsheets',
         "https://www.googleapis.com/auth/drive.file",
         "https://www.googleapis.com/auth/drive"
     ]
```


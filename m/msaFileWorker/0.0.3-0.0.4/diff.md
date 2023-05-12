# Comparing `tmp/msaFileWorker-0.0.3.tar.gz` & `tmp/msaFileWorker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msaFileWorker-0.0.3.tar", last modified: Thu Apr 13 12:11:15 2023, max compression
+gzip compressed data, was "msaFileWorker-0.0.4.tar", last modified: Fri May 12 16:08:45 2023, max compression
```

## Comparing `msaFileWorker-0.0.3.tar` & `msaFileWorker-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1100 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/LICENCE
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       58 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/MANIFEST.in
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2889 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/PKG-INFO
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1589 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/README.md
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/msaFileWorker/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      477 2023-04-13 12:11:06.000000 msaFileWorker-0.0.3/msaFileWorker/__init__.py
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/msaFileWorker/utils/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      229 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/msaFileWorker/utils/__init__.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       83 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/msaFileWorker/utils/constans.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     8195 2023-04-13 11:41:41.000000 msaFileWorker-0.0.3/msaFileWorker/utils/file_worker.py
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/msaFileWorker.egg-info/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2889 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/PKG-INFO
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      442 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       22 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/requires.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       14 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/top_level.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/zip-safe
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      855 2023-04-13 12:11:06.000000 msaFileWorker-0.0.3/pyproject.toml
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       42 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/requirements.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       38 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/setup.cfg
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2168 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/setup.py
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/tests/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     7642 2023-04-13 11:41:41.000000 msaFileWorker-0.0.3/tests/test_file_worker_func.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1100 2023-03-26 10:33:44.000000 msaFileWorker-0.0.4/LICENCE
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       58 2023-03-26 10:33:44.000000 msaFileWorker-0.0.4/MANIFEST.in
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2889 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/PKG-INFO
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1589 2023-03-26 10:33:44.000000 msaFileWorker-0.0.4/README.md
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/msaFileWorker/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      477 2023-05-12 16:07:39.000000 msaFileWorker-0.0.4/msaFileWorker/__init__.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/msaFileWorker/utils/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      229 2023-03-26 10:33:44.000000 msaFileWorker-0.0.4/msaFileWorker/utils/__init__.py
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       75 2023-05-12 12:17:04.000000 msaFileWorker-0.0.4/msaFileWorker/utils/constans.py
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     8187 2023-05-12 12:17:04.000000 msaFileWorker-0.0.4/msaFileWorker/utils/file_worker.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/msaFileWorker.egg-info/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2889 2023-05-12 16:08:45.000000 msaFileWorker-0.0.4/msaFileWorker.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      442 2023-05-12 16:08:45.000000 msaFileWorker-0.0.4/msaFileWorker.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-05-12 16:08:45.000000 msaFileWorker-0.0.4/msaFileWorker.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       22 2023-05-12 16:08:45.000000 msaFileWorker-0.0.4/msaFileWorker.egg-info/requires.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       14 2023-05-12 16:08:45.000000 msaFileWorker-0.0.4/msaFileWorker.egg-info/top_level.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-13 12:11:15.000000 msaFileWorker-0.0.4/msaFileWorker.egg-info/zip-safe
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      855 2023-05-12 16:08:42.000000 msaFileWorker-0.0.4/pyproject.toml
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       42 2023-03-26 10:33:44.000000 msaFileWorker-0.0.4/requirements.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       38 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/setup.cfg
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2168 2023-03-26 10:33:44.000000 msaFileWorker-0.0.4/setup.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-12 16:08:45.350429 msaFileWorker-0.0.4/tests/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     7634 2023-05-12 12:17:04.000000 msaFileWorker-0.0.4/tests/test_file_worker_func.py
```

### Comparing `msaFileWorker-0.0.3/LICENCE` & `msaFileWorker-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `msaFileWorker-0.0.3/PKG-INFO` & `msaFileWorker-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaFileWorker
-Version: 0.0.3
+Version: 0.0.4
 Summary: msaFileWorker - file management library
 Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaFileWorker.u2d.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.3 Summary: msaFileWorker
+Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.4 Summary: msaFileWorker
 - file management library Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker Author: Stefan Welcker
 Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
 msaFileWorker.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/
 msaFileWorker Project-URL: Tracker, https://github.com/u2d-ai/msaFileWorker/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `msaFileWorker-0.0.3/README.md` & `msaFileWorker-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `msaFileWorker-0.0.3/msaFileWorker/utils/file_worker.py` & `msaFileWorker-0.0.4/msaFileWorker/utils/file_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import BytesIO
 from typing import Dict, List, Tuple, Union
 from zipfile import ZIP_DEFLATED, ZipFile
 
 from msaFilesystem import msafs as fs
-from msaFileWorker.utils.constans import CLIENT_ID, SPK_NFS_SHARE
+from msaFileWorker.utils.constans import CLIENT_ID, NFS_SHARE
 
 
 class FileWorker:
     """
     Working with files
 
     Parameters:
@@ -18,15 +18,15 @@
         path_to_filestorage: path to shared filestorage. Work directory default
 
     """
 
     def __init__(
         self, subdomain: str, document_id: str, client_id: str = CLIENT_ID, path_to_filestorage: str = "."
     ) -> None:
-        self.client_folder_path = path_to_filestorage + f"/{SPK_NFS_SHARE}/{subdomain}/{client_id}/{document_id}"
+        self.client_folder_path = path_to_filestorage + f"/{NFS_SHARE}/{subdomain}/{client_id}/{document_id}"
         try:
             self.filesystem = fs.open_fs(self.client_folder_path)
         except fs.errors.CreateFailed:
             self.filesystem = fs.open_fs(".")
             self.filesystem.makedirs(self.client_folder_path)
             self.filesystem = fs.open_fs(self.client_folder_path)
```

### Comparing `msaFileWorker-0.0.3/msaFileWorker.egg-info/PKG-INFO` & `msaFileWorker-0.0.4/msaFileWorker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaFileWorker
-Version: 0.0.3
+Version: 0.0.4
 Summary: msaFileWorker - file management library
 Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaFileWorker.u2d.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.3 Summary: msaFileWorker
+Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.4 Summary: msaFileWorker
 - file management library Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker Author: Stefan Welcker
 Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
 msaFileWorker.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/
 msaFileWorker Project-URL: Tracker, https://github.com/u2d-ai/msaFileWorker/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `msaFileWorker-0.0.3/pyproject.toml` & `msaFileWorker-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "msaFileWorker"
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.black]
 line-length = 119
 
 [tool.isort]
 profile = "black"
 line_length = 119
```

### Comparing `msaFileWorker-0.0.3/setup.py` & `msaFileWorker-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `msaFileWorker-0.0.3/tests/test_file_worker_func.py` & `msaFileWorker-0.0.4/tests/test_file_worker_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
         subdomain=C.SUBDOMAIN,
         client_id=C.CLIENT_ID,
         path_to_filestorage=C.FILE_STORAGE_PATH,
         document_id=C.DOCUMENT_ID,
     )
     yield worker
     filesystem = fs.open_fs(C.FILE_STORAGE_PATH)
-    filesystem.removetree(C.SPK_NFS_SHARE)
+    filesystem.removetree(C.NFS_SHARE)
 
 
-local_path = f"{C.SPK_NFS_SHARE}/{C.SUBDOMAIN}/{C.CLIENT_ID}/{C.DOCUMENT_ID}/"
+local_path = f"{C.NFS_SHARE}/{C.SUBDOMAIN}/{C.CLIENT_ID}/{C.DOCUMENT_ID}/"
 
 
 class TestFileWorker:
     """Testing FileWoker functions"""
 
     @pytest.mark.asyncio
     async def test_save_bytes_file(self, worker) -> None:
```


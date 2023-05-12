# Comparing `tmp/driveup-0.4.0.tar.gz` & `tmp/driveup-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.4.0.tar", last modified: Tue May  9 12:36:56 2023, max compression
+gzip compressed data, was "driveup-0.5.0.tar", last modified: Fri May 12 11:45:54 2023, max compression
```

## Comparing `driveup-0.4.0.tar` & `driveup-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/Driveup/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/features/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 12:36:40.000000 driveup-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 12:36:56.903078 driveup-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 12:36:40.000000 driveup-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:36:56.903078 driveup-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 12:36:40.000000 driveup-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.997913 driveup-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.993914 driveup-0.5.0/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.997913 driveup-0.5.0/Driveup/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/features/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 11:45:39.000000 driveup-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 11:45:53.997913 driveup-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 11:45:39.000000 driveup-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.997913 driveup-0.5.0/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:45:53.997913 driveup-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-12 11:45:39.000000 driveup-0.5.0/setup.py
```

### Comparing `driveup-0.4.0/Driveup/drive.py` & `driveup-0.5.0/Driveup/drive.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,83 @@
+from typing import overload,Union,List
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload
 import os
 import re
 
 class Drive:
     def __init__(self,creds):
         self.mode = creds['type']
         self.service = build('drive', 'v3', credentials=creds['creds'])
     
-    def upload(self,file_path,folder_id,file_title=None,file_id=None,update=True,convert=False,url=True):
+    @overload
+    def upload(self,file_path:list,folder_id:Union[str, List[str]],file_title:str=None,file_id:Union[str, List[str]]=None,update=True,convert=False,url=True):
+        ...
+    @overload
+    def upload(self,file_path:str,folder_id:Union[str, List[str]],file_title:str=None,file_id:Union[str, List[str]]=None,update=True,convert=False,url=True):
+        ...
+    
+    def upload(self,file_path: Union[str, List[str]],folder_id:Union[str, List[str]],file_title:str=None,file_id: Union[str, List[str]]=None,update=True,convert=False,url=True):
 
-        if url == True:
-            folder_id = self.url_to_id(folder_id)
+        if isinstance(file_path, list):
+            if isinstance(folder_id, list): # needs a warning saying that will ignore file ids 
+                for file,folder in zip(file_path,folder_id):
+                    self.upload(file,folder_id=folder,file_title=file_title,file_id=file_id,update=update,convert=convert,url=url)
+            else:
+                if file_id == None: 
+                    for file in file_path:
+                        self.upload(file,folder_id,file_title=file_title,file_id=file_id,update=update,convert=convert,url=url)
+                else: # needs a warning controlling if sizes of both lists are the same
+                    for file,id in zip(file_path,file_id):
+                        self.upload(file,folder_id,file_title=file_title,file_id=id,update=update,convert=convert,url=url)
+        else:
+            if isinstance(file_id, list): # needs a warning saying that file_id as 'list' is not intended for a single path
+                # print ('warning')
+                file_id = file_id[0]
+            
+            if isinstance(folder_id, list): # needs a warning saying that folder_id as 'list' is not intended for a single path
+                # print ('warning')
+                folder_id = folder_id[0]
+                
+            if url == True:
+                folder_id = self.url_to_id(folder_id)
 
-        if file_title == None:
-            file_title = self.get_filename(file_path)
+            if file_title == None:
+                file_title = self.get_filename(file_path)
 
-        drive_service = self.service
+            drive_service = self.service
 
-        file_metadata = None
+            file_metadata = None
 
-        media = MediaFileUpload(file_path, resumable=True)
+            media = MediaFileUpload(file_path, resumable=True)
 
-        # possible refactor
-        if update == True:
-            file_metadata = self.get_update(file_title,file_id,folder_id,drive_service)
-                
-        if file_metadata == None: # Doesn't exist in the folder already or update=False
-            if self.mode == 'client':
-                file_metadata = {'name': file_title,'parents': [folder_id]}
-            else:
-                file_metadata = {'name': file_title,'parents': folder_id}
+            # possible refactor
+            if update == True:
+                file_metadata = self.get_update(file_title,file_id,folder_id,drive_service)
+                    
+            if file_metadata == None: # Doesn't exist in the folder already or update=False
+                if self.mode == 'client':
+                    file_metadata = {'name': file_title,'parents': [folder_id]}
+                else:
+                    file_metadata = {'name': file_title,'parents': folder_id}
 
-            if convert == True:
-                file_metadata = self.convert(file_metadata,self.get_file_extension(file_path))
+                if convert == True:
+                    file_metadata = self.convert(file_metadata,self.get_file_extension(file_path))
 
-            gfile = drive_service.files().create(body=file_metadata, media_body=media, fields='id').execute()
-        else:
-            file_id = file_metadata['id']
-            void_metadata = {}
-            gfile = drive_service.files().update(fileId=file_id, body=void_metadata, media_body=media).execute()
-
-        if self.mode == 'service':
-                old_parents = gfile.get('parents')
-                file_id = gfile.get('id')
+                gfile = drive_service.files().create(body=file_metadata, media_body=media, fields='id').execute()
+            else:
+                file_id = file_metadata['id']
+                void_metadata = {}
+                gfile = drive_service.files().update(fileId=file_id, body=void_metadata, media_body=media).execute()
+
+            if self.mode == 'service':
+                    old_parents = gfile.get('parents')
+                    file_id = gfile.get('id')
 
-                drive_service.files().update(fileId=file_id,removeParents=old_parents,addParents=folder_id).execute()
+                    drive_service.files().update(fileId=file_id,removeParents=old_parents,addParents=folder_id).execute()
 
     # returns metadata for the file (whether it exists or not)
     def get_update(self,name,file_id,folder_id,service):
         if self.mode == 'client':
             if file_id != None: # use specified id
                     file_metadata = {'id':file_id,'name': name,'parents': [folder_id]} # Change name: doesn't work
             else: # obtain id for duplicated file (file with same name) and overwrite
```

### Comparing `driveup-0.4.0/Driveup/features/auth.py` & `driveup-0.5.0/Driveup/features/auth.py`

 * *Files identical despite different names*

### Comparing `driveup-0.4.0/LICENSE` & `driveup-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.4.0/setup.py` & `driveup-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 # ...
 
 setup(
     long_description=README_DESCRIPTION,
     long_description_content_type="text/markdown",
     name='driveup',
-    version='0.4.0',
+    version='0.5.0',
     author='Raúl M.R.',
     author_email="raul.martin4bc@gmail.com",
+    url="https://github.com/raul-martin-dev/Driveup",
     license="MIT",
     description='Python package for uploading files and folders to Google Drive.',
     packages=find_packages(include=["Driveup","Driveup.features"]),
     install_requires=[
         'google-api-python-client',
         'google-auth-httplib2',
         'google-auth-oauthlib',
```


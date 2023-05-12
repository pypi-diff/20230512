# Comparing `tmp/ykenan_file-0.1.8.tar.gz` & `tmp/ykenan_file-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.8.tar", last modified: Wed May 10 10:51:58 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.9.tar", last modified: Thu May 11 01:03:38 2023, max compression
```

## Comparing `ykenan_file-0.1.8.tar` & `ykenan_file-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.414476 ykenan_file-0.1.8/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      827 2023-05-10 10:51:58.414476 ykenan_file-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.1.8/README.md
--rw-rw-rw-   0        0        0      696 2023-05-10 10:46:17.000000 ykenan_file-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       50 2023-05-10 10:43:14.000000 ykenan_file-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 10:51:58.414476 ykenan_file-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.399476 ykenan_file-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.403476 ykenan_file-0.1.8/src/ykenan_file/
--rw-rw-rw-   0        0        0    24001 2023-05-10 10:43:14.000000 ykenan_file-0.1.8/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.8/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:51:58.412476 ykenan_file-0.1.8/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      827 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 10:51:58.000000 ykenan_file-0.1.8/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 01:03:38.558085 ykenan_file-0.1.9/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      827 2023-05-11 01:03:38.558085 ykenan_file-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.1.9/README.md
+-rw-rw-rw-   0        0        0      716 2023-05-11 00:56:35.000000 ykenan_file-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       50 2023-05-10 10:43:14.000000 ykenan_file-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 01:03:38.559085 ykenan_file-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 01:03:38.521085 ykenan_file-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 01:03:38.546098 ykenan_file-0.1.9/src/ykenan_file/
+-rw-rw-rw-   0        0        0    27160 2023-05-11 01:02:52.000000 ykenan_file-0.1.9/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.9/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:03:38.557084 ykenan_file-0.1.9/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      827 2023-05-11 01:03:38.000000 ykenan_file-0.1.9/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-11 01:03:38.000000 ykenan_file-0.1.9/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 01:03:38.000000 ykenan_file-0.1.9/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-11 01:03:38.000000 ykenan_file-0.1.9/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 01:03:38.000000 ykenan_file-0.1.9/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.8/LICENSE` & `ykenan_file-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.8/PKG-INFO` & `ykenan_file-0.1.9/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ykenan_file
-Version: 0.1.8
+Name: ykenan-file
+Version: 0.1.9
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.8/pyproject.toml` & `ykenan_file-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3", "requests>=2.30.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["ykenan-log>=0.2.0", "pandas>=1.5.3"]
+dependencies = ["ykenan-log>=0.2.0", "pandas>=1.5.3", "requests>=2.30.0"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 github = "https://github.com/YuZhengM/ykenan_file"
```

### Comparing `ykenan_file-0.1.8/src/ykenan_file/__init__.py` & `ykenan_file-0.1.9/src/ykenan_file/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
-
+import gzip
 import os
+import shutil
+from multiprocessing.dummy import Lock
 
 import pandas as pd
 import requests
 from ykenan_log import Logger
 from pandas import DataFrame
 
 '''
@@ -599,16 +601,90 @@
         """
         Obtain all files in the specified path
         :param path: path
         :return: dirs
         """
         return self.entry_contents_dict(path, 2)
 
-    def download_file(self, url: str, filename: str, chunk_size: int = 1024):
-        self.log.info(f"下载 {url} 文件")
-        response_data_file = requests.get(url, stream=True)
-        self.log.info(f"创建 {filename} 文件")
-        with open(filename, 'wb') as f:
-            for chunk in response_data_file.iter_content(chunk_size=chunk_size):
-                if chunk:
-                    f.write(chunk)
-        self.log.info(f"下载 {url} ===> {filename} 文件完成")
+    def unzip_gz(self, gz_file: str, generate_file: str = None, is_force: bool = False) -> list:
+        if generate_file:
+            if os.path.exists(generate_file) and not is_force:
+                self.log.warn(f"{generate_file} The file already exists, it has been moved by default")
+            else:
+                self.log.info(f"Start unzip file {gz_file}")
+                w = open(generate_file, 'wb')
+                f = gzip.open(gz_file, 'rb')
+                read = f.read()
+                # Form a file
+                w.write(read)
+                # Obtaining Content Information
+                file_content: list = read.decode().rstrip().split("\n")
+                f.close()
+                w.close()
+                self.log.info(f"End of unzip file  {gz_file}")
+                return file_content
+        f = gzip.open(gz_file, 'rb')
+        # Obtaining Content Information
+        file_content: list = f.read().decode().rstrip().split("\n")
+        f.close()
+        return file_content
+
+    def download_file(self, url: str, filename: str, chunk_size: int = 1024, is_force: bool = False):
+        """
+        download file
+        :param url: 下载的 url
+        :param filename: 下载后的文件名
+        :param chunk_size: 下载流的大小
+        :param is_force: 是否强制覆盖
+        :return:
+        """
+        if os.path.exists(filename) and not is_force:
+            self.log.warn(f"{filename} The file already exists, it has been downloaded by default")
+        else:
+            self.log.info(f"下载 {url} 文件")
+            response_data_file = requests.get(url, stream=True)
+            self.log.info(f"创建 {filename} 文件")
+            with open(filename, 'wb') as f:
+                for chunk in response_data_file.iter_content(chunk_size=chunk_size):
+                    if chunk:
+                        f.write(chunk)
+            self.log.info(f"下载 {url} ===> {filename} 文件完成")
+
+    def copy_file(self, source_file: str, target_file: str, is_force: bool = False) -> None:
+        """
+        复制文件
+        :param source_file: 源文件
+        :param target_file: 目标文件
+        :param is_force: 是否强制覆盖
+        :return:
+        """
+        if os.path.exists(target_file) and not is_force:
+            self.log.warn(f"{target_file} The file already exists, it has been copied by default")
+        else:
+            self.log.info(f"Start copying file {source_file}")
+            shutil.copy(source_file, target_file)
+            self.log.info(f"End of copying file  {source_file}")
+
+    def move_file(self, source_file: str, target_file: str, is_force: bool = False) -> None:
+        """
+        移动文件
+        :param source_file: 源文件
+        :param target_file: 目标文件
+        :param is_force: 是否强制覆盖
+        :return:
+        """
+        if os.path.exists(target_file) and not is_force:
+            self.log.warn(f"{target_file} The file already exists, it has been moved by default")
+        else:
+            self.log.info(f"Start moving file {source_file}")
+            shutil.move(source_file, target_file)
+            self.log.info(f"End of moving file  {source_file}")
+
+    def makedirs(self, dirs: str, is_lock: bool = False):
+        lock = Lock()
+        if is_lock:
+            lock.locked()
+        if not os.path.exists(dirs):
+            self.log.info(f"创建 {dirs} 文件夹")
+            os.makedirs(dirs)
+        if is_lock:
+            lock.release()
```

### Comparing `ykenan_file-0.1.8/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ykenan-file
-Version: 0.1.8
+Name: ykenan_file
+Version: 0.1.9
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/netcdf-to-csv-1.0.1.tar.gz` & `tmp/netcdf-to-csv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcdf-to-csv-1.0.1.tar", last modified: Fri May 12 12:56:31 2023, max compression
+gzip compressed data, was "netcdf-to-csv-1.0.2.tar", last modified: Fri May 12 12:58:07 2023, max compression
```

## Comparing `netcdf-to-csv-1.0.1.tar` & `netcdf-to-csv-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 12:56:31.788656 netcdf-to-csv-1.0.1/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1221 2023-05-12 12:56:31.788554 netcdf-to-csv-1.0.1/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1122 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 12:56:31.788390 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1221 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      259 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       53 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        8 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     1364 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/netcdf_to_csv.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 12:56:31.788689 netcdf-to-csv-1.0.1/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      516 2023-05-12 12:56:31.000000 netcdf-to-csv-1.0.1/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 12:58:07.636977 netcdf-to-csv-1.0.2/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1233 2023-05-12 12:58:07.636868 netcdf-to-csv-1.0.2/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1134 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 12:58:07.636701 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1233 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      259 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       53 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        8 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     1364 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/netcdf_to_csv.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 12:58:07.637008 netcdf-to-csv-1.0.2/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      516 2023-05-12 12:58:07.000000 netcdf-to-csv-1.0.2/setup.py
```

### Comparing `netcdf-to-csv-1.0.1/PKG-INFO` & `netcdf-to-csv-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: netcdf-to-csv
-Version: 1.0.1
+Version: 1.0.2
 Description-Content-Type: text/markdown
 
 # netCDF 轉換工具
 
 這個專案包含兩個 Python 模組，用於操作 netCDF 格式的檔案。第一個模組 `netcdf_to_csv.py` 可將 netCDF 檔案轉換成 CSV 格式。第二個模組 `netcdf_meta.py` 可用來檢視 netCDF 檔案的元數據信息。
 
 ## 安裝
 
 首先，使用以下命令安裝所需的套件：
 
 ```bash
-python3 -m pip install netcdf-to-csv
+python3 -m pip install netcdf-to-csv netcdf-meta
 ```
 
 ## 模組使用
 
 ### netcdf_to_csv
 
 這個模組將 netCDF 檔案轉換成 CSV 格式。以下為使用方法和範例：
```

### Comparing `netcdf-to-csv-1.0.1/README.md` & `netcdf-to-csv-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 這個專案包含兩個 Python 模組，用於操作 netCDF 格式的檔案。第一個模組 `netcdf_to_csv.py` 可將 netCDF 檔案轉換成 CSV 格式。第二個模組 `netcdf_meta.py` 可用來檢視 netCDF 檔案的元數據信息。
 
 ## 安裝
 
 首先，使用以下命令安裝所需的套件：
 
 ```bash
-python3 -m pip install netcdf-to-csv
+python3 -m pip install netcdf-to-csv netcdf-meta
 ```
 
 ## 模組使用
 
 ### netcdf_to_csv
 
 這個模組將 netCDF 檔案轉換成 CSV 格式。以下為使用方法和範例：
```

### Comparing `netcdf-to-csv-1.0.1/netcdf_to_csv.egg-info/PKG-INFO` & `netcdf-to-csv-1.0.2/netcdf_to_csv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: netcdf-to-csv
-Version: 1.0.1
+Version: 1.0.2
 Description-Content-Type: text/markdown
 
 # netCDF 轉換工具
 
 這個專案包含兩個 Python 模組，用於操作 netCDF 格式的檔案。第一個模組 `netcdf_to_csv.py` 可將 netCDF 檔案轉換成 CSV 格式。第二個模組 `netcdf_meta.py` 可用來檢視 netCDF 檔案的元數據信息。
 
 ## 安裝
 
 首先，使用以下命令安裝所需的套件：
 
 ```bash
-python3 -m pip install netcdf-to-csv
+python3 -m pip install netcdf-to-csv netcdf-meta
 ```
 
 ## 模組使用
 
 ### netcdf_to_csv
 
 這個模組將 netCDF 檔案轉換成 CSV 格式。以下為使用方法和範例：
```

### Comparing `netcdf-to-csv-1.0.1/netcdf_to_csv.py` & `netcdf-to-csv-1.0.2/netcdf_to_csv.py`

 * *Files identical despite different names*

### Comparing `netcdf-to-csv-1.0.1/setup.py` & `netcdf-to-csv-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="netcdf-to-csv",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     py_modules=['netcdf_to_csv'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'netcdf_to_csv = netcdf_to_csv:main',
         ],
```


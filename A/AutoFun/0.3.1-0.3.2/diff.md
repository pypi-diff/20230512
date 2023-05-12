# Comparing `tmp/AutoFun-0.3.1.tar.gz` & `tmp/AutoFun-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFun-0.3.1.tar", last modified: Sat May  6 01:45:12 2023, max compression
+gzip compressed data, was "AutoFun-0.3.2.tar", last modified: Fri May 12 06:25:37 2023, max compression
```

## Comparing `AutoFun-0.3.1.tar` & `AutoFun-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.105734 AutoFun-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.077720 AutoFun-0.3.1/AutoFun/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.084725 AutoFun-0.3.1/AutoFun/CutPdf/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.086720 AutoFun-0.3.1/AutoFun/CutPdf/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/CutPdf/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.087720 AutoFun-0.3.1/AutoFun/CutPdf/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/CutPdf/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/CutPdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.088722 AutoFun-0.3.1/AutoFun/OcrFinish/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.089758 AutoFun-0.3.1/AutoFun/OcrFinish/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrFinish/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrFinish/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.090721 AutoFun-0.3.1/AutoFun/OcrPicFun/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.091721 AutoFun-0.3.1/AutoFun/OcrPicFun/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrPicFun/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.092721 AutoFun-0.3.1/AutoFun/OcrPicFun/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrPicFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrPicFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.094721 AutoFun-0.3.1/AutoFun/OcrTableFun/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.096721 AutoFun-0.3.1/AutoFun/OcrTableFun/Function/
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:53.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/Function/__init__.py
--rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:41.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/Function/saveLoad.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.100725 AutoFun-0.3.1/AutoFun/OcrTableFun/Ui/
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.102727 AutoFun-0.3.1/AutoFun/SplitPdfFun/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.103744 AutoFun-0.3.1/AutoFun/SplitPdfFun/Function/
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.1/AutoFun/SplitPdfFun/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.104727 AutoFun-0.3.1/AutoFun/SplitPdfFun/Ui/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:00:01.000000 AutoFun-0.3.1/AutoFun/SplitPdfFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:59.000000 AutoFun-0.3.1/AutoFun/SplitPdfFun/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.083734 AutoFun-0.3.1/AutoFun.egg-info/
--rw-rw-rw-   0        0        0      429 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      429 2023-05-06 01:45:12.106725 AutoFun-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.1/README.md
--rw-rw-rw-   0        0        0      135 2023-05-06 01:45:12.106725 AutoFun-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-06 01:45:07.000000 AutoFun-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.057476 AutoFun-0.3.2/
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.960801 AutoFun-0.3.2/AutoFun/
+-rw-rw-rw-   0        0        0    97792 2023-05-12 06:04:02.000000 AutoFun-0.3.2/AutoFun/AutoFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.972803 AutoFun-0.3.2/AutoFun/CutPdf/
+-rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.2/AutoFun/CutPdf/CutPdf.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.975801 AutoFun-0.3.2/AutoFun/CutPdf/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/CutPdf/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.2/AutoFun/CutPdf/Function/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.979801 AutoFun-0.3.2/AutoFun/CutPdf/Ui/
+-rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.2/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/CutPdf/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/CutPdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.984816 AutoFun-0.3.2/AutoFun/OcrFinish/
+-rw-rw-rw-   0        0        0   177664 2023-05-05 03:14:26.000000 AutoFun-0.3.2/AutoFun/OcrFinish/OcrFinish.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.988801 AutoFun-0.3.2/AutoFun/OcrFinish/Ui/
+-rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.2/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/OcrFinish/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/OcrFinish/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.992801 AutoFun-0.3.2/AutoFun/OcrPicFun/
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.002449 AutoFun-0.3.2/AutoFun/OcrPicFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/Function/dict_to_json.pyd
+-rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/Function/get_json.pyd
+-rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/Function/splitJpg.pyd
+-rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/OcrPicFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.007444 AutoFun-0.3.2/AutoFun/OcrPicFun/Ui/
+-rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/OcrPicFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.011443 AutoFun-0.3.2/AutoFun/OcrTableFun/
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.027445 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/saveLoad.py
+-rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Function/txt_OCR.db
+-rw-rw-rw-   0        0        0   194048 2023-05-05 06:43:24.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/OcrTableFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.031444 AutoFun-0.3.2/AutoFun/OcrTableFun/Ui/
+-rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.2/AutoFun/OcrTableFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.036444 AutoFun-0.3.2/AutoFun/SplitPdfFun/
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.051476 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
+-rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
+-rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
+-rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0   165376 2023-05-05 03:32:38.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/SplitPdfFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:37.055475 AutoFun-0.3.2/AutoFun/SplitPdfFun/Ui/
+-rw-rw-rw-   0        0        0    69632 2023-05-05 03:33:02.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.2/AutoFun/SplitPdfFun/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.2/AutoFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:25:36.967801 AutoFun-0.3.2/AutoFun.egg-info/
+-rw-rw-rw-   0        0        0      396 2023-05-12 06:25:36.000000 AutoFun-0.3.2/AutoFun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1695 2023-05-12 06:25:36.000000 AutoFun-0.3.2/AutoFun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 06:25:36.000000 AutoFun-0.3.2/AutoFun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 06:25:36.000000 AutoFun-0.3.2/AutoFun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      396 2023-05-12 06:25:37.057476 AutoFun-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.2/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-12 06:25:37.058443 AutoFun-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-05-12 06:20:01.000000 AutoFun-0.3.2/setup.py
```

### Comparing `AutoFun-0.3.1/AutoFun/OcrTableFun/Function/saveLoad.py` & `AutoFun-0.3.2/AutoFun/OcrTableFun/Function/saveLoad.py`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.1/LICENSE.txt` & `AutoFun-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.1/setup.py` & `AutoFun-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AutoFun",
 	version = VERSION,
-    author ="wangweidong",
-    author_email = "17891967090@163.com",
-    description='Due Diligence Toolkit Python project',
+    author="wangweidong",
+    author_email="17891967090@163.com",
+    description='文件拆分与加书签',
     long_description_content_type="text/markdown",
-	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
-	long_description = open('README.md',encoding="utf-8").read(),
+    url='https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
+    long_description=open('README.md', encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
-    # package_dir = {"":"aaa"},
-    # packages = find_packages(where="aaa"),
-	packages = find_packages(),
- 	# license = 'Apache',
-   	classifiers = [
-       'Programming Language :: Python',
+
+    packages=find_packages(),
+    # license = '',
+    classifiers=[
+        'Programming Language :: Python',
 
     ],
-    #包含的类型
-    package_data={'': ['*.csv', '*.txt','.toml', "*.pyd",'*.exe', '*.db']}, #这个很重要
-    include_package_data=True #也选上
+    # 包含的类型
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db']},  # 这个很重要
+    include_package_data=True  # 也选上
 
 )
```


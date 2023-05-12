# Comparing `tmp/google-sheet-downloader-1.0.2.tar.gz` & `tmp/google-sheet-downloader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheet-downloader-1.0.2.tar", last modified: Fri May 12 07:25:11 2023, max compression
+gzip compressed data, was "google-sheet-downloader-1.0.3.tar", last modified: Fri May 12 07:29:38 2023, max compression
```

## Comparing `google-sheet-downloader-1.0.2.tar` & `google-sheet-downloader-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:25:11.865649 google-sheet-downloader-1.0.2/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4959 2023-05-12 07:25:11.865544 google-sheet-downloader-1.0.2/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4778 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:25:11.865368 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4959 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      130 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       44 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3051 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/google_sheet_downloader.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 07:25:11.865682 google-sheet-downloader-1.0.2/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      638 2023-05-12 07:25:11.000000 google-sheet-downloader-1.0.2/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:29:38.854849 google-sheet-downloader-1.0.3/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4983 2023-05-12 07:29:38.854749 google-sheet-downloader-1.0.3/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4802 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:29:38.854577 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4983 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      130 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       44 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3051 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 07:29:38.854880 google-sheet-downloader-1.0.3/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      638 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/setup.py
```

### Comparing `google-sheet-downloader-1.0.2/PKG-INFO` & `google-sheet-downloader-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-Metadata-Version: 2.1
-Name: google-sheet-downloader
-Version: 1.0.2
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Google Sheets 下載器
 
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
 
-2023-05-12 15:23 小積木塊 google-sheet-downloader v1.0.2 Release Notes by Bowen Chiu
-
-Google Sheets 下載器:
-這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
+2023-05-12 15:26 
+- 小積木塊 google-sheet-downloader 
+- v1.0.3 Release Notes 
+- by Bowen Chiu
+
+Google Sheets 下載器介紹:
+- 這是一個能夠下載 Google Sheets 試算表的小工具。
+- 使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊
+- 程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 特色:
-. 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
-. 支援多個檔案下載
-. 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
+- 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
+- 支援多個檔案下載
+- 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
 
 使用:
-. 可以 CLI 運用 command line 可操作
-. 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
+- 可以 CLI 運用 command line 可操作
+- 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
 
 安裝:
-python3 -m pip install google-sheet-downloader
+- python3 -m pip install google-sheet-downloader
 
 用法:
-usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
+- usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
                                   OUTPUT_FOLDER [--force]
 
 ## 詳細說明
 
 1. 申請 Google 服務帳戶金鑰
     1. 進入 [Google Cloud Console](https://console.cloud.google.com/)
     2. 建立一個專案或使用現有的專案
@@ -118,9 +114,7 @@
 ```
 
 CLI 參數設計：
 
 - `--key-file`: Google 服務帳戶的密鑰 JSON 檔案路徑
 - `--sheet-ids`: 要下載的多個 Google 試算表的 ID，以逗號分隔
 - `--output-folder`: 輸出 CSV 檔案的資料夾路徑
-
-
```

### Comparing `google-sheet-downloader-1.0.2/README.md` & `google-sheet-downloader-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,46 @@
+Metadata-Version: 2.1
+Name: google-sheet-downloader
+Version: 1.0.3
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # Google Sheets 下載器
 
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
 
-2023-05-12 15:23 小積木塊 google-sheet-downloader v1.0.2 Release Notes by Bowen Chiu
-
-Google Sheets 下載器:
-這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
+2023-05-12 15:26 
+- 小積木塊 google-sheet-downloader 
+- v1.0.3 Release Notes 
+- by Bowen Chiu
+
+Google Sheets 下載器介紹:
+- 這是一個能夠下載 Google Sheets 試算表的小工具。
+- 使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊
+- 程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 特色:
-. 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
-. 支援多個檔案下載
-. 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
+- 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
+- 支援多個檔案下載
+- 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
 
 使用:
-. 可以 CLI 運用 command line 可操作
-. 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
+- 可以 CLI 運用 command line 可操作
+- 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
 
 安裝:
-python3 -m pip install google-sheet-downloader
+- python3 -m pip install google-sheet-downloader
 
 用法:
-usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
+- usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
                                   OUTPUT_FOLDER [--force]
 
 ## 詳細說明
 
 1. 申請 Google 服務帳戶金鑰
     1. 進入 [Google Cloud Console](https://console.cloud.google.com/)
     2. 建立一個專案或使用現有的專案
@@ -109,7 +123,9 @@
 ```
 
 CLI 參數設計：
 
 - `--key-file`: Google 服務帳戶的密鑰 JSON 檔案路徑
 - `--sheet-ids`: 要下載的多個 Google 試算表的 ID，以逗號分隔
 - `--output-folder`: 輸出 CSV 檔案的資料夾路徑
+
+
```

### Comparing `google-sheet-downloader-1.0.2/google_sheet_downloader.egg-info/PKG-INFO` & `google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Google Sheets 下載器
 
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
 
-2023-05-12 15:23 小積木塊 google-sheet-downloader v1.0.2 Release Notes by Bowen Chiu
-
-Google Sheets 下載器:
-這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
+2023-05-12 15:26 
+- 小積木塊 google-sheet-downloader 
+- v1.0.3 Release Notes 
+- by Bowen Chiu
+
+Google Sheets 下載器介紹:
+- 這是一個能夠下載 Google Sheets 試算表的小工具。
+- 使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊
+- 程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 特色:
-. 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
-. 支援多個檔案下載
-. 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
+- 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
+- 支援多個檔案下載
+- 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
 
 使用:
-. 可以 CLI 運用 command line 可操作
-. 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
+- 可以 CLI 運用 command line 可操作
+- 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
 
 安裝:
-python3 -m pip install google-sheet-downloader
+- python3 -m pip install google-sheet-downloader
 
 用法:
-usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
+- usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
                                   OUTPUT_FOLDER [--force]
 
 ## 詳細說明
 
 1. 申請 Google 服務帳戶金鑰
     1. 進入 [Google Cloud Console](https://console.cloud.google.com/)
     2. 建立一個專案或使用現有的專案
```

### Comparing `google-sheet-downloader-1.0.2/google_sheet_downloader.py` & `google-sheet-downloader-1.0.3/google_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `google-sheet-downloader-1.0.2/setup.py` & `google-sheet-downloader-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="google-sheet-downloader",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     py_modules=['google_sheet_downloader', 'requirements', 'README'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'google_sheet_downloader = google_sheet_downloader:main, requirements = requirements:main, README = README:main',
         ],
```


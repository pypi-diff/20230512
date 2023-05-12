# Comparing `tmp/google-sheet-downloader-1.0.3.tar.gz` & `tmp/google-sheet-downloader-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheet-downloader-1.0.3.tar", last modified: Fri May 12 07:29:38 2023, max compression
+gzip compressed data, was "google-sheet-downloader-1.0.4.tar", last modified: Fri May 12 07:34:40 2023, max compression
```

## Comparing `google-sheet-downloader-1.0.3.tar` & `google-sheet-downloader-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:29:38.854849 google-sheet-downloader-1.0.3/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4983 2023-05-12 07:29:38.854749 google-sheet-downloader-1.0.3/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4802 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:29:38.854577 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4983 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      130 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       44 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3051 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/google_sheet_downloader.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 07:29:38.854880 google-sheet-downloader-1.0.3/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      638 2023-05-12 07:29:38.000000 google-sheet-downloader-1.0.3/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:34:40.837172 google-sheet-downloader-1.0.4/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4694 2023-05-12 07:34:40.837065 google-sheet-downloader-1.0.4/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4513 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 07:34:40.836887 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4694 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      130 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       44 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3051 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/google_sheet_downloader.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 07:34:40.837205 google-sheet-downloader-1.0.4/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      638 2023-05-12 07:34:40.000000 google-sheet-downloader-1.0.4/setup.py
```

### Comparing `google-sheet-downloader-1.0.3/PKG-INFO` & `google-sheet-downloader-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# Google Sheets 下載器
-
+# 積木塊：Google Sheets 下載器 v1.0.4 by Bowen Chiu 2023-05-12 15:32
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
-
-2023-05-12 15:26 
-- 小積木塊 google-sheet-downloader 
-- v1.0.3 Release Notes 
-- by Bowen Chiu
-
-Google Sheets 下載器介紹:
-- 這是一個能夠下載 Google Sheets 試算表的小工具。
-- 使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊
-- 程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
-
 特色:
 - 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
 - 支援多個檔案下載
 - 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
-
-使用:
-- 可以 CLI 運用 command line 可操作
-- 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
+- 可 CLI 運用 command line 操作
+- 可 pip install package 當成套件呼叫而無須透過 CLI 也能用
 
 安裝:
-- python3 -m pip install google-sheet-downloader
+```
+python3 -m pip install google-sheet-downloader
+```
 
-用法:
-- usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
-                                  OUTPUT_FOLDER [--force]
+使用:
+```
+python3 -m google_sheet_downloader [-h] 
+   --key-file KEY_FILE 
+   --sheet-ids SHEET_IDS 
+   --output-folder OUTPUT_FOLDER 
+   [--force]                               
+```
 
 ## 詳細說明
 
 1. 申請 Google 服務帳戶金鑰
     1. 進入 [Google Cloud Console](https://console.cloud.google.com/)
     2. 建立一個專案或使用現有的專案
     3. 選擇左上角的導覽功能表 > API 和服務 > 憑證
@@ -50,15 +43,15 @@
 2. 安裝 Python 3.x
 3. 安裝相依套件
    ```sh
    pip install -r requirements.txt
    ```
 4. 執行程式
    ```sh
-   python main.py --key-file <金鑰檔案路徑> --sheet-ids <試算表 ID> --output-folder <輸出資料夾路徑>
+   python google-sheet-downloader.py --key-file <金鑰檔案路徑> --sheet-ids <試算表 ID> --output-folder <輸出資料夾路徑>
    ```
    可以同時下載多個試算表，試算表 ID 以逗號分隔。
    可以使用 `--force` 強制重新下載資料，忽略快取的檢查。
 
 ## 參數說明
 
 - `--key-file`：必填參數，Google 服務帳戶金鑰的 JSON 檔案路徑
```

### Comparing `google-sheet-downloader-1.0.3/README.md` & `google-sheet-downloader-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-# Google Sheets 下載器
-
+# 積木塊：Google Sheets 下載器 v1.0.4 by Bowen Chiu 2023-05-12 15:32
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
-
-2023-05-12 15:26 
-- 小積木塊 google-sheet-downloader 
-- v1.0.3 Release Notes 
-- by Bowen Chiu
-
-Google Sheets 下載器介紹:
-- 這是一個能夠下載 Google Sheets 試算表的小工具。
-- 使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊
-- 程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
-
 特色:
 - 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
 - 支援多個檔案下載
 - 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
-
-使用:
-- 可以 CLI 運用 command line 可操作
-- 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
+- 可 CLI 運用 command line 操作
+- 可 pip install package 當成套件呼叫而無須透過 CLI 也能用
 
 安裝:
-- python3 -m pip install google-sheet-downloader
+```
+python3 -m pip install google-sheet-downloader
+```
 
-用法:
-- usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
-                                  OUTPUT_FOLDER [--force]
+使用:
+```
+python3 -m google_sheet_downloader [-h] 
+   --key-file KEY_FILE 
+   --sheet-ids SHEET_IDS 
+   --output-folder OUTPUT_FOLDER 
+   [--force]                               
+```
 
 ## 詳細說明
 
 1. 申請 Google 服務帳戶金鑰
     1. 進入 [Google Cloud Console](https://console.cloud.google.com/)
     2. 建立一個專案或使用現有的專案
     3. 選擇左上角的導覽功能表 > API 和服務 > 憑證
@@ -41,15 +34,15 @@
 2. 安裝 Python 3.x
 3. 安裝相依套件
    ```sh
    pip install -r requirements.txt
    ```
 4. 執行程式
    ```sh
-   python main.py --key-file <金鑰檔案路徑> --sheet-ids <試算表 ID> --output-folder <輸出資料夾路徑>
+   python google-sheet-downloader.py --key-file <金鑰檔案路徑> --sheet-ids <試算表 ID> --output-folder <輸出資料夾路徑>
    ```
    可以同時下載多個試算表，試算表 ID 以逗號分隔。
    可以使用 `--force` 強制重新下載資料，忽略快取的檢查。
 
 ## 參數說明
 
 - `--key-file`：必填參數，Google 服務帳戶金鑰的 JSON 檔案路徑
```

### Comparing `google-sheet-downloader-1.0.3/google_sheet_downloader.egg-info/PKG-INFO` & `google-sheet-downloader-1.0.4/google_sheet_downloader.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# Google Sheets 下載器
-
+# 積木塊：Google Sheets 下載器 v1.0.4 by Bowen Chiu 2023-05-12 15:32
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
-
-2023-05-12 15:26 
-- 小積木塊 google-sheet-downloader 
-- v1.0.3 Release Notes 
-- by Bowen Chiu
-
-Google Sheets 下載器介紹:
-- 這是一個能夠下載 Google Sheets 試算表的小工具。
-- 使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊
-- 程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
-
 特色:
 - 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
 - 支援多個檔案下載
 - 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
-
-使用:
-- 可以 CLI 運用 command line 可操作
-- 可以 pip install package 當成套件呼叫無須用 CLI 也能呼叫
+- 可 CLI 運用 command line 操作
+- 可 pip install package 當成套件呼叫而無須透過 CLI 也能用
 
 安裝:
-- python3 -m pip install google-sheet-downloader
+```
+python3 -m pip install google-sheet-downloader
+```
 
-用法:
-- usage: google_sheet_downloader.py [-h] --key-file KEY_FILE --sheet-ids SHEET_IDS --output-folder
-                                  OUTPUT_FOLDER [--force]
+使用:
+```
+python3 -m google_sheet_downloader [-h] 
+   --key-file KEY_FILE 
+   --sheet-ids SHEET_IDS 
+   --output-folder OUTPUT_FOLDER 
+   [--force]                               
+```
 
 ## 詳細說明
 
 1. 申請 Google 服務帳戶金鑰
     1. 進入 [Google Cloud Console](https://console.cloud.google.com/)
     2. 建立一個專案或使用現有的專案
     3. 選擇左上角的導覽功能表 > API 和服務 > 憑證
@@ -50,15 +43,15 @@
 2. 安裝 Python 3.x
 3. 安裝相依套件
    ```sh
    pip install -r requirements.txt
    ```
 4. 執行程式
    ```sh
-   python main.py --key-file <金鑰檔案路徑> --sheet-ids <試算表 ID> --output-folder <輸出資料夾路徑>
+   python google-sheet-downloader.py --key-file <金鑰檔案路徑> --sheet-ids <試算表 ID> --output-folder <輸出資料夾路徑>
    ```
    可以同時下載多個試算表，試算表 ID 以逗號分隔。
    可以使用 `--force` 強制重新下載資料，忽略快取的檢查。
 
 ## 參數說明
 
 - `--key-file`：必填參數，Google 服務帳戶金鑰的 JSON 檔案路徑
```

### Comparing `google-sheet-downloader-1.0.3/google_sheet_downloader.py` & `google-sheet-downloader-1.0.4/google_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `google-sheet-downloader-1.0.3/setup.py` & `google-sheet-downloader-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="google-sheet-downloader",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     py_modules=['google_sheet_downloader', 'requirements', 'README'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'google_sheet_downloader = google_sheet_downloader:main, requirements = requirements:main, README = README:main',
         ],
```


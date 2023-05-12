# Comparing `tmp/AutoFun-0.3.3.tar.gz` & `tmp/AutoFun-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFun-0.3.3.tar", last modified: Fri May 12 08:11:37 2023, max compression
+gzip compressed data, was "AutoFun-0.3.4.tar", last modified: Fri May 12 09:20:57 2023, max compression
```

## Comparing `AutoFun-0.3.3.tar` & `AutoFun-0.3.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.756861 AutoFun-0.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.528169 AutoFun-0.3.3/AutoFun/
--rw-rw-rw-   0        0        0    97792 2023-05-12 06:04:02.000000 AutoFun-0.3.3/AutoFun/AutoFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.555244 AutoFun-0.3.3/AutoFun/CutPdf/
--rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.3/AutoFun/CutPdf/CutPdf.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.563337 AutoFun-0.3.3/AutoFun/CutPdf/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/CutPdf/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.3/AutoFun/CutPdf/Function/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.576362 AutoFun-0.3.3/AutoFun/CutPdf/Ui/
--rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.3/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/CutPdf/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/CutPdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.587409 AutoFun-0.3.3/AutoFun/OcrFinish/
--rw-rw-rw-   0        0        0   177664 2023-05-05 03:14:26.000000 AutoFun-0.3.3/AutoFun/OcrFinish/OcrFinish.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.597119 AutoFun-0.3.3/AutoFun/OcrFinish/Ui/
--rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.3/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/OcrFinish/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/OcrFinish/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.609069 AutoFun-0.3.3/AutoFun/OcrPicFun/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.629099 AutoFun-0.3.3/AutoFun/OcrPicFun/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/Function/__init__.py
--rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/Function/dict_to_json.pyd
--rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/Function/get_json.pyd
--rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/Function/splitJpg.pyd
--rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/OcrPicFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.640145 AutoFun-0.3.3/AutoFun/OcrPicFun/Ui/
--rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/OcrPicFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.652218 AutoFun-0.3.3/AutoFun/OcrTableFun/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.686708 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/
--rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/optionDb.pyd
--rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/saveLoad.py
--rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Function/txt_OCR.db
--rw-rw-rw-   0        0        0   194048 2023-05-05 06:43:24.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/OcrTableFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.697115 AutoFun-0.3.3/AutoFun/OcrTableFun/Ui/
--rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.3/AutoFun/OcrTableFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.705118 AutoFun-0.3.3/AutoFun/SplitPdfFun/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.742860 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/
--rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/optionDb.pyd
--rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
--rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
--rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
--rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
--rw-rw-rw-   0        0        0   167936 2023-05-12 08:06:13.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/SplitPdfFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.752860 AutoFun-0.3.3/AutoFun/SplitPdfFun/Ui/
--rw-rw-rw-   0        0        0    72192 2023-05-12 08:06:23.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.3/AutoFun/SplitPdfFun/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.3/AutoFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:11:37.544404 AutoFun-0.3.3/AutoFun.egg-info/
--rw-rw-rw-   0        0        0      396 2023-05-12 08:11:37.000000 AutoFun-0.3.3/AutoFun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1695 2023-05-12 08:11:37.000000 AutoFun-0.3.3/AutoFun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 08:11:37.000000 AutoFun-0.3.3/AutoFun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 08:11:37.000000 AutoFun-0.3.3/AutoFun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      396 2023-05-12 08:11:37.756861 AutoFun-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.3/README.md
--rw-rw-rw-   0        0        0      136 2023-05-12 08:11:37.758860 AutoFun-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-05-12 08:11:11.000000 AutoFun-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.277441 AutoFun-0.3.4/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.158741 AutoFun-0.3.4/AutoFun/
+-rw-rw-rw-   0        0        0    97792 2023-05-12 09:18:59.000000 AutoFun-0.3.4/AutoFun/AutoFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.176720 AutoFun-0.3.4/AutoFun/CutPdf/
+-rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.4/AutoFun/CutPdf/CutPdf.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.180720 AutoFun-0.3.4/AutoFun/CutPdf/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/CutPdf/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.4/AutoFun/CutPdf/Function/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.186721 AutoFun-0.3.4/AutoFun/CutPdf/Ui/
+-rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.4/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/CutPdf/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/CutPdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.191733 AutoFun-0.3.4/AutoFun/OcrFinish/
+-rw-rw-rw-   0        0        0   177664 2023-05-05 03:14:26.000000 AutoFun-0.3.4/AutoFun/OcrFinish/OcrFinish.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.197441 AutoFun-0.3.4/AutoFun/OcrFinish/Ui/
+-rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.4/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/OcrFinish/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/OcrFinish/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.203441 AutoFun-0.3.4/AutoFun/OcrPicFun/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.212441 AutoFun-0.3.4/AutoFun/OcrPicFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/Function/dict_to_json.pyd
+-rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/Function/get_json.pyd
+-rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/Function/splitJpg.pyd
+-rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/OcrPicFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.218443 AutoFun-0.3.4/AutoFun/OcrPicFun/Ui/
+-rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/OcrPicFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.223442 AutoFun-0.3.4/AutoFun/OcrTableFun/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.239475 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/saveLoad.py
+-rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Function/txt_OCR.db
+-rw-rw-rw-   0        0        0   194048 2023-05-05 06:43:24.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/OcrTableFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.244441 AutoFun-0.3.4/AutoFun/OcrTableFun/Ui/
+-rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.4/AutoFun/OcrTableFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.249441 AutoFun-0.3.4/AutoFun/SplitPdfFun/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.270441 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
+-rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
+-rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
+-rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0   167936 2023-05-12 08:06:13.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/SplitPdfFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.275441 AutoFun-0.3.4/AutoFun/SplitPdfFun/Ui/
+-rw-rw-rw-   0        0        0    72192 2023-05-12 08:06:23.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.4/AutoFun/SplitPdfFun/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.4/AutoFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:20:57.169729 AutoFun-0.3.4/AutoFun.egg-info/
+-rw-rw-rw-   0        0        0      396 2023-05-12 09:20:57.000000 AutoFun-0.3.4/AutoFun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1695 2023-05-12 09:20:57.000000 AutoFun-0.3.4/AutoFun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:20:57.000000 AutoFun-0.3.4/AutoFun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 09:20:57.000000 AutoFun-0.3.4/AutoFun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      396 2023-05-12 09:20:57.277441 AutoFun-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.4/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-12 09:20:57.278441 AutoFun-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-05-12 09:20:48.000000 AutoFun-0.3.4/setup.py
```

### Comparing `AutoFun-0.3.3/AutoFun/OcrTableFun/Function/saveLoad.py` & `AutoFun-0.3.4/AutoFun/OcrTableFun/Function/saveLoad.py`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.3/AutoFun.egg-info/SOURCES.txt` & `AutoFun-0.3.4/AutoFun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.3/LICENSE.txt` & `AutoFun-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.3/setup.py` & `AutoFun-0.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AutoFun",
```


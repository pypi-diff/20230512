# Comparing `tmp/alacorder-80.4.3.tar.gz` & `tmp/alacorder-80.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.4.3.tar", max compression
+gzip compressed data, was "alacorder-80.4.4.tar", max compression
```

## Comparing `alacorder-80.4.3.tar` & `alacorder-80.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.4.3/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.4.3/README.md
--rw-r--r--   0        0        0      697 2023-05-12 18:00:27.991352 alacorder-80.4.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-12 17:52:44.701723 alacorder-80.4.3/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.4.3/src/alacorder/__init__.py
--rw-r--r--   0        0        0   211579 2023-05-12 17:52:26.709216 alacorder-80.4.3/src/alacorder/__main__.py
--rw-r--r--   0        0        0   211579 2023-05-12 17:52:19.290694 alacorder-80.4.3/src/alacorder/alac.py
--rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 alacorder-80.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.4.4/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.4.4/README.md
+-rw-r--r--   0        0        0      697 2023-05-12 18:33:16.155816 alacorder-80.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-12 18:32:14.158198 alacorder-80.4.4/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.4.4/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   214884 2023-05-12 18:33:19.717988 alacorder-80.4.4/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   214884 2023-05-12 18:33:23.767750 alacorder-80.4.4/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 alacorder-80.4.4/PKG-INFO
```

### Comparing `alacorder-80.4.3/LICENSE` & `alacorder-80.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.4.3/README.md` & `alacorder-80.4.4/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.4.3/pyproject.toml` & `alacorder-80.4.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.4.3"
+version = "80.4.4"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.4.3/src/alacorder/.DS_Store` & `alacorder-80.4.4/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.4.3/src/alacorder/__main__.py` & `alacorder-80.4.4/src/alacorder/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     polars ^0.17.6, PyMuPDF ^1.21.1, 
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.4.3"
+version = "80.4.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2355,15 +2355,15 @@
                     pl.lit(" "),
                     pl.col("CourtActionDate"),
                 ]
             )
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
-            .str.replace(r'\.\s\.\s','.')
+            .str.replace(r"\.\s\.\s", ".")
             .alias("ChargesSummary")
         ]
     )
     charges = charges.with_columns(
         [
             pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
             pl.col("Category").cast(pl.Categorical),
@@ -3049,17 +3049,17 @@
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
 
 
 def read_query(path, qmax=0, qskip=0, window=None):
     if isinstance(path, dict):
         cf = path
-        qmax = cf['FETCH_MAX']
-        qskip = cf['FETCH_SKIP']
-        path = cf['INPUTS']
+        qmax = cf["FETCH_MAX"]
+        qskip = cf["FETCH_SKIP"]
+        path = cf["INPUTS"]
     if os.path.splitext(path)[1] in (".xlsx", ".xls"):
         query = pl.read_excel(
             path,
             xlsx2csv_options={"ignore_errors": True},
             read_csv_options={"ignore_errors": True},
         )
     elif os.path.splitext(path)[1] == ".csv":
@@ -5620,17 +5620,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
-def _cli_archive(
-    input_path, output_path, count, overwrite, no_log, no_prompt, debug
-):
+def _cli_archive(input_path, output_path, count, overwrite, no_log, no_prompt, debug):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to archive output
         count (int): Total cases to pull from input
@@ -6655,14 +6653,171 @@
             .group(1)
             .strip()
         )
     except:
         return ""
 
 
+def getTurnOverDate(text):
+    try:
+        return re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getTurnOverAmt(text):
+    try:
+        return float(re.search(r"TurnOver Amt\: \$(\d+\.\d\d)", str(text)).group(1))
+    except:
+        return ""
+
+
+def getFrequencyAmt(text):
+    try:
+        return float(re.search(r"Frequency Amt\: \$(\d+\.\d\d)", str(text)).group(1))
+    except:
+        return ""
+
+
+def getDueDate(text):
+    try:
+        return re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getLastPaidDate(text):
+    try:
+        return re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getPayor(text):
+    try:
+        return re.search(r"Payor\: ([A-Z0-9]{4})", str(text)).group(1)
+    except:
+        return ""
+
+
+def getEnforcementStatus(text):
+    try:
+        return re.sub(
+            r"F$",
+            "",
+            re.search(r"Enforcement Status\: ([A-Z\:,\s]+)", str(text)).group(1),
+        ).strip()
+    except:
+        return ""
+
+
+def getFrequency(text):
+    try:
+        return re.sub(
+            r"Cost Paid By\:", "", re.search(r"Frequency\: ([W|M])", str(text)).group(1)
+        )
+    except:
+        return ""
+
+
+def getPlacementStatus(text):
+    try:
+        return re.search(r"Placement Status\: (.+)", str(text)).group(1).strip()
+    except:
+        return ""
+
+
+def getPreTrial(text):
+    try:
+        return re.search(r"PreTrial\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getPreTrialDate(text):
+    try:
+        return re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip()
+    except:
+        return ""
+
+
+def getPreTrialTerms(text):
+    try:
+        return re.search(r"PreTrial Terms\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getPreTermsDate(text):
+    try:
+        return re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getDelinquent(text):
+    try:
+        return re.search(r"Delinquent\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getDelinquentDate(text):
+    try:
+        return re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(
+            1
+        )
+    except:
+        return ""
+
+
+def getDAMailer(text):
+    try:
+        return re.search(r"DA Mailer\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getDAMailerDate(text):
+    try:
+        return re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getWarrantMailer(text):
+    try:
+        return re.search(r"Warrant Mailer\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getWarrantMailerDate(text):
+    try:
+        return re.search(
+            r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)
+        ).group(1)
+    except:
+        return ""
+
+
+def getEnforcementLastUpdate(text):
+    try:
+        return re.search(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getEnforcementUpdatedBy(text):
+    try:
+        return re.search(r"Updated By\: ([A-Z]{3})", str(text)).group(1)
+    except:
+        return ""
+
+
 def getSentencingRequirementsCompleted(text):
     try:
         return re.sub(
             r"[\n:]|Requrements Completed",
             "",
             ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
         )
```

### Comparing `alacorder-80.4.3/src/alacorder/alac.py` & `alacorder-80.4.4/src/alacorder/alac.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     polars ^0.17.6, PyMuPDF ^1.21.1, 
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.4.3"
+version = "80.4.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2355,15 +2355,15 @@
                     pl.lit(" "),
                     pl.col("CourtActionDate"),
                 ]
             )
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
-            .str.replace(r'\.\s\.\s','.')
+            .str.replace(r"\.\s\.\s", ".")
             .alias("ChargesSummary")
         ]
     )
     charges = charges.with_columns(
         [
             pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
             pl.col("Category").cast(pl.Categorical),
@@ -3049,17 +3049,17 @@
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
 
 
 def read_query(path, qmax=0, qskip=0, window=None):
     if isinstance(path, dict):
         cf = path
-        qmax = cf['FETCH_MAX']
-        qskip = cf['FETCH_SKIP']
-        path = cf['INPUTS']
+        qmax = cf["FETCH_MAX"]
+        qskip = cf["FETCH_SKIP"]
+        path = cf["INPUTS"]
     if os.path.splitext(path)[1] in (".xlsx", ".xls"):
         query = pl.read_excel(
             path,
             xlsx2csv_options={"ignore_errors": True},
             read_csv_options={"ignore_errors": True},
         )
     elif os.path.splitext(path)[1] == ".csv":
@@ -5620,17 +5620,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
-def _cli_archive(
-    input_path, output_path, count, overwrite, no_log, no_prompt, debug
-):
+def _cli_archive(input_path, output_path, count, overwrite, no_log, no_prompt, debug):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to archive output
         count (int): Total cases to pull from input
@@ -6655,14 +6653,171 @@
             .group(1)
             .strip()
         )
     except:
         return ""
 
 
+def getTurnOverDate(text):
+    try:
+        return re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getTurnOverAmt(text):
+    try:
+        return float(re.search(r"TurnOver Amt\: \$(\d+\.\d\d)", str(text)).group(1))
+    except:
+        return ""
+
+
+def getFrequencyAmt(text):
+    try:
+        return float(re.search(r"Frequency Amt\: \$(\d+\.\d\d)", str(text)).group(1))
+    except:
+        return ""
+
+
+def getDueDate(text):
+    try:
+        return re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getLastPaidDate(text):
+    try:
+        return re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getPayor(text):
+    try:
+        return re.search(r"Payor\: ([A-Z0-9]{4})", str(text)).group(1)
+    except:
+        return ""
+
+
+def getEnforcementStatus(text):
+    try:
+        return re.sub(
+            r"F$",
+            "",
+            re.search(r"Enforcement Status\: ([A-Z\:,\s]+)", str(text)).group(1),
+        ).strip()
+    except:
+        return ""
+
+
+def getFrequency(text):
+    try:
+        return re.sub(
+            r"Cost Paid By\:", "", re.search(r"Frequency\: ([W|M])", str(text)).group(1)
+        )
+    except:
+        return ""
+
+
+def getPlacementStatus(text):
+    try:
+        return re.search(r"Placement Status\: (.+)", str(text)).group(1).strip()
+    except:
+        return ""
+
+
+def getPreTrial(text):
+    try:
+        return re.search(r"PreTrial\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getPreTrialDate(text):
+    try:
+        return re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip()
+    except:
+        return ""
+
+
+def getPreTrialTerms(text):
+    try:
+        return re.search(r"PreTrial Terms\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getPreTermsDate(text):
+    try:
+        return re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getDelinquent(text):
+    try:
+        return re.search(r"Delinquent\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getDelinquentDate(text):
+    try:
+        return re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(
+            1
+        )
+    except:
+        return ""
+
+
+def getDAMailer(text):
+    try:
+        return re.search(r"DA Mailer\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getDAMailerDate(text):
+    try:
+        return re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getWarrantMailer(text):
+    try:
+        return re.search(r"Warrant Mailer\: (YES|NO)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getWarrantMailerDate(text):
+    try:
+        return re.search(
+            r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)
+        ).group(1)
+    except:
+        return ""
+
+
+def getEnforcementLastUpdate(text):
+    try:
+        return re.search(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+    except:
+        return ""
+
+
+def getEnforcementUpdatedBy(text):
+    try:
+        return re.search(r"Updated By\: ([A-Z]{3})", str(text)).group(1)
+    except:
+        return ""
+
+
 def getSentencingRequirementsCompleted(text):
     try:
         return re.sub(
             r"[\n:]|Requrements Completed",
             "",
             ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
         )
```

### Comparing `alacorder-80.4.3/PKG-INFO` & `alacorder-80.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.4.3
+Version: 80.4.4
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


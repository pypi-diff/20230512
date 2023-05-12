# Comparing `tmp/countryguess-0.3.0.tar.gz` & `tmp/countryguess-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countryguess-0.3.0.tar", last modified: Sun Mar  5 16:41:39 2023, max compression
+gzip compressed data, was "countryguess-0.4.0.tar", last modified: Fri May 12 14:30:14 2023, max compression
```

## Comparing `countryguess-0.3.0.tar` & `countryguess-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-03-05 16:41:39.967961 countryguess-0.3.0/
--rw-------   0 ich       (1000) ich       (1000)    35149 2022-10-10 15:59:38.000000 countryguess-0.3.0/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     6941 2023-03-05 16:41:39.967961 countryguess-0.3.0/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     6516 2023-03-05 16:25:25.000000 countryguess-0.3.0/README.md
-drwx------   0 ich       (1000) ich       (1000)        0 2023-03-05 16:41:39.967961 countryguess-0.3.0/countryguess/
--rw-------   0 ich       (1000) ich       (1000)      316 2023-03-05 16:35:36.000000 countryguess-0.3.0/countryguess/__init__.py
--rw-------   0 ich       (1000) ich       (1000)       31 2022-10-10 15:59:38.000000 countryguess-0.3.0/countryguess/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     1166 2022-10-10 15:59:38.000000 countryguess-0.3.0/countryguess/_cli.py
--rw-------   0 ich       (1000) ich       (1000)   255206 2023-03-05 16:19:13.000000 countryguess-0.3.0/countryguess/_countrydata.json
--rw-------   0 ich       (1000) ich       (1000)     5971 2023-03-05 16:19:17.000000 countryguess-0.3.0/countryguess/_countrydata.py
--rw-------   0 ich       (1000) ich       (1000)      655 2023-03-05 16:31:28.000000 countryguess-0.3.0/countryguess/_guess_country.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-03-05 16:41:39.967961 countryguess-0.3.0/countryguess.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     6941 2023-03-05 16:41:39.000000 countryguess-0.3.0/countryguess.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      371 2023-03-05 16:41:39.000000 countryguess-0.3.0/countryguess.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-03-05 16:41:39.000000 countryguess-0.3.0/countryguess.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       55 2023-03-05 16:41:39.000000 countryguess-0.3.0/countryguess.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       13 2023-03-05 16:41:39.000000 countryguess-0.3.0/countryguess.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)       38 2023-03-05 16:41:39.967961 countryguess-0.3.0/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1247 2023-03-05 16:33:41.000000 countryguess-0.3.0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-12 14:30:14.906351 countryguess-0.4.0/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2022-10-10 15:59:38.000000 countryguess-0.4.0/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     7030 2023-05-12 14:30:14.906351 countryguess-0.4.0/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     6605 2023-05-12 12:01:04.000000 countryguess-0.4.0/README.md
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-12 14:30:14.906351 countryguess-0.4.0/countryguess/
+-rw-------   0 ich       (1000) ich       (1000)      316 2023-05-12 14:25:58.000000 countryguess-0.4.0/countryguess/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)       31 2022-10-10 15:59:38.000000 countryguess-0.4.0/countryguess/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     1166 2022-10-10 15:59:38.000000 countryguess-0.4.0/countryguess/_cli.py
+-rw-------   0 ich       (1000) ich       (1000)   262399 2023-05-12 12:01:03.000000 countryguess-0.4.0/countryguess/_countrydata.json
+-rw-------   0 ich       (1000) ich       (1000)     6074 2023-03-12 11:09:04.000000 countryguess-0.4.0/countryguess/_countrydata.py
+-rw-------   0 ich       (1000) ich       (1000)      655 2023-03-05 16:31:28.000000 countryguess-0.4.0/countryguess/_guess_country.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-12 14:30:14.906351 countryguess-0.4.0/countryguess.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     7030 2023-05-12 14:30:14.000000 countryguess-0.4.0/countryguess.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      371 2023-05-12 14:30:14.000000 countryguess-0.4.0/countryguess.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-05-12 14:30:14.000000 countryguess-0.4.0/countryguess.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       55 2023-05-12 14:30:14.000000 countryguess-0.4.0/countryguess.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       13 2023-05-12 14:30:14.000000 countryguess-0.4.0/countryguess.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-05-12 14:30:14.906351 countryguess-0.4.0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1247 2023-03-05 16:33:41.000000 countryguess-0.4.0/setup.py
```

### Comparing `countryguess-0.3.0/LICENSE` & `countryguess-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `countryguess-0.3.0/PKG-INFO` & `countryguess-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countryguess
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fuzzy lookup of country information
 Home-page: https://codeberg.org/plotski/countryguess
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
@@ -159,14 +159,15 @@
 30. [GBDcode](http://ghdx.healthdata.org/) (numeric - Global Burden of
     Disease country codes)
 31. [IEA](https://www.iea.org/countries) (World Energy Balances 2021)
 32. [DACcode](https://www.oecd.org/dac/financing-sustainable-development/development-finance-standards/dacandcrscodelists.htm)
     (numeric - OECD Development Assistance Committee)
 33. [ccTLD](https://en.wikipedia.org/wiki/Country_code_top-level_domain) - country code top-level domains
 34. [GWcode](https://www.tandfonline.com/doi/abs/10.1080/03050629908434958) - Gledisch & Ward numerical codes as published in https://www.andybeger.com/states/articles/statelists.html
+35. CC41 - common classification for MRIOs (list of countries found in all public MRIOs)
 <!-- CLASSIFICATION_SCHEMES -->
 
 ### Command Line Interface
 
 **countryguess** comes with a simple CLI with the same name. It takes one or two
 arguments:
```

### Comparing `countryguess-0.3.0/README.md` & `countryguess-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 30. [GBDcode](http://ghdx.healthdata.org/) (numeric - Global Burden of
     Disease country codes)
 31. [IEA](https://www.iea.org/countries) (World Energy Balances 2021)
 32. [DACcode](https://www.oecd.org/dac/financing-sustainable-development/development-finance-standards/dacandcrscodelists.htm)
     (numeric - OECD Development Assistance Committee)
 33. [ccTLD](https://en.wikipedia.org/wiki/Country_code_top-level_domain) - country code top-level domains
 34. [GWcode](https://www.tandfonline.com/doi/abs/10.1080/03050629908434958) - Gledisch & Ward numerical codes as published in https://www.andybeger.com/states/articles/statelists.html
+35. CC41 - common classification for MRIOs (list of countries found in all public MRIOs)
 <!-- CLASSIFICATION_SCHEMES -->
 
 ### Command Line Interface
 
 **countryguess** comes with a simple CLI with the same name. It takes one or two
 arguments:
```

### Comparing `countryguess-0.3.0/countryguess/_cli.py` & `countryguess-0.4.0/countryguess/_cli.py`

 * *Files identical despite different names*

### Comparing `countryguess-0.3.0/countryguess/_countrydata.json` & `countryguess-0.4.0/countryguess/_countrydata.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.979166666666663%*

 * *Differences: {'0': "{'cc41': 'Rest of World'}",*

 * * '1': "{'cc41': 'Rest of World'}",*

 * * '10': "{'cc41': 'Rest of World'}",*

 * * '100': "{'cc41': 'Rest of World'}",*

 * * '101': "{'cc41': 'Rest of World'}",*

 * * '102': "{'cc41': 'Rest of World'}",*

 * * '103': "{'cc41': 'Hungary'}",*

 * * '104': "{'cc41': 'Rest of World'}",*

 * * '105': "{'cc41': 'India'}",*

 * * '106': "{'cc41': 'Indonesia'}",*

 * * '107': "{'cc41': 'Rest of World'}",*

 * * '108': "{'cc41': 'Rest of World'}",*

 * * '109': "{'cc41': 'Ireland'}",*

 * * '11': "{'cc41': 'Rest of World'}",*

 * * '110': "{'cc41': 'Rest  […]*

```diff
@@ -1,12 +1,13 @@
 [
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "af",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "625",
         "eea": "",
         "eora": "AFG",
@@ -48,14 +49,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ax",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "ALA",
@@ -97,14 +99,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "al",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "71",
         "eea": "",
         "eora": "ALB",
@@ -146,14 +149,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "dz",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "130",
         "eea": "",
         "eora": "DZA",
@@ -195,14 +199,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "as",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "880",
         "eea": "",
         "eora": "ASM",
@@ -244,14 +249,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ad",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "AND",
@@ -293,14 +299,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ao",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "225",
         "eea": "",
         "eora": "AGO",
@@ -342,14 +349,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ai",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "AIA",
@@ -391,14 +399,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "aq",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Antarctica",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -440,14 +449,15 @@
         "unregion": "Antarctica",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ag",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "377",
         "eea": "",
         "eora": "ATG",
@@ -489,14 +499,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ar",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "425",
         "eea": "",
         "eora": "ARG",
@@ -538,14 +549,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "am",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Asia",
         "daccode": "610",
         "eea": "",
         "eora": "ARM",
@@ -587,14 +599,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "aw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "ABW",
@@ -636,14 +649,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Australia",
         "cctld": "au",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "Oceania",
         "daccode": "801",
         "eea": "",
         "eora": "AUS",
@@ -685,14 +699,15 @@
         "unregion": "Australia and New Zealand",
         "wiod": "AUS"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Austria",
         "cctld": "at",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "1",
         "eea": "EEA",
         "eora": "AUT",
@@ -734,14 +749,15 @@
         "unregion": "Western Europe",
         "wiod": "AUT"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "az",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Asia",
         "daccode": "611",
         "eea": "",
         "eora": "AZE",
@@ -783,14 +799,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bs",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "BHS",
@@ -832,14 +849,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bh",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "BHR",
@@ -881,14 +899,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bd",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "666",
         "eea": "",
         "eora": "BGD",
@@ -930,14 +949,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bb",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "BRB",
@@ -979,14 +999,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "by",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Europe",
         "daccode": "86",
         "eea": "",
         "eora": "BLR",
@@ -1028,14 +1049,15 @@
         "unregion": "Eastern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Belgium",
         "cctld": "be",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "2",
         "eea": "EEA",
         "eora": "BEL",
@@ -1077,14 +1099,15 @@
         "unregion": "Western Europe",
         "wiod": "BEL"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bz",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "352",
         "eea": "",
         "eora": "BLZ",
@@ -1126,14 +1149,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bj",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "236",
         "eea": "",
         "eora": "BEN",
@@ -1175,14 +1199,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "BMU",
@@ -1224,14 +1249,15 @@
         "unregion": "Northern America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bt",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "630",
         "eea": "",
         "eora": "BTN",
@@ -1273,14 +1299,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bo",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "428",
         "eea": "",
         "eora": "BOL",
@@ -1322,14 +1349,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bq",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -1371,14 +1399,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ba",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "64",
         "eea": "",
         "eora": "BIH",
@@ -1420,14 +1449,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "227",
         "eea": "",
         "eora": "BWA",
@@ -1469,14 +1499,15 @@
         "unregion": "Southern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Antarctica",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -1518,14 +1549,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "BASIC",
         "bric": "BRIC",
+        "cc41": "Brazil",
         "cctld": "br",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "America",
         "daccode": "431",
         "eea": "",
         "eora": "BRA",
@@ -1567,14 +1599,15 @@
         "unregion": "South America",
         "wiod": "BRA"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Antarctica",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -1616,14 +1649,15 @@
         "unregion": "",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "io",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -1665,14 +1699,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "vg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "VGB",
@@ -1714,14 +1749,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "BRN",
@@ -1763,14 +1799,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Bulgaria",
         "cctld": "bg",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "72",
         "eea": "EEA",
         "eora": "BGR",
@@ -1812,14 +1849,15 @@
         "unregion": "Eastern Europe",
         "wiod": "BGR"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "287",
         "eea": "",
         "eora": "BFA",
@@ -1861,14 +1899,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "bi",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "228",
         "eea": "",
         "eora": "BDI",
@@ -1910,14 +1949,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cv",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "230",
         "eea": "",
         "eora": "CPV",
@@ -1959,14 +1999,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "kh",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "728",
         "eea": "",
         "eora": "KHM",
@@ -2008,14 +2049,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "229",
         "eea": "",
         "eora": "CMR",
@@ -2057,14 +2099,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Canada",
         "cctld": "ca",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "America",
         "daccode": "301",
         "eea": "",
         "eora": "CAN",
@@ -2106,14 +2149,15 @@
         "unregion": "Northern America",
         "wiod": "CAN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ky",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "CYM",
@@ -2155,14 +2199,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "231",
         "eea": "",
         "eora": "CAF",
@@ -2204,14 +2249,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "td",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "232",
         "eea": "",
         "eora": "TCD",
@@ -2253,14 +2299,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -2302,14 +2349,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cl",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "CHL",
@@ -2351,14 +2399,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "BASIC",
         "bric": "BRIC",
+        "cc41": "China",
         "cctld": "cn",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "Asia",
         "daccode": "730",
         "eea": "",
         "eora": "CHN",
@@ -2400,14 +2449,15 @@
         "unregion": "Eastern Asia",
         "wiod": "CHN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cx",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -2449,14 +2499,15 @@
         "unregion": "Australia and New Zealand",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -2498,14 +2549,15 @@
         "unregion": "Australia and New Zealand",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "co",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "437",
         "eea": "",
         "eora": "COL",
@@ -2547,14 +2599,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "km",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "233",
         "eea": "",
         "eora": "COM",
@@ -2596,14 +2649,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "234",
         "eea": "",
         "eora": "COG",
@@ -2645,14 +2699,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ck",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "COK",
@@ -2694,14 +2749,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "336",
         "eea": "",
         "eora": "CRI",
@@ -2743,14 +2799,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ci",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "247",
         "eea": "",
         "eora": "CIV",
@@ -2792,14 +2849,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "hr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "62",
         "eea": "EEA",
         "eora": "HRV",
@@ -2841,14 +2899,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cu",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "338",
         "eea": "",
         "eora": "CUB",
@@ -2890,14 +2949,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -2939,14 +2999,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Cyprus",
         "cctld": "cy",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Asia",
         "daccode": "30",
         "eea": "EEA",
         "eora": "CYP",
@@ -2988,14 +3049,15 @@
         "unregion": "Western Asia",
         "wiod": "CYP"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Czech Republic",
         "cctld": "cz",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "68",
         "eea": "EEA",
         "eora": "CZE",
@@ -3037,14 +3099,15 @@
         "unregion": "Eastern Europe",
         "wiod": "CZE"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Denmark",
         "cctld": "dk",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "3",
         "eea": "EEA",
         "eora": "DNK",
@@ -3086,14 +3149,15 @@
         "unregion": "Northern Europe",
         "wiod": "DNK"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "dj",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "274",
         "eea": "",
         "eora": "DJI",
@@ -3135,14 +3199,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "dm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "378",
         "eea": "",
         "eora": "DMA",
@@ -3184,14 +3249,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "do",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "340",
         "eea": "",
         "eora": "DOM",
@@ -3233,14 +3299,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "cd",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "235",
         "eea": "",
         "eora": "COD",
@@ -3282,14 +3349,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ec",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "440",
         "eea": "",
         "eora": "ECU",
@@ -3331,14 +3399,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "eg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "142",
         "eea": "",
         "eora": "EGY",
@@ -3380,14 +3449,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sv",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "342",
         "eea": "",
         "eora": "SLV",
@@ -3429,14 +3499,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gq",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "245",
         "eea": "",
         "eora": "GNQ",
@@ -3478,14 +3549,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "er",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "271",
         "eea": "",
         "eora": "ERI",
@@ -3527,14 +3599,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Estonia",
         "cctld": "ee",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "82",
         "eea": "EEA",
         "eora": "EST",
@@ -3576,14 +3649,15 @@
         "unregion": "Northern Europe",
         "wiod": "EST"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sz",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "280",
         "eea": "",
         "eora": "SWZ",
@@ -3625,14 +3699,15 @@
         "unregion": "Southern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "et",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "238",
         "eea": "",
         "eora": "ETH",
@@ -3674,14 +3749,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "fo",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "FRO",
@@ -3723,14 +3799,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "fk",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "FLK",
@@ -3772,14 +3849,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "fj",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "832",
         "eea": "",
         "eora": "FJI",
@@ -3821,14 +3899,15 @@
         "unregion": "Melanesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Finland",
         "cctld": "fi",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "18",
         "eea": "EEA",
         "eora": "FIN",
@@ -3870,14 +3949,15 @@
         "unregion": "Northern Europe",
         "wiod": "FIN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "France",
         "cctld": "fr",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "4",
         "eea": "EEA",
         "eora": "FRA",
@@ -3919,14 +3999,15 @@
         "unregion": "Western Europe",
         "wiod": "FRA"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "GUF",
@@ -3968,14 +4049,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "PYF",
@@ -4017,14 +4099,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -4066,14 +4149,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ga",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "239",
         "eea": "",
         "eora": "GAB",
@@ -4115,14 +4199,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "240",
         "eea": "",
         "eora": "GMB",
@@ -4164,14 +4249,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ge",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "612",
         "eea": "",
         "eora": "GEO",
@@ -4213,14 +4299,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Germany",
         "cctld": "de",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "5",
         "eea": "EEA",
         "eora": "DEU",
@@ -4262,14 +4349,15 @@
         "unregion": "Western Europe",
         "wiod": "DEU"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gh",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "241",
         "eea": "",
         "eora": "GHA",
@@ -4311,14 +4399,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gi",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "GIB",
@@ -4360,14 +4449,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Greece",
         "cctld": "gr",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "40",
         "eea": "EEA",
         "eora": "GRC",
@@ -4409,14 +4499,15 @@
         "unregion": "Southern Europe",
         "wiod": "GRC"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gl",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "GRL",
@@ -4458,14 +4549,15 @@
         "unregion": "Northern America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gd",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "381",
         "eea": "",
         "eora": "GRD",
@@ -4507,14 +4599,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gp",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "GLP",
@@ -4556,14 +4649,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gu",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "GUM",
@@ -4605,14 +4699,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gt",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "347",
         "eea": "",
         "eora": "GTM",
@@ -4654,14 +4749,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "GGY",
@@ -4703,14 +4799,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "243",
         "eea": "",
         "eora": "GIN",
@@ -4752,14 +4849,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "244",
         "eea": "",
         "eora": "GNB",
@@ -4801,14 +4899,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gy",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "446",
         "eea": "",
         "eora": "GUY",
@@ -4850,14 +4949,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ht",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "349",
         "eea": "",
         "eora": "HTI",
@@ -4899,14 +4999,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "hm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -4948,14 +5049,15 @@
         "unregion": "Australia and New Zealand",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "hn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "351",
         "eea": "",
         "eora": "HND",
@@ -4997,14 +5099,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "hk",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "HKG",
@@ -5046,14 +5149,15 @@
         "unregion": "Eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Hungary",
         "cctld": "hu",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "75",
         "eea": "EEA",
         "eora": "HUN",
@@ -5095,14 +5199,15 @@
         "unregion": "Eastern Europe",
         "wiod": "HUN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "is",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "20",
         "eea": "EEA",
         "eora": "ISL",
@@ -5144,14 +5249,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "BASIC",
         "bric": "BRIC",
+        "cc41": "India",
         "cctld": "in",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "Asia",
         "daccode": "645",
         "eea": "",
         "eora": "IND",
@@ -5193,14 +5299,15 @@
         "unregion": "Southern Asia",
         "wiod": "IND"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Indonesia",
         "cctld": "id",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "Asia",
         "daccode": "738",
         "eea": "",
         "eora": "IDN",
@@ -5242,14 +5349,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "IDN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ir",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "540",
         "eea": "",
         "eora": "IRN",
@@ -5291,14 +5399,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "iq",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "543",
         "eea": "",
         "eora": "IRQ",
@@ -5340,14 +5449,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Ireland",
         "cctld": "ie",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "21",
         "eea": "EEA",
         "eora": "IRL",
@@ -5389,14 +5499,15 @@
         "unregion": "Northern Europe",
         "wiod": "IRL"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "im",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "IMN",
@@ -5438,14 +5549,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "il",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "546",
         "eea": "",
         "eora": "ISR",
@@ -5487,14 +5599,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Italy",
         "cctld": "it",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "6",
         "eea": "EEA",
         "eora": "ITA",
@@ -5536,14 +5649,15 @@
         "unregion": "Southern Europe",
         "wiod": "ITA"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "jm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "354",
         "eea": "",
         "eora": "JAM",
@@ -5585,14 +5699,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Japan",
         "cctld": "jp",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "Asia",
         "daccode": "701",
         "eea": "",
         "eora": "JPN",
@@ -5634,14 +5749,15 @@
         "unregion": "Eastern Asia",
         "wiod": "JPN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "je",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "JEY",
@@ -5683,14 +5799,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "jo",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "549",
         "eea": "",
         "eora": "JOR",
@@ -5732,14 +5849,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "kz",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Asia",
         "daccode": "613",
         "eea": "",
         "eora": "KAZ",
@@ -5781,14 +5899,15 @@
         "unregion": "Central Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ke",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "248",
         "eea": "",
         "eora": "KEN",
@@ -5830,14 +5949,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ki",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "836",
         "eea": "",
         "eora": "KIR",
@@ -5879,14 +5999,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "57",
         "eea": "",
         "eora": "KSV",
@@ -5928,14 +6049,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "kw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "552",
         "eea": "",
         "eora": "KWT",
@@ -5977,14 +6099,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "kg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "614",
         "eea": "",
         "eora": "KGZ",
@@ -6026,14 +6149,15 @@
         "unregion": "Central Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "la",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "745",
         "eea": "",
         "eora": "LAO",
@@ -6075,14 +6199,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Latvia",
         "cctld": "lv",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "83",
         "eea": "EEA",
         "eora": "LVA",
@@ -6124,14 +6249,15 @@
         "unregion": "Northern Europe",
         "wiod": "LVA"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "lb",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "555",
         "eea": "",
         "eora": "LBN",
@@ -6173,14 +6299,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ls",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "249",
         "eea": "",
         "eora": "LSO",
@@ -6222,14 +6349,15 @@
         "unregion": "Southern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "lr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "251",
         "eea": "",
         "eora": "LBR",
@@ -6271,14 +6399,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ly",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "133",
         "eea": "",
         "eora": "LBY",
@@ -6320,14 +6449,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "li",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "70",
         "eea": "EEA",
         "eora": "LIE",
@@ -6369,14 +6499,15 @@
         "unregion": "Western Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Lithuania",
         "cctld": "lt",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "84",
         "eea": "EEA",
         "eora": "LTU",
@@ -6418,14 +6549,15 @@
         "unregion": "Northern Europe",
         "wiod": "LTU"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Luxembourg",
         "cctld": "lu",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "22",
         "eea": "EEA",
         "eora": "LUX",
@@ -6467,14 +6599,15 @@
         "unregion": "Western Europe",
         "wiod": "LUX"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mo",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "MAC",
@@ -6516,14 +6649,15 @@
         "unregion": "Eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mk",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "66",
         "eea": "",
         "eora": "MKD",
@@ -6565,14 +6699,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "252",
         "eea": "",
         "eora": "MDG",
@@ -6614,14 +6749,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "253",
         "eea": "",
         "eora": "MWI",
@@ -6663,14 +6799,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "my",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "751",
         "eea": "",
         "eora": "MYS",
@@ -6712,14 +6849,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mv",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "655",
         "eea": "",
         "eora": "MDV",
@@ -6761,14 +6899,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ml",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "255",
         "eea": "",
         "eora": "MLI",
@@ -6810,14 +6949,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Malta",
         "cctld": "mt",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "45",
         "eea": "EEA",
         "eora": "MLT",
@@ -6859,14 +6999,15 @@
         "unregion": "Southern Europe",
         "wiod": "MLT"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mh",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "859",
         "eea": "",
         "eora": "MHL",
@@ -6908,14 +7049,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mq",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "MTQ",
@@ -6957,14 +7099,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "256",
         "eea": "",
         "eora": "MRT",
@@ -7006,14 +7149,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mu",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "257",
         "eea": "",
         "eora": "MUS",
@@ -7055,14 +7199,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "yt",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "MYT",
@@ -7104,14 +7249,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Mexico",
         "cctld": "mx",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "America",
         "daccode": "358",
         "eea": "",
         "eora": "MEX",
@@ -7153,14 +7299,15 @@
         "unregion": "Central America",
         "wiod": "MEX"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "fm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "860",
         "eea": "",
         "eora": "FSM",
@@ -7202,14 +7349,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "md",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Europe",
         "daccode": "93",
         "eea": "",
         "eora": "MDA",
@@ -7251,14 +7399,15 @@
         "unregion": "Eastern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "MCO",
@@ -7300,14 +7449,15 @@
         "unregion": "Western Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "753",
         "eea": "",
         "eora": "MNG",
@@ -7349,14 +7499,15 @@
         "unregion": "Eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "me",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "65",
         "eea": "",
         "eora": "MNE",
@@ -7398,14 +7549,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ms",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "385",
         "eea": "",
         "eora": "MSR",
@@ -7447,14 +7599,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ma",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "136",
         "eea": "",
         "eora": "MAR",
@@ -7496,14 +7649,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mz",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "259",
         "eea": "",
         "eora": "MOZ",
@@ -7545,14 +7699,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "635",
         "eea": "",
         "eora": "MMR",
@@ -7594,14 +7749,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "na",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "275",
         "eea": "",
         "eora": "NAM",
@@ -7643,14 +7799,15 @@
         "unregion": "Southern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "nr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "845",
         "eea": "",
         "eora": "NRU",
@@ -7692,14 +7849,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "np",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "660",
         "eea": "",
         "eora": "NPL",
@@ -7741,14 +7899,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Netherlands",
         "cctld": "nl",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "7",
         "eea": "EEA",
         "eora": "NLD",
@@ -7790,14 +7949,15 @@
         "unregion": "Western Europe",
         "wiod": "NLD"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "ANT",
@@ -7839,14 +7999,15 @@
         "unregion": "",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "nc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "NCL",
@@ -7888,14 +8049,15 @@
         "unregion": "Melanesia",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "nz",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "820",
         "eea": "",
         "eora": "NZL",
@@ -7937,14 +8099,15 @@
         "unregion": "Australia and New Zealand",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ni",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "364",
         "eea": "",
         "eora": "NIC",
@@ -7986,14 +8149,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ne",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "260",
         "eea": "",
         "eora": "NER",
@@ -8035,14 +8199,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ng",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "261",
         "eea": "",
         "eora": "NGA",
@@ -8084,14 +8249,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "nu",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "856",
         "eea": "",
         "eora": "NIU",
@@ -8133,14 +8299,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "nf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "NFK",
@@ -8182,14 +8349,15 @@
         "unregion": "Australia and New Zealand",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "kp",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "740",
         "eea": "",
         "eora": "PRK",
@@ -8231,14 +8399,15 @@
         "unregion": "Eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "mp",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "MNP",
@@ -8280,14 +8449,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "no",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "Europe",
         "daccode": "8",
         "eea": "EEA",
         "eora": "NOR",
@@ -8329,14 +8499,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "om",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "OMN",
@@ -8378,14 +8549,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pk",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "665",
         "eea": "",
         "eora": "PAK",
@@ -8427,14 +8599,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "861",
         "eea": "",
         "eora": "PLW",
@@ -8476,14 +8649,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ps",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "550",
         "eea": "",
         "eora": "PSE",
@@ -8525,14 +8699,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pa",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "366",
         "eea": "",
         "eora": "PAN",
@@ -8574,14 +8749,15 @@
         "unregion": "Central America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "862",
         "eea": "",
         "eora": "PNG",
@@ -8623,14 +8799,15 @@
         "unregion": "Melanesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "py",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "451",
         "eea": "",
         "eora": "PRY",
@@ -8672,14 +8849,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pe",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "454",
         "eea": "",
         "eora": "PER",
@@ -8721,14 +8899,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ph",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "755",
         "eea": "",
         "eora": "PHL",
@@ -8770,14 +8949,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "PCN",
@@ -8819,14 +8999,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Poland",
         "cctld": "pl",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "76",
         "eea": "EEA",
         "eora": "POL",
@@ -8868,14 +9049,15 @@
         "unregion": "Eastern Europe",
         "wiod": "POL"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Portugal",
         "cctld": "pt",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "9",
         "eea": "EEA",
         "eora": "PRT",
@@ -8917,14 +9099,15 @@
         "unregion": "Southern Europe",
         "wiod": "PRT"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -8966,14 +9149,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "qa",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "561",
         "eea": "",
         "eora": "QAT",
@@ -9015,14 +9199,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "re",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "REU",
@@ -9064,14 +9249,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Romania",
         "cctld": "ro",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "77",
         "eea": "EEA",
         "eora": "ROU",
@@ -9113,14 +9299,15 @@
         "unregion": "Eastern Europe",
         "wiod": "ROU"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "BRIC",
+        "cc41": "Russia",
         "cctld": "ru",
         "cecilia2050": "BX",
         "cis": "CIS",
         "continent": "Europe",
         "daccode": "87",
         "eea": "",
         "eora": "RUS",
@@ -9162,14 +9349,15 @@
         "unregion": "Eastern Europe",
         "wiod": "RUS"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "rw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "266",
         "eea": "",
         "eora": "RWA",
@@ -9211,14 +9399,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "MAF",
@@ -9260,14 +9449,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ws",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "WSM",
@@ -9309,14 +9499,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "SMR",
@@ -9358,14 +9549,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "st",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "268",
         "eea": "",
         "eora": "STP",
@@ -9407,14 +9599,15 @@
         "unregion": "Middle Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sa",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "566",
         "eea": "",
         "eora": "SAU",
@@ -9456,14 +9649,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "269",
         "eea": "",
         "eora": "SEN",
@@ -9505,14 +9699,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "rs",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "63",
         "eea": "",
         "eora": "SRB",
@@ -9554,14 +9749,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "SYC",
@@ -9603,14 +9799,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sl",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "272",
         "eea": "",
         "eora": "SLE",
@@ -9652,14 +9849,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "",
         "eea": "",
         "eora": "SGP",
@@ -9701,14 +9899,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sx",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -9750,14 +9949,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Slovakia",
         "cctld": "sk",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "69",
         "eea": "EEA",
         "eora": "SVK",
@@ -9799,14 +9999,15 @@
         "unregion": "Eastern Europe",
         "wiod": "SVK"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Slovenia",
         "cctld": "si",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "61",
         "eea": "EEA",
         "eora": "SVN",
@@ -9848,14 +10049,15 @@
         "unregion": "Southern Europe",
         "wiod": "SVN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sb",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "866",
         "eea": "",
         "eora": "SLB",
@@ -9897,14 +10099,15 @@
         "unregion": "Melanesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "so",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "273",
         "eea": "",
         "eora": "SOM",
@@ -9946,14 +10149,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "BASIC",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "za",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "Africa",
         "daccode": "218",
         "eea": "",
         "eora": "ZAF",
@@ -9995,14 +10199,15 @@
         "unregion": "Southern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "gs",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Antarctica",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -10044,14 +10249,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Korea",
         "cctld": "kr",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "Asia",
         "daccode": "742",
         "eea": "",
         "eora": "KOR",
@@ -10093,14 +10299,15 @@
         "unregion": "Eastern Asia",
         "wiod": "KOR"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ss",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "279",
         "eea": "",
         "eora": "SDS",
@@ -10142,14 +10349,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "su",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "USR",
@@ -10191,14 +10399,15 @@
         "unregion": "Eastern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Spain",
         "cctld": "es",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "50",
         "eea": "EEA",
         "eora": "ESP",
@@ -10240,14 +10449,15 @@
         "unregion": "Southern Europe",
         "wiod": "ESP"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "lk",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "640",
         "eea": "",
         "eora": "LKA",
@@ -10289,14 +10499,15 @@
         "unregion": "Southern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "BLM",
@@ -10338,14 +10549,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sh",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "276",
         "eea": "",
         "eora": "SHN",
@@ -10387,14 +10599,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "kn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "KNA",
@@ -10436,14 +10649,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "lc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "383",
         "eea": "",
         "eora": "LCA",
@@ -10485,14 +10699,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "pm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "SPM",
@@ -10534,14 +10749,15 @@
         "unregion": "Northern America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "vc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "384",
         "eea": "",
         "eora": "VCT",
@@ -10583,14 +10799,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sd",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "278",
         "eea": "",
         "eora": "SUD",
@@ -10632,14 +10849,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sr",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "457",
         "eea": "",
         "eora": "SUR",
@@ -10681,14 +10899,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "SJM",
@@ -10730,14 +10949,15 @@
         "unregion": "Northern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Sweden",
         "cctld": "se",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "10",
         "eea": "EEA",
         "eora": "SWE",
@@ -10779,14 +10999,15 @@
         "unregion": "Northern Europe",
         "wiod": "SWE"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ch",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "Europe",
         "daccode": "11",
         "eea": "",
         "eora": "CHE",
@@ -10828,14 +11049,15 @@
         "unregion": "Western Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "sy",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "573",
         "eea": "",
         "eora": "SYR",
@@ -10877,14 +11099,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Taiwan",
         "cctld": "tw",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "Asia",
         "daccode": "732",
         "eea": "",
         "eora": "TWN",
@@ -10926,14 +11149,15 @@
         "unregion": "Eastern Asia",
         "wiod": "TWN"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tj",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Asia",
         "daccode": "615",
         "eea": "",
         "eora": "TJK",
@@ -10975,14 +11199,15 @@
         "unregion": "Central Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -11024,14 +11249,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tz",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "282",
         "eea": "",
         "eora": "TZA",
@@ -11073,14 +11299,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "th",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "764",
         "eea": "",
         "eora": "THA",
@@ -11122,14 +11349,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tl",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "765",
         "eea": "",
         "eora": "TLS",
@@ -11171,14 +11399,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tg",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "283",
         "eea": "",
         "eora": "TGO",
@@ -11220,14 +11449,15 @@
         "unregion": "Western Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tk",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "868",
         "eea": "",
         "eora": "TKL",
@@ -11269,14 +11499,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "to",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "870",
         "eea": "",
         "eora": "TON",
@@ -11318,14 +11549,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tt",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "TTO",
@@ -11367,14 +11599,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "139",
         "eea": "",
         "eora": "TUN",
@@ -11416,14 +11649,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Turkey",
         "cctld": "tr",
         "cecilia2050": "BX",
         "cis": "",
         "continent": "Asia",
         "daccode": "55",
         "eea": "",
         "eora": "TUR",
@@ -11465,14 +11699,15 @@
         "unregion": "Western Asia",
         "wiod": "TUR"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "616",
         "eea": "",
         "eora": "TKM",
@@ -11514,14 +11749,15 @@
         "unregion": "Central Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tc",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "TCA",
@@ -11563,14 +11799,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "tv",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "872",
         "eea": "",
         "eora": "TUV",
@@ -11612,14 +11849,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ug",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "285",
         "eea": "",
         "eora": "UGA",
@@ -11661,14 +11899,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ua",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "85",
         "eea": "",
         "eora": "UKR",
@@ -11710,14 +11949,15 @@
         "unregion": "Eastern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ae",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "576",
         "eea": "",
         "eora": "ARE",
@@ -11759,14 +11999,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Great Britain and N.I.",
         "cctld": "uk",
         "cecilia2050": "EU",
         "cis": "",
         "continent": "Europe",
         "daccode": "12",
         "eea": "",
         "eora": "GBR",
@@ -11808,14 +12049,15 @@
         "unregion": "Northern Europe",
         "wiod": "GBR"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "USA",
         "cctld": "us",
         "cecilia2050": "HI",
         "cis": "",
         "continent": "America",
         "daccode": "302",
         "eea": "",
         "eora": "USA",
@@ -11857,14 +12099,15 @@
         "unregion": "Northern America",
         "wiod": "USA"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -11906,14 +12149,15 @@
         "unregion": "Micronesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "vi",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "VIR",
@@ -11955,14 +12199,15 @@
         "unregion": "Caribbean",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "uy",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "",
         "eea": "",
         "eora": "URY",
@@ -12004,14 +12249,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "uz",
         "cecilia2050": "RoW",
         "cis": "CIS",
         "continent": "Asia",
         "daccode": "617",
         "eea": "",
         "eora": "UZB",
@@ -12053,14 +12299,15 @@
         "unregion": "Central Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "vu",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "854",
         "eea": "",
         "eora": "VUT",
@@ -12102,14 +12349,15 @@
         "unregion": "Melanesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "va",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Europe",
         "daccode": "",
         "eea": "",
         "eora": "VAT",
@@ -12151,14 +12399,15 @@
         "unregion": "Southern Europe",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ve",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "America",
         "daccode": "463",
         "eea": "",
         "eora": "VEN",
@@ -12200,14 +12449,15 @@
         "unregion": "South America",
         "wiod": "RoW"
     },
     {
         "apec": "APEC",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "vn",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "769",
         "eea": "",
         "eora": "VNM",
@@ -12249,14 +12499,15 @@
         "unregion": "South-eastern Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "wf",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Oceania",
         "daccode": "876",
         "eea": "",
         "eora": "WLF",
@@ -12298,14 +12549,15 @@
         "unregion": "Polynesia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "eh",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "ESH",
@@ -12347,14 +12599,15 @@
         "unregion": "Northern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "ye",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Asia",
         "daccode": "580",
         "eea": "",
         "eora": "YEM",
@@ -12396,14 +12649,15 @@
         "unregion": "Western Asia",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "zm",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "288",
         "eea": "",
         "eora": "ZMB",
@@ -12445,14 +12699,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "",
         "eea": "",
         "eora": "",
@@ -12494,14 +12749,15 @@
         "unregion": "Eastern Africa",
         "wiod": "RoW"
     },
     {
         "apec": "",
         "basic": "",
         "bric": "",
+        "cc41": "Rest of World",
         "cctld": "zw",
         "cecilia2050": "RoW",
         "cis": "",
         "continent": "Africa",
         "daccode": "265",
         "eea": "",
         "eora": "ZWE",
```

### Comparing `countryguess-0.3.0/countryguess/_countrydata.py` & `countryguess-0.4.0/countryguess/_countrydata.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,20 @@
         if len(string) == 3:
             info = self._find_country_by_code(string, self.codes_iso3)
             if info:
                 return info
 
         # Custom regular expressions
         if regex_map:
-            self._validate_regex_map(regex_map)
             for iso2, regex in regex_map.items():
                 if regex.search(string):
                     return self._find_country_by_code(iso2, self.codes_iso2)
+            # Because validation is expensive, we only do it if we couldn't find
+            # a match
+            self._validate_regex_map(regex_map)
 
         # Hardcoded regular expressions
         for info in self._countries:
             if info['regex'].search(string):
                 return info
 
         # Fuzzy country name
```

### Comparing `countryguess-0.3.0/countryguess/_guess_country.py` & `countryguess-0.4.0/countryguess/_guess_country.py`

 * *Files identical despite different names*

### Comparing `countryguess-0.3.0/countryguess.egg-info/PKG-INFO` & `countryguess-0.4.0/countryguess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countryguess
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fuzzy lookup of country information
 Home-page: https://codeberg.org/plotski/countryguess
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
@@ -159,14 +159,15 @@
 30. [GBDcode](http://ghdx.healthdata.org/) (numeric - Global Burden of
     Disease country codes)
 31. [IEA](https://www.iea.org/countries) (World Energy Balances 2021)
 32. [DACcode](https://www.oecd.org/dac/financing-sustainable-development/development-finance-standards/dacandcrscodelists.htm)
     (numeric - OECD Development Assistance Committee)
 33. [ccTLD](https://en.wikipedia.org/wiki/Country_code_top-level_domain) - country code top-level domains
 34. [GWcode](https://www.tandfonline.com/doi/abs/10.1080/03050629908434958) - Gledisch & Ward numerical codes as published in https://www.andybeger.com/states/articles/statelists.html
+35. CC41 - common classification for MRIOs (list of countries found in all public MRIOs)
 <!-- CLASSIFICATION_SCHEMES -->
 
 ### Command Line Interface
 
 **countryguess** comes with a simple CLI with the same name. It takes one or two
 arguments:
```

### Comparing `countryguess-0.3.0/setup.py` & `countryguess-0.4.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/fly_tracker-0.0.3.tar.gz` & `tmp/fly_tracker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fly_tracker-0.0.3.tar", last modified: Thu May 11 21:02:30 2023, max compression
+gzip compressed data, was "fly_tracker-1.0.0.tar", last modified: Fri May 12 21:48:05 2023, max compression
```

## Comparing `fly_tracker-0.0.3.tar` & `fly_tracker-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 21:02:30.595438 fly_tracker-0.0.3/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1819 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/CONTRIBUTING.md
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1068 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/LICENSE
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      172 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/MANIFEST.in
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4673 2023-05-11 21:02:30.595438 fly_tracker-0.0.3/PKG-INFO
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2450 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/README.md
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4844 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/Results_2023-03-28 13:22:57.090774.csv
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 21:02:30.591438 fly_tracker-0.0.3/fly_tracker/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     6148 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/.DS_Store
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2656 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/Notifier.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4044 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/Scraper.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       87 2023-05-11 20:53:08.000000 fly_tracker-0.0.3/fly_tracker/__init__.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1335 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/__main__.py
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 21:02:30.595438 fly_tracker-0.0.3/fly_tracker/testing/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     6148 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/testing/.DS_Store
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/testing/__init__.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1145 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/testing/integration_tests.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4830 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/testing/test_all.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)    28330 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/testing/test_data.json
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)  2982029 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/fly_tracker/testing/test_source_page.html
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 21:02:30.591438 fly_tracker-0.0.3/fly_tracker.egg-info/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4673 2023-05-11 21:02:30.000000 fly_tracker-0.0.3/fly_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      628 2023-05-11 21:02:30.000000 fly_tracker-0.0.3/fly_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        1 2023-05-11 21:02:30.000000 fly_tracker-0.0.3/fly_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      156 2023-05-11 21:02:30.000000 fly_tracker-0.0.3/fly_tracker.egg-info/requires.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       12 2023-05-11 21:02:30.000000 fly_tracker-0.0.3/fly_tracker.egg-info/top_level.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2338 2023-05-11 20:53:02.000000 fly_tracker-0.0.3/pyproject.toml
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       69 2023-05-11 20:51:24.000000 fly_tracker-0.0.3/requirements.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       38 2023-05-11 21:02:30.595438 fly_tracker-0.0.3/setup.cfg
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       72 2023-05-11 20:53:42.000000 fly_tracker-0.0.3/setup.py
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-12 21:48:05.974635 fly_tracker-1.0.0/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1819 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/CONTRIBUTING.md
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1068 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/LICENSE
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      169 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/MANIFEST.in
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4668 2023-05-12 21:48:05.974635 fly_tracker-1.0.0/PKG-INFO
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2446 2023-05-12 21:46:44.000000 fly_tracker-1.0.0/README.md
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4919 2023-05-12 04:46:22.000000 fly_tracker-1.0.0/Results_2023-05-12 00:46:22.074858.csv
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1733 2023-05-12 19:51:03.000000 fly_tracker-1.0.0/Results_2023-05-12 15:51:03.095820.csv
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1733 2023-05-12 19:51:33.000000 fly_tracker-1.0.0/Results_2023-05-12 15:51:33.703511.csv
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1670 2023-05-12 19:52:07.000000 fly_tracker-1.0.0/Results_2023-05-12 15:52:07.233936.csv
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1775 2023-05-12 19:52:58.000000 fly_tracker-1.0.0/Results_2023-05-12 15:52:58.582487.csv
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-12 21:48:05.946634 fly_tracker-1.0.0/fly_tracker/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     6148 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/.DS_Store
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2656 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/Notifier.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4044 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/Scraper.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       87 2023-05-12 21:46:44.000000 fly_tracker-1.0.0/fly_tracker/__init__.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1348 2023-05-12 04:45:28.000000 fly_tracker-1.0.0/fly_tracker/__main__.py
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-12 21:48:05.962634 fly_tracker-1.0.0/fly_tracker/testing/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     6148 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/testing/.DS_Store
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        0 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/testing/__init__.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1145 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/testing/integration_tests.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4830 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/testing/test_all.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)    28330 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/testing/test_data.json
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)  2982029 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/fly_tracker/testing/test_source_page.html
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-12 21:48:05.958634 fly_tracker-1.0.0/fly_tracker.egg-info/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4668 2023-05-12 21:48:05.000000 fly_tracker-1.0.0/fly_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      784 2023-05-12 21:48:05.000000 fly_tracker-1.0.0/fly_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        1 2023-05-12 21:48:05.000000 fly_tracker-1.0.0/fly_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      156 2023-05-12 21:48:05.000000 fly_tracker-1.0.0/fly_tracker.egg-info/requires.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       12 2023-05-12 21:48:05.000000 fly_tracker-1.0.0/fly_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2338 2023-05-12 21:46:44.000000 fly_tracker-1.0.0/pyproject.toml
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       69 2023-05-12 04:44:48.000000 fly_tracker-1.0.0/requirements.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       38 2023-05-12 21:48:05.974635 fly_tracker-1.0.0/setup.cfg
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       72 2023-05-12 21:46:44.000000 fly_tracker-1.0.0/setup.py
```

### Comparing `fly_tracker-0.0.3/CONTRIBUTING.md` & `fly_tracker-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/LICENSE` & `fly_tracker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/PKG-INFO` & `fly_tracker-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fly_tracker
-Version: 0.0.3
+Version: 1.0.0
 Summary: The Fly Tracker library lets you monitor the flight prices for any route. The user has the option to set up notifications for the tracked route which can help him book tickets when he wants to.
 Author-email: Ritik Panda <ritik.panda@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Ritik Panda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,44 +50,44 @@
 [![PyPI](https://img.shields.io/pypi/v/fly-tracker)](https://pypi.org/project/fly-tracker/)
 ## Code Coverage
 
 [![codecov](https://codecov.io/gh/Ritik3111/fly_tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/Ritik3111/fly_tracker)
 ## Overview
 
 The Fly Tracker library lets you monitor the flight prices for any route.
-The user has the option to set up notifications for the tracked route which can help him book tickets when he/she wants to. Once you run the command(mentioned in [Usage]#Usage) to start the notifications, the script runs at 12 AM and 12 PM Everyday and this is exactly when you receive the email.
+The user has the option to set up notifications for the tracked route which can help him book tickets when he/she wants to. Once you run the command to start the notifications, the script runs at 12 AM and 12 PM Everyday and this is exactly when you receive the email.
 The source of our data is Google Flights, which is very reliable since it lists the best price for every option and
-hence, we notify you with all options avalaible to you. 
+hence, we notify you with all options avalaible to you.
 
 ## Table of Contents
 
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [Example](#Example)
 
-## Installation 
+## Installation
 
-To install the library: 
+To install the library:
 
-`pip install fly_tracker`
+`pip install fly-tracker`
 
 ## Usage
 
 The library takes the following arguments:
 
 | Argument | Name | Type | Description
 | -------- | -------- | -------- | -------- |
-| src | Source | string | Source City |
-| dst | Destination | string |Destination City |
+| src | Source | string | Source City/Airport |
+| dst | Destination | string |Destination City/Airport |
 | price | Price | int |The threshold price that you want to set |
 | date | Date | string | The date you want to fly on |
 | email | Email Address | string | The email address where you want to receive the notifications |
 
 Run the following command:
-`python flytracker --src < src-city > --dest < dest-city > --price < price > --date < date > --email < email >`
+`python3 -m fly_tracker --src < src-city > --dest < dest-city > --price < price > --date < date > --email < email >`
 
 Replace < src-city >, < dest-city >, < price >, < date > and < email > with your desired values. This will start tracking the flight prices for the specified route.
 
 ## Example
 To receive notifications regarding fares below $100 for the New York to Boston route on May 12th, please execute the following command, with the specified email address included:
 
-`python flytracker --src "New York" --dest "Boston" --price 100 --date "12th May" --email "pandaritik39@gmail.com"`
+`python3 -m fly_tracker --src "New York" --dest "Boston" --price 100 --date "12th May" --email "pandaritik39@gmail.com"`
```

### Comparing `fly_tracker-0.0.3/README.md` & `fly_tracker-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 [![PyPI](https://img.shields.io/pypi/v/fly-tracker)](https://pypi.org/project/fly-tracker/)
 ## Code Coverage
 
 [![codecov](https://codecov.io/gh/Ritik3111/fly_tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/Ritik3111/fly_tracker)
 ## Overview
 
 The Fly Tracker library lets you monitor the flight prices for any route.
-The user has the option to set up notifications for the tracked route which can help him book tickets when he/she wants to. Once you run the command(mentioned in [Usage]#Usage) to start the notifications, the script runs at 12 AM and 12 PM Everyday and this is exactly when you receive the email.
+The user has the option to set up notifications for the tracked route which can help him book tickets when he/she wants to. Once you run the command to start the notifications, the script runs at 12 AM and 12 PM Everyday and this is exactly when you receive the email.
 The source of our data is Google Flights, which is very reliable since it lists the best price for every option and
-hence, we notify you with all options avalaible to you. 
+hence, we notify you with all options avalaible to you.
 
 ## Table of Contents
 
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [Example](#Example)
 
-## Installation 
+## Installation
 
-To install the library: 
+To install the library:
 
-`pip install fly_tracker`
+`pip install fly-tracker`
 
 ## Usage
 
 The library takes the following arguments:
 
 | Argument | Name | Type | Description
 | -------- | -------- | -------- | -------- |
-| src | Source | string | Source City |
-| dst | Destination | string |Destination City |
+| src | Source | string | Source City/Airport |
+| dst | Destination | string |Destination City/Airport |
 | price | Price | int |The threshold price that you want to set |
 | date | Date | string | The date you want to fly on |
 | email | Email Address | string | The email address where you want to receive the notifications |
 
 Run the following command:
-`python flytracker --src < src-city > --dest < dest-city > --price < price > --date < date > --email < email >`
+`python3 -m fly_tracker --src < src-city > --dest < dest-city > --price < price > --date < date > --email < email >`
 
 Replace < src-city >, < dest-city >, < price >, < date > and < email > with your desired values. This will start tracking the flight prices for the specified route.
 
 ## Example
 To receive notifications regarding fares below $100 for the New York to Boston route on May 12th, please execute the following command, with the specified email address included:
 
-`python flytracker --src "New York" --dest "Boston" --price 100 --date "12th May" --email "pandaritik39@gmail.com"`
+`python3 -m fly_tracker --src "New York" --dest "Boston" --price 100 --date "12th May" --email "pandaritik39@gmail.com"`
```

### Comparing `fly_tracker-0.0.3/fly_tracker/.DS_Store` & `fly_tracker-1.0.0/fly_tracker/.DS_Store`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/Notifier.py` & `fly_tracker-1.0.0/fly_tracker/Notifier.py`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/Scraper.py` & `fly_tracker-1.0.0/fly_tracker/Scraper.py`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/__main__.py` & `fly_tracker-1.0.0/fly_tracker/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 args = parser.parse_args()
 
 def main():
     """
     Main Function
     """
+    script()
     try:
         # Schedule the function to run at 12:00 am and 12:00 pm
         schedule.every().day.at("00:00").do(script)
         schedule.every().day.at("12:00").do(script)
 
         # Run the scheduled jobs indefinitely
         while True:
```

### Comparing `fly_tracker-0.0.3/fly_tracker/testing/.DS_Store` & `fly_tracker-1.0.0/fly_tracker/testing/.DS_Store`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/testing/integration_tests.py` & `fly_tracker-1.0.0/fly_tracker/testing/integration_tests.py`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/testing/test_all.py` & `fly_tracker-1.0.0/fly_tracker/testing/test_all.py`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/testing/test_data.json` & `fly_tracker-1.0.0/fly_tracker/testing/test_data.json`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker/testing/test_source_page.html` & `fly_tracker-1.0.0/fly_tracker/testing/test_source_page.html`

 * *Files identical despite different names*

### Comparing `fly_tracker-0.0.3/fly_tracker.egg-info/PKG-INFO` & `fly_tracker-1.0.0/fly_tracker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fly-tracker
-Version: 0.0.3
+Version: 1.0.0
 Summary: The Fly Tracker library lets you monitor the flight prices for any route. The user has the option to set up notifications for the tracked route which can help him book tickets when he wants to.
 Author-email: Ritik Panda <ritik.panda@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Ritik Panda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,44 +50,44 @@
 [![PyPI](https://img.shields.io/pypi/v/fly-tracker)](https://pypi.org/project/fly-tracker/)
 ## Code Coverage
 
 [![codecov](https://codecov.io/gh/Ritik3111/fly_tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/Ritik3111/fly_tracker)
 ## Overview
 
 The Fly Tracker library lets you monitor the flight prices for any route.
-The user has the option to set up notifications for the tracked route which can help him book tickets when he/she wants to. Once you run the command(mentioned in [Usage]#Usage) to start the notifications, the script runs at 12 AM and 12 PM Everyday and this is exactly when you receive the email.
+The user has the option to set up notifications for the tracked route which can help him book tickets when he/she wants to. Once you run the command to start the notifications, the script runs at 12 AM and 12 PM Everyday and this is exactly when you receive the email.
 The source of our data is Google Flights, which is very reliable since it lists the best price for every option and
-hence, we notify you with all options avalaible to you. 
+hence, we notify you with all options avalaible to you.
 
 ## Table of Contents
 
 - [Installation](#Installation)
 - [Usage](#Usage)
 - [Example](#Example)
 
-## Installation 
+## Installation
 
-To install the library: 
+To install the library:
 
-`pip install fly_tracker`
+`pip install fly-tracker`
 
 ## Usage
 
 The library takes the following arguments:
 
 | Argument | Name | Type | Description
 | -------- | -------- | -------- | -------- |
-| src | Source | string | Source City |
-| dst | Destination | string |Destination City |
+| src | Source | string | Source City/Airport |
+| dst | Destination | string |Destination City/Airport |
 | price | Price | int |The threshold price that you want to set |
 | date | Date | string | The date you want to fly on |
 | email | Email Address | string | The email address where you want to receive the notifications |
 
 Run the following command:
-`python flytracker --src < src-city > --dest < dest-city > --price < price > --date < date > --email < email >`
+`python3 -m fly_tracker --src < src-city > --dest < dest-city > --price < price > --date < date > --email < email >`
 
 Replace < src-city >, < dest-city >, < price >, < date > and < email > with your desired values. This will start tracking the flight prices for the specified route.
 
 ## Example
 To receive notifications regarding fares below $100 for the New York to Boston route on May 12th, please execute the following command, with the specified email address included:
 
-`python flytracker --src "New York" --dest "Boston" --price 100 --date "12th May" --email "pandaritik39@gmail.com"`
+`python3 -m fly_tracker --src "New York" --dest "Boston" --price 100 --date "12th May" --email "pandaritik39@gmail.com"`
```

### Comparing `fly_tracker-0.0.3/fly_tracker.egg-info/SOURCES.txt` & `fly_tracker-1.0.0/fly_tracker.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
-Results_2023-03-28 13:22:57.090774.csv
+Results_2023-05-12 00:46:22.074858.csv
+Results_2023-05-12 15:51:03.095820.csv
+Results_2023-05-12 15:51:33.703511.csv
+Results_2023-05-12 15:52:07.233936.csv
+Results_2023-05-12 15:52:58.582487.csv
 pyproject.toml
 requirements.txt
 setup.py
 fly_tracker/.DS_Store
 fly_tracker/Notifier.py
 fly_tracker/Scraper.py
 fly_tracker/__init__.py
```

### Comparing `fly_tracker-0.0.3/pyproject.toml` & `fly_tracker-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "fly_tracker"
 authors = [{name = "Ritik Panda", email = "ritik.panda@columbia.edu"}]
 description="The Fly Tracker library lets you monitor the flight prices for any route. The user has the option to set up notifications for the tracked route which can help him book tickets when he wants to."
 readme = "README.md"
-version = "0.0.3"
+version = "1.0.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```


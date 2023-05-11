# Comparing `tmp/iso3166-updates-0.0.7.tar.gz` & `tmp/iso3166-updates-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-0.0.7.tar", last modified: Thu Jan 12 15:50:51 2023, max compression
+gzip compressed data, was "iso3166-updates-1.0.1.tar", last modified: Thu May 11 23:01:45 2023, max compression
```

## Comparing `iso3166-updates-0.0.7.tar` & `iso3166-updates-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:50:51.147403 iso3166-updates-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-01-12 15:50:33.000000 iso3166-updates-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-01-12 15:50:51.147403 iso3166-updates-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-01-12 15:50:33.000000 iso3166-updates-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:50:51.143402 iso3166-updates-0.0.7/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-12 15:50:33.000000 iso3166-updates-0.0.7/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-01-12 15:50:33.000000 iso3166-updates-0.0.7/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:50:51.147403 iso3166-updates-0.0.7/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-01-12 15:50:51.000000 iso3166-updates-0.0.7/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-12 15:50:51.000000 iso3166-updates-0.0.7/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:50:51.000000 iso3166-updates-0.0.7/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:50:44.000000 iso3166-updates-0.0.7/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-12 15:50:51.000000 iso3166-updates-0.0.7/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-12 15:50:51.000000 iso3166-updates-0.0.7/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-12 15:50:51.147403 iso3166-updates-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-01-12 15:50:33.000000 iso3166-updates-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:01:45.659933 iso3166-updates-1.0.1/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:01:37.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/setup.py
```

### Comparing `iso3166-updates-0.0.7/LICENSE` & `iso3166-updates-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-0.0.7/PKG-INFO` & `iso3166-updates-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 0.0.7
+Version: 1.0.1
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
 Description: # iso3166-updates
         
         [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
-        [![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-updates/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-updates/actions)
+        [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
         [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
         [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-        [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-flag-icons)](https://github.com/amckenna41/iso3166-updates/issues)
+        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
+        [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
         [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
         [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
           <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
         </div>
         
-        > Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here](https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing).
+        > Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
         
         Table of Contents
         -----------------
-        
           * [Introduction](#introduction)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
-          * [Issues](#Issues)
           * [Directories](#Directories)
+          * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
         
         The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
         
-        **Problem Statement:**
+        ## Problem Statement:
         
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform or Online Browsing Platform or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published throughout the year [[4]](#references). 
+        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published at various times throughout the year [[4]](#references). 
         
-        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of countrys' ISO 3166-2 codes for free, with an easy-to-use interface and Python package, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
+        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
         
-        **Intended Audience:**
+        ## Intended Audience:
         
-        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy -to-use API. 
+        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API. 
         
         <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
         
         Updates
         -------
         **Last Updated:**
-        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function (iso3166-check-for-updates). This function  
         
+        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+        The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO3166-2 wiki's to check for the latest updates within a certain period e.g the past 3 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the main GCP Cloud Function returns the latest data. Additionally, a GitHub Issue in the `iso3166-2` repository will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` JSONs and repo.
+        Ultimately, this function ensures that the software and assoicated APIs are up-to-date with the latest ISO3166-2 information for all countries/territories/subdivisions etc.
         
         API
         ---
         An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
         
-        >                               https://www.iso3166-updates.com
-        <!-- > https://us-central1-iso3166-updates.cloudfunctions.net/iso3166-updates -->
+        > https://www.iso3166-updates.com/api
         
-        Two query string parameters / paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE. A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY, HU, ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO3166 updates. A complete diagram of the architecture is available in the iso3166-updates-api/README. This JSON is updated regularly using a CRON GithHub Action workflow that is called every 6 months (.github/workflows/check_for_updates.yml) that also utilises a Cloud Func and the Python software to check for the most latest ISO3166 updates (<=6 months) - <i>in development</i>.
+        Two query string parameters/paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE". A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY", "HU", "ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below.
         
         The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
         
          <!-- "?year" can be a specific year or year range to get updates for (e.g "2017", "2010-2015"), you can also get updates less than or greater than a year (e.g ">2004", "<2020") and "?months" which allows you to get the updates of the past X months. If months and year input params are set then months will take precedence. -->
         <p align="center">
-          <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/gcp_cloud_arch.png" alt="gcp_arch" height="200" width="400"/>
+          <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
         </p>
         
-        
         Requirements
         ------------
         * [python][python] >= 3.7
         * [pandas][pandas] >= 1.4.3
         * [numpy][numpy] >= 1.23.2
         * [requests][requests] >= 2.28.1
         * [beautifulsoup4][beautifulsoup4] >= 4.11.1
         * [iso3166][iso3166] >= 2.1.1
         
         Installation
         ------------
-        Install the latest version of iso3166-updates via [PyPi][PyPi] using pip:
+        Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
         
         ```bash
         pip3 install iso3166-updates --upgrade
         ```
         
         Installation from source:
         ```bash
@@ -125,95 +125,102 @@
           #                       Whether to export all found updates to csv files in export folder.
           # -year YEAR, --year YEAR
           #                       Selected year to check for updates.
           # -concat_updates, --concat_updates
           #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
         ```
         
+        **Get all listed changes/updates for all countries which happens by default if no alpha2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+        ```python
+        iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
+        ```
+        
         **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
         ```python
         iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
         ```
         
-        <!-- def get_updates(alpha2_codes, year=[''], export_filename="iso3166-updates",
-                export_json_filename="iso3166-updates", export_folder="../test/iso3166-updates", 
-                concat_updates=True, export_json=True, export_csv=False): -->
-        
         **Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
         ```python
-        iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=1))
+        iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0))
         ```
         
         **Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
         ```python
-        iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_json_filename="iso3166-updates")
+        iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_json_filename="iso3166-updates", concat_updates=0)
         ```
         
         **Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
         ```python
         iso3166_updates.get_updates("IE", year="2012-2021")
         ```
         
-        **Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years > 2015, export only to CSV with filename "iso3166-output.csv":**
+        **Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename "iso3166-output.csv":**
         ```python
-        iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output")
+        iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output.csv")
         ```
         
         **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
         ```python
-        iso3166_updates.get_updates("YE", year=">2010")
+        iso3166_updates.get_updates("YE", year="<2010")
         ```
         
         The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
         Edition/Newsletter, Date Issued, Description of change in newsletter and Code/Subdivision change. 
+        
+        * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+        * Date Issued: Date that the change was communicated.
+        * Description of change in newsletter: More in-depth info about the change/update that was made.
+        * Code/Subdivision change: Overall summary of change/update made.
+        
         E.g. The output format of the exported CSV for AD (Andorra) is:
         
         | Edition/Newsletter | Date Issued | Description of change in newsletter | Code/Subdivision change |   
         |:-------------------|:------------|------------------------------------:|------------------------:|
         | Newsletter I-8     | 2007-04-17  | Addition of the administrative subdivisions...   | Subdivisions added: 7 parishes...                 | 
         | Online Browsing Platform (OBP) | 2014-11-03 | Update List Source | No subdivision changes listed |
         | Online Browsing Platform (OBP) | 2015-11-27 | Update List Source | No subdivision changes listed | 
         
         E.g. The output format of the exported JSON for AD (Andorra) is:
-        ```json
+        ```javascript
         {
           AD: [
               {
-                Code/Subdivision change: "",
-                Date Issued: "2015-11-27",
-                Description of change in newsletter: "Update List Source",
-                Edition/Newsletter: "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+                "Code/Subdivision change": "",
+                "Date Issued": "2015-11-27",
+                "Description of change in newsletter": "Update List Source",
+                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
               },
               {
-                Code/Subdivision change: "",
-                Date Issued: "2014-11-03",
-                Description of change in newsletter: "Update List Source",
-                Edition/Newsletter: "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+                "Code/Subdivision change": "",
+                "Date Issued": "2014-11-03",
+                "Description of change in newsletter": "Update List Source",
+                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
               },
               {
-                Code/Subdivision change: "Subdivisions added:7 parishes",
-                Date Issued: "2007-04-17",
-                Description of change in newsletter: "Addition of the administrative subdivisions and of their code elements",
-                Edition/Newsletter: "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
+                "Code/Subdivision change:" "Subdivisions added:7 parishes",
+                "Date Issued": "2007-04-17",
+                "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
+                "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
               }
           ]
         }
         ```
         
         Directories
         -----------
-        * `/docs` - documentation for iso3166-updates Python package.
-        * `/iso3166_updates` - source code for iso3166-updates Python package.
-        * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the iso3166-updates API, including the main.py, requirements.txt and API config file.
+        * `/docs` - documentation for `iso3166-updates` Python package.
+        * `/iso3166_updates` - source code for `iso3166-updates` Python package.
+        * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
         * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Func that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt.
-        * `/tests` - unit and integration tests for iso3166-updates.
+        * `/tests` - unit and integration tests for `iso3166-updates`.
         
         Issues
         ------
-        Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+        Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
         
         Contact
         -------
         If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
         [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
         
         References
@@ -226,21 +233,23 @@
         
         Support
         -------
         <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
         
         [Back to top](#TOP)
         
+        [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
         [python]: https://www.python.org/downloads/release/python-360/
         [pandas]: https://pandas.pydata.org/
         [numpy]: https://numpy.org/
         [requests]: https://requests.readthedocs.io/
         [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
         [iso3166]: https://github.com/deactivated/python-iso3166
-        [PyPi]: https://pypi.org/project/pysar/
+        [PyPi]: https://pypi.org/project/iso3166-updates/
+        [Issues]: https://github.com/amckenna41/iso3166-updates/issues
 Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csviso3166-2,iso3166-1,alpha2,alpha3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iso3166-updates-0.0.7/README.md` & `iso3166-updates-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 # iso3166-updates
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
-[![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-updates/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-updates/actions)
+[![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-[![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-flag-icons)](https://github.com/amckenna41/iso3166-updates/issues)
+<!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
+[![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
 [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
 [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here](https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing).
+> Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
 
 Table of Contents
 -----------------
-
   * [Introduction](#introduction)
   * [Requirements](#requirements)
   * [Installation](#installation)
   * [Usage](#usage)
-  * [Issues](#Issues)
   * [Directories](#Directories)
+  * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
 
 The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
 
-**Problem Statement:**
+## Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform or Online Browsing Platform or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published at various times throughout the year [[4]](#references). 
 
-This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of countrys' ISO 3166-2 codes for free, with an easy-to-use interface and Python package, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
+This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-**Intended Audience:**
+## Intended Audience:
 
-This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy -to-use API. 
+This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API. 
 
 <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
 
 Updates
 -------
 **Last Updated:**
-The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function (iso3166-check-for-updates). This function  
 
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO3166-2 wiki's to check for the latest updates within a certain period e.g the past 3 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the main GCP Cloud Function returns the latest data. Additionally, a GitHub Issue in the `iso3166-2` repository will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` JSONs and repo.
+Ultimately, this function ensures that the software and assoicated APIs are up-to-date with the latest ISO3166-2 information for all countries/territories/subdivisions etc.
 
 API
 ---
 An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
 
->                               https://www.iso3166-updates.com
-<!-- > https://us-central1-iso3166-updates.cloudfunctions.net/iso3166-updates -->
+> https://www.iso3166-updates.com/api
 
-Two query string parameters / paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE. A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY, HU, ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO3166 updates. A complete diagram of the architecture is available in the iso3166-updates-api/README. This JSON is updated regularly using a CRON GithHub Action workflow that is called every 6 months (.github/workflows/check_for_updates.yml) that also utilises a Cloud Func and the Python software to check for the most latest ISO3166 updates (<=6 months) - <i>in development</i>.
+Two query string parameters/paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE". A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY", "HU", "ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below.
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
  <!-- "?year" can be a specific year or year range to get updates for (e.g "2017", "2010-2015"), you can also get updates less than or greater than a year (e.g ">2004", "<2020") and "?months" which allows you to get the updates of the past X months. If months and year input params are set then months will take precedence. -->
 <p align="center">
-  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/gcp_cloud_arch.png" alt="gcp_arch" height="200" width="400"/>
+  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
-
 Requirements
 ------------
 * [python][python] >= 3.7
 * [pandas][pandas] >= 1.4.3
 * [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
 * [iso3166][iso3166] >= 2.1.1
 
 Installation
 ------------
-Install the latest version of iso3166-updates via [PyPi][PyPi] using pip:
+Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
 ```
 
 Installation from source:
 ```bash
@@ -115,95 +115,102 @@
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year to check for updates.
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
 ```
 
+**Get all listed changes/updates for all countries which happens by default if no alpha2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
+```
+
 **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
 ```
 
-<!-- def get_updates(alpha2_codes, year=[''], export_filename="iso3166-updates",
-        export_json_filename="iso3166-updates", export_folder="../test/iso3166-updates", 
-        concat_updates=True, export_json=True, export_csv=False): -->
-
 **Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
 ```python
-iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=1))
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0))
 ```
 
 **Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
 ```python
-iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_json_filename="iso3166-updates")
+iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_json_filename="iso3166-updates", concat_updates=0)
 ```
 
 **Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 ```
 
-**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years > 2015, export only to CSV with filename "iso3166-output.csv":**
+**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename "iso3166-output.csv":**
 ```python
-iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output")
+iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output.csv")
 ```
 
 **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
 ```python
-iso3166_updates.get_updates("YE", year=">2010")
+iso3166_updates.get_updates("YE", year="<2010")
 ```
 
 The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
 Edition/Newsletter, Date Issued, Description of change in newsletter and Code/Subdivision change. 
+
+* Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+* Date Issued: Date that the change was communicated.
+* Description of change in newsletter: More in-depth info about the change/update that was made.
+* Code/Subdivision change: Overall summary of change/update made.
+
 E.g. The output format of the exported CSV for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Description of change in newsletter | Code/Subdivision change |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
 | Newsletter I-8     | 2007-04-17  | Addition of the administrative subdivisions...   | Subdivisions added: 7 parishes...                 | 
 | Online Browsing Platform (OBP) | 2014-11-03 | Update List Source | No subdivision changes listed |
 | Online Browsing Platform (OBP) | 2015-11-27 | Update List Source | No subdivision changes listed | 
 
 E.g. The output format of the exported JSON for AD (Andorra) is:
-```json
+```javascript
 {
   AD: [
       {
-        Code/Subdivision change: "",
-        Date Issued: "2015-11-27",
-        Description of change in newsletter: "Update List Source",
-        Edition/Newsletter: "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+        "Code/Subdivision change": "",
+        "Date Issued": "2015-11-27",
+        "Description of change in newsletter": "Update List Source",
+        "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
       },
       {
-        Code/Subdivision change: "",
-        Date Issued: "2014-11-03",
-        Description of change in newsletter: "Update List Source",
-        Edition/Newsletter: "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+        "Code/Subdivision change": "",
+        "Date Issued": "2014-11-03",
+        "Description of change in newsletter": "Update List Source",
+        "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
       },
       {
-        Code/Subdivision change: "Subdivisions added:7 parishes",
-        Date Issued: "2007-04-17",
-        Description of change in newsletter: "Addition of the administrative subdivisions and of their code elements",
-        Edition/Newsletter: "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
+        "Code/Subdivision change:" "Subdivisions added:7 parishes",
+        "Date Issued": "2007-04-17",
+        "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
+        "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
       }
   ]
 }
 ```
 
 Directories
 -----------
-* `/docs` - documentation for iso3166-updates Python package.
-* `/iso3166_updates` - source code for iso3166-updates Python package.
-* `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the iso3166-updates API, including the main.py, requirements.txt and API config file.
+* `/docs` - documentation for `iso3166-updates` Python package.
+* `/iso3166_updates` - source code for `iso3166-updates` Python package.
+* `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Func that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt.
-* `/tests` - unit and integration tests for iso3166-updates.
+* `/tests` - unit and integration tests for `iso3166-updates`.
 
 Issues
 ------
-Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
 
 Contact
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
 
 References
@@ -216,14 +223,16 @@
 
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
+[demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [iso3166]: https://github.com/deactivated/python-iso3166
-[PyPi]: https://pypi.org/project/pysar/
+[PyPi]: https://pypi.org/project/iso3166-updates/
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iso3166-updates-0.0.7/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.0.1/iso3166_updates/iso3166_updates.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,83 +7,102 @@
 import getpass
 import json
 import logging
 import re
 from bs4 import BeautifulSoup
 from importlib import metadata
 import datetime
-from pprint import pprint
 
 #initialise logging library 
 __version__ = metadata.metadata('iso3166_updates')['version']
 log = logging.getLogger(__name__)
 
 #initalise User-agent header for requests library 
 USER_AGENT_HEADER = {'User-Agent': 'iso3166-updates/{} ({}; {})'.format(__version__,
                                        'https://github.com/amckenna41/iso3166-updates', getpass.getuser())}
 
 #base URL for ISO3166-2 wiki
 wiki_base_url = "https://en.wikipedia.org/wiki/ISO_3166-2:"
 
-def get_updates(alpha2_codes, year=[''], export_filename="iso3166-updates",
-        export_json_filename="iso3166-updates", export_folder="../test/iso3166-updates", 
+
+def get_updates(alpha2_codes=[], year=[], export_filename="iso3166-updates",
+        export_json_filename="iso3166-updates", export_folder="test_iso3166-updates", 
         concat_updates=True, export_json=True, export_csv=False):
     """
-    Get all listed updates to a country's ISO3166-2 subdivision codes via 
-    the "Changes" section on its wiki. The "Changes" section lists updates 
-    or changes to any ISO3166-2 codes according to the ISO newsletter which
-    is realeased peridically by the ISO.
-    The ISO newsletters are not easily discoverable online and may require
-    a subscription to the ISO3166-2 database (https://www.iso.org/iso/updating_information.pdf).
+    Get all listed updates to a country/country's ISO3166-2 subdivision codes/names 
+    via the "Changes" section on its wiki page. All wiki pages follow the convention
+    https://en.wikipedia.org/wiki/ISO_3166-2:XX where XX is the 2 letter alpha-2 code
+    for a country. The "Changes" section lists updates or changes to any ISO3166-2 codes 
+    according to the ISO newsletter which is realeased peridically by the ISO as well as 
+    its Online Browsing Platform (OBP). The ISO newsletters are not easily discoverable 
+    and accessinle online and may require a subscription to the ISO3166-2 database 
+    (https://www.iso.org/iso/updating_information.pdf).
 
     The changes/updates table is converted to a DataFrame and then exported to a 
-    CSV for further analysis. You can also get the updates from a particular year
-    by using the Year parameter. 
+    CSV for further analysis. You can also get the updates from a particular year, 
+    list of years, year range or updates greater than or less than specified year, 
+    using the Year parameter. All of the updates are ordered alphabetically by there
+    2 letter country code and exported to a JSON and or CSV file.
 
     Parameters
     ----------
-    : alpha2_codes : str / list
+    :alpha2_codes : str / list (default=[])
         single string or list of alpha-2 ISO3166 codes to get the latest ISO3166-2 updates from. If
-        single alpha2 code passed in then it is converted to an iterable list.
-    : year : list (default = [''])
-        list of 1 or more years to get the specific ISO3166-2 updates from per country.
-    : export_filename : str (default = "iso3166-updates")
+        single alpha-2 code passed in then it is converted to an iterable list. If no value passed
+        into param then all updates for all ISO3166 gotten. 
+    :year : list (default = [])
+        list of 1 or more years to get the specific ISO3166-2 updates from, per country. By default, 
+        the year param will be empty meaning all changes/updates for all years will be gotten.
+    :export_filename : str (default = "iso3166-updates")
         filename for csv output of inputted country's ISO3166-2 updates. 
-    : export_json_filename : str (default = "iso3166-updates")
+    :export_json_filename : str (default = "iso3166-updates")
         filename for json output of all country's ISO3166-2 updates. 
     :export_folder : str (default = "../iso3166-updates")
-        folder name to store all csv outputs for country's ISO3166-2 updates. 
+        folder name to store all csv outputs for all country's ISO3166-2 updates. 
     :concat_updates : bool (default = True)
-        if multiple alpha2 codes input, concatenate updates into one json file or into seperately
+        if multiple alpha-2 codes input, concatenate updates into one json file or into seperately
         named files in export folder. Not available for csv output.
-    : export_json : bool (default = True)
+    :export_json : bool (default = True)
         export all ISO3166 updates for inputted country's into json format. 
-    : export_csv : bool (default = False)
+    :export_csv : bool (default = False)
         export all ISO3166 updates for inputted country's to csv files in export folder.
 
     Returns
     -------
     None
     """
     year_range = False
     greater_than = False
     less_than = False
     
-    #if alpha2 codes input param isn't str or list raise type error
+    #if alpha-2 codes input param isn't str or list raise type error
     if not isinstance(alpha2_codes, str) and not isinstance(alpha2_codes, list):
         raise TypeError('alpha2_codes input param should be a 2 letter '
-            'ISO3166 alpha2 code or a list of the same, got type {}.'.format(type(alpha2_codes)))
+            'ISO3166 alpha-2 code or a list of the same, got input of type {}.'.format(type(alpha2_codes)))
 
-    #if single str input then convert to array, remove whitespace
+    #if single str input for alpha2 codes param then convert to array, remove whitespace
     if isinstance(alpha2_codes, str):
-        # alpha2_codes = [alpha2_codes]
         alpha2_codes = alpha2_codes.replace(' ', '').split(',')
 
-    #a '-' seperating 2 years implies a year range of sought country updates, validate format of years in range
-    if (year != ['']):
+    #if single str input for Year param then convert to array, remove whitespace
+    if isinstance(year, str):
+        year = year.replace(' ', '').split(',')
+
+    #use all ISO3166 codes if invalid alpha-2 code input, otherwise convert alpha-2 to array
+    if (alpha2_codes == []):
+        alpha2_codes = sorted(list(iso3166.countries_by_alpha2.keys()))
+
+    #sort codes in alphabetical order
+    alpha2_codes.sort()
+    alpha2_codes = [code.upper() for code in alpha2_codes]
+
+    #'-' seperating 2 years implies a year range of sought country updates, validate format of years in range
+    #'>' before year means get all country updates greater than or equal to specified year
+    #'<' before year means get all country updates less than to specified year
+    if (year != []):
         if ('-' in year[0]):
             year_range = True
             year = year[0].split('-')
             #only 2 years should be included in input parameter
             if (len(year) > 2):
                 year = []
                 year_range = False
@@ -121,25 +140,24 @@
 
     export_fname = export_filename + '-'
 
     #iterate over all input ISO country codes
     for alpha2 in alpha2_codes:
 
         # if len(alpha2_codes) == 1: 
-        #     export_fname = export_filename + alpha2  
+        #     export_fname = export_filename + alpha-2  
         # else:
-        #     export_fname += "," + alpha2
+        #     export_fname += "," + alpha-2
         export_fname = export_filename + '-' + alpha2  
 
-        print(export_fname)
-        #skip to next iteration if alpha2 not valid
+        #skip to next iteration if alpha-2 not valid
         if (alpha2 not in list(iso3166.countries_by_alpha2.keys())):
             continue
 
-        print("ISO Code: {} ({}) ".format(alpha2, wiki_base_url + alpha2))
+        print("ISO Code: {} ({})".format(alpha2, wiki_base_url + alpha2))
 
         all_changes[alpha2] = {}
 
         #get html content from wiki of ISO3166 page, raise exception if status code != 200
         try:
             page = requests.get(wiki_base_url + alpha2, headers=USER_AGENT_HEADER)
             page.raise_for_status()
@@ -166,14 +184,15 @@
         iso3166_df = get_updates_df(iso3166_table, year, year_range, less_than, greater_than)
 
         #some wiki's have two updates tables  
         iso3166_table_2 = table.findNext('table', {"class": "wikitable"})
 
         #concat both updates table to 1 df, if applicable 
         if (iso3166_table_2 != None):
+            #convert secondary table into 2D array
             temp_iso3166_table = table_to_array(iso3166_table_2)
             #several tables have extra unwanted cols meaning we ignore those tables
             if ('former code' not in [col.lower() for col in temp_iso3166_table[0]] and 
                 'in region' not in [col.lower() for col in temp_iso3166_table[0]] and 
                 'before' not in [col.lower() for col in temp_iso3166_table[0]]): 
                 temp_iso3166_df = get_updates_df(temp_iso3166_table, year)
 
@@ -189,36 +208,40 @@
         iso3166_df["Edition/Newsletter"] = iso3166_df["Edition/Newsletter"].str.replace('BrowsingPlatform', "Browsing Platform")
 
         #append year onto filename, if not empty
         export_fname = export_fname + (("-" + str(year)) if year != [] else '')  #potentially need to add strip to export_fname
         
         #create output folder if doesn't exist and files are set to be exported
         if (export_csv or export_json) and not (os.path.isdir(export_folder)):
-            print('here')
             os.mkdir(export_folder)
 
         #only export non-empty dataframes         
         if not (iso3166_df.empty):
             
-            #sort and order by date
+            #convert date column to datetime object
+            iso3166_df['Date Issued'] = pd.to_datetime(iso3166_df["Date Issued"])
+            #sort and order by date, newest to oldest
             iso3166_df = iso3166_df.sort_values(by=['Date Issued'], ascending=False)
+            #convert date column back to string 
+            iso3166_df['Date Issued'] = iso3166_df['Date Issued'].astype(str)
+
+            def convert_date_format(row):
+                """ convert date in rows of df into dd-mm-yyyy data format from date object. """
+                return datetime.datetime.strptime(row.replace('\n', ''), '%Y-%m-%d').strftime('%d-%m-%Y')
+
+            #convert date column into dd-mm-yyyy format  
+            iso3166_df["Date Issued"] = iso3166_df["Date Issued"].apply(convert_date_format)
 
             #export to csv
             if (export_csv): 
                 iso3166_df.to_csv(os.path.join(export_folder, export_fname + '.csv'), index=False)
         
             #add ISO updates to object of all ISO3166 updates, convert to json 
             all_changes[alpha2] = json.loads(iso3166_df.to_json(orient='records'))
 
-            #print output to terminal if less than 10 ISO3166 codes input
-            # if len(alpha2_codes) < 10:
-            #     pprint(all_changes[alpha2], depth=2, sort_dicts=False)
-            #     print('\n')
-                # export_json_filename += '-' + alpha2
-
         #reset export filename var 
         export_fname = export_filename
 
     #append extension to json filename, if applicable 
     if (os.path.splitext(export_json_filename)[1] != "json"):
         export_json_filename = export_json_filename + ".json"
 
@@ -231,105 +254,105 @@
                     json.dump(all_changes, write_file, indent=4, ensure_ascii=False)
             else:
                 #seperate country updates into individual json files
                 for update in all_changes:
                     with open(os.path.join(export_folder, os.path.splitext(export_json_filename)[0] + "-" + update + ".json"), "w") as write_file:
                         json.dump(all_changes[update], write_file, indent=4, ensure_ascii=False)
             
-            print("All ISO3166 changes exported to folder {}".format(export_folder))
+            print("All ISO3166 changes exported to folder {}.".format(export_folder))
     
 def get_updates_df(iso3166_updates_table, year=[], year_range=False, less_than=False, greater_than=False):
     """
-    Convert parsed html table, from Changes Section in the respective ISO3166-2 wiki
+    Convert parsed html table, from the Changes Section in the respective ISO3166-2 wiki
     page, into a pandas dataframe. Convert columns/headers using correct naming 
-    conventions, correct "Date Issued" column into correct date format. If year param 
-    not empty then remove any rows that don't have specified year/s or year range.
+    conventions. If year param not empty then remove any rows that don't have 
+    specified year(s) or year range.
 
     Parameters
     ----------
     :iso3166_updates_table : array
-        2D array of ISO3166-2 updates from Changes section in wiki
+        2D array of ISO3166-2 updates from Changes section in wiki.
     :year : array
-        array/list of year(s), if not empty only the ISO3166 updates for the selected
+        array/list of year(s). If not empty only the ISO3166 updates for the selected
         year for a particular country will be returned. If empty then all years of 
         updates are returned.
 
     Returns
     -------
     :iso3166_df : pd.DataFrame
-        comverted pandas dataframe of all ISO3166-2 changes for particular country
+        converted pandas dataframe of all ISO3166-2 changes for particular country
         from 2D input array.
     """
     #update column names to correct naming conventions
     cols = correct_columns(iso3166_updates_table[0])
 
     #convert 2D array into dataframe    
     iso3166_df = pd.DataFrame(iso3166_updates_table[1:], columns=cols)
 
     #get index and name of Date column in DataFrame, i.e the column that has 'date' in it
-    dateColIndex = [idx for idx, s in enumerate(list(map(lambda x: x.lower(), iso3166_df.columns))) if 'date' in s]
-    dateColName = list(iso3166_df.columns)[dateColIndex[0]]
+    date_col_index = [idx for idx, s in enumerate(list(map(lambda x: x.lower(), iso3166_df.columns))) if 'date' in s]
+    date_col_name = list(iso3166_df.columns)[date_col_index[0]]
 
     def correct_date(row):
-        """ parse new date from row if changes have been "corrected". """
-        if "corrected" in row:
-            # wordEndIndex = row.index("corrected") + len("corrected")
+        """ parse new date from row if date of changes has been "corrected". """
+        if ("corrected" in row):
             return row[row.index("corrected") + len("corrected"):].strip().replace(')', '')
         else:
             return row 
 
-    def convert_date(row):
-        """ convert string date in rows of df into year from date object. """
-        return datetime.datetime.strptime(row.replace('\n', ''), '%Y-%m-%d').year
+    def get_year(row):
+        """ convert string date in rows of df into dd-mm-yyyy data format from date object. """
+        return datetime.datetime.strptime(row, '%d-%m-%Y').year
 
-    #parse date column to get corrected & most recent date, if applicable 
-    iso3166_df[dateColName] = iso3166_df[dateColName].apply(correct_date)
+    #reformat date column if date has been corrected
+    iso3166_df[date_col_name] = iso3166_df[date_col_name].apply(correct_date)
     
     #only include rows of dataframe where date updated is same as year parameter, drop year col
     if (year != []): 
-        print('year_range', year_range)
-        iso3166_df['Year'] = iso3166_df[dateColName].apply(convert_date)         #create temp new column to get year of updates from date column 
+        #create temp year column to get year of updates from date column 
+        iso3166_df['Year'] = iso3166_df[date_col_name].apply(get_year)         
         temp_iso3166_df_array = []
         for year_ in year:
-            # temp_year = str(datetime.datetime.strptime(input_data[code][update]["Date Issued"].replace('\n', ''), '%Y-%m-%d').year)
             temp_iso3166_df = iso3166_df[iso3166_df.Year == int(year_)]
             temp_iso3166_df_array.append(temp_iso3166_df)
 
+        #concatenate list of correct rows, drop temp year column from dataframe
         iso3166_df = pd.concat(temp_iso3166_df_array)
         iso3166_df = iso3166_df.drop('Year', axis=1)
 
     #add below columns if not present so all DF's follow same format
     if ("Edition/Newsletter" not in iso3166_df):
         iso3166_df["Edition/Newsletter"] = ""
 
     if ("Code/Subdivision change" not in iso3166_df):
         iso3166_df["Code/Subdivision change"] = ""
 
     #reindex/reorder columns in df
-    iso3166_df = iso3166_df.reindex(columns=['Date Issued', 'Edition/Newsletter', 'Description of change in newsletter', 'Code/Subdivision change'])
+    iso3166_df = iso3166_df.reindex(columns=['Date Issued', 'Edition/Newsletter', 
+        'Code/Subdivision change', 'Description of change in newsletter'])
 
     #replace all null/nan with empty string
     iso3166_df.fillna("", inplace = True)
 
     return iso3166_df
 
 def correct_columns(cols):
     """ 
     Update column names so all dataframes follow the column format of:
-    ["Edition/Newsletter", "Date Issued", "Description of change in newsletter", 
-    "Code/Subdivision change"]. 
+    ["Date Issued", "Edition/Newsletter", "Code/Subdivision change",
+    "Description of change in newsletter"].
 
     Parameters
     ----------
-    : cols : list
+    :cols : list
         list of column names from header of parsed Changes table on wiki.
     
     Returns
     -------
-    : cols : list
+    :cols : list
         list of columns updated to correct naming conventions. 
     """
     if ("Newsletter" in cols):
         cols = list(map(lambda x: x.replace("Newsletter", 'Edition/Newsletter'), cols))
     cols = list(map(lambda x: x.replace("Newsletter/OBP", 'Edition/Newsletter'), cols))
     cols = list(map(lambda x: x.replace("Source", 'Edition/Newsletter'), cols))
     cols = list(map(lambda x: x.replace("Date issued", 'Date Issued'), cols))
@@ -344,73 +367,71 @@
     """
     Convert html table into 2D array. Much of the function code was inspired from [1] which 
     provides an optimal and working solution for handling tables with different rowspans & 
     colspans. 
 
     Parameters
     ----------
-    : table_tag : bs4.element.Tag
-        bs4 object of table element.
+    :table_tag : bs4.element.Tag
+      bs4 object of table element.
     
     Returns
     -------
-    : table : tuple
-        tuple of parsed data from html table in Changes section of ISO3166 wiki.
+    :table : tuple
+      tuple of parsed data from html table in Changes section of ISO3166 wiki.
     
     Reference
     ---------
     [1]: https://stackoverflow.com/questions/48393253/how-to-parse-table-with-rowspan-and-colspan
-
     """
     #if invalid table tag input return empty array
     if (table_tag is None):
         return []
 
-    rowspans = []  # track pending rowspans
+    rowspans = []  #track pending rowspans
     rows = table_tag.find_all('tr') #all table rows
 
-    # first scan, see how many columns we need
+    #count columns (including spanned).
+    #add active rowspans from preceding rows
+    #we *ignore* the colspan value on the last cell, to prevent
+    #creating 'phantom' columns with no actual cells, only extended
+    #colspans. This is achieved by hardcoding the last cell width as 1. 
+    #a colspan of 0 means “fill until the end” but can really only apply
+    #to the last cell; ignore it elsewhere. 
     colcount = 0
     for r, row in enumerate(rows):
         cells = row.find_all(['td', 'th'], recursive=False)
-        # count columns (including spanned).
-        # add active rowspans from preceding rows
-        # we *ignore* the colspan value on the last cell, to prevent
-        # creating 'phantom' columns with no actual cells, only extended
-        # colspans. This is achieved by hardcoding the last cell width as 1. 
-        # a colspan of 0 means “fill until the end” but can really only apply
-        # to the last cell; ignore it elsewhere. 
         colcount = max(
             colcount,
             sum(int(c.get('colspan', 1)) or 1 for c in cells[:-1]) + len(cells[-1:]) + len(rowspans))
         # update rowspan bookkeeping; 0 is a span to the bottom. 
         rowspans += [int(c.get('rowspan', 1)) or len(rows) - r for c in cells]
         rowspans = [s - 1 for s in rowspans if s > 1]
 
-    # it doesn't matter if there are still rowspan numbers 'active'; no extra
-    # rows to show in the table means the larger than 1 rowspan numbers in the
-    # last table row are ignored.
+    #it doesn't matter if there are still rowspan numbers 'active'; no extra
+    #rows to show in the table means the larger than 1 rowspan numbers in the
+    #last table row are ignored.
 
-    # build an empty matrix for all possible cells
+    #build an empty matrix for all possible cells
     table = [[None] * colcount for row in rows]
-    # fill matrix from row data
-    rowspans = {}  # track pending rowspans, column number mapping to count
+    #fill matrix from row data
+    rowspans = {}  #track pending rowspans, column number mapping to count
     for row, row_elem in enumerate(rows):
-        span_offset = 0  # how many columns are skipped due to row and colspans 
+        span_offset = 0  #how many columns are skipped due to row and colspans 
         for col, cell in enumerate(row_elem.find_all(['td', 'th'], recursive=False)):
-            # adjust for preceding row and colspans
+            #adjust for preceding row and colspans
             col += span_offset
             while rowspans.get(col, 0):
                 span_offset += 1
                 col += 1
 
-            # fill table data
+            #fill table data
             rowspan = rowspans[col] = int(cell.get('rowspan', 1)) or len(rows) - row
             colspan = int(cell.get('colspan', 1)) or colcount - col
-            # next column is offset by the colspan
+            #next column is offset by the colspan
             span_offset += colspan - 1
 
             # if table cell is a newline character set to empty string
             if (cell.get_text() == "\n"):
                 value = ""
             #if text has breakpoint (<br>), replace with space
             # elif ("<br/>" in str(cell)):
@@ -422,49 +443,48 @@
             if not (cell.find('a') is None):
                 if not (cell.find('a')['href'].startswith('/wiki/')):
                     value = value + " (" + cell.find('a')['href'] + ')'
 
             for drow, dcol in product(range(rowspan), range(colspan)):
                 try:
                     table[row + drow][col + dcol] = value
-                    # print(table[row + drow][col + dcol])
                     rowspans[col + dcol] = rowspan
                 except IndexError:
-                    # rowspan or colspan outside the confines of the table
+                    #rowspan or colspan outside the confines of the table
                     pass
           
-        # update rowspan bookkeeping
+        #update rowspan bookkeeping
         rowspans = {c: s - 1 for c, s in rowspans.items() if s > 1}
 
     #iterate through converted table, removing any newline characters
     for row in range(0, len(table)):
         for col in range(0, len(table[row])):
             if not (table[row][col] is None):
                 table[row][col] = table[row][col].replace('\n', '')
 
-    return table 
+    return table
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser(description='Get latest changes/updates of ISO3166-2 country codes.')
     parser.add_argument('-alpha2', '--alpha2', type=str, required=False, default="", 
-        help='Alpha2 code/s of ISO3166 countries to check for updates.')
+        help='Alpha-2 code/s of ISO3166 countries to check for updates.')
     parser.add_argument('-year', '--year', type=str, required=False, default="", 
         help='Selected year to check for updates.')
     parser.add_argument('-export_filename', '--export_filename', type=str, required=False, default="iso3166-updates", 
         help='Filename for exported ISO3166 updates csv file.')
     parser.add_argument('-export_json_filename', '--export_json_filename', type=str, required=False, default="iso3166-updates", 
         help='Filename for exported ISO3166 updates json file.')
-    parser.add_argument('-export_folder', '--export_folder', type=str, required=False, default="../test-iso3166-updates", 
+    parser.add_argument('-export_folder', '--export_folder', type=str, required=False, default="test-iso3166-updates", 
         help='Folder where to store exported ISO files.')
     parser.add_argument('-export_json', '--export_json', action="store_false", required=False, 
         help='Whether to export all found updates to json.')
     parser.add_argument('-export_csv', '--export_csv', required=False, action="store_true", 
         help='Whether to export all found updates to csv files in export folder.')
-    parser.add_argument('-concat_updates', '--concat_updates', action="store_true", required=False, 
+    parser.add_argument('-concat_updates', '--concat_updates', action="store_true", default=True, required=False, 
         help='Whether to concatenate updates of individual countrys into the same json file or seperate.')
 
     #parse input args
     args = parser.parse_args()
     alpha2_codes = [args.alpha2]
     if (',' in alpha2_codes[0]):
         alpha2_codes = alpha2_codes[0].split(',')
@@ -475,18 +495,18 @@
     export_json = args.export_json
     export_csv = args.export_csv
     year = [args.year]
     if (',' in year[0]):
         year = year[0].split(',')
     alpha_codes = []
 
-    #use all ISO3166 codes if invalid alpha2 code input, otherwise convert alpha2 to array
+    #use all ISO3166 codes if invalid alpha-2 code input, otherwise convert alpha-2 to array
     if (alpha2_codes == [''] or not isinstance(alpha2_codes, list)):
         alpha2_codes = sorted(list(iso3166.countries_by_alpha2.keys()))
 
     #sort codes in alphabetical order
     alpha2_codes.sort()
     alpha2_codes = [code.upper() for code in alpha2_codes]
     
-    #output ISO3166 updates/changes for selected alpha2 code/s
+    #output ISO3166 updates/changes for selected alpha-2 code/s
     get_updates(alpha2_codes, year, export_filename, export_json_filename,
         export_folder, concat_updates, export_json, export_csv)
```

### Comparing `iso3166-updates-0.0.7/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.0.1/iso3166_updates.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 0.0.7
+Version: 1.0.1
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
 Description: # iso3166-updates
         
         [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
-        [![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-updates/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-updates/actions)
+        [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
         [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
         [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-        [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-flag-icons)](https://github.com/amckenna41/iso3166-updates/issues)
+        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
+        [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
         [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
         [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
           <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
         </div>
         
-        > Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here](https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing).
+        > Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
         
         Table of Contents
         -----------------
-        
           * [Introduction](#introduction)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
-          * [Issues](#Issues)
           * [Directories](#Directories)
+          * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
         
         The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
         
-        **Problem Statement:**
+        ## Problem Statement:
         
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform or Online Browsing Platform or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published throughout the year [[4]](#references). 
+        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published at various times throughout the year [[4]](#references). 
         
-        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of countrys' ISO 3166-2 codes for free, with an easy-to-use interface and Python package, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
+        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
         
-        **Intended Audience:**
+        ## Intended Audience:
         
-        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy -to-use API. 
+        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API. 
         
         <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
         
         Updates
         -------
         **Last Updated:**
-        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function (iso3166-check-for-updates). This function  
         
+        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+        The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO3166-2 wiki's to check for the latest updates within a certain period e.g the past 3 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the main GCP Cloud Function returns the latest data. Additionally, a GitHub Issue in the `iso3166-2` repository will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` JSONs and repo.
+        Ultimately, this function ensures that the software and assoicated APIs are up-to-date with the latest ISO3166-2 information for all countries/territories/subdivisions etc.
         
         API
         ---
         An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
         
-        >                               https://www.iso3166-updates.com
-        <!-- > https://us-central1-iso3166-updates.cloudfunctions.net/iso3166-updates -->
+        > https://www.iso3166-updates.com/api
         
-        Two query string parameters / paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE. A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY, HU, ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO3166 updates. A complete diagram of the architecture is available in the iso3166-updates-api/README. This JSON is updated regularly using a CRON GithHub Action workflow that is called every 6 months (.github/workflows/check_for_updates.yml) that also utilises a Cloud Func and the Python software to check for the most latest ISO3166 updates (<=6 months) - <i>in development</i>.
+        Two query string parameters/paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE". A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY", "HU", "ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below.
         
         The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
         
          <!-- "?year" can be a specific year or year range to get updates for (e.g "2017", "2010-2015"), you can also get updates less than or greater than a year (e.g ">2004", "<2020") and "?months" which allows you to get the updates of the past X months. If months and year input params are set then months will take precedence. -->
         <p align="center">
-          <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/gcp_cloud_arch.png" alt="gcp_arch" height="200" width="400"/>
+          <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
         </p>
         
-        
         Requirements
         ------------
         * [python][python] >= 3.7
         * [pandas][pandas] >= 1.4.3
         * [numpy][numpy] >= 1.23.2
         * [requests][requests] >= 2.28.1
         * [beautifulsoup4][beautifulsoup4] >= 4.11.1
         * [iso3166][iso3166] >= 2.1.1
         
         Installation
         ------------
-        Install the latest version of iso3166-updates via [PyPi][PyPi] using pip:
+        Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
         
         ```bash
         pip3 install iso3166-updates --upgrade
         ```
         
         Installation from source:
         ```bash
@@ -125,95 +125,102 @@
           #                       Whether to export all found updates to csv files in export folder.
           # -year YEAR, --year YEAR
           #                       Selected year to check for updates.
           # -concat_updates, --concat_updates
           #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
         ```
         
+        **Get all listed changes/updates for all countries which happens by default if no alpha2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+        ```python
+        iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
+        ```
+        
         **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
         ```python
         iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
         ```
         
-        <!-- def get_updates(alpha2_codes, year=[''], export_filename="iso3166-updates",
-                export_json_filename="iso3166-updates", export_folder="../test/iso3166-updates", 
-                concat_updates=True, export_json=True, export_csv=False): -->
-        
         **Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
         ```python
-        iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=1))
+        iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0))
         ```
         
         **Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
         ```python
-        iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_json_filename="iso3166-updates")
+        iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_json_filename="iso3166-updates", concat_updates=0)
         ```
         
         **Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
         ```python
         iso3166_updates.get_updates("IE", year="2012-2021")
         ```
         
-        **Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years > 2015, export only to CSV with filename "iso3166-output.csv":**
+        **Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename "iso3166-output.csv":**
         ```python
-        iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output")
+        iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output.csv")
         ```
         
         **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
         ```python
-        iso3166_updates.get_updates("YE", year=">2010")
+        iso3166_updates.get_updates("YE", year="<2010")
         ```
         
         The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
         Edition/Newsletter, Date Issued, Description of change in newsletter and Code/Subdivision change. 
+        
+        * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+        * Date Issued: Date that the change was communicated.
+        * Description of change in newsletter: More in-depth info about the change/update that was made.
+        * Code/Subdivision change: Overall summary of change/update made.
+        
         E.g. The output format of the exported CSV for AD (Andorra) is:
         
         | Edition/Newsletter | Date Issued | Description of change in newsletter | Code/Subdivision change |   
         |:-------------------|:------------|------------------------------------:|------------------------:|
         | Newsletter I-8     | 2007-04-17  | Addition of the administrative subdivisions...   | Subdivisions added: 7 parishes...                 | 
         | Online Browsing Platform (OBP) | 2014-11-03 | Update List Source | No subdivision changes listed |
         | Online Browsing Platform (OBP) | 2015-11-27 | Update List Source | No subdivision changes listed | 
         
         E.g. The output format of the exported JSON for AD (Andorra) is:
-        ```json
+        ```javascript
         {
           AD: [
               {
-                Code/Subdivision change: "",
-                Date Issued: "2015-11-27",
-                Description of change in newsletter: "Update List Source",
-                Edition/Newsletter: "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+                "Code/Subdivision change": "",
+                "Date Issued": "2015-11-27",
+                "Description of change in newsletter": "Update List Source",
+                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
               },
               {
-                Code/Subdivision change: "",
-                Date Issued: "2014-11-03",
-                Description of change in newsletter: "Update List Source",
-                Edition/Newsletter: "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+                "Code/Subdivision change": "",
+                "Date Issued": "2014-11-03",
+                "Description of change in newsletter": "Update List Source",
+                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
               },
               {
-                Code/Subdivision change: "Subdivisions added:7 parishes",
-                Date Issued: "2007-04-17",
-                Description of change in newsletter: "Addition of the administrative subdivisions and of their code elements",
-                Edition/Newsletter: "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
+                "Code/Subdivision change:" "Subdivisions added:7 parishes",
+                "Date Issued": "2007-04-17",
+                "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
+                "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
               }
           ]
         }
         ```
         
         Directories
         -----------
-        * `/docs` - documentation for iso3166-updates Python package.
-        * `/iso3166_updates` - source code for iso3166-updates Python package.
-        * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the iso3166-updates API, including the main.py, requirements.txt and API config file.
+        * `/docs` - documentation for `iso3166-updates` Python package.
+        * `/iso3166_updates` - source code for `iso3166-updates` Python package.
+        * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
         * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Func that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt.
-        * `/tests` - unit and integration tests for iso3166-updates.
+        * `/tests` - unit and integration tests for `iso3166-updates`.
         
         Issues
         ------
-        Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+        Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
         
         Contact
         -------
         If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
         [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
         
         References
@@ -226,21 +233,23 @@
         
         Support
         -------
         <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
         
         [Back to top](#TOP)
         
+        [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
         [python]: https://www.python.org/downloads/release/python-360/
         [pandas]: https://pandas.pydata.org/
         [numpy]: https://numpy.org/
         [requests]: https://requests.readthedocs.io/
         [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
         [iso3166]: https://github.com/deactivated/python-iso3166
-        [PyPi]: https://pypi.org/project/pysar/
+        [PyPi]: https://pypi.org/project/iso3166-updates/
+        [Issues]: https://github.com/amckenna41/iso3166-updates/issues
 Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csviso3166-2,iso3166-1,alpha2,alpha3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iso3166-updates-0.0.7/setup.cfg` & `iso3166-updates-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 0.0.7
+version = 1.0.1
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-0.0.7/setup.py` & `iso3166-updates-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 import pathlib
 from setuptools import setup, find_packages
 import sys
 # import iso3166_updates
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "0.0.7"
+__version__ = "1.0.1"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
-__credits__ = ['AJ McKenna']
 __status__ = 'Development'
 __maintainer__ = "AJ McKenna"
 __keywords__ = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv" \
             "iso3166-2", "iso3166-1", "alpha2", "alpha3"]
 __test_suite__ = "tests"
  
 #ensure python version is greater than 3
```


# Comparing `tmp/sustainalytics-0.2.2.tar.gz` & `tmp/sustainalytics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sustainalytics-0.2.2.tar", max compression
+gzip compressed data, was "sustainalytics-0.3.0.tar", max compression
```

## Comparing `sustainalytics-0.2.2.tar` & `sustainalytics-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      711 2023-04-05 12:20:23.905581 sustainalytics-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6240 2022-12-09 15:11:26.064961 sustainalytics-0.2.2/README.md
--rw-r--r--   0        0        0       23 2023-04-05 12:18:53.991537 sustainalytics-0.2.2/sustainalytics/__init__.py
--rw-r--r--   0        0        0    28667 2022-10-05 13:30:13.748480 sustainalytics-0.2.2/sustainalytics/api.py
--rw-r--r--   0        0        0     7182 2023-04-05 12:23:18.686851 sustainalytics-0.2.2/setup.py
--rw-r--r--   0        0        0     7149 2023-04-05 12:23:18.686851 sustainalytics-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      777 2023-05-12 13:09:40.916939 sustainalytics-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8007 2023-05-12 13:02:20.064810 sustainalytics-0.3.0/README.md
+-rw-r--r--   0        0        0       23 2023-05-12 13:08:55.770785 sustainalytics-0.3.0/sustainalytics/__init__.py
+-rw-r--r--   0        0        0    41747 2023-05-11 08:44:19.260290 sustainalytics-0.3.0/sustainalytics/api.py
+-rw-r--r--   0        0        0     9139 1970-01-01 00:00:00.000000 sustainalytics-0.3.0/PKG-INFO
```

### Comparing `sustainalytics-0.2.2/PKG-INFO` & `sustainalytics-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,204 +1,202 @@
-Metadata-Version: 2.1
-Name: sustainalytics
-Version: 0.2.2
-Summary: This is a package that helps clients access sustainalytics API
-Home-page: https://github.com/Kienka/sustainalytics
-License: MIT
-Author: Kienka Cromwell Kio
-Author-email: kienka.kio@sustainalytics.com
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
-Description-Content-Type: text/markdown
-
-#### Introduction
+## Introduction
 
 **Starting with sustainalytics 0.2.0, the package is compatible with API v2 only. If a v1-compatible version is needed, please install version 0.1.2 via this command:**
 
 ```python
 pip install sustainalytics==0.1.2
 ```
 
 
 This python package provides access to Sustainalytics API (Application Programming Interface) service which provides developers with 24x7 programmatic access to Sustainalytics data. The API has been developed based on market standards with a primary focus on secure connectivity and ease of use. It allows users to retrieve and integrate Sustainalytics data into their own internal systems and custom or third-party applications
 
 This document is meant to provide developers with python sample code for the Sustainalytics API service.
 Technical documentation can also be found on the dedicated [website](https://api.sustainalytics.com/swagger/ui/index/index.html) for the API.
 
-![Figure1](https://github.com/Kienka/sustainalytics/raw/master/sustainalytics/Figure1.PNG)
 
-#### Installation
+## Installation
 <p>Install the package via pip with code below:
 
 
 ```python
 pip install sustainalytics
 ```
 
 To Upgrade:
 
 
 ```python
 pip install --upgrade sustainalytics
 ```
 
-#### Connection
+## Connection
 A clientid and a secret key must be provided by the Sustainalytics Team in order to access the API.
 See connection via python:
 
 
 ```python
 from sustainalytics.api import API
 
-#Access
+# Access
 client_id = 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
 client_secret_key = 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
 
 con = API(client_id=client_id, client_secretkey=client_secret_key)
 
-#returns Bearer
+# Returns Bearer
 print(con.access_headers)
 ```
 
-### Endpoints
+## Helper functions
+These helper functions are meant to help you in calling the endpoint functions.
 
-#### DataService
+```python
+fieldClusterIds = con.get_fieldClusterIds()
+print(fieldClusterIds)
 
-The DataService enables the user to call the research data associated with the companies in the universe of access. Within this service there are two endpoints, as described below.
+fieldIds = con.get_fieldIds()
+print(fieldIds)
 
-![](https://github.com/Kienka/sustainalytics/raw/master/sustainalytics/dataservice.png)
+fieldsInfo = con.get_fieldsInfo()
+print(fieldsInfo)
 
-The code below shows you how to extract data from these endpoints
+productIds = con.get_productIds()
+print(productIds)
 
-#### GetData 
+packageIds = con.get_packageIds()
+print(packageIds)
 
-Retrieves data from the DataService endpoint. 'identifiers' and 'productId' are **mandatory** endpoints
+packageInfo = con.get_packageInfo()
+print(packageInfo)
+```
 
+## Endpoints
 
-##### __The 'identifiers' and 'productId' arguments can be combined with only one of the other arguments:__
+### DataService
 
-__identifiers__ : A list of security or entity identifiers separated by comma. You can obtain list of EntityIds from the con.get_universe_entityIds(keep_duplicates=True)
+The DataService enables the user to call the research data associated with the companies in the universe of access. Within this service there are 6 endpoints, as described below.
 
-__packageIds__ : A list of package ids separated by comma. You can obtain list of PackageIds from the con.get_packageIds()
+<ul>
+    <li>DataService - Get research data by query</li>
+    <li>DataService/{identifier} - Get research data by identifier </li>
+    <li>DataServiceWTimestamps - Get timestamped research data by query </li>
+    <li>DataServiceWTimestamps/{identifier} - Get timestamped research data by identifier </li>
+    <li>LastChangesSince - Get last changes since research data by query </li>
+    <li>LastChangesSince/{identifier} - Get last changes since research data by identifier </li>
+</ul>
 
-__fieldClusterIds__ : A list of field cluster ids separated by comma. You can obtain list of FieldClusterIds from the con.get_fieldClusterIds()
+The code below shows you how to extract data from these endpoints:
 
-__fieldIds__ : A list of field ids separated by comma. You can obtain list of FieldIds from the con.get_fieldIds()
+#### Get Data 
 
-![](https://github.com/Kienka/sustainalytics/raw/master/sustainalytics/ds_params.png)
+Retrieves data from the DataService or from the DataServiceWTimestamps endpoint. 'identifiers' and 'productId' are **mandatory** arguments.
 
+__identifiers__ : A list of security or entity identifiers separated by comma. You can obtain a list of EntityIds from the con.get_universe_entityIds(keep_duplicates=True)
+
+__productid__ : The Product ID. Only one integer value is accepted. You can obtain a list of ProductIds from the con.get_productIds()
+
+__timestamps__ : optional boolean argument present only in the get_data function that let's you choose between timestamped research data and research data. 
+
+In addition to the 3 arguments, one of the following arguments can also be chosen:
+
+__packageIds__ : A list of package ids separated by comma. You can obtain a list of PackageIds from the con.get_packageIds()
+
+__fieldClusterIds__ : A list of field cluster ids separated by comma. You can obtain a list of FieldClusterIds from the con.get_fieldClusterIds()
+
+__fieldIds__ : A list of field ids separated by comma. You can obtain a list of FieldIds from the con.get_fieldIds()
+
+```python
+# GetData for research data (default dtype='json') - DataService endpoint.
+research_data = con.get_data(identifiers=[], productId=x, packageIds=[], fieldClusterIds=[], fieldIds=[], dtype='dataframe', timestamps=False)
+print(research_data)
+```
 
 ```python
-#### GetData
-data = con.get_data(identifiers=[], productId=[], packageIds=[], fieldClusterIds=[], fieldIds=[])
-#returns data for the specified identifier(s). 'identifiers' and 'productId' are required for the function to work.
-print(data)
+# GetData for timestamped research data (default dtype='json') - DataServiceWTimestamps endpoint.
+timestamped_research_data = con.get_data(identifiers=[], packageIds=[], productId=x, fieldClusterIds=[], fieldIds=[], dtype='dataframe', timestamps=True)
+print(timestamped_research_data)
 ```
 
-#### Product Structure & Definitions
+#### Get LastChangesSince
+Retrieves data from the LastChangesSince endpoint. 'startdate' and 'productId' are **mandatory** arguments.
+
+Additional arguments compared to get_data:
+
+__startdate__ : Date filter for last changes query. The format of the date is "yyyy-mm-dd". Can retrieve data only for last 3 months from current date.
+
+```python
+# Get LastChangesSince returns timestamped research data that has changed since a specific date (default dtype='json') - LastChangeSince endpoint
+last_changes_since_data = con.get_LastChangesSince(startdate="x", productId=x, identifiers=[], packageIds=[], fieldClusterIds=[], fieldIds=[], dtype='dataframe')
+print(last_changes_since_data)
+```
+
+### Product Structure & Definitions
 
 Each product is built from __data packages__ and each data package is built from __field clusters__. The __datafields__ are the smallest components of the product structure. 
 
 The Product Structure service provides an overview  of the data fields available in the  Sustainalytics API and the unique __FieldIds__ linked to each of these data fields. Within this service there are three endpoints, as described below.
 
-![Figure2](https://github.com/Kienka/sustainalytics/raw/master/sustainalytics/fids.png)
-
-The code below shows you how to extract data from these endpoints
+<ul>
+  <li>FieldDefinitions - Get field definitions</li>
+  <li>FieldMappings - Get product structure </li>
+  <li>FieldMappingDefinitions - Get product structure with field definitions </li>
+</ul>
 
+The code below shows you how to extract data from these endpoints:
 
 ```python
-#### FieldDefinitions
-field_definitions = con.get_fieldDefinitions(dtype='dataframe') #by default dtype='json'
+# FieldDefinitions (default dtype='json')
+field_definitions = con.get_fieldDefinitions(dtype='dataframe')
 print(field_definitions)
 
-#### FieldMappings
-field_mappings = con.get_fieldMappings(dtype='dataframe') #by default dtype='json'
+# FieldMappings (default dtype='json')
+field_mappings = con.get_fieldMappings(dtype='dataframe') 
 print(field_mappings)
 
-#### FieldMappingDefinitions
-field_mapping_definition = con.get_fieldMappingDefinitions(dtype='dataframe') #by default dtype='json'
+# FieldMappingDefinitions (default dtype='json')
+field_mapping_definition = con.get_fieldMappingDefinitions(dtype='dataframe')
 print(field_mapping_definition)
 
-#### Extra FieldDefinition (non-Swagger)
-fullFieldDef = con.get_fullFieldDefinitions(dtype='dataframe')
-print(fullFieldDef)
+# Extra FieldDefinition (non-Swagger) (default dtype='json')
+full_field_definitions = con.get_fullFieldDefinitions(dtype='dataframe')
+print(full_field_definitions)
 ```
 
-#### Reports
+### Reports
 
 The ReportService endpoint allows users to retrieve a list of all available PDF report types by ReportId, ReportType, and ReportName for companies belonging to the universe of access. 
-
 __(Please note this Endpoint is not part of the standard API product.)__
 
-![Figure3](https://github.com/Kienka/sustainalytics/raw/master/sustainalytics/reports.png)
-
-The code below shows you how to extract data from these endpoints
-
+<ul>
+  <li>ReportService - Get available report types</li>
+  <li>ReportService/{identifier} - Get available report types by entity identifier</li>
+  <li>ReportService/url/{identifier}/{reportId} - Get report url (recommended endpoint as it has the fastest response time) </li>
+</ul>
+
+The code below shows you how to extract data from these endpoints:
 
 ```python
-####ReportService
-report_info = con.get_pdfReportInfo(productId=x,dtype='dataframe')  #by default dtype='json'
-where x be any integer value of existing product ids (for example, 10 for Corporate Data)
-#returns all the available report fieldIDs (reportids)
+# ReportService - returns all the available report fieldIDs (reportids) (default dtype='json')
+report_info = con.get_pdfReportInfo(productId=x, dtype='dataframe') 
+# Where x can be any integer value of existing product ids (for example, 10 for Corporate Data)
 print(report_info)
 
-####ReportService(identifier)(reportid)
+# ReportService(identifier/reportid) - returns the URL to given pdf report for specified companies (if available) (default dtype='json')
 report_identifier_reportid = con.get_pdfReportUrl(identifier=x, reportId=y)
-#returns the url to given pdf report for specified companies (if available)
 print(report_identifier_reportid)
 ```
 
 The function supports only 1 identifier and reportID per call.
 
-####  Universe of Access
+###  Universe of Access
 
 The UniverseOfAccess endpoint allows users to determine the list of EntityIds contained in the universe of access (all permissioned securities lists).
 
-![Figure4](https://github.com/Kienka/sustainalytics/raw/master/sustainalytics/univ.png)
-
+<ul>
+  <li>UniverseOfAccess - Get universe of access</li>
+</ul>
 
 ```python
-####UniverseofAccess
-universe = con.get_universe_access(dtype='dataframe') #by default dtype='json'
-#returns all universe constituents
+# UniverseofAccess - returns all universe constituents (default dtype='json')
+universe = con.get_universe_access(dtype='dataframe')
 print(universe)
 ```
-
-
-```python
-#### Extra non-Swagger functions
-fieldClusterIds = con.get_fieldClusterIds()
-#returns all clusterIds
-print(fieldClusterIds)
-
-fieldIds = con.get_fieldIds()
-#returns all fieldIDs
-print(fieldIds)
-
-fieldsInfo = con.get_fieldsInfo()
-#returns fields info
-print(fieldsInfo)
-
-productIds = con.get_productIds()
-#returns product IDs
-print(productIds)
-
-packageIds = con.get_packageIds()
-#returns package IDs
-print(packageIds)
-
-packageInfo = con.get_packageInfo()
-#returns package info
-print(packageInfo)
-```
-
```


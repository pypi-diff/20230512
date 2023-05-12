# Comparing `tmp/salure_helpers_profit-1.2.4.tar.gz` & `tmp/salure_helpers_profit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-1.2.4.tar", last modified: Wed Mar  8 13:35:18 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-1.3.0.tar", last modified: Fri May 12 07:18:59 2023, max compression
```

## Comparing `salure_helpers_profit-1.2.4.tar` & `salure_helpers_profit-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/
--rw-r--r--   0 root         (0) root         (0)      262 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-03-08 13:35:03.000000 salure_helpers_profit-1.2.4/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-03-08 13:35:03.000000 salure_helpers_profit-1.2.4/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    12953 2023-03-08 13:35:03.000000 salure_helpers_profit-1.2.4/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    16113 2023-03-08 13:35:03.000000 salure_helpers_profit-1.2.4/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   130036 2023-03-08 13:35:03.000000 salure_helpers_profit-1.2.4/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-08 13:35:18.000000 salure_helpers_profit-1.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      553 2023-03-08 13:35:03.000000 salure_helpers_profit-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17549 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   130048 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-12 07:18:58.000000 salure_helpers_profit-1.3.0/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 07:18:59.000000 salure_helpers_profit-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-12 07:18:44.000000 salure_helpers_profit-1.3.0/setup.py
```

### Comparing `salure_helpers_profit-1.2.4/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.2.4/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 import base64
 import json
 import time
+import sys
 import pandas as pd
 from urllib import parse
 import requests
+from requests.adapters import HTTPAdapter
 from salure_helpers.salureconnect import SalureConnect
 from typing import Union, List
+from tenacity import retry, stop_after_attempt, wait_exponential_jitter, retry_if_exception
+
+
+def is_request_exception(e: BaseException) -> bool:
+    if isinstance(e, requests.RequestException) and (e.response.status_code >= 500 or e.response.status_code == 408):
+        error = str(e)[:400].replace('\'', '').replace('\"', '')
+        print(f"{error}, retrying")
+        return True
+    else:
+        return False
 
 
 class GetConnector(SalureConnect):
     def __init__(self, label: Union[str, List], test_environment: bool = False, debug: bool = False):
         super().__init__()
         if test_environment:
             self.base_url = 'resttest.afas.online'
         else:
             self.base_url = 'rest.afas.online'
         credentials = self.get_system_credential(system='profit', label=label, test_environment=test_environment)
         self.environment = credentials['environment']
         base64token = base64.b64encode(credentials['token'].encode('utf-8')).decode()
-        self.headers = {'Authorization': 'AfasToken ' + base64token}
+        self.session = requests.Session()
+        self.session.headers.update({'Authorization': 'AfasToken ' + base64token,
+                                     'IntegrationId': '38092_135680'})
         self.debug = debug
 
     def get_metadata(self, connector: str = None):
         url = f"https://{self.environment}.{self.base_url}/profitrestservices/metainfo{f'/get/{connector}' if connector is not None else ''}"
-        vResponse = requests.get(url, headers=self.headers).json()[f"{'getConnectors' if connector is None else 'fields'}"]
+        response = self.session.get(url=url)
+        response = response.json()[f"{'getConnectors' if connector is None else 'fields'}"]
 
-        return vResponse
+        return response
 
     def get_data(self, connector, fields=None, values=None, operators=None, orderbyfields=None):
         """
         Possible filter operators are:
         1: is gelijk aan
         2: is groter of gelijk aan
         3: is kleiner of gelijk aan
@@ -45,15 +60,14 @@
         14 :veld eindigt niet met tekst	                            Plaats het teken % aan het begin van de filterwaarde, bijvoorbeeld %MiMicrosoft
 
         If you use a skip and take, highly recommended to specify orderbyfields. This makes the requests much faster.
         You should use unique fields or combinations of most unique fields in the dataset
 
         Using ';' between filters is OR, ',' is AND
         """
-
         total_response = []
         loop_boolean = True
         no_of_loops = 0
         no_of_results = 0
 
         if fields is not None:
             parameters = {"filterfieldids": fields, "filtervalues": values, "operatortypes": operators}
@@ -64,26 +78,25 @@
             parameters["orderbyfieldids"] = "-{}".format(orderbyfields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, connector)
 
         while loop_boolean:
             loop_parameters = {"skip": 40000 * no_of_loops, "take": 40000}
             parameters.update(loop_parameters)
-            response = requests.get(url.encode("utf-8"), parameters, headers=self.headers, timeout=30000)
-            if response.status_code == 200:
-                response_json = response.json()['rows']
-                no_of_loops += 1
-                no_of_results += len(response_json)
-                loop_boolean = True if len(response_json) == 40000 else False
-
-                if self.debug:
-                    print(time.strftime('%H:%M:%S'), 'Got next connector from profit: ', connector, ' With nr of rows: ', no_of_results)
-                total_response += response_json
-            else:
-                return response.text
+            request = requests.Request('GET', url=url, params=parameters)
+            prepared_request = self.session.prepare_request(request)
+            response = self.do_request(prepared_request)
+            response_json = response.json()['rows']
+            no_of_loops += 1
+            no_of_results += len(response_json)
+            loop_boolean = True if len(response_json) == 40000 else False
+
+            if self.debug:
+                print(time.strftime('%H:%M:%S'), 'Got next connector from profit: ', connector, ' With nr of rows: ', no_of_results)
+            total_response += response_json
 
         return total_response
 
     def get_complex_filtered_data(self, connector: str, fields: list, values: list, operators: list, orderbyfields: str = None):
         """
         This method is meant for complex combined filters like (a and b) or (a and c)
 
@@ -129,78 +142,79 @@
             for number in range(0, len(fields_values)):
                 filter["Field"].append({"@FieldId": fields_values[number],
                                         "@OperatorType": operators_values[number],
                                         "#text": values_values[number]})
             parameters['Filters']['Filter'].append(filter)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, connector)
-        # Dit stukje hieronder heeft JJ een paar uur van zn leven gekost. Do not touch
+        # eliminate whitespaces and escape special characters
         querystring = parse.quote(json.dumps(parameters, separators=(',', ':')))
         if orderbyfields is not None:
             querystring = querystring + '&orderbyfieldids={}'.format(orderbyfields)
 
         while loop_boolean:
             loop_parameters = "&skip={}&take={}".format(40000 * no_of_loops, 40000)
-            response = requests.get(url, data='', headers=self.headers, timeout=30000, params="filterjson={}{}".format(querystring, loop_parameters))
-            if response.status_code == 200:
-                response_json = response.json()['rows']
-                no_of_loops += 1
-                no_of_results += len(response_json)
-                loop_boolean = True if len(response_json) == 40000 else False
-
-                if self.debug:
-                    print(time.strftime('%H:%M:%S'), 'Got next connector from profit: ', connector, ' With nr of rows: ', no_of_results)
-                total_response += response_json
-            else:
-                return response.text
+            request = requests.Request('GET', url=url, params="filterjson={}{}".format(querystring, loop_parameters))
+            prepared_request = self.session.prepare_request(request)
+            response = self.do_request(prepared_request)
+            response_json = response.json()['rows']
+            no_of_loops += 1
+            no_of_results += len(response_json)
+            loop_boolean = True if len(response_json) == 40000 else False
+
+            if self.debug:
+                print(time.strftime('%H:%M:%S'), 'Got next connector from profit: ', connector, ' With nr of rows: ', no_of_results)
+            total_response += response_json
 
         return total_response
 
     def get_dossier_attachments(self, dossieritem_id, dossieritem_guid) -> requests.Response:
         """
         This method returns base64encoded binary data in the filedata key of the json response. You can process this by decoding it and writing it to a file using:
         blob = base64.b64decode(response.json()['filedata'])
         with open('{}/{}'.format(self.file_directory, filename), 'wb') as f:
             f.write(blob)
         :param dossieritem_id: dossieritem_id
         :param dossieritem_guid: dossieritem_guid
         :return: response object
         """
         url = f"https://{self.environment}.{self.base_url}/profitrestservices/subjectconnector/{dossieritem_id}/{dossieritem_guid}"
-        response = requests.get(url=url, headers=self.headers)
+        request = requests.Request('GET', url=url)
+        prepared_request = self.session.prepare_request(request)
+        response = self.do_request(prepared_request)
 
         return response
 
     def download_file(self, file_id: str, filename: str, output_folder: str):
         """
         This method is for downloading a file from AFAS.
         :param file_id: the file_id of the file you want to download
         :param filename: the filename of the file you want to download
         :param output_folder: The folder where the file should be saved
         """
 
         url = f"https://{self.environment}.{self.base_url}/profitrestservices/fileconnector/{file_id}/{filename}"
-
-        response = requests.get(url, headers=self.headers)
-        response.raise_for_status()
+        request = requests.Request('GET', url=url)
+        prepared_request = self.session.prepare_request(request)
+        response = self.do_request(prepared_request)
 
         with open(f"{output_folder}/{filename}", 'wb') as f:
             blob = base64.b64decode(response.json()['filedata'])
             f.write(blob)
 
     def download_report(self, report_id: str, output_filepath: str):
         """
         This method is for downloading a report from AFAS.
         :param report_id: the ID of the report you want to download
         :param output_filepath: The full path (folder and filename) to where you want to store the report
         """
         url = f"https://{self.environment}.{self.base_url}/profitrestservices/reportconnector/{report_id}"
-
-        response = requests.get(url, headers=self.headers)
-        response.raise_for_status()
+        request = requests.Request('GET', url=url)
+        prepared_request = self.session.prepare_request(request)
+        response = self.do_request(prepared_request)
 
         with open(f"{output_filepath}", 'wb') as f:
             blob = base64.b64decode(response.json()['filedata'])
             f.write(blob)
 
     def convert_datatypes_to_afas_datatypes(self, data: list, connector: str) -> pd.DataFrame:
         """
@@ -242,7 +256,19 @@
                 else:
                     data[column['id']] = data[column['id']].astype(new_type)
             else:
                 data[column['id']] = data[column['id']].astype(new_type)
 
         # returns the dataframe with the correct datatypes
         return data
+
+    # this method should be used to execute all requests so retry and raising are handled in one place
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_request_exception), reraise=True)
+    def do_request(self, prepped_request: requests.PreparedRequest) -> requests.Response:
+        adapter = HTTPAdapter()
+        response = adapter.send(prepped_request, timeout=3000)
+        if response.status_code >= 400:
+            raise requests.exceptions.ConnectionError(f"Error occured: {response.status_code, response.text} while retrieving data for URL: {prepped_request.url}",
+                                                      response=response, request=prepped_request)
+
+        return response
+
```

### Comparing `salure_helpers_profit-1.2.4/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_get_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 import base64
 import asyncio
 import time
 import aiohttp
 import json
-import pandas as pd
 from typing import List, Union
 from salure_helpers.salureconnect import SalureConnect
 from salure_helpers.profit.profit_get import GetConnector
+from tenacity import retry, stop_after_attempt, wait_exponential_jitter, retry_if_exception
 
 
-class GetConnectorAsync(SalureConnect):
+# This method makes sure that the request is retried if the request fails with a 5xx error or a 408 error
+def is_request_exception(e: BaseException) -> bool:
+    if isinstance(e, aiohttp.ClientResponseError) and (e.status >= 500 or e.status == 408):
+        error = str(e)[:400].replace('\'', '').replace('\"', '')
+        print(f"{error}, retrying")
+        return True
+    else:
+        return False
+
+
+class GetConnectorAsync:
     def __init__(self, label: Union[str, List], test_environment: bool = False, debug: bool = False):
         self.profit = GetConnector(label=label, test_environment=test_environment)
         self.profit_async = ProfitExtractAsync(label=label, test_environment=test_environment, debug=debug)
 
     def get_data(self, connector_information: Union[dict, list, str], batch_size: int = 8, take: int = 40000) -> dict:
         """
         A synchronous method is needed to be able to run multiple asynchronous functions. Within this function, a call
@@ -173,15 +183,16 @@
         if test_environment:
             self.base_url = 'resttest.afas.online'
         else:
             self.base_url = 'rest.afas.online'
         credentials = self.get_system_credential(system='profit', label=label, test_environment=test_environment)
         self.environment = credentials['environment']
         base64token = base64.b64encode(credentials['token'].encode('utf-8')).decode()
-        self.headers = {'Authorization': 'AfasToken ' + base64token}
+        self.headers = {'Authorization': 'AfasToken ' + base64token,
+                        'IntegrationId': '38092_135680'}
         self.got_all_results = False
         self.debug = debug
 
     async def get_data(self, connectors: List = None, parameters: dict = {}, batch_size: int = 8, take: int = 40000) -> dict:
         """
         This (asynchronous) function functions as a wrapper that can carry out multiple single get requests to be able
         to get all data from profit in an asynchronous and efficient way. Only use this function in async code, otherwise use the profit class to call this from a sync function.
@@ -213,50 +224,60 @@
                         else:
                             total_response[key] = value
 
                 batch_number += 1
 
         return total_response
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_request_exception), reraise=True)
     async def get_request(self, url: str, connector: str, params: dict, session: aiohttp.ClientSession, take: int):
         """
         This function carries out a single get request given the inputs. It is used as input for the abovementioned wrapper,
         get_data_content. Note that this function cannot be called it itself, but has to be started via get_data_content.
 
         :param url: profit url to retrieve the data.
         :param params: body of the request.
         :param session: type of the request.
         :return: data in json format
         """
         if self.debug:
             print(f"started request for {connector} at: {time.time()}")
         async with session.get(url=f"{url}{connector}", params=params) as resp:
             if resp.status >= 400:
-                raise ConnectionError(f"Got error: {resp.status, await resp.text()} while retrieving data from connector {connector}")
+                raise aiohttp.ClientResponseError(message=f"Error occured: {resp.status, await resp.text()} while retrieving data for URL: {url}",
+                                                  request_info=resp.request_info,
+                                                  history=resp.history,
+                                                  status=resp.status,
+                                                  headers=resp.headers)
             response = await resp.json()
             response = response['rows']
             if len(response) < take:
                 if self.debug:
                     print(f"request with params: {params} was the last request with {len(response)} rows")
                 self.got_all_results = True
             else:
                 if self.debug:
                     print(f"request with params: {params} has {len(response)} rows")
 
             return {connector: response}
 
+    @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_request_exception), reraise=True)
     async def get_meta_data(self, connector: str = None):
         """
         This function makes sure that you can create a list of connector names without having to call another class.
         :return: returns a list of all connectors in the environment.
         """
 
         url = f"https://{self.environment}.{self.base_url}/profitrestservices/metainfo{f'/get/{connector}' if connector is not None else ''}"
 
-        async with aiohttp.ClientSession(headers=self.headers, timeout=aiohttp.ClientTimeout(), raise_for_status=True) as session:
+        async with aiohttp.ClientSession(headers=self.headers, timeout=aiohttp.ClientTimeout()) as session:
             async with session.get(url=f"{url}") as resp:
                 if resp.status >= 400:
-                    raise ConnectionError(f"Got error: {resp.status, await resp.text()} while retrieving data from connector {connector}")
+                    raise aiohttp.ClientResponseError(message=f"Error occured: {resp.status, await resp.text()} while retrieving data for URL: {resp.url}",
+                                                      request_info=resp.request_info,
+                                                      history=resp.history,
+                                                      status=resp.status,
+                                                      headers=resp.headers)
                 response = await resp.json()
                 response = response[f"{'getConnectors' if connector is None else 'fields'}"]
 
                 return response
```

### Comparing `salure_helpers_profit-1.2.4/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-1.3.0/salure_helpers/profit/profit_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,16 @@
         if test_environment:
             self.base_url = 'resttest.afas.online'
         else:
             self.base_url = 'rest.afas.online'
         credentials = self.get_system_credential(system='profit', label=label, test_environment=test_environment)
         self.environment = credentials['environment']
         base64token = base64.b64encode(credentials['token'].encode('utf-8')).decode()
-        self.headers = {'Authorization': 'AfasToken ' + base64token}
+        self.headers = {'Authorization': 'AfasToken ' + base64token,
+                        'IntegrationId': '38092_135680'}
         self.debug = debug
 
     def update(self, updateconnector, data) -> requests.Response:
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, updateconnector)
 
         update = requests.request("PUT", url, data=data, headers=self.headers)
 
@@ -1962,15 +1963,15 @@
         if self.debug:
             print(json.dumps(payload))
 
         update = requests.post(url, data=json.dumps(payload), headers=self.headers)
 
         return update
 
-    def upload_dossieritem(self, data: dict, attachments: Union[dict, None] = None, overload_fields: list = None) -> requests.Response:
+    def upload_dossieritem(self, data: dict, attachments: Union[list[dict], None] = None, overload_fields: list = None) -> requests.Response:
         """
         :param data: any fields that are in required and allowed_fields
         :param attachments: list of dicts that should each contain a filename and attachment_filepath
         :param overload_fields: list of dicts that should each contain a complete object for a free dossieritem. Example:
         [{
             "KnS15": {
                 "Element": {
@@ -1990,15 +1991,15 @@
             'date_created': 'Da',
             'created_by': 'UsId',
             'person_responsible': 'EmId',
             'is_done': 'St',
             'property_1': 'FvF1',
             'property_2': 'FvF2',
             'property_3': 'FvF3',
-            'save_file_with_subject': 'FileTrans',
+            'save_file_with_subject': 'FileTrans'
         }
         allowed_fields_subject_link = {
             'sales_administration_id': "SiUn",
             'sales_invoice_type_id': "SiTp",
             'sales_invoice_id': "SiId",
             'purchase_administration_id': "PiUn",
             'purchase_invoice_type_id': "PiTp",
@@ -2045,15 +2046,15 @@
                     "Objects": [
                         {
                             "KnSubjectLink": {
                                 "Element": {
                                     # "@SbId": id, # optional dossieritem ID
                                     "Fields": {
                                         "ToEm": data['to_employee'] if 'to_employee' in data else 2,
-                                        "SfId": data['destination'] if 'destination' in data else data['employee_id'],
+                                        "SfId": data['destination'],
                                         "SfTp": data['destination_id'] if 'destination_id' in data else 2
                                     }
                                 }
                             }
                         }
                     ]
                 }
```

### Comparing `salure_helpers_profit-1.2.4/setup.py` & `salure_helpers_profit-1.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='1.2.4',
+    version='1.3.0',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
         'salure-helpers-salureconnect>=1',
         'salure-helpers-salure-functions>=0',
         'aiohttp>=3,<=4',
         'pandas>=1,<=1.35',
-        'requests>=2,<=3'
+        'requests>=2,<=3',
+        'tenacity>=8,<9',
     ],
     zip_safe=False,
 )
```


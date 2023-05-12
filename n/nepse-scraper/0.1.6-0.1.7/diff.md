# Comparing `tmp/nepse_scraper-0.1.6.tar.gz` & `tmp/nepse_scraper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepse_scraper-0.1.6.tar", last modified: Thu May 11 02:05:59 2023, max compression
+gzip compressed data, was "nepse_scraper-0.1.7.tar", last modified: Fri May 12 02:18:44 2023, max compression
```

## Comparing `nepse_scraper-0.1.6.tar` & `nepse_scraper-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 02:05:59.391182 nepse_scraper-0.1.6/
--rw-rw-rw-   0        0        0     1085 2023-05-03 09:07:21.000000 nepse_scraper-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2879 2023-05-11 02:05:59.391182 nepse_scraper-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2203 2023-05-10 16:47:44.000000 nepse_scraper-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 02:05:59.357246 nepse_scraper-0.1.6/nepse_scraper/
--rw-rw-rw-   0        0        0    25906 2023-05-11 01:51:35.000000 nepse_scraper-0.1.6/nepse_scraper/Scraper.py
--rw-rw-rw-   0        0        0       50 2023-05-10 16:47:44.000000 nepse_scraper-0.1.6/nepse_scraper/__init__.py
--rw-rw-rw-   0        0        0     1717 2023-05-03 11:26:30.000000 nepse_scraper-0.1.6/nepse_scraper/apis.py
--rw-rw-rw-   0        0        0     5032 2023-05-01 16:07:59.000000 nepse_scraper-0.1.6/nepse_scraper/nepse.wasm
-drwxrwxrwx   0        0        0        0 2023-05-11 02:05:59.389182 nepse_scraper-0.1.6/nepse_scraper.egg-info/
--rw-rw-rw-   0        0        0     2879 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-11 02:05:59.393608 nepse_scraper-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-05-11 02:04:25.000000 nepse_scraper-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:18:44.549617 nepse_scraper-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2023-05-12 02:14:44.000000 nepse_scraper-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3106 2023-05-12 02:18:44.549617 nepse_scraper-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2415 2023-05-12 02:12:32.000000 nepse_scraper-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 02:18:44.504817 nepse_scraper-0.1.7/nepse_scraper/
+-rw-rw-rw-   0        0        0    25847 2023-05-12 02:13:43.000000 nepse_scraper-0.1.7/nepse_scraper/Scraper.py
+-rw-rw-rw-   0        0        0       49 2023-05-12 02:12:32.000000 nepse_scraper-0.1.7/nepse_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-05-03 11:26:30.000000 nepse_scraper-0.1.7/nepse_scraper/apis.py
+-rw-rw-rw-   0        0        0     5032 2023-05-01 16:07:59.000000 nepse_scraper-0.1.7/nepse_scraper/nepse.wasm
+drwxrwxrwx   0        0        0        0 2023-05-12 02:18:44.547129 nepse_scraper-0.1.7/nepse_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3106 2023-05-12 02:18:44.000000 nepse_scraper-0.1.7/nepse_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-12 02:18:44.000000 nepse_scraper-0.1.7/nepse_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 02:18:44.000000 nepse_scraper-0.1.7/nepse_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-12 02:18:44.000000 nepse_scraper-0.1.7/nepse_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 02:18:44.000000 nepse_scraper-0.1.7/nepse_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-12 02:18:44.551880 nepse_scraper-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2023-05-12 02:17:34.000000 nepse_scraper-0.1.7/setup.py
```

### Comparing `nepse_scraper-0.1.6/LICENSE.txt` & `nepse_scraper-0.1.7/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 MIT License
 
 Copyright (c) 2023 Shrawan Sunar
 
-Permission is hereby granted, free of charge, to any person obtaining a copy\of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy\of 
+this software and associated documentation files (the "Software"), to deal in the 
+Software without restriction, including without limitation the rights to use, copy, 
+modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
```

### Comparing `nepse_scraper-0.1.6/PKG-INFO` & `nepse_scraper-0.1.7/nepse_scraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
-Name: nepse_scraper
-Version: 0.1.6
+Name: nepse-scraper
+Version: 0.1.7
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.6.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.7.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
-Keywords: python,nepse data,nepse scraper
+Keywords: python,nepse data,nepse scraper,nepse,scraping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Nepse scraper
 > Python module that provides convenient access to the Nepal Stock Exchange (NEPSE) API, enabling developers and analysts to retrieve stock market data and improve investment decisions.
 
+> If you're looking for more detailed documentation on how to use my project called "nepse_scraper," I would recommend checking out the project's GitHub page at [https://github.com/polymorphisma/nepse_scraper/].
+
 # Table of content
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
   - [Using Pip](#using-pip)
 - [Usage](#usage)
 - [Documentation](/docs/index.md)
@@ -61,18 +63,18 @@
 ```
 pip install nepse-scraper
 ```
 
 
 ## Usage
 ```py
-from nepse_scraper import Request_module
+from nepse_scraper import Nepse_scraper
 
-# create object from Request_module class
-request_obj = Request_module()
+# create object from Nepse_scraper class
+request_obj = Nepse_scraper()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
 
 # "Please refer to the documentation for more detailed usage instructions."
 ```
```

### Comparing `nepse_scraper-0.1.6/README.md` & `nepse_scraper-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Nepse scraper
 > Python module that provides convenient access to the Nepal Stock Exchange (NEPSE) API, enabling developers and analysts to retrieve stock market data and improve investment decisions.
 
+> If you're looking for more detailed documentation on how to use my project called "nepse_scraper," I would recommend checking out the project's GitHub page at [https://github.com/polymorphisma/nepse_scraper/].
+
 # Table of content
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
   - [Using Pip](#using-pip)
 - [Usage](#usage)
 - [Documentation](/docs/index.md)
@@ -44,18 +46,18 @@
 ```
 pip install nepse-scraper
 ```
 
 
 ## Usage
 ```py
-from nepse_scraper import Request_module
+from nepse_scraper import Nepse_scraper
 
-# create object from Request_module class
-request_obj = Request_module()
+# create object from Nepse_scraper class
+request_obj = Nepse_scraper()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
 
 # "Please refer to the documentation for more detailed usage instructions."
 ```
```

### Comparing `nepse_scraper-0.1.6/nepse_scraper/Scraper.py` & `nepse_scraper-0.1.7/nepse_scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         return [self.token_parser.parse_token_response(token_response)[0], token_response]
     
     def return_data(self, url, access_token, method='GET', which_payload=None,  querystring = None, payload=None):
         return self.request_api(method=method, url = url, access_token = access_token, which_payload=which_payload, querystring=querystring, payload=payload)
 
 from retrying import retry
 
-class Request_module:
+class Nepse_scraper:
     
     SLEEP_TIME = 3000 # -> wait time for every failed request(in milisecond)
 
     def __init__(self) -> None:
         self.nepse_obj = Nepse()
         self.desired_status = 200
 
@@ -206,15 +206,14 @@
     def call_nepse_function(self, url, method,  querystring=None, payload=None):
         try:
             access_token = self.nepse_obj.get_valid_token()
             response = self.nepse_obj.return_data(url, access_token=access_token, method=method, querystring=querystring, payload=payload)
 
             if response.status_code != self.desired_status:
                 raise ValueError('Unexpected status code: {}'.format(response.status_code))
-            # print(response.json())
             return response.json()
         
         except Exception as exp:
             raise ValueError('Unexpected Error: {}'.format(exp))
         
     def is_trading_day(self) -> bool:
         """
@@ -292,15 +291,14 @@
         This method reads the head indices file located at paths.headindices_path and queries the NEPSE API to retrieve
         data. The data is returned as a dictionary containing index as keys and the corresponding index data as values.
 
         Returns:
             dict: A dictionary containing the latest data for each head index, with index as keys and response as a value.
         """
         api = ROOT_URL + api_dict['head_indices_api']['api']
-        print(api)
         method = api_dict['head_indices_api']['method']
 
         querystring = {"page":"0","size":"500"}
 
         dicts = {}
 
         sector_index = self._get_sector_index()
```

### Comparing `nepse_scraper-0.1.6/nepse_scraper/apis.py` & `nepse_scraper-0.1.7/nepse_scraper/apis.py`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.6/nepse_scraper/nepse.wasm` & `nepse_scraper-0.1.7/nepse_scraper/nepse.wasm`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.6/nepse_scraper.egg-info/PKG-INFO` & `nepse_scraper-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
-Name: nepse-scraper
-Version: 0.1.6
+Name: nepse_scraper
+Version: 0.1.7
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.6.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.7.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
-Keywords: python,nepse data,nepse scraper
+Keywords: python,nepse data,nepse scraper,nepse,scraping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Nepse scraper
 > Python module that provides convenient access to the Nepal Stock Exchange (NEPSE) API, enabling developers and analysts to retrieve stock market data and improve investment decisions.
 
+> If you're looking for more detailed documentation on how to use my project called "nepse_scraper," I would recommend checking out the project's GitHub page at [https://github.com/polymorphisma/nepse_scraper/].
+
 # Table of content
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
   - [Using Pip](#using-pip)
 - [Usage](#usage)
 - [Documentation](/docs/index.md)
@@ -61,18 +63,18 @@
 ```
 pip install nepse-scraper
 ```
 
 
 ## Usage
 ```py
-from nepse_scraper import Request_module
+from nepse_scraper import Nepse_scraper
 
-# create object from Request_module class
-request_obj = Request_module()
+# create object from Nepse_scraper class
+request_obj = Nepse_scraper()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
 
 # "Please refer to the documentation for more detailed usage instructions."
 ```
```

### Comparing `nepse_scraper-0.1.6/setup.py` & `nepse_scraper-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path
 
 current_dir = path.abspath(path.dirname(__file__))
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Python Scraper for Nepse'
 
 with open(path.join(current_dir, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
@@ -18,16 +18,16 @@
     package_data={'nepse_scraper': ['*.wasm']},
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url='https://github.com/polymorphisma/nepse_scraper/',  
     install_requires=['requests','urllib3','wasmtime', 'retrying'],
-    keywords=['python', 'nepse data', 'nepse scraper'],
-    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.6.tar.gz",
+    keywords=['python', 'nepse data', 'nepse scraper','nepse', 'scraping'],
+    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.7.tar.gz",
     classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
```


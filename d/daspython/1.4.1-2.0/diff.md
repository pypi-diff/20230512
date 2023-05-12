# Comparing `tmp/daspython-1.4.1.tar.gz` & `tmp/daspython-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daspython-1.4.1.tar", last modified: Wed Mar 29 10:51:08 2023, max compression
+gzip compressed data, was "daspython-2.0.tar", last modified: Fri May 12 15:45:30 2023, max compression
```

## Comparing `daspython-1.4.1.tar` & `daspython-2.0.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.943158 daspython-1.4.1/
--rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     2183 2023-03-29 10:51:08.942139 daspython-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1658 2023-03-29 10:27:14.000000 daspython-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.833754 daspython-1.4.1/daspython/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.875790 daspython-1.4.1/daspython/auth/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/auth/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/auth/authenticate.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.884017 daspython-1.4.1/daspython/common/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/common/__init__.py
--rw-rw-rw-   0        0        0     5566 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/common/api.py
--rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/common/response.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.886223 daspython-1.4.1/daspython/services/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.890884 daspython-1.4.1/daspython/services/alcs/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/alcs/__init__.py
--rw-rw-rw-   0        0        0      500 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/alcs/aclservice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.896219 daspython-1.4.1/daspython/services/attributes/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/attributes/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/attributes/attributeservice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.901345 daspython-1.4.1/daspython/services/digitalobjects/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/digitalobjects/__init__.py
--rw-rw-rw-   0        0        0    11286 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/digitalobjects/digitalobjectservice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.908217 daspython-1.4.1/daspython/services/entries/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/entries/__init__.py
--rw-rw-rw-   0        0        0    17184 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/entries/entryservice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.914217 daspython-1.4.1/daspython/services/entryfields/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/entryfields/__init__.py
--rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/entryfields/entryfieldservice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.918699 daspython-1.4.1/daspython/services/searches/
--rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/searches/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-03-29 09:37:21.000000 daspython-1.4.1/daspython/services/searches/searchservice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.869789 daspython-1.4.1/daspython.egg-info/
--rw-rw-rw-   0        0        0     2183 2023-03-29 10:51:08.000000 daspython-1.4.1/daspython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2023-03-29 10:51:08.000000 daspython-1.4.1/daspython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 10:51:08.000000 daspython-1.4.1/daspython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-03-29 10:51:08.000000 daspython-1.4.1/daspython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-29 10:51:08.000000 daspython-1.4.1/daspython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      842 2023-03-29 10:50:48.000000 daspython-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 10:51:08.944455 daspython-1.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 10:51:08.936422 daspython-1.4.1/tests/
--rw-rw-rw-   0        0        0      935 2023-03-29 09:37:21.000000 daspython-1.4.1/tests/test_aclservice.py
--rw-rw-rw-   0        0        0     1085 2023-03-29 09:37:21.000000 daspython-1.4.1/tests/test_attributeservice.py
--rw-rw-rw-   0        0        0      448 2023-03-29 09:37:21.000000 daspython-1.4.1/tests/test_authenticate.py
--rw-rw-rw-   0        0        0     2017 2023-03-29 09:37:21.000000 daspython-1.4.1/tests/test_digital_object_service.py
--rw-rw-rw-   0        0        0      845 2023-03-29 09:37:21.000000 daspython-1.4.1/tests/test_entry_field_service.py
--rw-rw-rw-   0        0        0     7191 2023-03-29 09:37:21.000000 daspython-1.4.1/tests/test_entry_service.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.687981 daspython-2.0/
+-rw-rw-rw-   0        0        0    35821 2023-03-29 09:37:21.000000 daspython-2.0/LICENSE
+-rw-rw-rw-   0        0        0     2183 2023-05-12 15:45:30.686990 daspython-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-03-29 15:15:01.000000 daspython-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.565903 daspython-2.0/daspython/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.632070 daspython-2.0/daspython/auth/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/auth/__init__.py
+-rw-rw-rw-   0        0        0     1969 2023-05-11 16:36:35.000000 daspython-2.0/daspython/auth/authenticate.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.636084 daspython-2.0/daspython/client/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:25:32.000000 daspython-2.0/daspython/client/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-04-06 09:00:06.000000 daspython-2.0/daspython/client/client.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.640517 daspython-2.0/daspython/common/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/common/__init__.py
+-rw-rw-rw-   0        0        0     5566 2023-05-11 16:05:46.000000 daspython-2.0/daspython/common/api.py
+-rw-rw-rw-   0        0        0      110 2023-03-29 09:37:21.000000 daspython-2.0/daspython/common/response.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.646054 daspython-2.0/daspython/dastypes/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:20:32.000000 daspython-2.0/daspython/dastypes/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-06 08:46:36.000000 daspython-2.0/daspython/dastypes/entry.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.648052 daspython-2.0/daspython/services/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.651060 daspython-2.0/daspython/services/alcs/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/alcs/__init__.py
+-rw-rw-rw-   0        0        0      500 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/alcs/aclservice.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.654205 daspython-2.0/daspython/services/attributes/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/attributes/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/attributes/attributeservice.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.656468 daspython-2.0/daspython/services/digitalobjects/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/digitalobjects/__init__.py
+-rw-rw-rw-   0        0        0    11310 2023-05-12 15:33:43.000000 daspython-2.0/daspython/services/digitalobjects/digitalobjectservice.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.660480 daspython-2.0/daspython/services/entries/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entries/__init__.py
+-rw-rw-rw-   0        0        0    17184 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entries/entryservice.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.666015 daspython-2.0/daspython/services/entryfields/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entryfields/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/entryfields/entryfieldservice.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.669013 daspython-2.0/daspython/services/searches/
+-rw-rw-rw-   0        0        0        0 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/searches/__init__.py
+-rw-rw-rw-   0        0        0     1960 2023-03-29 09:37:21.000000 daspython-2.0/daspython/services/searches/searchservice.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.629565 daspython-2.0/daspython.egg-info/
+-rw-rw-rw-   0        0        0     2183 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 15:45:30.000000 daspython-2.0/daspython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      841 2023-05-12 15:40:43.000000 daspython-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 15:45:30.688981 daspython-2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 15:45:30.684970 daspython-2.0/tests/
+-rw-rw-rw-   0        0        0     1033 2023-05-11 16:51:54.000000 daspython-2.0/tests/test_aclservice.py
+-rw-rw-rw-   0        0        0     1187 2023-05-11 16:47:49.000000 daspython-2.0/tests/test_attributeservice.py
+-rw-rw-rw-   0        0        0      526 2023-05-11 16:47:21.000000 daspython-2.0/tests/test_authenticate.py
+-rw-rw-rw-   0        0        0      700 2023-04-06 09:25:24.000000 daspython-2.0/tests/test_dasclient.py
+-rw-rw-rw-   0        0        0     2489 2023-05-12 15:34:51.000000 daspython-2.0/tests/test_digital_object_service.py
+-rw-rw-rw-   0        0        0      861 2023-05-11 16:47:43.000000 daspython-2.0/tests/test_entry_field_service.py
+-rw-rw-rw-   0        0        0     7078 2023-05-11 16:47:47.000000 daspython-2.0/tests/test_entry_service.py
```

### Comparing `daspython-1.4.1/LICENSE` & `daspython-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daspython-1.4.1/PKG-INFO` & `daspython-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 1.4.1
+Version: 2.0
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to the DAS Python package
 
 The [Royal Netherlands Institute for Sea Research](https://www.nioz.nl) has its data management system to help scientists archive and access their data. This tool is called: **Data Archive System (DAS)** and this package is its Python client.
 
-_*NOTE: This package requires Python 3.8 and plus*_
+_*NOTE: This package requires Python 3.11 and plus*_
 
 # To install using pip
 
 ```
     $ pip install daspython
 ```
```

### Comparing `daspython-1.4.1/README.md` & `daspython-2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Welcome to the DAS Python package
 
 The [Royal Netherlands Institute for Sea Research](https://www.nioz.nl) has its data management system to help scientists archive and access their data. This tool is called: **Data Archive System (DAS)** and this package is its Python client.
 
-_*NOTE: This package requires Python 3.8 and plus*_
+_*NOTE: This package requires Python 3.11 and plus*_
 
 # To install using pip
 
 ```
     $ pip install daspython
 ```
```

### Comparing `daspython-1.4.1/daspython/auth/authenticate.py` & `daspython-2.0/daspython/auth/authenticate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import json
 import requests
-from datetime import datetime
-from daspython.common.api import Token
+from common.api import Token
 
 class DasAuth(Token):
     '''This object represents the authenticator to the DAS API and keeps your token.'''
 
     def __init__(self, base_url, username, password):
         '''
         Parameters
```

### Comparing `daspython-1.4.1/daspython/common/api.py` & `daspython-2.0/daspython/common/api.py`

 * *Files identical despite different names*

### Comparing `daspython-1.4.1/daspython/services/attributes/attributeservice.py` & `daspython-2.0/daspython/services/attributes/attributeservice.py`

 * *Files identical despite different names*

### Comparing `daspython-1.4.1/daspython/services/digitalobjects/digitalobjectservice.py` & `daspython-2.0/daspython/services/digitalobjects/digitalobjectservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from datetime import datetime
 import json
-from json import JSONEncoder
-import re
-from tkinter.messagebox import NO
 import uuid
 import requests
 import os
 from os.path import exists
-from daspython.common import response
-from daspython.common import api
-from daspython.common.api import ApiMethods, Response, Token
+from daspython.common.api import ApiMethods, Token
 from daspython.services.entries.entryservice import EntryService
 from enum import Enum
 
 
 class FileUploadForm():
     description = None
     digitalObjectTypeId = None
@@ -33,15 +28,15 @@
 class AttributeDigitalObjectInput():
     attributeId: int
     attributeValueId: str
     digitalObjectId: str
     isDeleted: bool
 
 
-class UpdateRelationsInput():
+class LinkExistingDigitalObjectInput():
     attributeId: int
     attributeValueId: str
     digitalObjects: list[dict]
 
 CHUNK_SIZE = 1000000
 
 class DownloadRequestItemStatus(Enum):
@@ -98,14 +93,22 @@
     def __read_in_chunks(self, file_object, CHUNK_SIZE):
         while True:
             data = file_object.read(CHUNK_SIZE)
             if not data:
                 break
             yield data
 
+    def upload_to_entry(self, entry_code, file_path, description):           
+        request = UploadDigitalObjectRequest()
+        request.entryCode = entry_code
+        request.filePath = file_path
+        request.description = description
+        self.upload(request)
+        
+
     def upload(self, request: UploadDigitalObjectRequest):
 
         if (request is None or request.entryCode is None or request.filePath is None):
             raise Exception(
                 'Invalid request. Entry Code and file path are required.')
 
         if not exists(request.filePath):
@@ -150,16 +153,14 @@
                 response = json.loads(r.content.decode('utf-8'))
 
                 if response.get('result') is None:
                     continue
 
                 digital_object_id = response.get('result')['id']
 
-                # print(r.json())
-                # print("r: %s, Content-Range: %s" % (r, headers['Content-Range']))
             except Exception as e:
                 print(e)
 
         binary_file.close()
 
         self.__set_digital_object_relation(request.entryCode, digital_object_id)
 
@@ -168,29 +169,29 @@
         entry_service = EntryService(self.token)
 
         response = entry_service.get_entry_by_code(code=entry_code)
 
         if response is None or response.entry is None:
             raise Exception(f'Entry not found with the code: {entry_code}')
 
-        input = UpdateRelationsInput()
+        input = LinkExistingDigitalObjectInput()
 
         input.attributeId = response.attributeId
         input.attributeValueId = response.entry['id']
         attribute_value_digital_object = {
             'attributeId': response.attributeId,
             'attributeValueId': response.entry['id'],
             'digitalObjectId': digital_obj_id,
             'isDeleted': False
         }
         input.digitalObjects = []
         input.digitalObjects.append(attribute_value_digital_object)
 
-        api_url = '/api/services/app/AttributeDigitalObject/UpdateRelations'
-        self.put_data(url=api_url, body=input)
+        api_url = '/api/services/app/DigitalObject/LinkExistingDigitalObject'
+        self.post_data(api_url, input)
 
     def __get_digital_object_type_id(self, digital_object_type: str) -> str:
 
         entry_service = EntryService(self.token)
         response = entry_service.get_entry_by_name(
             name=digital_object_type, attribute_name='Digital Object Type')
```

### Comparing `daspython-1.4.1/daspython/services/entries/entryservice.py` & `daspython-2.0/daspython/services/entries/entryservice.py`

 * *Files identical despite different names*

### Comparing `daspython-1.4.1/daspython/services/entryfields/entryfieldservice.py` & `daspython-2.0/daspython/services/entryfields/entryfieldservice.py`

 * *Files identical despite different names*

### Comparing `daspython-1.4.1/daspython/services/searches/searchservice.py` & `daspython-2.0/daspython/services/searches/searchservice.py`

 * *Files identical despite different names*

### Comparing `daspython-1.4.1/daspython.egg-info/PKG-INFO` & `daspython-2.0/daspython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: daspython
-Version: 1.4.1
+Version: 2.0
 Summary: DAS api client.
 Author: Royal Netherlands Institute for Sea Research
 Project-URL: Homepage, https://git.nioz.nl/ict-projects/das-python
 Project-URL: Bug Tracker, https://git.nioz.nl/ict-projects/das-python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to the DAS Python package
 
 The [Royal Netherlands Institute for Sea Research](https://www.nioz.nl) has its data management system to help scientists archive and access their data. This tool is called: **Data Archive System (DAS)** and this package is its Python client.
 
-_*NOTE: This package requires Python 3.8 and plus*_
+_*NOTE: This package requires Python 3.11 and plus*_
 
 # To install using pip
 
 ```
     $ pip install daspython
 ```
```

### Comparing `daspython-1.4.1/pyproject.toml` & `daspython-2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daspython"
-version = "1.4.1"
+version = "2.0"
 authors = [
   { name="Royal Netherlands Institute for Sea Research" },
 ]
 description = "DAS api client."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
```

### Comparing `daspython-1.4.1/tests/test_aclservice.py` & `daspython-2.0/tests/test_aclservice.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import unittest
-import secrets
+import sys 
+sys.path.insert(0, "C:\Workspace\das-python\daspython")
+import os
+from dotenv import load_dotenv
 from daspython.auth.authenticate import DasAuth
-from daspython.common.api import ApiMethods, Response, Token
+from daspython.common.api import Token
 from daspython.services.alcs.aclservice import AclService, ChangeOwnershipRequest
 
-
 class TestAclService(unittest.TestCase):
 
     def _get_token(self) -> Token:
-        auth = DasAuth(secrets.das_url, secrets.das_username,
-                       secrets.das_password)
-        auth.authenticate(secrets.check_https)
+        load_dotenv()
+        auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
+        auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
         return auth
 
     def test_change_ownership(self):
 
         acl_service = AclService(self._get_token())
 
         payload = ChangeOwnershipRequest()
```

### Comparing `daspython-1.4.1/tests/test_attributeservice.py` & `daspython-2.0/tests/test_attributeservice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+import os
+from dotenv import load_dotenv
 from daspython.services.attributes.attributeservice import AttributeService
-import secrets
 import unittest
 from daspython.auth.authenticate import DasAuth
 from daspython.services.attributes.attributeservice import AttributeService
 
 class TestAttributeService(unittest.TestCase):
 
     def test_get_attribute_name(self):
 
-        auth = DasAuth(secrets.das_url, secrets.das_username, secrets.das_password)
-        auth.authenticate(secrets.check_https)
+        load_dotenv()
+        auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
+        auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
 
         service = AttributeService(auth)        
         result = service.get_attribute_name(55)
 
         self.assertEqual(result, 'Core',f'Expected value is Core but got {result}')
 
     def test_get_attribute_id(self):
 
-        auth = DasAuth(secrets.das_url, secrets.das_username, secrets.das_password)
-        auth.authenticate(secrets.check_https)
+        auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
+        auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
 
         service = AttributeService(auth)        
         result = service.get_attribute_id('Core')
         
         self.assertEqual(result, 55,f'Expected value is 55 but got {result}')
```

### Comparing `daspython-1.4.1/tests/test_digital_object_service.py` & `daspython-2.0/tests/test_digital_object_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import unittest
-import secrets
-
+import sys 
+sys.path.insert(0, "C:\Workspace\das-python\daspython")
+import os
+from dotenv import load_dotenv
 from daspython.common.api import Token
 from daspython.auth.authenticate import DasAuth
 from daspython.services.digitalobjects.digitalobjectservice import DigitalObjectService, UploadDigitalObjectRequest
 
-
 class TestDigitalObjectService(unittest.TestCase):
     
     def _get_token(self) -> Token:
-        auth = DasAuth(secrets.das_url, secrets.das_username,
-                       secrets.das_password)
-        auth.authenticate(secrets.check_https)
+        load_dotenv()
+        auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
+        auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
         return auth
 
     def test_upload_digital_object(self):
 
         digital_object_service = DigitalObjectService(self._get_token())
 
         request = UploadDigitalObjectRequest()
         request.entryCode = 'zb.b.9w'
         request.filePath = 'C:\\Temp\\TEST-01.txt'
         request.description = 'Uploaded from Python'
         digital_object_service.upload(request)
 
+    def test_simplified_upload_digital_object(self):
+        digital_object_service = DigitalObjectService(self._get_token())        
+        digital_object_service.upload_to_entry('zb.b.9w', 'C:\\Temp\\TEST-01.txt', 'Uploaded from Python')
+        digital_object_service.upload_to_entry('zb.b.9w', 'C:\\Temp\\TEST-02.txt', 'Uploaded from Python')
+
     def test_link_existing(self):
          digital_object_service = DigitalObjectService(self._get_token())
          digital_object_service.link_existing(self.ENTRY_CODE,'h.b.wq3c')
 
     def test_download_request(self):
         digital_object_service = DigitalObjectService(self._get_token())
         digital_object_service.download_request('zb.b.tw')
```

### Comparing `daspython-1.4.1/tests/test_entry_field_service.py` & `daspython-2.0/tests/test_entry_field_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import secrets
+import os
 import unittest
-
-from requests.api import request
+from dotenv import load_dotenv
 from daspython.common.api import Token
 from daspython.auth.authenticate import DasAuth
 from daspython.services.entryfields.entryfieldservice import EntryFieldService, DisplayType
 
 
 class TestEntryService(unittest.TestCase):
     def _get_token(self) -> Token:
-        auth = DasAuth(secrets.das_url, secrets.das_username,
-                       secrets.das_password)
-        auth.authenticate(secrets.check_https)
+        load_dotenv()
+        auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
+        auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
         return auth
 
     def test_getall(self):
 
        service = EntryFieldService(self._get_token())       
        response = service.get_all(55, DisplayType.FORM)
        self.assertGreater(response.total, 0, f'EntryFieldService - Get All function should return totalCount greater than 0.')
```

### Comparing `daspython-1.4.1/tests/test_entry_service.py` & `daspython-2.0/tests/test_entry_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-import csv
-import json
-from os import read
+import os
 from os.path import exists
-import secrets
 import unittest
 import random
 from pathlib import Path
+from dotenv import load_dotenv
 
-from requests import get
 from daspython.common.api import Token
 from daspython.auth.authenticate import DasAuth
 from daspython.services.searches.searchservice import SearchEntriesRequest, SearchService
 from daspython.services.entries.entryservice import EntryService, GetAllEntriesRequest, GetEntryRequest, InsertRequest, UpdateRequest
-from daspython.services.entryfields.entryfieldservice import DisplayType, EntryFieldService
 
 
 class TestEntryService(unittest.TestCase):
 
     def _get_token(self) -> Token:
-        auth = DasAuth(secrets.das_url, secrets.das_username,
-                       secrets.das_password)
-        auth.authenticate(secrets.check_https)
+        load_dotenv()
+        auth = DasAuth(os.getenv("DAS_URL"), os.getenv("DAS_USERNAME"), os.getenv("DAS_PASSWORD"))
+        auth.authenticate(bool(os.getenv("CHECK_HTTPS")))
         return auth
 
     def test_getall(self):
 
         service = EntryService(self._get_token())
         request = GetAllEntriesRequest()
         request.attributeid = 55
```


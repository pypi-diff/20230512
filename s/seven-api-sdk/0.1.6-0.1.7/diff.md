# Comparing `tmp/seven_api_sdk-0.1.6.tar.gz` & `tmp/seven_api_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven_api_sdk-0.1.6.tar", max compression
+gzip compressed data, was "seven_api_sdk-0.1.7.tar", max compression
```

## Comparing `seven_api_sdk-0.1.6.tar` & `seven_api_sdk-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1147 2023-03-13 16:31:16.646178 seven_api_sdk-0.1.6/README.md
--rw-r--r--   0        0        0      448 2023-03-13 18:25:11.227045 seven_api_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 16:31:16.647859 seven_api_sdk-0.1.6/seven_api_sdk/.DS_Store
--rw-r--r--   0        0        0     7864 2023-03-13 18:25:11.221159 seven_api_sdk-0.1.6/seven_api_sdk/__init__.py
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 seven_api_sdk-0.1.6/setup.py
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 seven_api_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-03-13 16:31:16.646178 seven_api_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0      448 2023-05-12 08:47:36.641096 seven_api_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 16:31:16.647859 seven_api_sdk-0.1.7/seven_api_sdk/.DS_Store
+-rw-r--r--   0        0        0     7882 2023-05-12 08:44:20.279024 seven_api_sdk-0.1.7/seven_api_sdk/__init__.py
+-rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 seven_api_sdk-0.1.7/setup.py
+-rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 seven_api_sdk-0.1.7/PKG-INFO
```

### Comparing `seven_api_sdk-0.1.6/README.md` & `seven_api_sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `seven_api_sdk-0.1.6/seven_api_sdk/.DS_Store` & `seven_api_sdk-0.1.7/seven_api_sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `seven_api_sdk-0.1.6/seven_api_sdk/__init__.py` & `seven_api_sdk-0.1.7/seven_api_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         if self.parameter is None:
             r = requests.get(self.api_url, headers=headers, timeout=20)
         else:
             payload = {"reqParam": self.parameter}
             r = requests.get(self.api_url, headers=headers, params=payload, timeout=20)
            
         response = {"status_code": r.status_code}
+        r.close()
         if response["status_code"] != 200:
             print("Something went wrong with the call")
             return response
         else:
             print("Successful call")
             response["content"] = json.loads(r.text)
```

### Comparing `seven_api_sdk-0.1.6/setup.py` & `seven_api_sdk-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.24,<2.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'seven-api-sdk',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'A package for end users to use the API endpoints of SEVEN with ease.',
     'long_description': '# SEVEN API endpoint package\n\nThis package was meant to help the end users to utilise the API endpoints of Seven. \nIn the current verison you can use the following endpoints:\n\n- Store Fields\n- Store Data\n- Process Fields\n- Process Data\n- Costs\n- Reports\n\nEach of these categories are represented by a class. You can initiate a class instance and use the .call_api() method to get a response.\n\n## Installation\n\nYou can use your package manager to install from PyPI.\n\nIf you are using pip:\n```\npython3 -m pip install seven-api-sdk\n```\n\n## Examples\n\n```\nimport seven_api_sdk\nimport json\n\npassword = "YOUR_SECRET_PASSWORD"\nusername = "YOUR_USERNAME"\nclient_id = "YOUR_CLIENT_ID"\nclient_name = "YOUR_TENANT_NAME"\n\n\nhandler = seven_api_sdk.StoreFields(username=username,password=password,client_id=client_id,client_name=client_name)\ndata = handler.call_api()\n\nprint (json.dumps(data,indent=4))\n\n#You can specify parameters for certain endpoints\nhandler = seven_api_sdk.ProcessData(username=username,password=password,client_id=client_id,client_name=client_name,parameter="proc_by_storeID")\ndata = handler.call_api()\nprint (json.dumps(data,indent=4))\n```',
     'author': 'Daniel Molnar',
     'author_email': 'daniel@prjct8.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `seven_api_sdk-0.1.6/PKG-INFO` & `seven_api_sdk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven-api-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for end users to use the API endpoints of SEVEN with ease.
 License: MIT
 Author: Daniel Molnar
 Author-email: daniel@prjct8.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


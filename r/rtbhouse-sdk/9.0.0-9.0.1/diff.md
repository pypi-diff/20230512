# Comparing `tmp/rtbhouse-sdk-9.0.0.tar.gz` & `tmp/rtbhouse_sdk-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtbhouse-sdk-9.0.0.tar", max compression
+gzip compressed data, was "rtbhouse_sdk-9.0.1.tar", max compression
```

## Comparing `rtbhouse-sdk-9.0.0.tar` & `rtbhouse_sdk-9.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2022-05-13 09:14:44.002759 rtbhouse-sdk-9.0.0/LICENSE
--rw-r--r--   0        0        0     1671 2022-07-11 15:00:18.522241 rtbhouse-sdk-9.0.0/pyproject.toml
--rw-r--r--   0        0        0       50 2022-07-11 15:00:00.138383 rtbhouse-sdk-9.0.0/rtbhouse_sdk/__init__.py
--rw-r--r--   0        0        0    18803 2022-07-11 15:00:16.726255 rtbhouse-sdk-9.0.0/rtbhouse_sdk/client.py
--rw-r--r--   0        0        0     1854 2022-07-11 15:00:17.634248 rtbhouse-sdk-9.0.0/rtbhouse_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2022-07-11 15:00:00.138383 rtbhouse-sdk-9.0.0/rtbhouse_sdk/py.typed
--rw-r--r--   0        0        0     5234 2022-07-11 15:00:18.966237 rtbhouse-sdk-9.0.0/rtbhouse_sdk/schema.py
--rw-r--r--   0        0        0      718 2022-07-11 15:06:21.873365 rtbhouse-sdk-9.0.0/setup.py
--rw-r--r--   0        0        0      988 2022-07-11 15:06:21.873570 rtbhouse-sdk-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2020-12-22 13:56:17.803191 rtbhouse_sdk-9.0.1/LICENSE
+-rw-r--r--   0        0        0     2123 2022-11-24 12:54:58.846969 rtbhouse_sdk-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2022-07-15 09:00:16.635938 rtbhouse_sdk-9.0.1/rtbhouse_sdk/__init__.py
+-rw-r--r--   0        0        0    18776 2022-11-24 12:54:58.847458 rtbhouse_sdk-9.0.1/rtbhouse_sdk/client.py
+-rw-r--r--   0        0        0     1854 2022-07-15 09:00:16.636428 rtbhouse_sdk-9.0.1/rtbhouse_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2022-07-15 09:00:16.636492 rtbhouse_sdk-9.0.1/rtbhouse_sdk/py.typed
+-rw-r--r--   0        0        0     5234 2022-07-15 09:00:16.636763 rtbhouse_sdk-9.0.1/rtbhouse_sdk/schema.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 rtbhouse_sdk-9.0.1/setup.py
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 rtbhouse_sdk-9.0.1/PKG-INFO
```

### Comparing `rtbhouse-sdk-9.0.0/LICENSE` & `rtbhouse_sdk-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtbhouse-sdk-9.0.0/rtbhouse_sdk/client.py` & `rtbhouse_sdk-9.0.1/rtbhouse_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,15 @@
         request_params = {
             "limit": MAX_CURSOR_ROWS,
         }
         request_params.update(params or {})
 
         while True:
             resp_data = self._get_dict(path, params=request_params)
-            for row in resp_data["rows"]:
-                yield row
+            yield from resp_data["rows"]
             next_cursor = resp_data["nextCursor"]
             if next_cursor is None:
                 break
             request_params["nextCursor"] = next_cursor
 
     def get_user_info(self) -> schema.UserInfo:
         data = self._get_dict("/user/info")
```

### Comparing `rtbhouse-sdk-9.0.0/rtbhouse_sdk/exceptions.py` & `rtbhouse_sdk-9.0.1/rtbhouse_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rtbhouse-sdk-9.0.0/rtbhouse_sdk/schema.py` & `rtbhouse_sdk-9.0.1/rtbhouse_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `rtbhouse-sdk-9.0.0/setup.py` & `rtbhouse_sdk-9.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['rtbhouse_sdk']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.23.0,<0.24.0', 'inflection>=0.5.1,<0.6.0', 'pydantic>=1.9.0,<2.0.0']
+['httpx==0.23.0', 'inflection>=0.5.1,<0.6.0', 'pydantic>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'rtbhouse-sdk',
-    'version': '9.0.0',
+    'version': '9.0.1',
     'description': 'RTB House SDK',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'RTB House Apps Team',
     'author_email': 'apps@rtbhouse.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/rtbhouse-apps/rtbhouse-python-sdk',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7.2,<4.0',
 }
```

### Comparing `rtbhouse-sdk-9.0.0/PKG-INFO` & `rtbhouse_sdk-9.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: rtbhouse-sdk
-Version: 9.0.0
+Version: 9.0.1
 Summary: RTB House SDK
 Home-page: https://github.com/rtbhouse-apps/rtbhouse-python-sdk
 License: BSD License
 Author: RTB House Apps Team
 Author-email: apps@rtbhouse.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: httpx (==0.23.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Project-URL: Repository, https://github.com/rtbhouse-apps/rtbhouse-python-sdk
```


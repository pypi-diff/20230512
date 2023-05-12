# Comparing `tmp/apicase-0.1.9.tar.gz` & `tmp/apicase-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicase-0.1.9.tar", max compression
+gzip compressed data, was "apicase-0.2.0.tar", max compression
```

## Comparing `apicase-0.1.9.tar` & `apicase-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1066 2023-01-14 09:49:43.568358 apicase-0.1.9/LICENSE
--rw-r--r--   0        0        0      703 2023-04-01 15:39:38.930000 apicase-0.1.9/apicase/__init__.py
--rw-r--r--   0        0        0      164 2023-02-25 19:05:42.436000 apicase-0.1.9/apicase/applications.py
--rw-r--r--   0        0        0        0 2023-01-29 12:17:33.442000 apicase-0.1.9/apicase/assertion/__init__.py
--rw-r--r--   0        0        0     1569 2023-03-05 10:18:32.213000 apicase-0.1.9/apicase/assertion/assertion.py
--rw-r--r--   0        0        0     5069 2023-04-01 15:53:19.196000 apicase-0.1.9/apicase/assertion/comparators.py
--rw-r--r--   0        0        0     2607 2023-04-01 15:39:38.928000 apicase-0.1.9/apicase/assertion/diff.py
--rw-r--r--   0        0        0     3084 2023-03-27 17:29:54.681000 apicase-0.1.9/apicase/assertion.py
--rw-r--r--   0        0        0      616 2023-01-08 15:50:22.623000 apicase-0.1.9/apicase/case.py
--rw-r--r--   0        0        0        0 2023-01-08 14:44:14.542000 apicase-0.1.9/apicase/client/__init__.py
--rw-r--r--   0        0        0     5059 2023-04-05 14:34:47.249409 apicase-0.1.9/apicase/client/response.py
--rw-r--r--   0        0        0    13834 2023-04-05 14:24:50.637664 apicase-0.1.9/apicase/client/reuquest.py
--rw-r--r--   0        0        0     4193 2023-02-26 09:07:26.243000 apicase-0.1.9/apicase/client/router.py
--rw-r--r--   0        0        0        0 2023-01-08 17:58:52.563000 apicase-0.1.9/apicase/common/__init__.py
--rw-r--r--   0        0        0      366 2023-01-29 12:09:59.112000 apicase-0.1.9/apicase/common/enumeration.py
--rw-r--r--   0        0        0       48 2023-01-08 18:07:57.260000 apicase-0.1.9/apicase/common/exception.py
--rw-r--r--   0        0        0      170 2023-02-25 19:09:16.150000 apicase-0.1.9/apicase/common/logger.py
--rw-r--r--   0        0        0     1386 2023-01-29 16:04:23.267000 apicase-0.1.9/apicase/common/schema.py
--rw-r--r--   0        0        0        0 2023-01-29 06:56:51.870000 apicase-0.1.9/apicase/report/__init__.py
--rw-r--r--   0        0        0     4954 2023-03-28 17:32:32.614000 apicase-0.1.9/apicase/report/attach.py
--rw-r--r--   0        0        0      335 2023-01-29 09:37:13.411000 apicase-0.1.9/apicase/report/html/__init__.py
--rw-r--r--   0        0        0     1011 2023-01-31 15:50:48.157000 apicase-0.1.9/apicase/report/html/gen_report.py
--rw-r--r--   0        0        0     4767 2023-01-31 16:11:40.141000 apicase-0.1.9/apicase/report/html/template.html
--rw-r--r--   0        0        0     2478 2023-01-29 18:10:36.629000 apicase-0.1.9/apicase/report/html/test.html
--rw-r--r--   0        0        0     2590 2023-01-08 15:50:22.625000 apicase-0.1.9/apicase/report.py
--rw-r--r--   0        0        0     2123 2023-01-16 17:06:49.195000 apicase-0.1.9/apicase/schema.py
--rw-r--r--   0        0        0     2308 2023-01-08 18:36:55.201000 apicase-0.1.9/apicase/script/cli.py
--rw-r--r--   0        0        0     1720 2023-03-27 17:33:20.227000 apicase-0.1.9/apicase/script/file.py
--rw-r--r--   0        0        0     1559 2023-02-05 10:18:30.617000 apicase-0.1.9/apicase/setting.py
--rw-r--r--   0        0        0      670 2023-04-05 14:34:54.831941 apicase-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1137 2023-04-05 14:35:25.783814 apicase-0.1.9/setup.py
--rw-r--r--   0        0        0      757 2023-04-05 14:35:25.783994 apicase-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-14 09:49:43.568358 apicase-0.2.0/LICENSE
+-rw-r--r--   0        0        0      703 2023-04-01 15:39:38.930000 apicase-0.2.0/apicase/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-25 19:05:42.436000 apicase-0.2.0/apicase/applications.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:17:33.442000 apicase-0.2.0/apicase/assertion/__init__.py
+-rw-r--r--   0        0        0     1569 2023-03-05 10:18:32.213000 apicase-0.2.0/apicase/assertion/assertion.py
+-rw-r--r--   0        0        0     5069 2023-04-01 15:53:19.196000 apicase-0.2.0/apicase/assertion/comparators.py
+-rw-r--r--   0        0        0     2607 2023-04-01 15:39:38.928000 apicase-0.2.0/apicase/assertion/diff.py
+-rw-r--r--   0        0        0     3084 2023-03-27 17:29:54.681000 apicase-0.2.0/apicase/assertion.py
+-rw-r--r--   0        0        0      616 2023-01-08 15:50:22.623000 apicase-0.2.0/apicase/case.py
+-rw-r--r--   0        0        0        0 2023-01-08 14:44:14.542000 apicase-0.2.0/apicase/client/__init__.py
+-rw-r--r--   0        0        0     5059 2023-04-05 14:34:47.249000 apicase-0.2.0/apicase/client/response.py
+-rw-r--r--   0        0        0    14546 2023-05-12 03:48:44.219000 apicase-0.2.0/apicase/client/reuquest.py
+-rw-r--r--   0        0        0     4193 2023-02-26 09:07:26.243000 apicase-0.2.0/apicase/client/router.py
+-rw-r--r--   0        0        0        0 2023-01-08 17:58:52.563000 apicase-0.2.0/apicase/common/__init__.py
+-rw-r--r--   0        0        0      366 2023-01-29 12:09:59.112000 apicase-0.2.0/apicase/common/enumeration.py
+-rw-r--r--   0        0        0       48 2023-01-08 18:07:57.260000 apicase-0.2.0/apicase/common/exception.py
+-rw-r--r--   0        0        0      170 2023-02-25 19:09:16.150000 apicase-0.2.0/apicase/common/logger.py
+-rw-r--r--   0        0        0     1386 2023-01-29 16:04:23.267000 apicase-0.2.0/apicase/common/schema.py
+-rw-r--r--   0        0        0        0 2023-01-29 06:56:51.870000 apicase-0.2.0/apicase/report/__init__.py
+-rw-r--r--   0        0        0     5079 2023-05-11 18:02:22.069000 apicase-0.2.0/apicase/report/attach.py
+-rw-r--r--   0        0        0      335 2023-01-29 09:37:13.411000 apicase-0.2.0/apicase/report/html/__init__.py
+-rw-r--r--   0        0        0     1011 2023-01-31 15:50:48.157000 apicase-0.2.0/apicase/report/html/gen_report.py
+-rw-r--r--   0        0        0     4767 2023-01-31 16:11:40.141000 apicase-0.2.0/apicase/report/html/template.html
+-rw-r--r--   0        0        0     2478 2023-01-29 18:10:36.629000 apicase-0.2.0/apicase/report/html/test.html
+-rw-r--r--   0        0        0     2590 2023-01-08 15:50:22.625000 apicase-0.2.0/apicase/report.py
+-rw-r--r--   0        0        0     2123 2023-01-16 17:06:49.195000 apicase-0.2.0/apicase/schema.py
+-rw-r--r--   0        0        0     2308 2023-01-08 18:36:55.201000 apicase-0.2.0/apicase/script/cli.py
+-rw-r--r--   0        0        0     1720 2023-03-27 17:33:20.227000 apicase-0.2.0/apicase/script/file.py
+-rw-r--r--   0        0        0     1559 2023-02-05 10:18:30.617000 apicase-0.2.0/apicase/setting.py
+-rw-r--r--   0        0        0      670 2023-05-12 08:37:26.637076 apicase-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1137 2023-05-12 08:40:05.579684 apicase-0.2.0/setup.py
+-rw-r--r--   0        0        0      757 2023-05-12 08:40:05.579841 apicase-0.2.0/PKG-INFO
```

### Comparing `apicase-0.1.9/LICENSE` & `apicase-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/__init__.py` & `apicase-0.2.0/apicase/__init__.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/assertion/assertion.py` & `apicase-0.2.0/apicase/assertion/assertion.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/assertion/comparators.py` & `apicase-0.2.0/apicase/assertion/comparators.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/assertion/diff.py` & `apicase-0.2.0/apicase/assertion/diff.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/assertion.py` & `apicase-0.2.0/apicase/assertion.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/case.py` & `apicase-0.2.0/apicase/case.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/client/response.py` & `apicase-0.2.0/apicase/client/response.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/client/reuquest.py` & `apicase-0.2.0/apicase/client/reuquest.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 urllib3.disable_warnings()
 
 from abc import ABC, abstractmethod
 import requests
 
 from typing import Callable, List, Dict, Any
 
+from enum import Enum
+
+
+class EnumEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, Enum):
+            return obj.value
+
 
 class HttpSession(requests.Session):
     """
     HttpSession
     """
     http_timeout: int = 60,
     http_allow_redirects = False,
@@ -128,89 +136,100 @@
         if not files:
             files = {}
         self.request.query_params = query_params
         self.request.path_params = path_params
         self.request.files = files
         self.request.data = data
 
+        # 本次执行数据
+        execution_default_json_asserter_list = self.default_json_asserter_list
+        execution_default_json_extraction = self.default_json_extraction
+        execution_default_custom_asserter_list = []
+
         if not is_default_json_extraction:
             # 不执行默认json提取
-            self.default_json_extraction = ''
+            execution_default_json_extraction = ''
         if default_json_asserter_list:
             # 替换默认断言列表
-            self.default_json_asserter_list = default_json_asserter_list
+            execution_default_json_asserter_list = default_json_asserter_list
         if not is_default_json_asserter:
-            # 不执行默认断言，情况列表
-            self.default_json_asserter_list = []
+            # 不执行默认断言，断言列表
+            # self.default_json_asserter_list = []
+            execution_default_json_asserter_list = []
         if default_custom_asserter_list:
             # 替换断言器列表
-            self.default_custom_asserter_list = default_custom_asserter_list
+            # self.default_custom_asserter_list = default_custom_asserter_list
+            execution_default_custom_asserter_list = default_custom_asserter_list
 
         if schema:
             self.request.data = schema.dict()
 
         self.set_content_type()
-        if self.pre:
-            self.request = self.execution_processor(self.pre, self.request)
 
         request_session = session
         if http_session:
             """
             使用自定义http_session
             """
             request_session = http_session
+
+        if self.pre:
+            self.request = self.execution_processor(self.pre, self.request, request_session)
+
         response = request_session.request(
             method=self.request.method,
             url=self.request.url,
             params=self.request.query_params,
             data=self.request.data,
             files=self.request.files,
             headers=self.request.headers,
             cookies=self.request.cookies,
             # timeout=self.request.timeout,
             # verify=False,  # 不认证证书
         )
         self.response = response
         if self.after:
-            self.response = self.execution_processor(self.after, self.response)
+            self.response = self.execution_processor(self.after, self.response, request_session)
 
         return APIResponse(self.response,
-                           default_json_extraction=self.default_json_extraction,
-                           default_json_asserter_list=self.default_json_asserter_list,
+                           default_json_extraction=execution_default_json_extraction,
+                           default_json_asserter_list=execution_default_json_asserter_list,
                            json_asserter_list=json_asserter_list,
-                           default_custom_asserter_list=self.default_custom_asserter_list,
+                           default_custom_asserter_list=execution_default_custom_asserter_list,
                            custom_asserter_list=custom_asserter_list,
                            description=self.request.description,
                            path=self.path
                            )
 
     @staticmethod
-    def execution_processor(exec_list: list, parameter):
+    def execution_processor(exec_list: list, parameter, request_session):
         """
         前后置处理器，函数列表
+        :param request_session:
         :param exec_list:
         :param parameter:
         :return:
         """
         for i in exec_list:
-            parameter = i(parameter)
+            parameter = i(parameter, request_session)
         return parameter
 
     def set_content_type(self):
         """
         根据不同的请求体类型设置请求头，
         json进行编码处理，request中文编码有问题
         :return:
         """
         body_type = self.request.body_type
         content_type = None
         if body_type:
             if body_type == BodyTypeEnum.JSON:
                 content_type = 'application/json'
-                self.request.data = json.dumps(self.request.data, ensure_ascii=False)
+                print(self.request.data)
+                self.request.data = json.dumps(self.request.data, ensure_ascii=False, cls=EnumEncoder)
                 self.request.data = self.request.data.encode('utf-8')
             elif body_type == BodyTypeEnum.TEXT:
                 content_type = 'text/plain'
             elif body_type == BodyTypeEnum.XML:
                 content_type = 'application/xml'
             elif body_type == BodyTypeEnum.FORM_URLENCODED:
                 content_type = 'application/x-www-form-urlencoded'
```

### Comparing `apicase-0.1.9/apicase/client/router.py` & `apicase-0.2.0/apicase/client/router.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/common/schema.py` & `apicase-0.2.0/apicase/common/schema.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/report/attach.py` & `apicase-0.2.0/apicase/report/attach.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
             k = i.copy()
             k.comparator = k.comparator.__name__
             k = k.dict()
             k['check'] = k['check'].value
             validate_extractor.append(k)
         title_name = "Request.{0}: {1} {2}".format(response.request.method, path, description)
         content_size = int(dict(response.headers).get("content-length") or 0)
+        if isinstance(response.request.body, bytes):
+            response.request.body = str(response.request.body, 'utf-8')
         summary = {
             'name': description,
             'path': response.request.url,
             'request': {
                 'url': response.request.url,
                 'headers': cls.headers_format(response.request.headers),
                 'body': response.request.body
```

### Comparing `apicase-0.1.9/apicase/report/html/gen_report.py` & `apicase-0.2.0/apicase/report/html/gen_report.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/report/html/template.html` & `apicase-0.2.0/apicase/report/html/template.html`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/report/html/test.html` & `apicase-0.2.0/apicase/report/html/test.html`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/report.py` & `apicase-0.2.0/apicase/report.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/schema.py` & `apicase-0.2.0/apicase/schema.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/script/cli.py` & `apicase-0.2.0/apicase/script/cli.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/script/file.py` & `apicase-0.2.0/apicase/script/file.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/apicase/setting.py` & `apicase-0.2.0/apicase/setting.py`

 * *Files identical despite different names*

### Comparing `apicase-0.1.9/pyproject.toml` & `apicase-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apicase"
-version = "0.1.9"
+version = "0.2.0"
 description = ""
 authors = ["guowenhe <18538570410@163.com>"]
 
 [tool.poetry.scripts]
 apicase = "apicase.script.cli:main"
 
 [tool.poetry.dependencies]
```

### Comparing `apicase-0.1.9/setup.py` & `apicase-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['apicase = apicase.script.cli:main']}
 
 setup_kwargs = {
     'name': 'apicase',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': '',
     'long_description': None,
     'author': 'guowenhe',
     'author_email': '18538570410@163.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `apicase-0.1.9/PKG-INFO` & `apicase-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicase
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: guowenhe
 Author-email: 18538570410@163.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
```


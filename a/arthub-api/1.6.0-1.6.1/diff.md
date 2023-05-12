# Comparing `tmp/arthub_api-1.6.0.tar.gz` & `tmp/arthub_api-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.0.tar", last modified: Wed May 10 04:30:10 2023, max compression
+gzip compressed data, was "arthub_api-1.6.1.tar", last modified: Fri May 12 03:07:27 2023, max compression
```

## Comparing `arthub_api-1.6.0.tar` & `arthub_api-1.6.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 04:30:10.863194 arthub_api-1.6.0/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-10 04:30:10.862196 arthub_api-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-10 04:20:06.000000 arthub_api-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 04:30:10.812388 arthub_api-1.6.0/arthub_api/
--rw-rw-rw-   0        0        0      507 2023-05-06 12:14:27.000000 arthub_api-1.6.0/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     2267 2023-02-08 16:32:42.000000 arthub_api-1.6.0/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-10 04:29:36.000000 arthub_api-1.6.0/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-02-08 16:32:42.000000 arthub_api-1.6.0/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       35 2023-02-08 16:32:42.000000 arthub_api-1.6.0/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.0/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    27698 2023-05-10 03:20:14.000000 arthub_api-1.6.0/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.0/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.0/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.0/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.0/arthub_api/models.py
--rw-rw-rw-   0        0        0    40620 2023-05-10 04:07:11.000000 arthub_api-1.6.0/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.0/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8099 2023-05-06 11:55:01.000000 arthub_api-1.6.0/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:30:10.821306 arthub_api-1.6.0/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-10 04:30:10.000000 arthub_api-1.6.0/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2023-05-10 04:30:10.000000 arthub_api-1.6.0/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 04:30:10.000000 arthub_api-1.6.0/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-10 04:30:10.000000 arthub_api-1.6.0/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.0/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-05-10 04:30:10.000000 arthub_api-1.6.0/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-10 04:30:10.000000 arthub_api-1.6.0/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 04:30:10.863194 arthub_api-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2930 2023-02-08 12:46:33.000000 arthub_api-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:30:10.850272 arthub_api-1.6.0/tests/
--rw-rw-rw-   0        0        0      136 2023-05-06 11:54:55.000000 arthub_api-1.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0      371 2023-05-06 11:54:55.000000 arthub_api-1.6.0/tests/_utils.py
--rw-rw-rw-   0        0        0      280 2023-05-06 11:54:55.000000 arthub_api-1.6.0/tests/conftest.py
--rw-rw-rw-   0        0        0     6110 2023-05-06 11:55:01.000000 arthub_api-1.6.0/tests/test_open_api.py
--rw-rw-rw-   0        0        0    12826 2023-05-10 04:16:54.000000 arthub_api-1.6.0/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3647 2023-05-06 11:54:55.000000 arthub_api-1.6.0/tests/test_storage.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.645915 arthub_api-1.6.1/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-12 03:07:27.644918 arthub_api-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.625466 arthub_api-1.6.1/arthub_api/
+-rw-rw-rw-   0        0        0      607 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     2316 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      233 2023-05-12 03:06:06.000000 arthub_api-1.6.1/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.1/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.1/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    37291 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.1/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.1/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.1/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.1/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.1/arthub_api/models.py
+-rw-rw-rw-   0        0        0    41051 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.1/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.1/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.634757 arthub_api-1.6.1/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.1/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       65 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-12 03:07:27.000000 arthub_api-1.6.1/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 03:07:27.645915 arthub_api-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:07:27.643921 arthub_api-1.6.1/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.1/tests/_utils.py
+-rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    15230 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.1/tests/test_storage.py
+-rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.1/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.0/LICENSE` & `arthub_api-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/PKG-INFO` & `arthub_api-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.0
+Version: 1.6.1
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.0/README.md` & `arthub_api-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/__main__.py` & `arthub_api-1.6.1/arthub_api/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     mod = {
         "__file__": file_path,
     }
 
     try:
         with open(file_path) as file_obj:
-            exec (compile(file_obj.read(), file_obj.name, "exec"), mod)
+            exec(compile(file_obj.read(), file_obj.name, "exec"), mod)
     except IOError:
         raise
 
     except Exception:
         raise UserError("Better double-check your user config.")
 
     for key in dir(arthub_api_config):
@@ -67,16 +67,20 @@
     # to stdout
     s_handler = logging.StreamHandler()
     s_handler.setLevel(logging.DEBUG)
     s_handler.setFormatter(logging.Formatter("%(message)s"))
     logger.addHandler(s_handler)
 
 
-def init_cli():
+def init_config():
     setup_logging()
     patch_config()
     load_config()
 
 
 def main():
-    init_cli()
+    init_config()
     cli.cli()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `arthub_api-1.6.0/arthub_api/_internal_utils.py` & `arthub_api-1.6.1/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/asset_matrix.py` & `arthub_api-1.6.1/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/config.py` & `arthub_api-1.6.1/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/exception.py` & `arthub_api-1.6.1/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/models.py` & `arthub_api-1.6.1/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/open_api.py` & `arthub_api-1.6.1/arthub_api/open_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 import requests
 from . import utils
 from . import models
 from . import _internal_utils
 from . import exception
 from xml.etree import ElementTree
+from . import arthub_api_config
 
 
 def _node_query_metas(simplified_meta=True):
     metas = [
         "name",
         "file_format",
         "node_type",
@@ -257,19 +258,23 @@
 
     @property
     def config(self):
         return self._config
 
     @property
     def api_host(self):
-        return self.config["host"]
+        if self.config:
+            return self.config["host"]
+        return ""
 
     @property
     def http_scheme(self):
-        return self.config["http_scheme"]
+        if self.config:
+            return self.config["http_scheme"]
+        return ""
 
     @staticmethod
     def get_node_permission_group(node_brief):
         p = node_brief.get("permission_mask")
         if p is None:
             raise exception.Error(value="node brief does not contain field \"permission_mask\"")
         permission_group = []
@@ -288,28 +293,35 @@
         return permission_group
 
     def clear_token(self):
         self._token = ""
         self._public_token = ""
 
     def clear_token_cache(self):
-        utils.remove_token_cache_file(self.api_host)
+        name = self.api_host
+        if name == "":
+            return
+        utils.remove_token_cache_file(name)
 
     def logout(self):
         self.clear_token()
         self.clear_token_cache()
 
     def get_token_from_cache(self):
-        token = utils.get_token_from_cache(self.api_host)
+        name = self.api_host
+        if name == "":
+            return
+        token = utils.get_token_from_cache(name)
         if token:
             self._token = token
 
     def save_token_to_cache(self):
-        if self._token:
-            utils.save_token_to_cache(self._token, self.api_host)
+        name = self.api_host
+        if self._token and name != "":
+            utils.save_token_to_cache(self._token, name)
 
     @property
     def token(self):
         return self._token
 
     def set_token(self, token, save_to_cache=True):
         r"""Set arthub token which is used to call api
@@ -337,14 +349,20 @@
         """
 
         if type(cookie) is str:
             self._cookies = utils.parse_cookies(cookie)
         elif type(cookie) is dict:
             self._cookies = cookie
 
+    def reset_config(self, config):
+        self._config = config
+
+    def init_from_config(self):
+        self.reset_config(utils.get_config_by_name(arthub_api_config.api_config_name, self.config))
+
     def _depot_url(self, asset_hub, api_method):
         return "%s//%s/%s/data/openapi/%s/core/%s" % (
             self.http_scheme, self.api_host, asset_hub, self._api_version_depot, api_method)
 
     def _gateway_url(self, api_method):
         return "%s//%s/gateway/gateway/openapi/%s/core/%s" % (
             self.http_scheme, self.api_host, self._api_version_gateway, api_method)
@@ -1117,10 +1135,7 @@
 
         :param asset_hub: str. Example: "trial".
         :rtype: arthub_api.APIResponse
         """
 
         url = self._depot_url(asset_hub, "get-depot-id")
         return self._make_api_request(url)
-
-    def reset_config(self, config):
-        self._config = config
```

### Comparing `arthub_api-1.6.0/arthub_api/storage.py` & `arthub_api-1.6.1/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.0/arthub_api/utils.py` & `arthub_api-1.6.1/arthub_api/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 import shutil
 import time
 import random
 import string
 import requests
 from . import models
 from platformdirs import user_cache_dir
+from .config import (
+    api_config_oa,
+    api_config_qq,
+    api_config_oa_test,
+    api_config_qq_test
+)
 
 
 def _path_preprocess(path):
     path = path.strip()
     path = path.rstrip("\\/")
     return path
 
@@ -61,41 +67,44 @@
 
 
 def get_random_string(length):
     return ''.join(random.sample(string.ascii_letters + string.digits, length))
 
 
 class UploadFilePartReader(object):
-    def __init__(self, file_, offset, length):
+    def __init__(self, file_, offset, length, callback=None):
         self._file = file_
         self._file.seek(offset)
         self._total_size = length
         self._completed_size = 0
         self._finished = False
+        self._callback = callback
 
     def read(self, size=-1):
         if size == -1:
             self._finished = True
             return ""
         uncompleted_size = self._total_size - self._completed_size
         size_to_read = min(uncompleted_size, size)
         if size_to_read == 0:
             self._finished = True
             return ""
         content = self._file.read(size_to_read)
         self._completed_size += len(content)
+        if self._callback:
+            self._callback(len(content))
         return content
 
 
-def upload_part_of_file(url, file_path, offset, length):
+def upload_part_of_file(url, file_path, offset, length, callback=None):
     try:
         if not os.path.isfile(file_path):
             return models.Result(False, error_message="file \"%s\" not exist" % file_path)
         with open(file_path, 'rb') as file_:
-            res = requests.put(url, data=UploadFilePartReader(file_, offset, length), headers={
+            res = requests.put(url, data=UploadFilePartReader(file_, offset, length, callback), headers={
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate, br",
                 "Connection": "keep-alive",
                 "Content-Type": "application/octet-stream",
                 "Content-Length": str(length)
             })
             if not res.ok:
@@ -104,45 +113,49 @@
     except Exception as e:
         error_message = "send request \"%s\" exception" % url
         logging.error("[UploadFilePart] %s" % error_message)
         return models.Result(False, error_message=error_message)
 
 
 class UploadFileReader(object):
-    def __init__(self, file_):
+    def __init__(self, file_, callback):
         self._file = file_
         self._file.seek(0)
+        self._total_size = os.path.getsize(file_.name)
         self._completed_size = 0
         self._finished = False
+        self._callback = callback
 
     def read(self, size=-1):
         if size == -1:
             self._finished = True
             return ""
         content = self._file.read(size)
         self._completed_size += len(content)
+        if self._callback:
+            self._callback(len(content))
         return content
 
 
-def upload_file(url, file_path):
+def upload_file(url, file_path, callback=None):
     try:
         if not os.path.isfile(file_path):
             return models.Result(False, error_message="file \"%s\" not exist" % file_path)
         with open(file_path, 'rb') as file_:
-            res = requests.put(url, data=UploadFileReader(file_), headers={
+            res = requests.put(url, data=UploadFileReader(file_, callback), headers={
                 "Accept-Encoding": "gzip, deflate, br",
                 "Connection": "keep-alive",
                 "Content-Type": "application/octet-stream",
                 "Content-Length": str(os.path.getsize(file_path))
             })
             if not res.ok:
                 return models.Result(False, error_message="status code: %d" % res.status_code)
             return models.Result(True, data=res)
     except Exception as e:
-        error_message = "send request \"%s\" exception" % url
+        error_message = "send request \"%s\" exception \"%s\"" % (url, str(e))
         logging.error("[UploadFile] %s" % error_message)
         return models.Result(False, error_message=error_message)
 
 
 def download_file(url, file_path):
     try:
         if os.path.exists(file_path):
@@ -273,7 +286,22 @@
     except Exception:
         logging.warning("[TokenCache] save token to file \"%s\" error: %s",
                         token_file, str(e))
 
 
 def remove_token_cache_file(api_host):
     remove(get_token_cache_file(api_host))
+
+
+def get_config_by_name(env, default_config=None):
+    _env_map = {
+        "oa": api_config_oa,
+        "qq": api_config_qq,
+        "oa_test": api_config_oa_test,
+        "qq_test": api_config_qq_test,
+    }
+    c = _env_map.get(env)
+    if not c:
+        if default_config:
+            return default_config
+        return api_config_oa
+    return c
```

### Comparing `arthub_api-1.6.0/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.1/arthub_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.0
+Version: 1.6.1
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.0/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.1/arthub_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 arthub_api/__init__.py
 arthub_api/__main__.py
 arthub_api/__version__.py
 arthub_api/_internal_utils.py
 arthub_api/arthub_api_config.py
 arthub_api/asset_matrix.py
 arthub_api/blade_api.py
+arthub_api/blade_storage.py
 arthub_api/cli.py
 arthub_api/config.py
 arthub_api/exception.py
 arthub_api/models.py
 arthub_api/open_api.py
 arthub_api/storage.py
 arthub_api/utils.py
@@ -25,8 +26,9 @@
 arthub_api.egg-info/requires.txt
 arthub_api.egg-info/top_level.txt
 tests/__init__.py
 tests/_utils.py
 tests/conftest.py
 tests/test_open_api.py
 tests/test_open_api_blade.py
-tests/test_storage.py
+tests/test_storage.py
+tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.0/setup.py` & `arthub_api-1.6.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,103 @@
-#!/usr/bin/env python
-import os
-import sys
-from codecs import open
-
-from setuptools import setup, find_packages
-from setuptools.command.test import test as TestCommand
-
-
-# CURRENT_PYTHON = sys.version_info[:2]
-# REQUIRED_PYTHON = (3, 7)
-
-# if CURRENT_PYTHON < REQUIRED_PYTHON:
-#     sys.stderr.write("""
-# ==========================
-# Unsupported Python version
-# ==========================
-# This version of arthub_api requires at least Python {}.{}, but
-# you're trying to install it on Python {}.{}. To resolve this,
-# consider upgrading to a supported Python version.
-# """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
-#     sys.exit(1)
-
-
-class PyTest(TestCommand):
-    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
-
-    def initialize_options(self):
-        TestCommand.initialize_options(self)
-        try:
-            from multiprocessing import cpu_count
-
-            self.pytest_args = ["-n", str(cpu_count()), "--boxed"]
-        except (ImportError, NotImplementedError):
-            self.pytest_args = ["-n", "1", "--boxed"]
-
-    def finalize_options(self):
-        TestCommand.finalize_options(self)
-        self.test_args = []
-        self.test_suite = True
-
-    def run_tests(self):
-        import pytest
-
-        errno = pytest.main(self.pytest_args)
-        sys.exit(errno)
-
-
-# 'setup.py publish' shortcut.
-if sys.argv[-1] == "publish":
-    os.system("python setup.py sdist bdist_wheel")
-    os.system("twine upload dist/*")
-    sys.exit()
-
-requires = [
-    "requests",
-    "platformdirs==2.0.2"
-]
-
-test_requirements = [
-    "pytest",
-]
-
-about = {}
-here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, "arthub_api", "__version__.py"), "r",
-          "utf-8") as f:
-    exec(f.read(), about)
-
-with open("README.md", "r", "utf-8") as f:
-    readme = f.read()
-
-setup(name=about["__title__"],
-      version=about["__version__"],
-      description=about["__description__"],
-      long_description=readme,
-      long_description_content_type="text/markdown",
-      author=about["__author__"],
-      author_email=about["__author_email__"],
-      url=about["__url__"],
-      package_dir={'arthub_api': 'arthub_api'},
-      packages=['arthub_api'],
-      package_data={"": ["LICENSE", "NOTICE"]},
-      include_package_data=True,
-      install_requires=requires,
-      license=about["__license__"],
-      zip_safe=False,
-      classifiers=[
-          "Development Status :: 5 - Production/Stable",
-          "Environment :: Web Environment",
-          "Intended Audience :: Developers",
-          "Natural Language :: English",
-          "Operating System :: OS Independent"],
-      cmdclass={"test": PyTest},
-      tests_require=test_requirements,
-      entry_points={
-          "console_scripts": [
-              "aha = arthub_api.__main__:main",
-          ]
-      })
+#!/usr/bin/env python
+import os
+import sys
+from codecs import open
+
+from setuptools import setup, find_packages
+from setuptools.command.test import test as TestCommand
+
+
+# CURRENT_PYTHON = sys.version_info[:2]
+# REQUIRED_PYTHON = (3, 7)
+
+# if CURRENT_PYTHON < REQUIRED_PYTHON:
+#     sys.stderr.write("""
+# ==========================
+# Unsupported Python version
+# ==========================
+# This version of arthub_api requires at least Python {}.{}, but
+# you're trying to install it on Python {}.{}. To resolve this,
+# consider upgrading to a supported Python version.
+# """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
+#     sys.exit(1)
+
+
+class PyTest(TestCommand):
+    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
+
+    def initialize_options(self):
+        TestCommand.initialize_options(self)
+        try:
+            from multiprocessing import cpu_count
+
+            self.pytest_args = ["-n", str(cpu_count()), "--boxed"]
+        except (ImportError, NotImplementedError):
+            self.pytest_args = ["-n", "1", "--boxed"]
+
+    def finalize_options(self):
+        TestCommand.finalize_options(self)
+        self.test_args = []
+        self.test_suite = True
+
+    def run_tests(self):
+        import pytest
+
+        errno = pytest.main(self.pytest_args)
+        sys.exit(errno)
+
+
+# 'setup.py publish' shortcut.
+if sys.argv[-1] == "publish":
+    os.system("python setup.py sdist bdist_wheel")
+    os.system("twine upload dist/*")
+    sys.exit()
+
+requires = [
+    "requests",
+    "platformdirs==2.0.2"
+]
+
+test_requirements = [
+    "pytest",
+]
+
+about = {}
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, "arthub_api", "__version__.py"), "r",
+          "utf-8") as f:
+    exec(f.read(), about)
+
+with open("README.md", "r", "utf-8") as f:
+    readme = f.read()
+
+setup(name=about["__title__"],
+      version=about["__version__"],
+      description=about["__description__"],
+      long_description=readme,
+      long_description_content_type="text/markdown",
+      author=about["__author__"],
+      author_email=about["__author_email__"],
+      url=about["__url__"],
+      package_dir={'arthub_api': 'arthub_api'},
+      packages=['arthub_api'],
+      package_data={"": ["LICENSE", "NOTICE"]},
+      include_package_data=True,
+      install_requires=requires,
+      license=about["__license__"],
+      zip_safe=False,
+      classifiers=[
+          "Development Status :: 5 - Production/Stable",
+          "Environment :: Web Environment",
+          "Intended Audience :: Developers",
+          "Natural Language :: English",
+          "Operating System :: OS Independent"],
+      cmdclass={"test": PyTest},
+      tests_require=test_requirements,
+      entry_points={
+          "console_scripts": [
+              "aha = arthub_api.__main__:main",
+          ]
+      },
+      extras_require={
+        ':python_version == "2.7"': ['futures']
+    })
```

### Comparing `arthub_api-1.6.0/tests/test_open_api.py` & `arthub_api-1.6.1/tests/test_open_api.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-import arthub_api
-import pytest
-import logging
-from arthub_api import arthub_api_config
-from . import _utils
-from arthub_api import (
-    OpenAPI,
-    utils
-)
-
-TEST_DEPOT_NAME = "apg"
-
-open_api = None
-
-
-def on_api_failed(res):
-    logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
-
-
-@pytest.mark.run(order=1)
-def test_init(env):
-    global open_api
-    _c = _utils.get_config(env)
-    open_api = OpenAPI(_c, False)
-    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        pytest.exit("login failed, exit test", returncode=1)
-
-    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
-
-
-def test_depot_get_root_id():
-    res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
-
-
-def test_depot_get_node_brief_by_ids():
-    res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node_1 = res.results.get(0)
-    node_2 = res.results.get(1)
-    logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
-
-
-def test_depot_get_child_node_count():
-    res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
-
-
-def test_depot_get_download_signature():
-    res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
-                                                nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
-
-
-def test_depot_get_upload_signature():
-    file_name = "new_asset_to_upload"
-    res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": file_name,
-        "add_new_version": False
-    }])
-    if not res_0.is_succeeded():
-        on_api_failed(res_0)
-        assert 0
-
-    asset_id = res_0.results.get(0)["id"]
-
-    res_1 = open_api.depot_get_upload_signature(TEST_DEPOT_NAME, nodes=[
-        {"object_id": asset_id, "object_meta": "origin_url", "file_name": file_name}])
-    if not res_1.is_succeeded():
-        on_api_failed(res_1)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
-
-
-def test_depot_get_child_node_id_in_range():
-    res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
-                                                    query_filters=[{"meta": "type", "condition": "x != directory"}],
-                                                    is_recursive=True)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    nodes = res.results.get(0)["nodes"]
-    logging.info("[TEST][API] \"%s\" success" % res.url)
-
-
-def test_depot_get_node_brief_by_path():
-    res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296,
-                                                path="open_api_test/asset.jpg")
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
-
-
-def test_depot_add_asset_tag():
-    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[utils.get_random_string(5)])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
-
-
-def test_get_account_detail():
-    res = open_api.get_account_detail()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
-
-
-def test_get_ticket():
-    res = open_api.get_ticket()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
-
-
-def test_get_last_access_location_by_account():
-    res = open_api.get_last_access_location_by_account()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
-
-
-def test_depot_create_directory():
-    res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": "new_dir",
-        "allowed_rename": True,
-        "return_existing_id": False
-    }])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
-
-
-def test_depot_create_multi_asset():
-    res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": "new_multi_asset"
-    }])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
-
-
-def test_depot_move_node():
-    res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success" % res.url)
+import arthub_api
+import pytest
+import logging
+from arthub_api import arthub_api_config
+from . import _utils
+from arthub_api import (
+    OpenAPI,
+    utils
+)
+
+TEST_DEPOT_NAME = "apg"
+
+open_api = None
+
+
+def on_api_failed(res):
+    logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
+
+
+@pytest.mark.run(order=1)
+def test_init(env):
+    global open_api
+    _c = _utils.get_config(env)
+    open_api = OpenAPI(_c, False)
+    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        pytest.exit("login failed, exit test", returncode=1)
+
+    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
+
+
+def test_depot_get_root_id():
+    res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
+
+
+def test_depot_get_node_brief_by_ids():
+    res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node_1 = res.results.get(0)
+    node_2 = res.results.get(1)
+    logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
+
+
+def test_depot_get_child_node_count():
+    res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
+
+
+def test_depot_get_download_signature():
+    res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
+                                                nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
+
+
+def test_depot_get_upload_signature():
+    file_name = "new_asset_to_upload"
+    res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": file_name,
+        "add_new_version": False
+    }])
+    if not res_0.is_succeeded():
+        on_api_failed(res_0)
+        assert 0
+
+    asset_id = res_0.results.get(0)["id"]
+
+    res_1 = open_api.depot_get_upload_signature(TEST_DEPOT_NAME, nodes=[
+        {"object_id": asset_id, "object_meta": "origin_url", "file_name": file_name}])
+    if not res_1.is_succeeded():
+        on_api_failed(res_1)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
+
+
+def test_depot_get_child_node_id_in_range():
+    res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
+                                                    query_filters=[{"meta": "type", "condition": "x != directory"}],
+                                                    is_recursive=True)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    nodes = res.results.get(0)["nodes"]
+    logging.info("[TEST][API] \"%s\" success" % res.url)
+
+
+def test_depot_get_node_brief_by_path():
+    res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296,
+                                                path="open_api_test/asset.jpg")
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
+
+
+def test_depot_add_asset_tag():
+    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[utils.get_random_string(5)])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
+
+
+def test_get_account_detail():
+    res = open_api.get_account_detail()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
+
+
+def test_get_ticket():
+    res = open_api.get_ticket()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
+
+
+def test_get_last_access_location_by_account():
+    res = open_api.get_last_access_location_by_account()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
+
+
+def test_depot_create_directory():
+    res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": "new_dir",
+        "allowed_rename": True,
+        "return_existing_id": False
+    }])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
+
+
+def test_depot_create_multi_asset():
+    res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": "new_multi_asset"
+    }])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
+
+
+def test_depot_move_node():
+    res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success" % res.url)
```

### Comparing `arthub_api-1.6.0/tests/test_open_api_blade.py` & `arthub_api-1.6.1/tests/test_open_api_blade.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,414 +1,515 @@
-import arthub_api
-import pytest
-import logging
-from arthub_api import arthub_api_config
-from . import _utils
-from arthub_api import (
-    BladeAPI,
-)
-
-
-def on_api_failed(res):
-    logging.error("[TEST][API][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
-
-
-def init_api(env, login=True):
-    api = BladeAPI(_utils.get_config(env), False)
-    if login:
-        res = api.login(arthub_api_config.account_email, arthub_api_config.password)
-        assert res.is_succeeded()
-    return api
-
-
-def get_current_role_id(env):
-    blade_api = init_api(env)
-    res = blade_api.get_account_detail()
-    assert res.is_succeeded()
-    return res.result["id"]
-
-
-def get_account_role_id(env, account_name):
-    blade_api = init_api(env)
-    res = blade_api.get_account_detail([account_name])
-    assert res.is_succeeded()
-    return res.result["id"]
-
-
-def get_root_id(env):
-    blade_api = init_api(env)
-    res = blade_api.blade_get_root_id()
-    assert res.is_succeeded()
-    return res.result
-
-
-def get_node(env, node_id, parent_id):
-    blade_api = init_api(env)
-    res = blade_api.blade_get_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
-    assert res.is_succeeded()
-    return res.first_result()
-
-
-def delete_node(env, node_id, parent_id):
-    blade_api = init_api(env)
-    res = blade_api.blade_delete_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
-    assert res.is_succeeded()
-    return res.first_result()
-
-
-def test_blade_type_option_info(env):
-    blade_api = init_api(env)
-    res = blade_api.blade_get_type_option_info()
-    if not res.is_succeeded() or type(res.result) != list:
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, current types length: %d" % (res.url, len(res.result)))
-
-
-def test_blade_toolbox(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    # create
-    toolbox_payload = {
-        "parent_id": root_id,
-        "name": "sdk_test_name",
-        "description": "toolbox for sdk test",
-        "short_name": "sdk_test_short_name",
-    }
-    res = blade_api.blade_create_toolbox(toolbox_payload)
-    assert res.is_succeeded()
-    toolbox_id = res.result
-
-    # get
-    node_brief = get_node(env, toolbox_id, root_id)
-    assert toolbox_payload["name"] == node_brief["name"]
-
-    # update
-    update_payload = {
-        "id": toolbox_id,
-        "name": "sdk_test_name",
-        "description": "toolbox for sdk test",
-        "short_name": "sdk_test_short_name",
-    }
-    res = blade_api.blade_update_toolbox(update_payload)
-    assert res.is_succeeded()
-
-    # get
-    node_brief = get_node(env, toolbox_id, root_id)
-    assert update_payload["name"] == node_brief["name"]
-    assert update_payload["description"] == node_brief["description"]
-    assert update_payload["short_name"] == node_brief["short_name"]
-
-    # delete
-    delete_node(env, toolbox_id, root_id)
-
-
-def test_blade_tool(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    # create first toolbox
-    toolbox_payload = {
-        "parent_id": root_id,
-        "name": "test_dir",
-        "short_name": "sdk_test_short_name",
-    }
-    res = blade_api.blade_create_toolbox(toolbox_payload)
-    assert res.is_succeeded()
-    toolbox_id_1 = res.result
-
-    # create tool
-    tool_payload = {
-        "parent_id": toolbox_id_1,
-        "name": "sdk_test_name",
-        "flag_color": "red",
-        "flag_content": "2020",
-    }
-    res = blade_api.blade_create_tool(tool_payload)
-    assert res.is_succeeded()
-    tool_id = res.result
-
-    # get
-    node_brief = get_node(env, tool_id, toolbox_id_1)
-    assert tool_payload["name"] == node_brief["name"]
-    assert node_brief["is_hard_link"]
-
-    # update
-    update_payload = {
-        "id": tool_id,
-        "name": "sdk_test_name_2",
-        "description": "tool for sdk test 2",
-        "command": "test command 2",
-        "command_type": "cmd",
-        "type_option": 2,
-        "flag_color": "blue",
-        "flag_content": "2022",
-    }
-    res = blade_api.blade_update_tool(update_payload)
-    assert res.is_succeeded()
-
-    # get
-    node_brief = get_node(env, tool_id, toolbox_id_1)
-    assert update_payload["name"] == node_brief["name"]
-    assert update_payload["description"] == node_brief["description"]
-    assert update_payload["command"] == node_brief["command"]
-    assert update_payload["command_type"] == node_brief["command_type"]
-    assert update_payload["type_option"] == node_brief["type_option"]
-    assert update_payload["flag_color"] == node_brief["flag_color"]
-    assert update_payload["flag_content"] == node_brief["flag_content"]
-
-    # test share
-    # create second toolbox
-    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "dir_to_move"})
-    assert res.is_succeeded()
-    toolbox_id_2 = res.result
-    # share
-    res = blade_api.blade_share_tool([tool_id], toolbox_id_1, toolbox_id_2)
-    assert res.is_succeeded()
-
-    # test get child
-    res = blade_api.blade_get_child_node_count(toolbox_id_2)
-    assert res.is_succeeded()
-    assert res.result == 1
-    res = blade_api.blade_get_child_node_brief_in_range(toolbox_id_2)
-    assert res.is_succeeded()
-    assert res.result[0]["is_hard_link"] is False
-
-    # delete toolbox
-    delete_node(env, toolbox_id_1, root_id)
-    delete_node(env, toolbox_id_2, root_id)
-
-
-def test_edit_user(env):
-    blade_api = init_api(env)
-    qywx_alias = "bytian"
-
-    # create origin
-    account_id = get_account_role_id(env, qywx_alias)
-    # delete
-    res = blade_api.blade_delete_user_by_id(account_id)
-    assert res.is_succeeded()
-
-    # create
-    res = blade_api.blade_create_user({
-        "qywxalias": qywx_alias,
-        "email": "12345@qq.com",
-        "fullname": "tian",
-        "position": "dev",
-    })
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-    user_id = res.result
-
-    # update
-    res = blade_api.blade_update_user_by_id({
-        "id": user_id,
-        "email": "6789@qq.com",
-        "fullname": "tian2",
-        "position": "art",
-    })
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_user_by_id(user_id)
-    assert res.is_succeeded()
-    user_info = res.result
-    res = blade_api.blade_get_user_by_qywx_alias(qywx_alias)
-    assert res.is_succeeded()
-    assert user_info == res.result
-    assert user_info["email"] == "6789@qq.com"
-    logging.info("[TEST][API] get user success: %s" % user_info)
-
-    # delete
-    res = blade_api.blade_delete_user_by_id(user_id)
-    assert res.is_succeeded()
-
-
-def test_edit_config(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-    role_id = get_current_role_id(env)
-
-    name = "test_sdk"
-    config = {"env": 1}
-    # create
-    res = blade_api.blade_create_config(name, root_id, "node", config)
-    assert res.is_succeeded()
-
-    # update
-    config_new = {"env_new": 2}
-    res = blade_api.blade_update_config(name, root_id, "node", config_new)
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_config(name, root_id, "node")
-    assert res.is_succeeded()
-    result_config = res.result["config"]
-    logging.info("[TEST][API] get config success: %s" % result_config)
-    assert result_config == config_new
-
-    # create on role
-    config_role = {"env_role": 3}
-    res = blade_api.blade_create_config(name, role_id, "role", config_role)
-    assert res.is_succeeded()
-    res = blade_api.blade_batch_get_config([name], [root_id])
-    logging.info("[TEST][API] batch get config success: %s" % res.result)
-
-    # delete
-    res = blade_api.blade_delete_config(name, root_id, "node")
-    assert res.is_succeeded()
-    res = blade_api.blade_delete_config(name, role_id, "role")
-    assert res.is_succeeded()
-
-
-def test_edit_plugin(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-    role_id = get_current_role_id(env)
-
-    name = "test_sdk"
-    plugin = {
-        "runnable": True,
-        "shellable": False,
-        "short_help": "start test",
-        "packages": [
-            "pkg_1",
-            "pkg_2"
-        ]
-    }
-    # create
-    res = blade_api.blade_create_plugin(name, root_id, "node", plugin)
-    assert res.is_succeeded()
-
-    # update
-    res = blade_api.blade_update_plugin(name, root_id, "node", {
-        "is_packages_change": True,
-        "packages": ["pkg_3"]
-    })
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_plugin(name, root_id, "node")
-    assert res.is_succeeded()
-    logging.info("[TEST][API] get plugin success: %s" % res.result)
-    assert res.result["short_help"] == plugin["short_help"]
-    assert res.result["packages"] == ["pkg_3"]
-
-    # create on role
-    plugin_role = {
-        "runnable": False,
-        "shellable": True,
-        "short_help": "start test on role",
-        "packages": [
-            "pkg_role"
-        ]
-    }
-    res = blade_api.blade_create_plugin(name, role_id, "role", plugin_role)
-    assert res.is_succeeded()
-    res = blade_api.blade_batch_get_plugin([name], [root_id])
-    logging.info("[TEST][API] batch get plugin success: %s" % res.result)
-
-    # delete
-    res = blade_api.blade_delete_config(name, root_id, "node")
-    res = blade_api.blade_delete_config(name, role_id, "role")
-    assert res.is_succeeded()
-
-
-def test_edit_public_token(env):
-    blade_api = init_api(env)
-    # create
-    res = blade_api.blade_create_public_token("sdk_test_token", 10)
-    assert res.is_succeeded()
-    token_id = res.result["id"]
-    token_str = res.result["name"]
-
-    # update
-    res = blade_api.blade_update_public_token_by_id({
-        "id": token_id,
-        "fullname": "sdk_test_token_new",
-        "duration": 100,
-    })
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_public_token_by_id(token_id)
-    assert res.is_succeeded()
-    token_info = res.result
-    res = blade_api.blade_get_public_token_by_name(token_str)
-    assert res.is_succeeded()
-    assert token_info == res.result
-    assert token_info["duration"] == 100
-    logging.info("[TEST][API] get token success: %s" % token_info)
-
-    # delete
-    res = blade_api.blade_delete_public_token_by_id(token_id)
-    assert res.is_succeeded()
-
-
-def test_permission_on_toolbox(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    res = blade_api.blade_create_public_token("sdk_test_token", 100)
-    assert res.is_succeeded()
-    token_id = res.result["id"]
-    token_str = res.result["name"]
-
-    # set public token to toolbox permission
-    # create toolbox
-    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "test_perm_dir"})
-    assert res.is_succeeded()
-    toolbox_id = res.result
-
-    # add
-    perm_item = {"account_name": token_str, "type": "public_token"}
-    res = blade_api.blade_add_permission_on_toolbox_by_account_name(toolbox_id, "developer", [perm_item])
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_permission_on_toolbox(toolbox_id)
-    assert res.is_succeeded()
-    assert res.result["developer"][0] == perm_item
-
-    # delete
-    res = blade_api.blade_delete_permission_on_toolbox_by_account_name(toolbox_id, [perm_item])
-    assert res.is_succeeded()
-
-    # delete toolbox
-    delete_node(env, toolbox_id, root_id)
-
-
-def test_permission_on_config(env):
-    blade_api = init_api(env)
-    root_id = get_root_id(env)
-
-    res = blade_api.blade_create_public_token("sdk_test_token_config", 100)
-    assert res.is_succeeded()
-    token_str = res.result["name"]
-
-    # set public token to config permission
-    # add
-    perm_item = {"account_name": token_str, "type": "public_token"}
-    res = blade_api.blade_add_permission_on_config_by_account_name("developer", [perm_item])
-    assert res.is_succeeded()
-
-    # get
-    res = blade_api.blade_get_permission_on_config()
-    assert res.is_succeeded()
-    assert res.result["developer"][0] == perm_item
-
-    # public token permission test
-    blade_api_token = init_api(env, False)
-    blade_api_token.set_blade_public_token(token_str)
-    res = blade_api_token.blade_list_user()
-    assert res.is_succeeded()
-    res = blade_api_token.blade_create_config("token_test", root_id, "node", {"hello": "world"})
-    assert res.is_succeeded()
-    res = blade_api_token.blade_delete_config("token_test", root_id, "node")
-    assert res.is_succeeded()
-
-    # delete
-    res = blade_api.blade_delete_permission_on_config_by_account_name([perm_item])
-    assert res.is_succeeded()
+import arthub_api
+import pytest
+import logging
+from arthub_api import arthub_api_config
+from . import _utils
+from arthub_api import (
+    BladeAPI,
+)
+
+
+def on_api_failed(res):
+    logging.error("[TEST][API][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
+
+
+def init_api(env, login=True):
+    api = BladeAPI(_utils.get_config(env), False)
+    if login:
+        res = api.login(arthub_api_config.account_email, arthub_api_config.password)
+        assert res.is_succeeded()
+    return api
+
+
+def get_current_role_id(env):
+    blade_api = init_api(env)
+    res = blade_api.get_account_detail()
+    assert res.is_succeeded()
+    return res.result["id"]
+
+
+def get_account_role_id(env, account_name):
+    blade_api = init_api(env)
+    res = blade_api.get_account_detail([account_name])
+    assert res.is_succeeded()
+    return res.result["id"]
+
+
+def get_root_id(env):
+    blade_api = init_api(env)
+    res = blade_api.blade_get_root_id()
+    assert res.is_succeeded()
+    return res.result
+
+
+def get_node(env, node_id, parent_id):
+    blade_api = init_api(env)
+    res = blade_api.blade_get_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
+    assert res.is_succeeded()
+    return res.first_result()
+
+
+def delete_node(env, node_id, parent_id):
+    blade_api = init_api(env)
+    res = blade_api.blade_delete_node_brief_by_id([{"id": node_id, "parent_id": parent_id}])
+    assert res.is_succeeded()
+    return res.first_result()
+
+
+def test_blade_type_option_info(env):
+    blade_api = init_api(env)
+    res = blade_api.blade_get_type_option_info()
+    if not res.is_succeeded() or type(res.result) != list:
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, current types length: %d" % (res.url, len(res.result)))
+
+
+def test_blade_toolbox(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    # create
+    toolbox_payload = {
+        "parent_id": root_id,
+        "name": "sdk_test_name",
+        "description": "toolbox for sdk test",
+        "short_name": "sdk_test_short_name",
+    }
+    res = blade_api.blade_create_toolbox(toolbox_payload)
+    assert res.is_succeeded()
+    toolbox_id = res.result
+
+    # get
+    node_brief = get_node(env, toolbox_id, root_id)
+    assert toolbox_payload["name"] == node_brief["name"]
+
+    # update
+    update_payload = {
+        "id": toolbox_id,
+        "name": "sdk_test_name",
+        "description": "toolbox for sdk test",
+        "short_name": "sdk_test_short_name",
+    }
+    res = blade_api.blade_update_toolbox(update_payload)
+    assert res.is_succeeded()
+
+    # get
+    node_brief = get_node(env, toolbox_id, root_id)
+    assert update_payload["name"] == node_brief["name"]
+    assert update_payload["description"] == node_brief["description"]
+    assert update_payload["short_name"] == node_brief["short_name"]
+
+    # delete
+    delete_node(env, toolbox_id, root_id)
+
+
+def test_blade_tool(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    # create first toolbox
+    toolbox_payload = {
+        "parent_id": root_id,
+        "name": "test_dir",
+        "short_name": "sdk_test_short_name",
+    }
+    res = blade_api.blade_create_toolbox(toolbox_payload)
+    assert res.is_succeeded()
+    toolbox_id_1 = res.result
+
+    # create tool
+    tool_payload = {
+        "parent_id": toolbox_id_1,
+        "name": "sdk_test_name",
+        "flag_color": "red",
+        "flag_content": "2020",
+    }
+    res = blade_api.blade_create_tool(tool_payload)
+    assert res.is_succeeded()
+    tool_id = res.result
+
+    # get
+    node_brief = get_node(env, tool_id, toolbox_id_1)
+    assert tool_payload["name"] == node_brief["name"]
+    assert node_brief["is_hard_link"]
+
+    # update
+    update_payload = {
+        "id": tool_id,
+        "name": "sdk_test_name_2",
+        "description": "tool for sdk test 2",
+        "command": "test command 2",
+        "command_type": "cmd",
+        "type_option": 2,
+        "flag_color": "blue",
+        "flag_content": "2022",
+    }
+    res = blade_api.blade_update_tool(update_payload)
+    assert res.is_succeeded()
+
+    # get
+    node_brief = get_node(env, tool_id, toolbox_id_1)
+    assert update_payload["name"] == node_brief["name"]
+    assert update_payload["description"] == node_brief["description"]
+    assert update_payload["command"] == node_brief["command"]
+    assert update_payload["command_type"] == node_brief["command_type"]
+    assert update_payload["type_option"] == node_brief["type_option"]
+    assert update_payload["flag_color"] == node_brief["flag_color"]
+    assert update_payload["flag_content"] == node_brief["flag_content"]
+
+    # test share
+    # create second toolbox
+    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "dir_to_move"})
+    assert res.is_succeeded()
+    toolbox_id_2 = res.result
+    # share
+    res = blade_api.blade_share_tool([tool_id], toolbox_id_1, toolbox_id_2)
+    assert res.is_succeeded()
+
+    # test get child
+    res = blade_api.blade_get_child_node_count(toolbox_id_2)
+    assert res.is_succeeded()
+    assert res.result == 1
+    res = blade_api.blade_get_child_node_brief_in_range(toolbox_id_2)
+    assert res.is_succeeded()
+    assert res.result[0]["is_hard_link"] is False
+
+    # delete toolbox
+    delete_node(env, toolbox_id_1, root_id)
+    delete_node(env, toolbox_id_2, root_id)
+
+
+def test_edit_user(env):
+    blade_api = init_api(env)
+    qywx_alias = "bytian"
+
+    # create origin
+    account_id = get_account_role_id(env, qywx_alias)
+    # delete
+    res = blade_api.blade_delete_user_by_id(account_id)
+    assert res.is_succeeded()
+
+    # create
+    res = blade_api.blade_create_user({
+        "qywxalias": qywx_alias,
+        "email": "12345@qq.com",
+        "fullname": "tian",
+        "position": "dev",
+    })
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+    user_id = res.result
+
+    # update
+    res = blade_api.blade_update_user_by_id({
+        "id": user_id,
+        "email": "6789@qq.com",
+        "fullname": "tian2",
+        "position": "art",
+    })
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_user_by_id(user_id)
+    assert res.is_succeeded()
+    user_info = res.result
+    res = blade_api.blade_get_user_by_qywx_alias(qywx_alias)
+    assert res.is_succeeded()
+    assert user_info == res.result
+    assert user_info["email"] == "6789@qq.com"
+    logging.info("[TEST][API] get user success: %s" % user_info)
+
+    # delete
+    res = blade_api.blade_delete_user_by_id(user_id)
+    assert res.is_succeeded()
+
+
+def test_edit_config(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+    role_id = get_current_role_id(env)
+
+    name = "test_sdk"
+    config = {"env": 1}
+    # create
+    res = blade_api.blade_create_config(name, root_id, "node", config)
+    assert res.is_succeeded()
+
+    # update
+    config_new = {"env_new": 2}
+    res = blade_api.blade_update_config(name, root_id, "node", config_new)
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_config(name, root_id, "node")
+    assert res.is_succeeded()
+    result_config = res.result["config"]
+    logging.info("[TEST][API] get config success: %s" % result_config)
+    assert result_config == config_new
+
+    # create on role
+    config_role = {"env_role": 3}
+    res = blade_api.blade_create_config(name, role_id, "role", config_role)
+    assert res.is_succeeded()
+    res = blade_api.blade_batch_get_config([name], [root_id])
+    logging.info("[TEST][API] batch get config success: %s" % res.result)
+
+    # delete
+    res = blade_api.blade_delete_config(name, root_id, "node")
+    assert res.is_succeeded()
+    res = blade_api.blade_delete_config(name, role_id, "role")
+    assert res.is_succeeded()
+
+
+def test_edit_plugin(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+    role_id = get_current_role_id(env)
+
+    name = "test_sdk"
+    plugin = {
+        "runnable": True,
+        "shellable": False,
+        "short_help": "start test",
+        "packages": [
+            "pkg_1",
+            "pkg_2"
+        ]
+    }
+    # create
+    res = blade_api.blade_create_plugin(name, root_id, "node", plugin)
+    assert res.is_succeeded()
+
+    # update
+    res = blade_api.blade_update_plugin(name, root_id, "node", {
+        "is_packages_change": True,
+        "packages": ["pkg_3"]
+    })
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_plugin(name, root_id, "node")
+    assert res.is_succeeded()
+    logging.info("[TEST][API] get plugin success: %s" % res.result)
+    assert res.result["short_help"] == plugin["short_help"]
+    assert res.result["packages"] == ["pkg_3"]
+
+    # create on role
+    plugin_role = {
+        "runnable": False,
+        "shellable": True,
+        "short_help": "start test on role",
+        "packages": [
+            "pkg_role"
+        ]
+    }
+    res = blade_api.blade_create_plugin(name, role_id, "role", plugin_role)
+    assert res.is_succeeded()
+    res = blade_api.blade_batch_get_plugin([name], [root_id])
+    logging.info("[TEST][API] batch get plugin success: %s" % res.result)
+
+    # delete
+    res = blade_api.blade_delete_config(name, root_id, "node")
+    res = blade_api.blade_delete_config(name, role_id, "role")
+    assert res.is_succeeded()
+
+
+def test_edit_public_token(env):
+    blade_api = init_api(env)
+    # create
+    res = blade_api.blade_create_public_token("sdk_test_token", 10)
+    assert res.is_succeeded()
+    token_id = res.result["id"]
+    token_str = res.result["name"]
+
+    # update
+    res = blade_api.blade_update_public_token_by_id({
+        "id": token_id,
+        "fullname": "sdk_test_token_new",
+        "duration": 100,
+    })
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_public_token_by_id(token_id)
+    assert res.is_succeeded()
+    token_info = res.result
+    res = blade_api.blade_get_public_token_by_name(token_str)
+    assert res.is_succeeded()
+    assert token_info == res.result
+    assert token_info["duration"] == 100
+    logging.info("[TEST][API] get token success: %s" % token_info)
+
+    # delete
+    res = blade_api.blade_delete_public_token_by_id(token_id)
+    assert res.is_succeeded()
+
+
+def test_permission_on_toolbox(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    res = blade_api.blade_create_public_token("sdk_test_token", 100)
+    assert res.is_succeeded()
+    token_id = res.result["id"]
+    token_str = res.result["name"]
+
+    # set public token to toolbox permission
+    # create toolbox
+    res = blade_api.blade_create_toolbox({"parent_id": root_id, "name": "test_perm_dir"})
+    assert res.is_succeeded()
+    toolbox_id = res.result
+
+    # add
+    perm_item = {"account_name": token_str, "type": "public_token"}
+    res = blade_api.blade_add_permission_on_toolbox_by_account_name(toolbox_id, "developer", [perm_item])
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_permission_on_toolbox(toolbox_id)
+    assert res.is_succeeded()
+    assert res.result["developer"][0] == perm_item
+
+    # delete
+    res = blade_api.blade_delete_permission_on_toolbox_by_account_name(toolbox_id, [perm_item])
+    assert res.is_succeeded()
+
+    # delete toolbox
+    delete_node(env, toolbox_id, root_id)
+
+
+def test_permission_on_config(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    res = blade_api.blade_create_public_token("sdk_test_token_config", 100)
+    assert res.is_succeeded()
+    token_str = res.result["name"]
+
+    # set public token to config permission
+    # add
+    perm_item = {"account_name": token_str, "type": "public_token"}
+    res = blade_api.blade_add_permission_on_config_by_account_name("developer", [perm_item])
+    assert res.is_succeeded()
+
+    # get
+    res = blade_api.blade_get_permission_on_config()
+    assert res.is_succeeded()
+    assert res.result["developer"][0] == perm_item
+
+    # public token permission test
+    blade_api_token = init_api(env, False)
+    blade_api_token.set_blade_public_token(token_str)
+    res = blade_api_token.blade_list_user()
+    assert res.is_succeeded()
+    res = blade_api_token.blade_create_config("token_test", root_id, "node", {"hello": "world"})
+    assert res.is_succeeded()
+    res = blade_api_token.blade_delete_config("token_test", root_id, "node")
+    assert res.is_succeeded()
+
+    # delete
+    res = blade_api.blade_delete_permission_on_config_by_account_name([perm_item])
+    assert res.is_succeeded()
+
+def test_convert_context_string(env):
+    blade_api = init_api(env)
+    root_id = get_root_id(env)
+
+    res = blade_api.blade_convert_context_string("globals:globals", "lightbox_config")
+    assert res.is_succeeded()
+    out = res.first_result()
+    context_id = out.get("context_id")
+    context_type = out.get("context_type")
+    assert root_id==context_id
+    assert "node"==context_type
+
+    res = blade_api.blade_convert_context_string("etc", "thm_plugins")
+    assert res.is_succeeded()
+    out = res.first_result()
+    context_id = out.get("context_id")
+    context_type = out.get("context_type")
+    assert root_id==context_id
+    assert "node"==context_type
+    
+def test_edit_package(env):
+    blade_api = init_api(env)
+    # create
+    pkg_info={
+        "authors": [
+            "Guido van Rossum"
+        ],
+        "category": "ext",
+        "description": "The Python programming language.",
+        "homepage": "https://www.python.org/",
+        "name": "arthub_test_pkg",
+        "requires": [],
+        "tools": [
+            "python"
+        ],
+        "variants": [
+            [
+            "platform-windows",
+            "python_embedded"
+            ],
+            [
+            "platform-windows",
+            "!python_embedded"
+            ]
+        ],
+        "version": "0.0.1"
+    }
+    
+    # upload
+    res = blade_api.blade_upload_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}], force=True)
+    assert res.is_succeeded()
+    
+    # create
+    res = blade_api.blade_create_package(pkg_info, upsert=True)
+    assert res.is_succeeded()
+    
+    # create failed
+    res = blade_api.blade_create_package(pkg_info, upsert=False)
+    assert not res.is_succeeded()
+    
+    # get 1
+    res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
+    assert res.is_succeeded()
+    pkg_info_1 = res.result
+    del pkg_info_1["api_modified"]
+
+    # update
+    res = blade_api.blade_update_package(**{
+        "name": "arthub_test_pkg",
+        "version": "0.0.1",
+        "tools": [
+            "no-tools"
+        ],
+        "requires": ["python"]
+    })
+    assert res.is_succeeded()
+    pkg_info_1.update({
+        "tools": [
+            "no-tools"
+        ],
+        "requires": ["python"],
+    })    
+    
+    # get 2
+    res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
+    assert res.is_succeeded()
+    pkg_info_2 = res.result
+    del pkg_info_2["api_modified"]
+    
+    # cmp
+    assert pkg_info_1 == pkg_info_2
+    assert pkg_info_2.get("tools") == ["no-tools"]
+    logging.info("[TEST][API] edit package success: %s" % pkg_info)
+
+    # download
+    res = blade_api.blade_download_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}])
+    assert res.is_succeeded()
+    
+    # no-delete-method
+
```


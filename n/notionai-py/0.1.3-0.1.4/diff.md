# Comparing `tmp/notionai-py-0.1.3.tar.gz` & `tmp/notionai-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionai-py-0.1.3.tar", last modified: Sun Apr  9 14:16:47 2023, max compression
+gzip compressed data, was "notionai-py-0.1.4.tar", last modified: Fri May 12 08:38:51 2023, max compression
```

## Comparing `notionai-py-0.1.3.tar` & `notionai-py-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-09 14:16:25.000000 notionai-py-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 14:16:25.000000 notionai-py-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-09 14:16:47.308513 notionai-py-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-09 14:16:25.000000 notionai-py-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-09 14:16:25.000000 notionai-py-0.1.3/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   336248 2023-04-09 14:16:25.000000 notionai-py-0.1.3/docs/images/example-webui.png
--rw-r--r--   0 runner    (1001) docker     (123)   278813 2023-04-09 14:16:25.000000 notionai-py-0.1.3/docs/images/get_notion_token.png
--rw-r--r--   0 runner    (1001) docker     (123)   217196 2023-04-09 14:16:25.000000 notionai-py-0.1.3/docs/images/notion-space-id.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.304513 notionai-py-0.1.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/examples/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/basic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/examples/webui/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/webui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/webui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 14:16:25.000000 notionai-py-0.1.3/examples/webui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/notionai/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 14:16:25.000000 notionai-py-0.1.3/notionai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-09 14:16:25.000000 notionai-py-0.1.3/notionai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-09 14:16:25.000000 notionai-py-0.1.3/notionai/notionai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/notionai_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 14:16:47.000000 notionai-py-0.1.3/notionai_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-09 14:16:25.000000 notionai-py-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:16:47.308513 notionai-py-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:47.308513 notionai-py-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:16:25.000000 notionai-py-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-09 14:16:25.000000 notionai-py-0.1.3/tests/notionai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.998901 notionai-py-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.994901 notionai-py-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.994901 notionai-py-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 08:38:29.000000 notionai-py-0.1.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-12 08:38:29.000000 notionai-py-0.1.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-12 08:38:29.000000 notionai-py-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-12 08:38:29.000000 notionai-py-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 08:38:29.000000 notionai-py-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-12 08:38:50.998901 notionai-py-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-12 08:38:29.000000 notionai-py-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-12 08:38:29.000000 notionai-py-0.1.4/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.994901 notionai-py-0.1.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.994901 notionai-py-0.1.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   336248 2023-05-12 08:38:29.000000 notionai-py-0.1.4/docs/images/example-webui.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278813 2023-05-12 08:38:29.000000 notionai-py-0.1.4/docs/images/get_notion_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)   217196 2023-05-12 08:38:29.000000 notionai-py-0.1.4/docs/images/notion-space-id.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.994901 notionai-py-0.1.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.994901 notionai-py-0.1.4/examples/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-12 08:38:29.000000 notionai-py-0.1.4/examples/basic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.998901 notionai-py-0.1.4/examples/webui/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 08:38:29.000000 notionai-py-0.1.4/examples/webui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-12 08:38:29.000000 notionai-py-0.1.4/examples/webui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 08:38:29.000000 notionai-py-0.1.4/examples/webui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.998901 notionai-py-0.1.4/notionai/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-12 08:38:29.000000 notionai-py-0.1.4/notionai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-12 08:38:29.000000 notionai-py-0.1.4/notionai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-05-12 08:38:29.000000 notionai-py-0.1.4/notionai/notionai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.998901 notionai-py-0.1.4/notionai_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-12 08:38:50.000000 notionai-py-0.1.4/notionai_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-12 08:38:50.000000 notionai-py-0.1.4/notionai_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:38:50.000000 notionai-py-0.1.4/notionai_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:38:50.000000 notionai-py-0.1.4/notionai_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:38:50.000000 notionai-py-0.1.4/notionai_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-12 08:38:29.000000 notionai-py-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:38:50.998901 notionai-py-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:50.998901 notionai-py-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:38:29.000000 notionai-py-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-12 08:38:29.000000 notionai-py-0.1.4/tests/notionai_test.py
```

### Comparing `notionai-py-0.1.3/.github/workflows/pypi.yml` & `notionai-py-0.1.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/.gitignore` & `notionai-py-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/LICENSE` & `notionai-py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/PKG-INFO` & `notionai-py-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionai-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unoffical Notion AI API
 Author-email: Vaayne <liu.vaayne@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Vaayne/NotionAI
 Project-URL: Bug Tracker, https://github.com/Vaayne/NotionAI/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
@@ -81,15 +81,14 @@
 
 ### Usage
 
 #### Install
 
 `pip install --upgrade notionai-py`
 
-
 #### Get Notion Token and Workspace ID
 
 To use the NotionAI Python SDK, you need to obtain a Notion token. You can do this by following these steps:
 
 1. Open Chrome or Firefox DevTools
 2. Find Cookies and copy the value for `token_v2`
 3. Find the `spaceId` of your Notion workspace
@@ -109,14 +108,27 @@
 spaces = NotionAI.get_spaces(TOKEN)
 print(spaces)
 # the result will looks like
 # [{'id': 'xxxxx', 'name': 'xxxxx'}]
 
 ```
 
+**Note2: Now supports custom api proxy links**
+
+```python
+import os
+from notionai import NotionAI
+TOKEN = os.getenv("NOTION_TOKEN")
+SPACE_ID = os.getenv("NOTION_SPACE_ID")
+API_URL = "https://xxx.xxx.xxx"  # this is your custom proxy links
+
+ai = NotionAI(TOKEN, SPACE_ID, api_url=API_URL)
+res = ai.blog_post("write a blog about the meaning of life")
+print(res)
+```
 
 #### Examples
 
 Check out the [examples](./examples/) directory for usage examples.
 
 1. Basic
 
@@ -149,16 +161,14 @@
 
 def main():
     ai = NotionAIStream(TOKEN, SPACE_ID)
     res = ai.blog_post("write a blog about the meaning of life")
     for item in res:
         sys.stdout.write(item)
 
-
 if __name__ == "__main__":
     main()
 ```
 
-
 3. WebUI
 
 Check out the [webui](./examples/webui/README.md) directory for instructions on how to use the NotionAI Python SDK with a web user interface.
```

### Comparing `notionai-py-0.1.3/README.md` & `notionai-py-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
 ### Usage
 
 #### Install
 
 `pip install --upgrade notionai-py`
 
-
 #### Get Notion Token and Workspace ID
 
 To use the NotionAI Python SDK, you need to obtain a Notion token. You can do this by following these steps:
 
 1. Open Chrome or Firefox DevTools
 2. Find Cookies and copy the value for `token_v2`
 3. Find the `spaceId` of your Notion workspace
@@ -96,14 +95,27 @@
 spaces = NotionAI.get_spaces(TOKEN)
 print(spaces)
 # the result will looks like
 # [{'id': 'xxxxx', 'name': 'xxxxx'}]
 
 ```
 
+**Note2: Now supports custom api proxy links**
+
+```python
+import os
+from notionai import NotionAI
+TOKEN = os.getenv("NOTION_TOKEN")
+SPACE_ID = os.getenv("NOTION_SPACE_ID")
+API_URL = "https://xxx.xxx.xxx"  # this is your custom proxy links
+
+ai = NotionAI(TOKEN, SPACE_ID, api_url=API_URL)
+res = ai.blog_post("write a blog about the meaning of life")
+print(res)
+```
 
 #### Examples
 
 Check out the [examples](./examples/) directory for usage examples.
 
 1. Basic
 
@@ -136,16 +148,14 @@
 
 def main():
     ai = NotionAIStream(TOKEN, SPACE_ID)
     res = ai.blog_post("write a blog about the meaning of life")
     for item in res:
         sys.stdout.write(item)
 
-
 if __name__ == "__main__":
     main()
 ```
 
-
 3. WebUI
 
 Check out the [webui](./examples/webui/README.md) directory for instructions on how to use the NotionAI Python SDK with a web user interface.
```

### Comparing `notionai-py-0.1.3/docs/images/example-webui.png` & `notionai-py-0.1.4/docs/images/example-webui.png`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/docs/images/get_notion_token.png` & `notionai-py-0.1.4/docs/images/get_notion_token.png`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/docs/images/notion-space-id.png` & `notionai-py-0.1.4/docs/images/notion-space-id.png`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/examples/basic/main.py` & `notionai-py-0.1.4/examples/basic/main.py`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/examples/webui/app.py` & `notionai-py-0.1.4/examples/webui/app.py`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/notionai/enums.py` & `notionai-py-0.1.4/notionai/enums.py`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/notionai/notionai.py` & `notionai-py-0.1.4/notionai/notionai.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 import uuid
 
 import requests
 
 from notionai.enums import PromptTypeEnum, ToneEnum, TopicEnum, TranslateLanguageEnum
 
 MODEL = "openai-3"
-URL = "https://www.notion.so/api/v3/getCompletion"
+API_URL = "https://www.notion.so"
 
 
 class NotionAIBase(object):
     stream = False
 
     def __init__(
         self,
         token: str,
         space_id: str,
         model: str = MODEL,
+        api_url: str = API_URL,
     ) -> None:
         """Init NotionAI
         Args:
             token (str): Notion token_v2
             space_id (str): Notion workspace id
             model (str, optional): AI model. Default to openai-1.1
+            api_url (str, optional): Notion api base url
             stream (bool, optional): use stream result. Defaults to False.
             pageTitle (str, optional): Title for your content. Defaults to PAGE_TITLE.
         """
         self.token = token
         self.space_id = space_id
         self.model = model
+        self.api_url = api_url
         self.is_space_permission = False
-        self.url = URL
+        self.url = f"{self.api_url}/api/v3/getCompletion"
 
     def _request(self, content: dict) -> str:
         payload = {
             "id": self._get_id(),
             "model": self.model,
             "spaceId": self.space_id,
             "isSpacePermission": self.is_space_permission,
@@ -77,28 +80,29 @@
 
     def _get_id(self) -> str:
         return str(uuid.uuid4())
 
 
 class NotionAI(NotionAIBase):
     @classmethod
-    def get_spaces(cls, token: str) -> list[dict]:
+    def get_spaces(cls, token: str, api_url: str = API_URL) -> list[dict]:
         """Get all spaces
         Params:
             token (str): Notion token_v2
+            api_url (str): Notion api base url
 
         Returns:
             list[dict]: list of spaces with id and name
 
         Example: [
             {"id": "space_id_1", "name": "space_name"},
             {"id": "space_id_2", "name": "space_name"}
         ]
         """
-        url = "https://www.notion.so/api/v3/getSpaces"
+        url = f"{api_url}/api/v3/getSpaces"
         r = requests.post(url, headers=cls._build_headers(token))
         if r.status_code != 200:
             raise ValueError("Cannot get spaces")
         res = r.json()
         spaces = []
         for _, val in res.items():
             space = val.get("space")
```

### Comparing `notionai-py-0.1.3/notionai_py.egg-info/PKG-INFO` & `notionai-py-0.1.4/notionai_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionai-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unoffical Notion AI API
 Author-email: Vaayne <liu.vaayne@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Vaayne/NotionAI
 Project-URL: Bug Tracker, https://github.com/Vaayne/NotionAI/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
@@ -81,15 +81,14 @@
 
 ### Usage
 
 #### Install
 
 `pip install --upgrade notionai-py`
 
-
 #### Get Notion Token and Workspace ID
 
 To use the NotionAI Python SDK, you need to obtain a Notion token. You can do this by following these steps:
 
 1. Open Chrome or Firefox DevTools
 2. Find Cookies and copy the value for `token_v2`
 3. Find the `spaceId` of your Notion workspace
@@ -109,14 +108,27 @@
 spaces = NotionAI.get_spaces(TOKEN)
 print(spaces)
 # the result will looks like
 # [{'id': 'xxxxx', 'name': 'xxxxx'}]
 
 ```
 
+**Note2: Now supports custom api proxy links**
+
+```python
+import os
+from notionai import NotionAI
+TOKEN = os.getenv("NOTION_TOKEN")
+SPACE_ID = os.getenv("NOTION_SPACE_ID")
+API_URL = "https://xxx.xxx.xxx"  # this is your custom proxy links
+
+ai = NotionAI(TOKEN, SPACE_ID, api_url=API_URL)
+res = ai.blog_post("write a blog about the meaning of life")
+print(res)
+```
 
 #### Examples
 
 Check out the [examples](./examples/) directory for usage examples.
 
 1. Basic
 
@@ -149,16 +161,14 @@
 
 def main():
     ai = NotionAIStream(TOKEN, SPACE_ID)
     res = ai.blog_post("write a blog about the meaning of life")
     for item in res:
         sys.stdout.write(item)
 
-
 if __name__ == "__main__":
     main()
 ```
 
-
 3. WebUI
 
 Check out the [webui](./examples/webui/README.md) directory for instructions on how to use the NotionAI Python SDK with a web user interface.
```

### Comparing `notionai-py-0.1.3/notionai_py.egg-info/SOURCES.txt` & `notionai-py-0.1.4/notionai_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notionai-py-0.1.3/pyproject.toml` & `notionai-py-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notionai-py"
 description = "Unoffical Notion AI API"
-version="0.1.3"
+version="0.1.4"
 authors = [
   { name="Vaayne", email="liu.vaayne@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3"
 license = {text = "MIT License"}
 classifiers = [
```

### Comparing `notionai-py-0.1.3/tests/notionai_test.py` & `notionai-py-0.1.4/tests/notionai_test.py`

 * *Files identical despite different names*


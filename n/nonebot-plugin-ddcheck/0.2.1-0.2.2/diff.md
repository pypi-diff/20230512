# Comparing `tmp/nonebot_plugin_ddcheck-0.2.1.tar.gz` & `tmp/nonebot_plugin_ddcheck-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ddcheck-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_ddcheck-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_ddcheck-0.2.1.tar` & `nonebot_plugin_ddcheck-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/LICENSE
--rw-r--r--   0        0        0     1029 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/README.md
--rw-r--r--   0        0        0     1967 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/__init__.py
--rw-r--r--   0        0        0      115 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/config.py
--rw-r--r--   0        0        0     6674 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/data_source.py
--rw-r--r--   0        0        0     4860 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/template/info.html
--rw-r--r--   0        0        0      753 2023-03-10 12:33:20.390493 nonebot_plugin_ddcheck-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 nonebot_plugin_ddcheck-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-12 13:20:56.298534 nonebot_plugin_ddcheck-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1029 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/README.md
+-rw-r--r--   0        0        0     1967 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/config.py
+-rw-r--r--   0        0        0     6768 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/data_source.py
+-rw-r--r--   0        0        0     4860 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/template/info.html
+-rw-r--r--   0        0        0      753 2023-05-12 13:20:56.302534 nonebot_plugin_ddcheck-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 nonebot_plugin_ddcheck-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_ddcheck-0.2.1/LICENSE` & `nonebot_plugin_ddcheck-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.1/README.md` & `nonebot_plugin_ddcheck-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/__init__.py` & `nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     description="查询B站用户关注的VTuber成分",
     usage="查成分 B站用户名/UID",
     config=Config,
     extra={
         "unique_name": "ddcheck",
         "example": "查成分 小南莓Official",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.1",
+        "version": "0.2.2",
     },
 )
 
 
 ddcheck = on_command("查成分", block=True, priority=12)
```

### Comparing `nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/data_source.py` & `nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_htmlrender import html_to_pic
 from nonebot_plugin_localstore import get_cache_dir
 
 from .config import Config
 
 dd_config = Config.parse_obj(get_driver().config.dict())
+headers = {
+    "cookie": dd_config.bilibili_cookie,
+    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.35",
+}
 
 data_path = get_cache_dir("nonebot_plugin_ddcheck")
 vtb_list_path = data_path / "vtb_list.json"
 
 dir_path = Path(__file__).parent
 template_path = dir_path / "template"
 env = jinja2.Environment(
@@ -91,15 +95,14 @@
     return load_vtb_list()
 
 
 async def get_uid_by_name(name: str) -> int:
     try:
         url = "http://api.bilibili.com/x/web-interface/search/type"
         params = {"search_type": "bili_user", "keyword": name}
-        headers = {"cookie": dd_config.bilibili_cookie}
         async with httpx.AsyncClient(timeout=10) as client:
             await client.get("https://www.bilibili.com", headers=headers)
             resp = await client.get(url, params=params)
             result = resp.json()
             for user in result["data"]["result"]:
                 if user["uname"] == name:
                     return user["mid"]
@@ -122,15 +125,14 @@
         return {}
 
 
 async def get_medals(uid: int) -> List[dict]:
     try:
         url = "https://api.live.bilibili.com/xlive/web-ucenter/user/MedalWall"
         params = {"target_id": uid}
-        headers = {"cookie": dd_config.bilibili_cookie}
         async with httpx.AsyncClient(timeout=10) as client:
             resp = await client.get(url, params=params, headers=headers)
             result = resp.json()
             return result["data"]["list"]
     except (KeyError, IndexError, httpx.TimeoutException) as e:
         logger.warning(f"Error in get_medals({uid}): {e}")
         return []
```

### Comparing `nonebot_plugin_ddcheck-0.2.1/nonebot_plugin_ddcheck/template/info.html` & `nonebot_plugin_ddcheck-0.2.2/nonebot_plugin_ddcheck/template/info.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ddcheck-0.2.1/pyproject.toml` & `nonebot_plugin_ddcheck-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_ddcheck"
-version = "0.2.1"
+version = "0.2.2"
 description = "Nonebot2 成分姬插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-ddcheck"
 repository = "https://github.com/noneplugin/nonebot-plugin-ddcheck"
```

### Comparing `nonebot_plugin_ddcheck-0.2.1/PKG-INFO` & `nonebot_plugin_ddcheck-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ddcheck
-Version: 0.2.1
+Version: 0.2.2
 Summary: Nonebot2 成分姬插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-ddcheck
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


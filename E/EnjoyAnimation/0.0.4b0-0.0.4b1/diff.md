# Comparing `tmp/EnjoyAnimation-0.0.4b0.tar.gz` & `tmp/EnjoyAnimation-0.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnjoyAnimation-0.0.4b0.tar", last modified: Fri May 12 10:03:02 2023, max compression
+gzip compressed data, was "EnjoyAnimation-0.0.4b1.tar", last modified: Fri May 12 10:21:48 2023, max compression
```

## Comparing `EnjoyAnimation-0.0.4b0.tar` & `EnjoyAnimation-0.0.4b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:03:02.842722 EnjoyAnimation-0.0.4b0/
-drwxrwxrwx   0        0        0        0 2023-05-12 10:03:02.827655 EnjoyAnimation-0.0.4b0/EnjoyAnimation/
--rw-rw-rw-   0        0        0    25605 2023-05-12 09:22:30.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation/EnjoyAnimation.py
--rw-rw-rw-   0        0        0       29 2023-05-09 08:39:57.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:03:02.839145 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/
--rw-rw-rw-   0        0        0     2834 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 10:03:02.000000 EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-05-06 02:32:29.000000 EnjoyAnimation-0.0.4b0/LICENSE
--rw-rw-rw-   0        0        0     2834 2023-05-12 10:03:02.841148 EnjoyAnimation-0.0.4b0/PKG-INFO
--rw-rw-rw-   0        0        0     2423 2023-05-12 09:24:31.000000 EnjoyAnimation-0.0.4b0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 10:03:02.843640 EnjoyAnimation-0.0.4b0/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-05-12 09:50:44.000000 EnjoyAnimation-0.0.4b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:21:48.991773 EnjoyAnimation-0.0.4b1/
+drwxrwxrwx   0        0        0        0 2023-05-12 10:21:48.975175 EnjoyAnimation-0.0.4b1/EnjoyAnimation/
+-rw-rw-rw-   0        0        0    25605 2023-05-12 10:21:42.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation/EnjoyAnimation.py
+-rw-rw-rw-   0        0        0       29 2023-05-09 08:39:57.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:21:48.987782 EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/
+-rw-rw-rw-   0        0        0     3212 2023-05-12 10:21:48.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-12 10:21:48.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:21:48.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-12 10:21:48.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 10:21:48.000000 EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-05-06 02:32:29.000000 EnjoyAnimation-0.0.4b1/LICENSE
+-rw-rw-rw-   0        0        0     3212 2023-05-12 10:21:48.989722 EnjoyAnimation-0.0.4b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2801 2023-05-12 10:18:51.000000 EnjoyAnimation-0.0.4b1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:21:48.991773 EnjoyAnimation-0.0.4b1/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-05-12 10:21:34.000000 EnjoyAnimation-0.0.4b1/setup.py
```

### Comparing `EnjoyAnimation-0.0.4b0/EnjoyAnimation/EnjoyAnimation.py` & `EnjoyAnimation-0.0.4b1/EnjoyAnimation/EnjoyAnimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 require("nonebot_plugin_htmlrender")
 from nonebot_plugin_htmlrender import (
     text_to_pic,
 )
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
-plugin_version="0.0.4b0"
+plugin_version="0.0.4b1"
 animation=on_command("番剧更新")
 animation_infor=on_command("番剧信息")
 search_number=on_command("番剧查询")
 animation_help=on_command("番剧帮助")
 upgrade_animation_today=on_command("今日新番")
 emmmm=on_keyword(keywords=["哦哦","奥奥","呃呃"])#5bCx5L2g5pW36KGN5oiR5piv5ZCn😅
 sub_drama=on_command("新增追番")
```

### Comparing `EnjoyAnimation-0.0.4b0/EnjoyAnimation.egg-info/PKG-INFO` & `EnjoyAnimation-0.0.4b1/EnjoyAnimation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: EnjoyAnimation
-Version: 0.0.4b0
+Version: 0.0.4b1
 Summary: 基于nonebot与gocqhttp的动漫番剧插件
 Home-page: https://github.com/small-bili/nonebot-plugin-EnjoyAnimation
 Author: slexce
 Author-email: sim69732@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nonebot-plugin-EnjoyAnimation
 这是一个基于nonebot，gocqhttp的qq-bot动漫番剧插件
 
+### PS:
+若插件版本为0.0.3及以下，手动删除bot根目录的```animations.json```,```pic文件夹```,```User_setting.json```
+
+（若不想删除```User_setting.json```,可以升级插件后运行一遍bot，然后将根目录的```User_setting.json```剪切到bot根目录中的```data```目录）
+
+更新插件
+```
+pip install --upgrade EnjoyAnimation
+```
+
 ### 插件依赖
 插件：```nonebot-plugin-apscheduler nonebot-plugin-htmlrender```
 
 库：```bs4 requests```
 
 ### 安装插件
 #### 自动安装
```

### Comparing `EnjoyAnimation-0.0.4b0/LICENSE` & `EnjoyAnimation-0.0.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `EnjoyAnimation-0.0.4b0/PKG-INFO` & `EnjoyAnimation-0.0.4b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: EnjoyAnimation
-Version: 0.0.4b0
+Version: 0.0.4b1
 Summary: 基于nonebot与gocqhttp的动漫番剧插件
 Home-page: https://github.com/small-bili/nonebot-plugin-EnjoyAnimation
 Author: slexce
 Author-email: sim69732@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nonebot-plugin-EnjoyAnimation
 这是一个基于nonebot，gocqhttp的qq-bot动漫番剧插件
 
+### PS:
+若插件版本为0.0.3及以下，手动删除bot根目录的```animations.json```,```pic文件夹```,```User_setting.json```
+
+（若不想删除```User_setting.json```,可以升级插件后运行一遍bot，然后将根目录的```User_setting.json```剪切到bot根目录中的```data```目录）
+
+更新插件
+```
+pip install --upgrade EnjoyAnimation
+```
+
 ### 插件依赖
 插件：```nonebot-plugin-apscheduler nonebot-plugin-htmlrender```
 
 库：```bs4 requests```
 
 ### 安装插件
 #### 自动安装
```

### Comparing `EnjoyAnimation-0.0.4b0/README.md` & `EnjoyAnimation-0.0.4b1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 # nonebot-plugin-EnjoyAnimation
 这是一个基于nonebot，gocqhttp的qq-bot动漫番剧插件
 
+### PS:
+若插件版本为0.0.3及以下，手动删除bot根目录的```animations.json```,```pic文件夹```,```User_setting.json```
+
+（若不想删除```User_setting.json```,可以升级插件后运行一遍bot，然后将根目录的```User_setting.json```剪切到bot根目录中的```data```目录）
+
+更新插件
+```
+pip install --upgrade EnjoyAnimation
+```
+
 ### 插件依赖
 插件：```nonebot-plugin-apscheduler nonebot-plugin-htmlrender```
 
 库：```bs4 requests```
 
 ### 安装插件
 #### 自动安装
```

### Comparing `EnjoyAnimation-0.0.4b0/setup.py` & `EnjoyAnimation-0.0.4b1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r",encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["bs4","requests"] # 这里填依赖包信息
-VERSION="0.0.4b0"
+VERSION="0.0.4b1"
 
 setup(
     name="",
     version=VERSION,
     author="slexce",
     author_email="sim69732@gmail.com",
     description="基于nonebot与gocqhttp的动漫番剧插件",
```


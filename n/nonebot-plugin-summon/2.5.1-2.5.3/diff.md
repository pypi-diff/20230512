# Comparing `tmp/nonebot_plugin_summon-2.5.1.tar.gz` & `tmp/nonebot_plugin_summon-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_summon-2.5.1.tar", last modified: Sat Feb 18 13:18:59 2023, max compression
+gzip compressed data, was "nonebot_plugin_summon-2.5.3.tar", last modified: Fri May 12 15:02:34 2023, max compression
```

## Comparing `nonebot_plugin_summon-2.5.1.tar` & `nonebot_plugin_summon-2.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 13:18:59.838223 nonebot_plugin_summon-2.5.1/
--rw-rw-rw-   0        0        0     1088 2022-12-24 04:11:04.000000 nonebot_plugin_summon-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     2040 2023-02-18 13:18:59.837223 nonebot_plugin_summon-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1320 2023-02-17 18:30:31.000000 nonebot_plugin_summon-2.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-18 13:18:59.831709 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon/
--rw-rw-rw-   0        0        0     6793 2023-02-18 13:17:09.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon/__init__.py
--rw-rw-rw-   0        0        0     1166 2023-02-18 13:17:09.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-18 13:18:59.836223 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-02-18 13:18:59.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-02-18 13:18:59.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 13:18:59.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-02-18 13:18:59.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-02-18 13:18:59.000000 nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-18 13:18:59.838223 nonebot_plugin_summon-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3954 2023-02-18 13:18:05.000000 nonebot_plugin_summon-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:02:34.128702 nonebot_plugin_summon-2.5.3/
+-rw-rw-rw-   0        0        0     1088 2023-02-17 16:11:24.000000 nonebot_plugin_summon-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0     2040 2023-05-12 15:02:34.128702 nonebot_plugin_summon-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1320 2023-02-17 18:30:31.000000 nonebot_plugin_summon-2.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 15:02:34.112663 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/
+-rw-rw-rw-   0        0        0     6795 2023-05-12 14:55:54.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/__init__.py
+-rw-rw-rw-   0        0        0     1166 2023-02-18 13:17:09.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:02:34.117688 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-12 15:02:34.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 15:02:34.129712 nonebot_plugin_summon-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     3954 2023-05-12 15:00:31.000000 nonebot_plugin_summon-2.5.3/setup.py
```

### Comparing `nonebot_plugin_summon-2.5.1/LICENSE` & `nonebot_plugin_summon-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_summon-2.5.1/PKG-INFO` & `nonebot_plugin_summon-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_summon
-Version: 2.5.1
+Version: 2.5.3
 Summary: Groupmates summoning
 Home-page: https://github.com/zhulinyv/nonebot_plugin_summon
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_summon-2.5.1/README.md` & `nonebot_plugin_summon-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_summon-2.5.1/nonebot_plugin_summon/__init__.py` & `nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     await model_switch.finish(msg, at_sender=True)
 
 
 @list_summoning.handle()
 async def _(event: GroupMessageEvent):
     gid = str(event.group_id)   # 获取群号
     if gid not in userdata or userdata[gid] == {}:    # 判断是否有这个群, 以及这个群的dict是否为空
-        await list_summoning.finish(f"在本群{NICKNAME}的记忆里还没有人捏......", at_sende=True)
+        await list_summoning.finish(f"在本群{NICKNAME}的记忆里还没有人捏......", at_sender=True)
     else:
         dataDict = userdata[gid]    # 获取dict
     msg = ""
     for i in dataDict:  # 遍历dict
         msg = msg + f"{i} -> {dataDict[i]}\n"
     await list_summoning.finish(msg)
 
@@ -122,15 +122,15 @@
     gid = str(event.group_id)   # 获取群号
     message = msg.extract_plain_text().strip()  # 获取纯文本信息
     variable_list = message.split(' ')  # 以空格分割
     variable_list = [word.strip() for word in variable_list if word.strip()]    # 去除空格
     await poke.finish("格式错误，请检查后重试\n戳+昵称+次数(数字)", at_sender=True) if len(variable_list) < 2 else ...  # 判断列表长度
     name = variable_list[0] # 名字
     nums = int(variable_list[1]) if variable_list[1].isdigit() else await poke.finish("格式错误，请检查后重试\n戳+昵称+次数(数字)", at_sender=True) # 次数
-    await poke.finish(f"要人家戳这么多次, 你想让{NICKNAME}风控嘛......", at_sende=True) if nums > 10 else ... # 判断次数
+    await poke.finish(f"要人家戳这么多次, 你想让{NICKNAME}风控嘛......", at_sender=True) if nums > 10 else ... # 判断次数
     try:
         qid = userdata[gid][name]   # 获取qq号
     except KeyError:
         await poke.finish(f"{NICKNAME}的记忆里没有这号人捏......", at_sender=True)    # 如果没有这个人，那么就是KeyError
 
     for i in range(nums):   # 循环戳
         try:
```

### Comparing `nonebot_plugin_summon-2.5.1/nonebot_plugin_summon/utils.py` & `nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_summon-2.5.1/nonebot_plugin_summon.egg-info/PKG-INFO` & `nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-summon
-Version: 2.5.1
+Version: 2.5.3
 Summary: Groupmates summoning
 Home-page: https://github.com/zhulinyv/nonebot_plugin_summon
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_summon-2.5.1/setup.py` & `nonebot_plugin_summon-2.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_summon'
 DESCRIPTION = 'Groupmates summoning'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_summon'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.5.1'
+VERSION = '2.5.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot'
 ]
 
 # What packages are optional?
```


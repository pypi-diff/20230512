# Comparing `tmp/nonebot_plugin_spark_gpt-0.1.3.tar.gz` & `tmp/nonebot_plugin_spark_gpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-0.1.3.tar` & `nonebot_plugin_spark_gpt-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,45 @@
--rw-r--r--   0        0        0     1894 2023-05-11 03:29:22.094362 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0       16 2023-05-10 17:23:53.939876 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
--rw-r--r--   0        0        0     8228 2023-05-10 17:23:58.319737 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/config.py
--rw-r--r--   0        0        0    28144 2023-05-10 17:24:00.050884 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/main.py
--rw-r--r--   0        0        0     6131 2023-05-10 17:24:01.276809 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
--rw-r--r--   0        0        0       16 2023-05-10 17:24:06.325142 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/__init__.py
--rw-r--r--   0        0        0     3036 2023-05-10 17:24:07.826903 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/claude_func.py
--rw-r--r--   0        0        0     8094 2023-05-10 17:24:09.084792 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/config.py
--rw-r--r--   0        0        0    25921 2023-05-10 17:24:10.744126 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/main.py
--rw-r--r--   0        0        0     4309 2023-05-10 17:24:12.141727 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/slack_api.py
--rw-r--r--   0        0        0       16 2023-05-10 17:24:16.477844 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     2633 2023-05-10 17:24:17.515144 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/common_func.py
--rw-r--r--   0        0        0     6158 2023-05-10 16:32:44.366675 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     5563 2023-05-11 03:26:38.959437 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/main.py
--rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
--rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/render.py
--rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
--rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
--rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
--rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
--rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/text.css
--rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/text.html
--rw-r--r--   0        0        0     4244 2023-05-10 17:24:24.469959 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/config.py
--rw-r--r--   0        0        0    18363 2023-05-10 17:24:26.071103 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/main.py
--rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/newbing_func.py
--rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/__init__.py
--rw-r--r--   0        0        0     9719 2023-05-10 14:13:15.440356 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/config.py
--rw-r--r--   0        0        0    29872 2023-05-11 03:40:59.740884 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/main.py
--rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_api.py
--rw-r--r--   0        0        0     6332 2023-05-10 17:24:38.505890 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_func.py
--rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/pwframework.py
--rw-r--r--   0        0        0      920 2023-05-11 03:43:01.601909 nonebot_plugin_spark_gpt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3042 2023-05-11 03:31:13.216645 nonebot_plugin_spark_gpt-0.1.3/README.md
--rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2049 2023-05-11 10:58:21.820619 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:23:53.939876 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
+-rw-r--r--   0        0        0     8228 2023-05-10 17:23:58.319737 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/config.py
+-rw-r--r--   0        0        0    27739 2023-05-11 12:36:29.916576 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/main.py
+-rw-r--r--   0        0        0     6131 2023-05-10 17:24:01.276809 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:24:06.325142 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/__init__.py
+-rw-r--r--   0        0        0     3036 2023-05-10 17:24:07.826903 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/claude_func.py
+-rw-r--r--   0        0        0     8094 2023-05-10 17:24:09.084792 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/config.py
+-rw-r--r--   0        0        0    25941 2023-05-11 12:36:25.212725 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/main.py
+-rw-r--r--   0        0        0     4309 2023-05-10 17:24:12.141727 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/slack_api.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:24:16.477844 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     2633 2023-05-10 17:24:17.515144 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/common_func.py
+-rw-r--r--   0        0        0     6158 2023-05-10 16:32:44.366675 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     6053 2023-05-11 11:40:42.573933 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/main.py
+-rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
+-rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/render.py
+-rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
+-rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
+-rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
+-rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
+-rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/text.html
+-rw-r--r--   0        0        0     4244 2023-05-10 17:24:24.469959 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/newbing/config.py
+-rw-r--r--   0        0        0    18363 2023-05-10 17:24:26.071103 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/newbing/main.py
+-rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/newbing/newbing_func.py
+-rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/__init__.py
+-rw-r--r--   0        0        0     9719 2023-05-10 14:13:15.440356 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/config.py
+-rw-r--r--   0        0        0    29870 2023-05-11 12:28:50.437523 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/main.py
+-rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/poe_api.py
+-rw-r--r--   0        0        0     6332 2023-05-10 17:24:38.505890 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/poe_func.py
+-rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/pwframework.py
+-rw-r--r--   0        0        0     7940 2023-05-11 09:56:25.548175 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/Spark_desk/config.py
+-rw-r--r--   0        0        0    26874 2023-05-11 12:36:02.709762 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/Spark_desk/main.py
+-rw-r--r--   0        0        0     4762 2023-05-11 09:15:30.854977 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/Spark_desk/spark_api.py
+-rw-r--r--   0        0        0     3905 2023-05-11 08:49:24.465346 nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/Spark_desk/spark_desk_func.py
+-rw-r--r--   0        0        0      920 2023-05-11 12:32:05.366216 nonebot_plugin_spark_gpt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3227 2023-05-11 12:38:54.453351 nonebot_plugin_spark_gpt-0.1.4/README.md
+-rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import nonebot
 
 from .poe import main
 from .newbing import main
 from .chatgpt_web import main
 from .common import main
 from .claude_slack import main
+from .Spark_desk import main
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import (
     Event,
     Bot,
     MessageSegment,
 )
@@ -55,15 +56,21 @@
 | --- | --- |
 | `/gwhelp / gwh` | 获取GPT_Web帮助说明。 |
 
 ## Claude_Slack帮助命令
 
 | 命令 | 描述 |
 | --- | --- |
-| `/chelp / ch` | 获取GPT_Web帮助说明。 |
+| `/chelp / ch` | 获取Claude_Slack帮助说明。 |
+
+## Spark_desk帮助命令
+
+| 命令 | 描述 |
+| --- | --- |
+| `/shelp / sh` | 获取Spark_desk帮助说明。 |
 
 # 通用命令
 
 - 所有用户均可使用
 
 | 命令 | 描述 |
 | --- | --- |
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/config.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/main.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,16 +428,15 @@
             "清空历史",
             "清除记录",
             "清空历史对话",
             "刷新对话",
         ]:
             truename = None
             parentname = str(random_uuid4())
-            prompt_nickname = gptweb_persistor.auto_prompt
-            prompt = prompts_dict[prompt_nickname]
+            prompt = botinfo.prompt
 
             if current_userinfo not in list(gptweb_persistor.user_dict.keys()):
                 gptweb_persistor.user_dict.setdefault(
                     current_userinfo, {"all": {}, "now": {}}
                 )
 
             if creat_lock.locked():
@@ -447,23 +446,15 @@
                 result = await gptweb_api.gpt_web_chat(truename, parentname, prompt)
                 current_userdata.is_waiting = False
                 if isinstance(result, str):
                     text_error = result
                 elif isinstance(result, tuple):
                     answer, parentname, truename = result
                     # 将更新后的字典写回到JSON文件中
-                    botinfo = BotInfo(
-                        nickname=nickname,
-                        truename=truename,
-                        parentname=parentname,
-                        source="gpt_web",
-                        prompt_nickname=prompt_nickname,
-                        prompt=prompt,
-                        owner="qq-" + str(event.user_id),
-                    )
+                    botinfo.parentname = parentname
                     gptweb_persistor.user_dict[current_userinfo]["all"][
                         nickname
                     ] = botinfo
                     if (
                         botinfo.nickname
                         == list(
                             gptweb_persistor.user_dict[current_userinfo]["now"].values()
@@ -667,34 +658,35 @@
     if not is_useable(event):
         await matcher.finish()
     msg = """
 # spark-gpt GPT_web使用说明
 
 - !!! 以下命令前面全部要加 '/' !!!  
 
-- 问答功能均支持以下特性：可以通过回复机器人的最后一个回答来继续对话，而无需命令；可以回复 "(清除/清空)(对话/历史)"或 "刷新对话" 或 "清除对话历史"来清空对话；可以通过建议回复的数字索引来使用建议回复。
-
+- 问答功能均支持以下特性：
+- 可以通过回复机器人的最后一个回答来继续对话，而无需命令；可以回复 "(清除/清空)(对话/历史)"或 "刷新对话" 或 "清除对话历史"来清空对话；  
+- 可以通过建议回复的数字索引来使用建议回复。
 ## 对话命令
 
 | 命令 | 描述 |
 | --- | --- |
 | `/gwtalk / gwt + 你要询问的内容` | 对话功能，如果没创建机器人，对话将自动创建默认机器人。 |
+| `/机器人名字 + 空格 + 你要询问的内容` | 指定机器人对话。 |
 
 ## 机器人管理命令
 
 | 命令 | 描述 |
 | --- | --- |
 | `/gwcreate / gwc` | 创建机器人。 |
 | `/gwremove / gwr (+ 机器人名称)` | 删除指定名称的机器人。 |
 | `/gwswitch / gws (+ 机器人名称)` | 切换到指定名称的机器人。 |
-| `/机器人名字 + 空格 + 你要询问的内容` | 指定机器人对话。 |
 
 ## 管理员命令
 
-- 仅限poe管理员使用
+- 仅限chatgpt_web管理员使用
 
 | 命令 | 描述 |
 | --- | --- |
 | `/gwcp / gwchangeprompt` | 切换自动创建的默认预设。 |"""
     pic = await md_to_pic(msg)
     await gw_help.send(MessageSegment.image(pic))
     await gw_help.finish()
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/claude_func.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/claude_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/config.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/main.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,34 +627,35 @@
     if not is_useable(event):
         await matcher.finish()
     msg = """
 # Spark-GPT Claude_slack使用说明
 
 - !!! 以下命令前面全部要加 '/' !!!  
 
-- 问答功能均支持以下特性：可以通过回复机器人的最后一个回答来继续对话，而无需命令；可以回复 "(清除/清空)(对话/历史)"或"刷新对话"或"清除对话历史"来清空对话；可以通过建议回复的数字索引来使用建议回复。
-
+- 问答功能均支持以下特性：
+- 可以通过回复机器人的最后一个回答来继续对话，而无需命令；可以回复 "(清除/清空)(对话/历史)"或 "刷新对话" 或 "清除对话历史"来清空对话；  
+- 可以通过建议回复的数字索引来使用建议回复。
 ## 对话命令
 
 | 命令 | 描述 |
 | --- | --- |
 | `/ctalk / ct + 你要询问的内容` | 对话功能，如果没创建机器人，对话将自动创建默认机器人。 |
+| `/机器人名字 + 空格 + 你要询问的内容` | 指定机器人对话。 |
 
 ## 机器人管理命令
 
 | 命令 | 描述 |
 | --- | --- |
 | `/ccreate / cc` | 创建机器人。 |
 | `/cremove / cr (+ 机器人名称)` | 删除指定名称的机器人。 |
 | `/cswitch / cs (+ 机器人名称)` | 切换到指定名称的机器人。 |
-| `/机器人名字 + 空格 + 你要询问的内容` | 指定机器人对话。 |
 
 ## 管理员命令
 
-- 仅限poe管理员使用
+- 仅限claude_slack管理员使用
 
 | 命令 | 描述 |
 | --- | --- |
 | `/ccp / cchangeprompt` | 切换自动创建的默认预设。 |"""
     pic = await md_to_pic(msg)
     await c_help.send(MessageSegment.image(pic))
     await c_help.finish()
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/slack_api.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/claude_slack/slack_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/common_func.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/common_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/main.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .render.render import md_to_pic
 from .common_func import reply_out
 from .config import spark_persistor, get_user_info_and_data
 from .common_func import is_auto_prompt
 from ..chatgpt_web.config import gptweb_persistor
 from ..poe.config import poe_persistor
 from ..claude_slack.config import claude_slack_persistor
-
+from ..Spark_desk.config import spark_desk_persistor
 spark_addprompt = on_command("添加预设", aliases={"ap"}, priority=4, block=False)
 
 
 @spark_addprompt.handle()
 async def __spark_addprompt__(matcher: Matcher, event: Event):
     global spark_persistor
     user_id = str(event.user_id)
@@ -119,16 +119,26 @@
         claude_slack_bots = list(
             claude_slack_persistor.user_dict[current_userinfo]["all"].keys()
         )
         claude_slack_bot_str = "claude_slack机器人有:\n"
         for i in range(len(claude_slack_bots)):
             claude_slack_bot_str += f"    {i+1}:{claude_slack_bots[i]}\n"
     except:
-        claude_slack_bot_str = "没有可用的poe机器人\n"
-    msg = "所有机器人信息如下:\n\n" + gw_bot_str + poe_bot_str + claude_slack_bot_str
+        claude_slack_bot_str = "没有可用的claude_slack机器人\n"
+    try:
+        spark_desk_bots = list(
+            spark_desk_persistor.user_dict[current_userinfo]["all"].keys()
+        )
+        spark_desk_bot_str = "spark_desk机器人有:\n"
+        for i in range(len(spark_desk_bots)):
+            spark_desk_bot_str += f"    {i+1}:{spark_desk_bots[i]}\n"
+    except:
+        spark_desk_bot_str = "没有可用的poe机器人\n"
+    
+    msg = "所有机器人信息如下:\n\n" + gw_bot_str + "\n" + poe_bot_str + "\n" + claude_slack_bot_str + "\n" + spark_desk_bot_str
     await matcher.finish(reply_out(event, msg))
 
 
 test = on_command("md2pic", priority=4, block=False)
 
 
 @test.handle()
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/render.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown.html` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/background.png` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/source/background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/config.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/newbing/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/main.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/newbing/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/newbing_func.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/newbing/newbing_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/config.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/main.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,15 +686,15 @@
                 await bot.delete_msg(message_id=waitmsg["message_id"])
             except:
                 pass
             await matcher.finish()
 
 
 ######################################################
-poe_help = on_command("poehelp", aliases={"poe帮助", "ph"}, priority=4, block=False)
+poe_help = on_command("poehelp", aliases={"p帮助", "ph"}, priority=4, block=False)
 
 
 @poe_help.handle()
 async def __poe_help__(bot: Bot, matcher: Matcher, event: Event):
     user_id = str(event.user_id)
     if not is_useable(event):
         await matcher.finish()
@@ -714,18 +714,18 @@
 ************************
 
 - 以下命令均支持用户隔离
 
 | 命令 | 描述 |
 | --- | --- |
 | `/ptalk / pt + 你要询问的内容` | 对话功能，如果没创建机器人，对话将自动创建默认机器人。 |
+| `你的机器人的名字 + 空格 + 你要询问的内容` | 指定机器人对话。 |
 | `/poecreate / pc` | 创建机器人。 |
 | `/poeremove / pr (+ 机器人名称)` | 删除指定名称的机器人。 |
 | `/poeswitch / ps (+ 机器人名称)` | 切换到指定名称的机器人。 |
-| `你的机器人的名字 + 空格 + 你要询问的内容` | 指定机器人对话。 |
 
 ************************
 
 - 以下命令均是多用户共享的
 
 | 命令 | 描述 |
 | --- | --- |
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_api.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/poe_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_func.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/poe_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/pwframework.py` & `nonebot_plugin_spark_gpt-0.1.4/nonebot_plugin_spark_gpt/poe/pwframework.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.3/pyproject.toml` & `nonebot_plugin_spark_gpt-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "0.1.3"
+version = "0.1.4"
 description = "Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_spark_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/README.md` & `nonebot_plugin_spark_gpt-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,22 @@
 >
 ## [必看教程-残心小站-文档库](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 
 > 用户交流群:[610948446](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=KHGqjjbiz6fpRr-W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 )
 ---
 
-- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token),Claude(slack)接入qq
+- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token),Claude(slack),讯飞星火模型(Spark_desk)接入qq
 
 | Image 1 | Image 2 |
 |:-------:|:-------:|
 | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) |
 | ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |
 | ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(6).png) |
-
+| ![7](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(7).png) |  |
 ## 更新
 
-- 2023.5.11 0.1.2:  
+- 2023.5.11 0.1.4:  
+    1.增加讯飞星火模型(Spark_desk)  
+- 2023.5.11 0.1.3:  
     1.增加claude_slack  
     2.修复一些小bug
```

#### html2text {}

```diff
@@ -10,16 +10,18 @@
 ç¹å»å¾çè·³è½¬âï¸ > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
 ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-
 æ®å¿å°ç«-ææ¡£åº](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 > ç¨æ·äº¤æµç¾¤:[610948446](http://qm.qq.com/cgi-bin/qm/
 qr?_wv=1027&k=KHGqjjbiz6fpRr-
 W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 ) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token),Claude
-(slack)æ¥å¥qq | Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://
-github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2]
-(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | |
-![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png)
-| ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo
-(4).png) | | ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/
-spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/
-source/spark/demo(6).png) | ## æ´æ° - 2023.5.11 0.1.2: 1.å¢å claude_slack
-2.ä¿®å¤ä¸äºå°bug
+(slack),è®¯é£æç«æ¨¡å(Spark_desk)æ¥å¥qq | Image 1 | Image 2 | |:-------:
+|:-------:| | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/
+spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/
+source/spark/demo(2).png) | | ![3](https://github.com/canxin121/Spark-GPT/blob/
+main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/
+blob/main/source/spark/demo(4).png) | | ![5](https://github.com/canxin121/
+Spark-GPT/blob/main/source/spark/demo(5).png) | ![6](https://github.com/
+canxin121/Spark-GPT/blob/main/source/spark/demo(6).png) | | ![7](https://
+github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(7).png) | | ##
+æ´æ° - 2023.5.11 0.1.4: 1.å¢å è®¯é£æç«æ¨¡å(Spark_desk) - 2023.5.11
+0.1.3: 1.å¢å claude_slack 2.ä¿®å¤ä¸äºå°bug
```

### Comparing `nonebot_plugin_spark_gpt-0.1.3/PKG-INFO` & `nonebot_plugin_spark_gpt-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -61,21 +61,23 @@
 >
 ## [必看教程-残心小站-文档库](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 
 > 用户交流群:[610948446](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=KHGqjjbiz6fpRr-W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 )
 ---
 
-- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token),Claude(slack)接入qq
+- 目前支持将Poe,NewBing,Dalle,ChatGPT (session token),Claude(slack),讯飞星火模型(Spark_desk)接入qq
 
 | Image 1 | Image 2 |
 |:-------:|:-------:|
 | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) |
 | ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |
 | ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(6).png) |
-
+| ![7](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(7).png) |  |
 ## 更新
 
-- 2023.5.11 0.1.2:  
+- 2023.5.11 0.1.4:  
+    1.增加讯飞星火模型(Spark_desk)  
+- 2023.5.11 0.1.3:  
     1.增加claude_slack  
     2.修复一些小bug
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.4 Summary:
 Spark-
 GPT,å°å¤æ¥æºçgptæ¥å¥qqåæ´å¤å¹³å°,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: bidict (>=0.22.1,<0.23.0)
@@ -27,16 +27,18 @@
 ç¹å»å¾çè·³è½¬âï¸ > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
 ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-
 æ®å¿å°ç«-ææ¡£åº](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 > ç¨æ·äº¤æµç¾¤:[610948446](http://qm.qq.com/cgi-bin/qm/
 qr?_wv=1027&k=KHGqjjbiz6fpRr-
 W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 ) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token),Claude
-(slack)æ¥å¥qq | Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://
-github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2]
-(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | |
-![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png)
-| ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo
-(4).png) | | ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/
-spark/demo(5).png) | ![6](https://github.com/canxin121/Spark-GPT/blob/main/
-source/spark/demo(6).png) | ## æ´æ° - 2023.5.11 0.1.2: 1.å¢å claude_slack
-2.ä¿®å¤ä¸äºå°bug
+(slack),è®¯é£æç«æ¨¡å(Spark_desk)æ¥å¥qq | Image 1 | Image 2 | |:-------:
+|:-------:| | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/
+spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/
+source/spark/demo(2).png) | | ![3](https://github.com/canxin121/Spark-GPT/blob/
+main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/
+blob/main/source/spark/demo(4).png) | | ![5](https://github.com/canxin121/
+Spark-GPT/blob/main/source/spark/demo(5).png) | ![6](https://github.com/
+canxin121/Spark-GPT/blob/main/source/spark/demo(6).png) | | ![7](https://
+github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(7).png) | | ##
+æ´æ° - 2023.5.11 0.1.4: 1.å¢å è®¯é£æç«æ¨¡å(Spark_desk) - 2023.5.11
+0.1.3: 1.å¢å claude_slack 2.ä¿®å¤ä¸äºå°bug
```


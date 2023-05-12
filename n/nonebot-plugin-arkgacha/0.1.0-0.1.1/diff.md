# Comparing `tmp/nonebot_plugin_arkgacha-0.1.0.tar.gz` & `tmp/nonebot_plugin_arkgacha-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_arkgacha-0.1.0.tar", last modified: Fri May 12 13:21:56 2023, max compression
+gzip compressed data, was "nonebot_plugin_arkgacha-0.1.1.tar", last modified: Fri May 12 14:11:33 2023, max compression
```

## Comparing `nonebot_plugin_arkgacha-0.1.0.tar` & `nonebot_plugin_arkgacha-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1553 2023-05-12 12:55:04.474163 nonebot_plugin_arkgacha-0.1.0/README.md
--rw-r--r--   0        0        0     4620 2023-05-12 13:16:20.817667 nonebot_plugin_arkgacha-0.1.0/nonebot_plugin_arkgacha/__init__.py
--rw-r--r--   0        0        0      175 2023-05-12 12:54:47.496416 nonebot_plugin_arkgacha-0.1.0/nonebot_plugin_arkgacha/config.py
--rw-r--r--   0        0        0      631 2023-05-12 13:21:56.948043 nonebot_plugin_arkgacha-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-12 13:39:48.087709 nonebot_plugin_arkgacha-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1553 2023-05-12 12:55:04.474163 nonebot_plugin_arkgacha-0.1.1/README.md
+-rw-r--r--   0        0        0     4620 2023-05-12 13:16:20.817667 nonebot_plugin_arkgacha-0.1.1/nonebot_plugin_arkgacha/__init__.py
+-rw-r--r--   0        0        0      175 2023-05-12 12:54:47.496416 nonebot_plugin_arkgacha-0.1.1/nonebot_plugin_arkgacha/config.py
+-rw-r--r--   0        0        0      631 2023-05-12 14:11:33.509398 nonebot_plugin_arkgacha-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_arkgacha-0.1.0/README.md` & `nonebot_plugin_arkgacha-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.1.0/nonebot_plugin_arkgacha/__init__.py` & `nonebot_plugin_arkgacha-0.1.1/nonebot_plugin_arkgacha/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.1.0/pyproject.toml` & `nonebot_plugin_arkgacha-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "nonebot-plugin-arkgacha"
-version = "0.1.0"
+version = "0.1.1"
 description = "Plugin for Arknights gacha, support multi platform"
 authors = [
     { name = "RF-Tar-Railt", email = "3165388245@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
     "nonebot-plugin-alconna>=0.4.1",
     "nonebot-plugin-send-anything-anywhere>=0.2.4",
-    "arknights-toolkit>=0.5.0",
+    "arknights-toolkit>=0.5.1",
     "nonebot-plugin-localstore>=0.4.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_arkgacha-0.1.0/PKG-INFO` & `nonebot_plugin_arkgacha-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-arkgacha
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plugin for Arknights gacha, support multi platform
 Author-Email: RF-Tar-Railt <3165388245@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.0.0rc4
 Requires-Dist: nonebot-plugin-alconna>=0.4.1
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
-Requires-Dist: arknights-toolkit>=0.5.0
+Requires-Dist: arknights-toolkit>=0.5.1
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.1.1 Summary:
 Plugin for Arknights gacha, support multi platform Author-Email: RF-Tar-Railt
 <3165388245@qq.com> License: MIT Requires-Python: >=3.8 Requires-Dist:
 nonebot2>=2.0.0rc4 Requires-Dist: nonebot-plugin-alconna>=0.4.1 Requires-Dist:
 nonebot-plugin-send-anything-anywhere>=0.2.4 Requires-Dist: arknights-
-toolkit>=0.5.0 Requires-Dist: nonebot-plugin-localstore>=0.4.1 Description-
+toolkit>=0.5.1 Requires-Dist: nonebot-plugin-localstore>=0.4.1 Description-
 Content-Type: text/markdown
                                    [nonebot]
         # NoneBot Plugin Arkgacha _â¨ ææ¥æ¹èæ½å¡æ¨¡æå¨ â¨_
                            [license] [pypi] [python]
 è¯¥æä»¶æä¾äºæ¨¡æææ¥æ¹èæ½å¡çåè½ï¼åæ¬æ å¤´å½¢å¼çæ½å¡æ¨¡æä¸æ¨¡æåè¿
 éè¿ä½¿ç¨ [`saa`](https://github.com/felinae98/nonebot-plugin-send-anything-
 anywhere) æä»¶ééå¤å¹³å° ## å®è£ ```bash pip install nonebot-plugin-
```


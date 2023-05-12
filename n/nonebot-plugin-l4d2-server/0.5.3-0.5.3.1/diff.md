# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.3.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.3.1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.3.tar` & `nonebot_plugin_l4d2_server-0.5.3.1.tar`

### file list

```diff
@@ -1,66 +1,59 @@
--rw-r--r--   0        0        0    35149 2023-05-07 15:21:10.728279 nonebot_plugin_l4d2_server-0.5.3/LICENSE
--rw-r--r--   0        0        0    11200 2023-05-07 15:21:10.728279 nonebot_plugin_l4d2_server-0.5.3/README.md
--rw-r--r--   0        0        0    17449 2023-05-07 15:21:10.732279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8619 2023-05-07 15:21:10.732279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     6069 2023-05-07 15:21:10.732279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-05-07 15:21:10.732279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-05-07 15:21:10.732279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8723 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1683 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3241 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-05-07 15:21:10.736279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3221 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1284 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4075 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2688 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4036 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     3996 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0      936 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3791 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10826 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1237 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4093 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     3872 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/art.png
--rw-r--r--   0        0        0     4448 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/bento.png
--rw-r--r--   0        0        0     3575 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/bug.png
--rw-r--r--   0        0        0     3760 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/feat.png
--rw-r--r--   0        0        0   137862 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/log_title.png
--rw-r--r--   0        0        0     3028 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/other.png
--rw-r--r--   0        0        0     2346 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/texture2d/zap.png
--rw-r--r--   0        0        0     1968 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8542 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14148 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1620 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0      337 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/rule.py
--rw-r--r--   0        0        0      992 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2133 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8624 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1493 2023-05-07 15:21:10.740279 nonebot_plugin_l4d2_server-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    13263 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-12 07:41:58.872104 nonebot_plugin_l4d2_server-0.5.3.1/LICENSE
+-rw-r--r--   0        0        0    11200 2023-05-12 07:41:58.872104 nonebot_plugin_l4d2_server-0.5.3.1/README.md
+-rw-r--r--   0        0        0    17491 2023-05-12 07:41:58.876104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-05-12 07:41:58.876104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8734 2023-05-12 07:41:58.880104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2688 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4061 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0      936 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3791 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10837 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4114 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1968 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8693 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6070 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2143 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8630 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1495 2023-05-12 07:41:58.884104 nonebot_plugin_l4d2_server-0.5.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13265 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/LICENSE` & `nonebot_plugin_l4d2_server-0.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/README.md` & `nonebot_plugin_l4d2_server-0.5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg,RawCommand,CommandStart
 from nonebot import get_driver, require
 from nonebot.plugin import PluginMetadata
 
 
-from .config import *
-from .utils import *
-from .command import *
+from l4d2_utils.config import *
+from l4d2_utils.utils import *
+from l4d2_utils.command import *
 from .l4d2_image.steam import url_to_byte,url_to_byte_name
 
 from .l4d2_data import sq_L4D2
 
 from .l4d2_image.vtfs import img_to_vtf
 from .l4d2_queries.ohter import load_josn
 from .l4d2_queries.qqgroup import write_json
 from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
 
-from .txt_to_img import mode_txt_to_img
+from l4d2_utils.txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
 
-__version__ = "0.5.2"
+__version__ = "0.5.3.1"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,15 @@
         await matcher.finish(msg)
         
     
     
 async def init():
     global matchers
     # print('启动辣')
+    from .l4d2_update import l4d_restart,l4d_update,get_update_log,driver
     await get_des_ip()
     
    
     
 @driver.on_bot_connect
 async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
     PRIVATE_FRIEND,
 )
 
-from .l4d2_queries.ohter import ALL_HOST
+from ..l4d2_queries.ohter import ALL_HOST
 file_format = (".vpk",".zip",".7z",'rar')
 # 权限
 
 driver = get_driver()
 COMMAND_START = list[driver.config.command_start]
 try:
     NICKNAME: str = list(driver.config.nickname)[0]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from nonebot.log import logger
 
 import pandas as pd
 from typing import List
 
 from .analysis import df_to_guoguanlv
-from ..seach import *
+from ..l4d2_utils.seach import *
 from ..l4d2_data.players import L4D2Player
 from ..l4d2_image import out_png
 # from .anne_telecom import ANNE_API
 
 
 s = L4D2Player()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import httpx
 from bs4 import BeautifulSoup
 import json
 from pathlib import Path
-from ..config import TEXT_PATH,anne_url,ANNE_IP,gamemode_list
+from ..l4d2_utils.config import TEXT_PATH,anne_url,ANNE_IP,gamemode_list
 from ..l4d2_queries.ohter import ALL_HOST
 
 # 储存anne服务器ip
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..config import (
+from ..l4d2_utils.config import (
     DATASQLITE,
     table_data,
     L4d2_players_tag,
     L4d2_server_tag,
     L4d2_INTEGER,
     L4d2_TEXT,
     L4d2_BOOLEAN,
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..config import DATASQLITE
+from ..l4d2_utils.config import DATASQLITE
 import sqlite3
 from typing import Union,Tuple
 
 
 class L4D2Player:
     """数据库L4D2_Player表的操作""" 
     def __init__(self):
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..config import DATASQLITE
+from ..l4d2_utils.config import DATASQLITE
 import sqlite3
 
 
 class L4D2Server():
     """数据库L4D2_server表的操作""" 
     def __init__(self):
         """连接数据库"""
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from zipfile import ZipFile
 from time import sleep
 import sys
 import os
 import io
 from typing import List
 
-from ..utils import get_file,get_vpk
-from ..config import systems
+from ..l4d2_utils.utils import get_file,get_vpk
+from ..l4d2_utils.config import systems
 from nonebot.log import logger
 from rarfile import RarFile
 import rarfile
 from pyunpack import Archive
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 
 from bs4 import BeautifulSoup
+import jinja2
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
 from typing import List,Optional
+
+
 # from .htmlimg import dict_to_dict_img
 # from ..l4d2_anne.anne_telecom import ANNE_API
-from ..config import TEXT_PATH
+from ..l4d2_utils.config import TEXT_PATH
 from .download import get_head_by_user_id_and_save
 from .send_image_tool import convert_img
-import jinja2
-from ..config import l4_config
+
+from ..l4d2_utils.config import l4_config
 template_path = TEXT_PATH/"template"
 
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 
 async def out_png(usr_id,data_dict:dict):
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.log import logger
 import asyncio
 import hashlib
 import os
 import random
 from PIL import Image,ImageDraw
 import io
-from ..config import PLAYERSDATA,TEXT_PATH
+from ..l4d2_utils.config import PLAYERSDATA,TEXT_PATH
 # from .steam import web_player
 
 async def download_url(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
         for i in range(3):
             try:
                 resp = await client.get(url, timeout=20)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ..l4d2_data.serverip import L4D2Server
 from ..l4d2_image import server_ip_pic
 from . import queries,player_queries,queries_dict,player_queries_anne_dict,msg_ip_to_list,server_rule_dict
 from nonebot.log import logger
 import random
 import asyncio
 import re
-from ..message import PRISON,QUEREN,KAILAO
+from ..l4d2_utils.message import PRISON,QUEREN,KAILAO
 from .ohter import ALL_HOST
 from typing import List,Dict
 try:
     import ujson as json
 except:
     import json
 si = L4D2Server()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rcon.source import rcon
 import asyncio
 from pathlib import Path
-from ..config import l4_config,CHECK_FILE
+from ..l4d2_utils.config import l4_config,CHECK_FILE
 # from ..config import l4_rcon,l4_host,l4_port,l4_rcon
 
 
 async def rcon_server(PASSWORD:str,msg:str):
     # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=PASSWORD,encoding='utf-8')
     # return response
     try:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import RegexGroup
 from nonebot.permission import SUPERUSER
 from nonebot import get_bot, on_regex, get_driver, on_command
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, MessageSegment
 
-from ..utils import register_menu
-from ..rule import FullCommand
+from ..l4d2_utils.utils import register_menu
+from ..l4d2_utils.rule import FullCommand
 from .draw_update_log import draw_update_log_img
 from .restart import restart_message, restart_genshinuid
 
 l4d_restart = on_command('l4重启', rule=FullCommand())
 get_update_log = on_command('更新记录', rule=FullCommand())
 l4d_update = on_regex(
-    r'^(l4d)(强行)?(强制)?(更新)$',
+    r'^(l4)(强行)?(强制)?(更新)$',
     block=True,
 )
 
 
 driver = get_driver()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
 from jose import jwt
 from nonebot import get_bot, get_app
 
 from pathlib import Path
 
 from nonebot import get_driver, logger
-from ..config import *
-from ..utils import split_maohao
+from ..l4d2_utils.config import *
+from ..l4d2_utils.utils import split_maohao
 from ..l4d2_queries.qqgroup import qq_ip_querie
 CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
 
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 
@@ -135,15 +135,15 @@
                 'status': -100,
                 'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
             }
             
     @app.get('/l4d2/api/get_query_contexts', response_class=JSONResponse, dependencies=[authentication()])
     async def get_query_context():
         try:
-            from ..command import ALL_HOST
+            from ..l4d2_utils.command import ALL_HOST
             this_ips = ALL_HOST
             ip_lists = []
             for ip_list, v in this_ips.items():
                 for d in v:
                     host, port = split_maohao(d['ip'])
                     ip_lists.append((d['id'], ip_list, host, port))
             data_dict = await qq_ip_querie(ip_lists)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from amis import  ActionType, TableCRUD, TableColumn
 from amis import  PageSchema, Switch, InputNumber, InputTag, Action, App
 from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper
 from amis import LevelEnum, Select,  Alert, Tpl, Flex
 
 
-from ..config import NICKNAME
+from ..l4d2_utils.config import NICKNAME
 
 logo = Html(html='''
 <p align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
         <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
          width="256" height="256" alt="l4d2-server">
     </a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 from amis import ActionType, TableCRUD, TableColumn from amis import
 PageSchema, Switch, InputNumber, InputTag, Action, App from amis import Form,
 InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page,
 AmisAPI, Wrapper from amis import LevelEnum, Select, Alert, Tpl, Flex from
-..config import NICKNAME logo = Html(html='''
+..l4d2_utils.config import NICKNAME logo = Html(html='''
                                  [l4d2-server]
               ****** Nonebot-Plugin-L4d2-Server æ§å¶å° ******
                                  Githubä»åº
 
 
 ''') login_api = AmisAPI( url='/l4d2/api/login', method='post', adaptor=''' if
 (payload.status == 0) { localStorage.setItem("token", payload.data.token); }
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import BytesIO
 from PIL import Image, ImageDraw, ImageFont
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot_plugin_txt2img import Txt2Img
-from .config import l4_config
+from l4d2_utils.config import l4_config
 
 l4_font = l4_config.l4_font
 """直接超的智障回复"""
 def txt_to_img(text: str, font_size=30, font_path=l4_font) -> bytes:
     text = line_break(text)
     d_font = ImageFont.truetype(font_path, font_size)
     lines = text.count('\n')  # 计算行数
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.5.3.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import httpx
 import os
 from pathlib import Path
 
 from typing import List,Dict,Union,Optional
 from .txt_to_img import txt_to_img
 from .config import *
-from .l4d2_anne import write_player,del_player,anne_messgae
-from .l4d2_server.rcon import read_server_cfg_rcon,rcon_server
-from .l4d2_queries import queries,player_queries
-from .l4d2_queries.qqgroup import *
-from .l4d2_server.workshop import workshop_to_dict
-from .l4d2_image.steam import url_to_byte
+from ..l4d2_anne import write_player,del_player,anne_messgae
+from ..l4d2_server.rcon import read_server_cfg_rcon,rcon_server
+from ..l4d2_queries import queries,player_queries
+from ..l4d2_queries.qqgroup import *
+from ..l4d2_server.workshop import workshop_to_dict
+from ..l4d2_image.steam import url_to_byte
 import tempfile
 import random
 
 
 
 async def get_file(url: str, down_file: Path):
     '''
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.3"
+version = "0.5.3.1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.3
+Version: 0.5.3.1
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.3 Summary:
-L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.3.1
+Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```


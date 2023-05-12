# Comparing `tmp/exceptnotifier-0.2.6.tar.gz` & `tmp/exceptnotifier-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.2.6.tar", last modified: Fri May 12 10:55:29 2023, max compression
+gzip compressed data, was "exceptnotifier-0.2.7.tar", last modified: Fri May 12 16:04:12 2023, max compression
```

## Comparing `exceptnotifier-0.2.6.tar` & `exceptnotifier-0.2.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.282724 exceptnotifier-0.2.6/
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.150112 exceptnotifier-0.2.6/ExceptNotifier/
--rw-rw-rw-   0        0        0     4847 2023-05-12 10:35:56.000000 exceptnotifier-0.2.6/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.211428 exceptnotifier-0.2.6/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1382 2023-05-12 10:54:50.000000 exceptnotifier-0.2.6/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-05-12 10:41:13.000000 exceptnotifier-0.2.6/ExceptNotifier/base/bard_receiver.py
--rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.6/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.6/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.6/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0     1009 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.6/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.6/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.6/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.6/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.6/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.6/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.6/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.6/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.6/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.6/ExceptNotifier/base/whatsapp_sender.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.238352 exceptnotifier-0.2.6/ExceptNotifier/ipycore/
--rw-rw-rw-   0        0        0     1472 2023-05-12 10:36:00.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/__init__.py
--rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/beep_notifier_ipython.py
--rw-rw-rw-   0        0        0     2578 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/chime_notifier_ipython.py
--rw-rw-rw-   0        0        0     2947 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/desktop_notifier_ipython.py
--rw-rw-rw-   0        0        0     2590 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/discord_notifier_ipython.py
--rw-rw-rw-   0        0        0     2570 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/kakao_notifier_ipython.py
--rw-rw-rw-   0        0        0     2584 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/line_notifier_ipython.py
--rw-rw-rw-   0        0        0     4013 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/mail_notifier_ipython.py
--rw-rw-rw-   0        0        0     2577 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/slack_notifier_ipython.py
--rw-rw-rw-   0        0        0     3049 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/sms_notifier_ipython.py
--rw-rw-rw-   0        0        0     2581 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/teams_notifier_ipython.py
--rw-rw-rw-   0        0        0     2583 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/telegram_notifier_ipython.py
--rw-rw-rw-   0        0        0     2591 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/wechat_notifier_ipython.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.271804 exceptnotifier-0.2.6/ExceptNotifier/pycore/
--rw-rw-rw-   0        0        0     2009 2023-05-12 10:54:52.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/beep_notifier.py
--rw-rw-rw-   0        0        0     7700 2023-05-12 10:13:08.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/chime_notifier.py
--rw-rw-rw-   0        0        0     7277 2023-05-12 10:13:17.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/desktop_notifier.py
--rw-rw-rw-   0        0        0     8013 2023-05-12 10:13:29.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/discord_notifier.py
--rw-rw-rw-   0        0        0     8080 2023-05-12 10:13:41.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/kakao_notifier.py
--rw-rw-rw-   0        0        0     7652 2023-05-12 10:13:54.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/line_notifier.py
--rw-rw-rw-   0        0        0    10267 2023-05-12 10:16:36.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/mail_notifier.py
--rw-rw-rw-   0        0        0     7606 2023-05-12 10:14:40.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/slack_notifier.py
--rw-rw-rw-   0        0        0     9034 2023-05-12 10:16:08.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/sms_notifier.py
--rw-rw-rw-   0        0        0     7588 2023-05-12 10:16:16.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/teams_notifier.py
--rw-rw-rw-   0        0        0     7815 2023-05-12 10:16:22.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/telegram_notifier.py
--rw-rw-rw-   0        0        0     7607 2023-05-12 10:16:28.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.276465 exceptnotifier-0.2.6/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      265 2023-05-12 10:36:03.000000 exceptnotifier-0.2.6/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.6/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.171651 exceptnotifier-0.2.6/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    45493 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2307 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    45493 2023-05-12 10:55:29.281288 exceptnotifier-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    44445 2023-05-12 10:55:07.000000 exceptnotifier-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 10:55:29.282724 exceptnotifier-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-05-12 10:35:52.000000 exceptnotifier-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.182014 exceptnotifier-0.2.7/
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.025685 exceptnotifier-0.2.7/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4847 2023-05-12 16:02:38.000000 exceptnotifier-0.2.7/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.097492 exceptnotifier-0.2.7/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1382 2023-05-12 16:02:41.000000 exceptnotifier-0.2.7/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0     2050 2023-05-12 16:01:41.000000 exceptnotifier-0.2.7/ExceptNotifier/base/bard_receiver.py
+-rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.7/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.7/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.7/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1009 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.7/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.7/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.7/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     2484 2023-05-12 16:01:32.000000 exceptnotifier-0.2.7/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.7/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.7/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.7/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.7/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.7/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.7/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.130072 exceptnotifier-0.2.7/ExceptNotifier/ipycore/
+-rw-rw-rw-   0        0        0     1472 2023-05-12 16:02:44.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2578 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2947 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2590 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2570 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2584 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     4013 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2577 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     3049 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2581 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2583 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2591 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/ipycore/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.165642 exceptnotifier-0.2.7/ExceptNotifier/pycore/
+-rw-rw-rw-   0        0        0     2009 2023-05-12 16:02:46.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-05-12 05:17:37.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/beep_notifier.py
+-rw-rw-rw-   0        0        0     7700 2023-05-12 10:13:08.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/chime_notifier.py
+-rw-rw-rw-   0        0        0     7277 2023-05-12 10:13:17.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/desktop_notifier.py
+-rw-rw-rw-   0        0        0     8013 2023-05-12 10:13:29.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/discord_notifier.py
+-rw-rw-rw-   0        0        0     8080 2023-05-12 10:13:41.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/kakao_notifier.py
+-rw-rw-rw-   0        0        0     7652 2023-05-12 10:13:54.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/line_notifier.py
+-rw-rw-rw-   0        0        0    10267 2023-05-12 10:16:36.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/mail_notifier.py
+-rw-rw-rw-   0        0        0     7606 2023-05-12 10:14:40.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/slack_notifier.py
+-rw-rw-rw-   0        0        0     9034 2023-05-12 10:16:08.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/sms_notifier.py
+-rw-rw-rw-   0        0        0     7588 2023-05-12 10:16:16.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/teams_notifier.py
+-rw-rw-rw-   0        0        0     7815 2023-05-12 10:16:22.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/telegram_notifier.py
+-rw-rw-rw-   0        0        0     7607 2023-05-12 10:16:28.000000 exceptnotifier-0.2.7/ExceptNotifier/pycore/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.176009 exceptnotifier-0.2.7/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      265 2023-05-12 16:02:50.000000 exceptnotifier-0.2.7/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.7/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:04:12.054991 exceptnotifier-0.2.7/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    45493 2023-05-12 16:04:11.000000 exceptnotifier-0.2.7/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2023-05-12 16:04:12.000000 exceptnotifier-0.2.7/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:04:11.000000 exceptnotifier-0.2.7/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-12 16:04:11.000000 exceptnotifier-0.2.7/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 16:04:11.000000 exceptnotifier-0.2.7/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 16:04:11.000000 exceptnotifier-0.2.7/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    45493 2023-05-12 16:04:12.181014 exceptnotifier-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    44445 2023-05-12 16:02:11.000000 exceptnotifier-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 16:04:12.182014 exceptnotifier-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-05-12 16:02:32.000000 exceptnotifier-0.2.7/setup.py
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/__init__.py` & `exceptnotifier-0.2.7/ExceptNotifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,9 +127,9 @@
     "ExceptMailIpython",
     "ExceptSlackIpython",
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
 ]
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     "send_whatsapp_msg",
     "send_sms_msg",
     "beep",
     "receive_openai_advice",
     "get_resp_openai_advice",
 ]
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/bard_receiver.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/bard_receiver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import bardapi
-import os
+from os import environ 
 
 
 def receive_bard_advice(_BARD_API_KEY: str, error_message: str) -> str:
     """Receive debugging information about your code from google bard.
     :param _OPEN_AI_API:__Secure-1PSID value of google bard
     :type _OPEN_AI_API: str
     :param error_message: Error message
     :type error_message: str
     :return: Returns a description and example of the code, the location of the error, and a debugging code example.
     :rtype: str
     """
-    os.environ["_BARD_API_KEY"] = _BARD_API_KEY
-    if os.environ["_BARD_ADVICE_LANG"]=='ko':
-        input_text = f"다음 error를 어떻게 고칠 수 있을까? 다음 에러에 대해서 설명해주고, 어떤 위치에서 어떤 코드가 잘못 되었는지 말해줘. 그리고 이 코드를 고칠 수 있는 예시 코드를 보여줘 error=={error_message}"
-    elif os.environ["_BARD_ADVICE_LANG"]=='jp':
-        input_text = f"次のエラーをどのように修正できますか？次のエラーについて説明し、どの場所でどのコードが間違っているかを教えてください。そして、このコードを修正できるサンプルコードを見せてください。 error=={error_message}"
+    environ["_BARD_API_KEY"] = _BARD_API_KEY
+
+    if environ.get("_PROMPT_COMMAND") is None:
+        if environ["_BARD_ADVICE_LANG"]=='ko':
+            input_text = f"다음 error를 어떻게 고칠 수 있을까? 다음 에러에 대해서 설명해주고, 어떤 위치에서 어떤 코드가 잘못 되었는지 말해줘. 그리고 이 코드를 고칠 수 있는 예시 코드를 보여줘 error=={error_message}"
+        elif environ["_BARD_ADVICE_LANG"]=='jp':
+            input_text = f"次のエラーをどのように修正できますか？次のエラーについて説明し、どの場所でどのコードが間違っているかを教えてください。そして、このコードを修正できるサンプルコードを見せてください。 error=={error_message}"
+        else:
+            input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix example. error=={error_message}"
     else:
-        input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix example. error=={error_message}"
-    
+        input_text = f"{environ['_PROMPT_COMMAND']} error=={error_message}" 
+
     response = bardapi.core.Bard().get_answer(input_text)
     advice_msg = response["content"]
 
     return advice_msg
 
 
 # if __name__ == "__main__":
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/discord_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/openai_receiver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import openai
-
+from os import environ
 
 def receive_openai_advice(
     _OPEN_AI_MODEL: str, _OPEN_AI_API: str, error_message: str
 ) -> str:
     """Receive debugging information about your code from models in open ai.
 
     :param _OPEN_AI_MODEL: model name of open ai
@@ -17,15 +17,18 @@
     :return: Returns a description and example of the code, the location of the error, and a debugging code example.
     :rtype: str
     """
 
     openai.api_key = _OPEN_AI_API
     model_engine = _OPEN_AI_MODEL
 
-    input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix exampel. error== {error_message}"
+    if environ.get("_PROMPT_COMMAND") is None:
+        input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix exampel. error== {error_message}"
+    else:
+        input_text = f"{environ['_PROMPT_COMMAND']} error=={error_message}" 
     resp = openai.ChatCompletion.create(
         model=model_engine, messages=[{"role": "user", "content": input_text}]
     )
     advice_msg = resp["choices"][0]["message"]["content"]
     return advice_msg
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/wechat_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.2.7/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/__init__.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
 ]
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/beep_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/beep_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/chime_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/chime_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/desktop_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/desktop_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/discord_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/discord_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/kakao_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/kakao_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/line_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/line_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/mail_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/mail_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/slack_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/slack_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/sms_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/sms_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/teams_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/teams_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/telegram_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/telegram_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/ipycore/wechat_notifier_ipython.py` & `exceptnotifier-0.2.7/ExceptNotifier/ipycore/wechat_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/__init__.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     "ExceptWechat",
     "SendWechat",
     "SuccessDesktop",
     "ExceptDesktop",
     "SendDesktop",
 ]
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/beep_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/chime_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/chime_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/desktop_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/desktop_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/discord_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/discord_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/kakao_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/kakao_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/line_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/line_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/mail_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/slack_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/sms_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/teams_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/telegram_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/pycore/wechat_notifier.py` & `exceptnotifier-0.2.7/ExceptNotifier/pycore/wechat_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.2.7/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.2.7/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.6
+Version: 0.2.7
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -107,15 +107,15 @@
   * [Sender in Ipython](#sender-in-ipython)
 <br>
 
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
-    + [c. Notifier with Google Bard API](#b-notifier-with-google-bard-api)
+    + [c. Notifier with Google Bard API](#c-notifier-with-google-bard-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
   * [*Slack*](#slack)
   * [*Line*](#line)
   * [*SMS*](#sms)
   * [*Teams*](#teams)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.6 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.7 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -72,15 +72,15 @@
 - [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
 (#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
 in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
 in Ipython](#sender-in-ipython)
 - [Applied in each application](#applied-in-each-application) * [*Telegram*]
 (#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
 + [b. Notifier with OpenAI API](#b-notifier-with-openai-api) + [c. Notifier
-with Google Bard API](#b-notifier-with-google-bard-api) * [*Mail*](#mail) *
+with Google Bard API](#c-notifier-with-google-bard-api) * [*Mail*](#mail) *
 [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line)
 * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*]
 (#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide]
 (#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
 conduct) - [Contacts](#contacts)
```

### Comparing `exceptnotifier-0.2.6/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.2.7/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/LICENSE` & `exceptnotifier-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.6/PKG-INFO` & `exceptnotifier-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.6
+Version: 0.2.7
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -107,15 +107,15 @@
   * [Sender in Ipython](#sender-in-ipython)
 <br>
 
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
-    + [c. Notifier with Google Bard API](#b-notifier-with-google-bard-api)
+    + [c. Notifier with Google Bard API](#c-notifier-with-google-bard-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
   * [*Slack*](#slack)
   * [*Line*](#line)
   * [*SMS*](#sms)
   * [*Teams*](#teams)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.6 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.7 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -72,15 +72,15 @@
 - [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
 (#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
 in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
 in Ipython](#sender-in-ipython)
 - [Applied in each application](#applied-in-each-application) * [*Telegram*]
 (#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
 + [b. Notifier with OpenAI API](#b-notifier-with-openai-api) + [c. Notifier
-with Google Bard API](#b-notifier-with-google-bard-api) * [*Mail*](#mail) *
+with Google Bard API](#c-notifier-with-google-bard-api) * [*Mail*](#mail) *
 [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line)
 * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*]
 (#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide]
 (#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
 conduct) - [Contacts](#contacts)
```

### Comparing `exceptnotifier-0.2.6/README.md` & `exceptnotifier-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
   * [Sender in Ipython](#sender-in-ipython)
 <br>
 
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
-    + [c. Notifier with Google Bard API](#b-notifier-with-google-bard-api)
+    + [c. Notifier with Google Bard API](#c-notifier-with-google-bard-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
   * [*Slack*](#slack)
   * [*Line*](#line)
   * [*SMS*](#sms)
   * [*Teams*](#teams)
```

#### html2text {}

```diff
@@ -58,15 +58,15 @@
 - [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
 (#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
 in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
 in Ipython](#sender-in-ipython)
 - [Applied in each application](#applied-in-each-application) * [*Telegram*]
 (#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
 + [b. Notifier with OpenAI API](#b-notifier-with-openai-api) + [c. Notifier
-with Google Bard API](#b-notifier-with-google-bard-api) * [*Mail*](#mail) *
+with Google Bard API](#c-notifier-with-google-bard-api) * [*Mail*](#mail) *
 [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line)
 * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*]
 (#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide]
 (#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
 conduct) - [Contacts](#contacts)
```

### Comparing `exceptnotifier-0.2.6/setup.py` & `exceptnotifier-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.2.6",
+    version="0.2.7",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```


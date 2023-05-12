# Comparing `tmp/exceptnotifier-0.2.4.tar.gz` & `tmp/exceptnotifier-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.2.4.tar", last modified: Mon Apr 24 16:22:10 2023, max compression
+gzip compressed data, was "exceptnotifier-0.2.5.tar", last modified: Fri May 12 10:20:32 2023, max compression
```

## Comparing `exceptnotifier-0.2.4.tar` & `exceptnotifier-0.2.5.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.703632 exceptnotifier-0.2.4/
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.541040 exceptnotifier-0.2.4/ExceptNotifier/
--rw-rw-rw-   0        0        0     4748 2023-04-24 16:21:28.000000 exceptnotifier-0.2.4/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.614047 exceptnotifier-0.2.4/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1382 2023-04-24 16:21:30.000000 exceptnotifier-0.2.4/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.4/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.4/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.4/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0     1005 2023-04-24 14:23:06.000000 exceptnotifier-0.2.4/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.4/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.4/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.4/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.4/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.4/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.4/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.4/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.4/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.4/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.4/ExceptNotifier/base/whatsapp_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.648251 exceptnotifier-0.2.4/ExceptNotifier/ipycore/
--rw-rw-rw-   0        0        0     1472 2023-04-24 16:21:35.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/__init__.py
--rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/beep_notifier_ipython.py
--rw-rw-rw-   0        0        0     2104 2023-04-24 13:50:33.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/chime_notifier_ipython.py
--rw-rw-rw-   0        0        0     2509 2023-04-24 15:05:53.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/desktop_notifier_ipython.py
--rw-rw-rw-   0        0        0     2114 2023-04-24 13:49:34.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/discord_notifier_ipython.py
--rw-rw-rw-   0        0        0     2101 2023-04-24 13:43:54.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/kakao_notifier_ipython.py
--rw-rw-rw-   0        0        0     2109 2023-04-24 13:43:24.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/line_notifier_ipython.py
--rw-rw-rw-   0        0        0     2813 2023-04-24 16:21:00.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/mail_notifier_ipython.py
--rw-rw-rw-   0        0        0     2105 2023-04-24 13:42:15.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/slack_notifier_ipython.py
--rw-rw-rw-   0        0        0     2390 2023-04-24 13:41:15.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/sms_notifier_ipython.py
--rw-rw-rw-   0        0        0     2109 2023-04-24 13:40:55.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/teams_notifier_ipython.py
--rw-rw-rw-   0        0        0     2111 2023-04-24 13:41:38.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/telegram_notifier_ipython.py
--rw-rw-rw-   0        0        0     2032 2023-04-24 13:41:53.000000 exceptnotifier-0.2.4/ExceptNotifier/ipycore/wechat_notifier_ipython.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.684739 exceptnotifier-0.2.4/ExceptNotifier/pycore/
--rw-rw-rw-   0        0        0     2009 2023-04-24 16:21:37.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/__init__.py
--rw-rw-rw-   0        0        0     2257 2023-04-24 13:57:14.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/beep_notifier.py
--rw-rw-rw-   0        0        0     6879 2023-04-24 13:58:46.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/chime_notifier.py
--rw-rw-rw-   0        0        0     6395 2023-04-24 14:24:50.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/desktop_notifier.py
--rw-rw-rw-   0        0        0     7190 2023-04-24 14:12:17.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/discord_notifier.py
--rw-rw-rw-   0        0        0     7260 2023-04-24 14:15:48.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/kakao_notifier.py
--rw-rw-rw-   0        0        0     6804 2023-04-24 14:17:18.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/line_notifier.py
--rw-rw-rw-   0        0        0     8862 2023-04-24 11:11:19.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/mail_notifier.py
--rw-rw-rw-   0        0        0     6786 2023-04-24 14:17:53.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/slack_notifier.py
--rw-rw-rw-   0        0        0     8002 2023-04-24 14:23:54.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/sms_notifier.py
--rw-rw-rw-   0        0        0     6767 2023-04-24 15:06:20.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/teams_notifier.py
--rw-rw-rw-   0        0        0     6994 2023-04-24 14:21:11.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/telegram_notifier.py
--rw-rw-rw-   0        0        0     6784 2023-04-24 14:21:51.000000 exceptnotifier-0.2.4/ExceptNotifier/pycore/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.696429 exceptnotifier-0.2.4/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      265 2023-04-24 16:21:40.000000 exceptnotifier-0.2.4/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.4/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:22:10.572765 exceptnotifier-0.2.4/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    34802 2023-04-24 16:22:10.000000 exceptnotifier-0.2.4/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-04-24 16:22:10.000000 exceptnotifier-0.2.4/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 16:22:10.000000 exceptnotifier-0.2.4/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-24 16:22:10.000000 exceptnotifier-0.2.4/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 16:22:10.000000 exceptnotifier-0.2.4/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-24 16:22:10.000000 exceptnotifier-0.2.4/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    34802 2023-04-24 16:22:10.702619 exceptnotifier-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    33754 2023-04-24 16:03:08.000000 exceptnotifier-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 16:22:10.703632 exceptnotifier-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-04-24 16:21:22.000000 exceptnotifier-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.401742 exceptnotifier-0.2.5/
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.256895 exceptnotifier-0.2.5/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4847 2023-05-12 10:19:31.000000 exceptnotifier-0.2.5/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.318189 exceptnotifier-0.2.5/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1382 2023-05-12 10:19:43.000000 exceptnotifier-0.2.5/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0     1174 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/base/bard_receiver.py
+-rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.5/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.5/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.5/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1009 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.5/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.5/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.5/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.5/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.5/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.5/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.5/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.5/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.5/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.5/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.351176 exceptnotifier-0.2.5/ExceptNotifier/ipycore/
+-rw-rw-rw-   0        0        0     1472 2023-05-12 10:19:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2578 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2947 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2590 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2570 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2584 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     4013 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2577 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     3049 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2581 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2583 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2591 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.384815 exceptnotifier-0.2.5/ExceptNotifier/pycore/
+-rw-rw-rw-   0        0        0     2009 2023-05-12 10:20:13.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/beep_notifier.py
+-rw-rw-rw-   0        0        0     7700 2023-05-12 10:13:08.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/chime_notifier.py
+-rw-rw-rw-   0        0        0     7277 2023-05-12 10:13:17.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/desktop_notifier.py
+-rw-rw-rw-   0        0        0     8013 2023-05-12 10:13:29.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/discord_notifier.py
+-rw-rw-rw-   0        0        0     8080 2023-05-12 10:13:41.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/kakao_notifier.py
+-rw-rw-rw-   0        0        0     7652 2023-05-12 10:13:54.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/line_notifier.py
+-rw-rw-rw-   0        0        0    10267 2023-05-12 10:16:36.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/mail_notifier.py
+-rw-rw-rw-   0        0        0     7606 2023-05-12 10:14:40.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/slack_notifier.py
+-rw-rw-rw-   0        0        0     9034 2023-05-12 10:16:08.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/sms_notifier.py
+-rw-rw-rw-   0        0        0     7588 2023-05-12 10:16:16.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/teams_notifier.py
+-rw-rw-rw-   0        0        0     7815 2023-05-12 10:16:22.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/telegram_notifier.py
+-rw-rw-rw-   0        0        0     7607 2023-05-12 10:16:28.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.394182 exceptnotifier-0.2.5/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      265 2023-05-12 10:19:40.000000 exceptnotifier-0.2.5/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.5/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.279040 exceptnotifier-0.2.5/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    42887 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    42887 2023-05-12 10:20:32.400730 exceptnotifier-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    41839 2023-05-11 20:54:05.000000 exceptnotifier-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:20:32.402739 exceptnotifier-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-05-12 10:18:36.000000 exceptnotifier-0.2.5/setup.py
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/__init__.py` & `exceptnotifier-0.2.5/ExceptNotifier/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,19 @@
 from ExceptNotifier.ipycore.slack_notifier_ipython import ExceptSlackIpython
 from ExceptNotifier.ipycore.sms_notifier_ipython import ExceptSMSIpython
 from ExceptNotifier.ipycore.teams_notifier_ipython import ExceptTeamsIpython
 from ExceptNotifier.ipycore.wechat_notifier_ipython import ExceptWechatIpython
 from ExceptNotifier.ipycore.beep_notifier_ipython import ExceptBeepIpython
 from ExceptNotifier.ipycore.desktop_notifier_ipython import ExceptDesktopIpython
 
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
+
+
 __all__ = [
+    "receive_bard_advice",
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
     "get_resp_openai_advice",
     "SuccessMail",
     "ExceptMail",
     "SendMail",
     "SuccessSlack",
@@ -123,9 +127,9 @@
     "ExceptMailIpython",
     "ExceptSlackIpython",
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
 ]
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     "send_whatsapp_msg",
     "send_sms_msg",
     "beep",
     "receive_openai_advice",
     "get_resp_openai_advice",
 ]
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/discord_sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,22 @@
     :param msg: Message text
     :type msg: str
     :return: Response according to REST API request
     :rtype: dict
     """
     try:
         from discord import Webhook, RequestsWebhookAdapter
+
         webhook = Webhook.from_url(
             _DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter()
         )
         resp = webhook.send(msg)
     except:
         from discord import SyncWebhook
+
         webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL)  # Initializing webhook
         resp = webhook.send(content=msg[:1900])
     return resp
 
 
 # if __name__ == "__main__":
 #     _DISCORD_WEBHOOK_URL = "xxxxx"
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/wechat_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.2.5/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/__init__.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
 ]
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/beep_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/beep_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/chime_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/telegram_notifier_ipython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.chime_sender import send_chime_msg
+from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptChimeIpython(
+def ExceptTelegramIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Chime message.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Telegram.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -27,22 +28,30 @@
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
-        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
-    if environ.get('_OPEN_AI_API') is not None:
+    send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
-            send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+            send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
+
+        except Exception as e:
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
 
         except Exception as e:
-            print(e)
             pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/desktop_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/desktop_notifier_ipython.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.desktop_sender import send_desktop_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptDesktopIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
@@ -35,18 +35,25 @@
         "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
     data["head"] = "[Except Notifier] :warning: Error! Python Code Exception Detected."
     data[
         "body"
     ] = f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     send_desktop_msg(data["head"], data["body"])
-    if environ.get('_OPEN_AI_API') is not None:
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
-            send_desktop_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+            send_desktop_msg(data["head"], advice_msg)
+
+        except Exception as e:
+            pass
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_desktop_msg(data["head"], advice_msg)
 
         except Exception as e:
-            print(e)
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/discord_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/chime_notifier_ipython.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.discord_sender import send_discord_msg
+from ExceptNotifier.base.chime_sender import send_chime_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptDiscordIpython(
+def ExceptChimeIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Discord.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Chime message.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -31,19 +31,27 @@
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
 
-    send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"])
-    if environ.get('_OPEN_AI_API') is not None:
+    send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
-            send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
+            send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
 
         except Exception as e:
-            print(e)
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/kakao_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/kakao_notifier_ipython.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptKakaoIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
@@ -32,18 +32,25 @@
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
     send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
-    if environ.get('_OPEN_AI_API') is not None:
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
             send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], advice_msg)
 
         except Exception as e:
-            print(e)
+            pass
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], advice_msg)
+
+        except Exception as e:
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/line_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/teams_notifier_ipython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.line_sender import send_line_msg
+from ExceptNotifier.base.teams_sender import send_teams_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptLineIpython(
+def ExceptTeamsIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Line message.
+    """ExceptNotifier function for overriding custom execute in ipython for sending teams message.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
     :param tb: TraceBack object of Ipython
     :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
+
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
+    send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
-    send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
-    if environ.get('_OPEN_AI_API') is not None:
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
-            send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
+            send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
 
         except Exception as e:
-            print(e)
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/mail_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/sms_notifier_ipython.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
-import smtplib
-import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-from ExceptNotifier.base.mail_sender import send_gmail_msg
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptMailIpython(
+def ExceptSMSIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Gmail.
+    """ExceptNotifier function for overriding custom execute in ipython for sending SMS.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
     :param tb: TraceBack object of Ipython
     :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    SMTP_SERVER = "smtp.gmail.com"
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    exceptNotifier = {
-        "TO": environ["_GAMIL_RECIPIENT_ADDR"],
-        "FROM": environ["_GMAIL_SENDER_ADDR"],
-        "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected.",
-        "BODY": f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}",
+    data = {
+        "text": f"[Except Notifier] ** Error ** Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}"
     }
-    send_gmail_msg(environ['_GMAIL_SENDER_ADDR'], environ['_GAMIL_RECIPIENT_ADDR'], environ['_GMAIL_APP_PASSWORD_OF_SENDER'], exceptNotifier['SUBJECT'], exceptNotifier['BODY'])
 
-    if environ.get('_OPEN_AI_API') is not None:
+    send_sms_msg(
+        environ["_TWILIO_SID"],
+        environ["_TWILIO_TOKEN"],
+        environ["_SENDER_PHONE_NUMBER"],
+        environ["_RECIPIENT_PHONE_NUMBER"],
+        data["text"],
+    )
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
-                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message,
-            )  # NO-QA
-            exceptNotifier_openai = {
-                "SUBJECT": "[Except AI Debugging] Error! chatGPT Debugging guide.",
-                "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}",
-            }
-            send_gmail_msg(environ['_GMAIL_SENDER_ADDR'], environ['_GAMIL_RECIPIENT_ADDR'], environ['_GMAIL_APP_PASSWORD_OF_SENDER'], exceptNotifier_openai['SUBJECT'], exceptNotifier_openai['BODY'])
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_sms_msg(
+                environ["_TWILIO_SID"],
+                environ["_TWILIO_TOKEN"],
+                environ["_SENDER_PHONE_NUMBER"],
+                environ["_RECIPIENT_PHONE_NUMBER"],
+                advice_msg,
+            )
+        except Exception as e:
+            pass
 
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_sms_msg(
+                environ["_TWILIO_SID"],
+                environ["_TWILIO_TOKEN"],
+                environ["_SENDER_PHONE_NUMBER"],
+                environ["_RECIPIENT_PHONE_NUMBER"],
+                advice_msg,
+            )
 
         except Exception as e:
-            print(e)
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/slack_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/slack_notifier_ipython.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 from os import environ
 import datetime
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.slack_sender import send_slack_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptSlackIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
@@ -32,18 +32,26 @@
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
 
     send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
-    if environ.get('_OPEN_AI_API') is not None:
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
             send_slack_msg(environ["_SLACK_WEBHOOK_URL"], advice_msg)
 
         except Exception as e:
-            print(e)
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_slack_msg(environ["_SLACK_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/teams_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/line_notifier_ipython.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.teams_sender import send_teams_msg
+from ExceptNotifier.base.line_sender import send_line_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptTeamsIpython(
+def ExceptLineIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending teams message.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Line message.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
     :param tb: TraceBack object of Ipython
     :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
-    send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
-    if environ.get('_OPEN_AI_API') is not None:
+    send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
-            send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+            send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
+
+        except Exception as e:
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
 
         except Exception as e:
-            print(e)
             pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/telegram_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/discord_notifier_ipython.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.telegram_sender import send_telegram_msg
+from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptTelegramIpython(
+def ExceptDiscordIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Telegram.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Discord.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -28,22 +28,30 @@
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
-        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
 
-    send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
-    if environ.get('_OPEN_AI_API') is not None:
+    send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"])
+    if environ.get("_OPEN_AI_API") is not None:
         try:
             error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
             advice_msg = receive_openai_advice(
                 environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
             )
-            send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
+            send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
 
         except Exception as e:
-            print(e)
             pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/ipycore/wechat_notifier_ipython.py` & `exceptnotifier-0.2.5/ExceptNotifier/ipycore/wechat_notifier_ipython.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import datetime
 from os import environ
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptWechatIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
@@ -33,17 +33,26 @@
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
     send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
-        )
-        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    if environ.get("_OPEN_AI_API") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            pass
+
+    if environ.get("_BARD_API_KEY") is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_bard_advice(environ["_BARD_API_KEY"], error_message)
+            send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            pass
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/__init__.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     "ExceptWechat",
     "SendWechat",
     "SuccessDesktop",
     "ExceptDesktop",
     "SendDesktop",
 ]
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/beep_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/beep_notifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     :type tb: _type_
     """
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        if environ.get('BEEP_TIME') is not None:
+        if environ.get("BEEP_TIME") is not None:
             beep(environ["BEEP_TIME"])
             beep(environ["BEEP_TIME"])
             beep(environ["BEEP_TIME"])
         else:
             beep()
             beep()
             beep()
@@ -54,30 +54,31 @@
     """Success beep
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
-        if environ.get('BEEP_TIME') is not None:
+        if environ.get("BEEP_TIME") is not None:
             beep(environ["BEEP_TIME"])
             beep(environ["BEEP_TIME"])
         else:
             beep()
             beep()
 
+
 class SendBeep:
     """Send beep
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
-        if environ.get('BEEP_TIME') is not None:
+        if environ.get("BEEP_TIME") is not None:
             beep(environ["BEEP_TIME"])
         else:
             beep()
 
 
 # if __name__ == "__main__":
 #     environ['BEEP_TIME'] = 1
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/chime_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/chime_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import urllib3
 import datetime
 import traceback
 from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.chime_sender import send_chime_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptChime(BaseException):
     """Override excepthook to send error message to AWS Chime.
@@ -69,29 +70,44 @@
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
                 )
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
             except Exception as e:
-                print(e)
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_chime_msg(_CHIME_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through chime app's webhook url.
 
         :param _CHIME_WEBHOOK_URL: Webhook url from chime app
@@ -122,15 +138,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 class SendChime:
@@ -145,15 +161,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/desktop_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/desktop_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 import traceback
 from os import environ
 from plyer import notification
 from email.message import EmailMessage
 from ExceptNotifier.base.desktop_sender import send_desktop_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptDesktop(BaseException):
     """Override excepthook to send error message to Desktop.
 
@@ -70,15 +71,15 @@
 
         print(exceptNotifier["BODY"])
 
         send_desktop_msg(
             title=exceptNotifier["SUBJECT"], message=exceptNotifier["BODY"]
         )
 
-        if environ.get('_OPEN_AI_API') is not None:
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
@@ -86,15 +87,32 @@
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_desktop_msg(
                     title="chatGPT: How to Debug your code.", message=advice_msg
                 )
             except Exception as e:
-                print(e)
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_desktop_msg(
+                    title="chatGPT: How to Debug your code.", message=advice_msg
+                )
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_desktop_msg(title_msg: str, body_msg: str, DISP_TIME=5) -> None:
         """Sending notification to desktop
 
         :param title_msg: Title of message
@@ -119,15 +137,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         send_desktop_msg(
             title=exceptNotifier["SUBJECT"][:20], message=exceptNotifier["BODY"][:200]
         )
 
 
 class SendDesktop:
@@ -142,15 +160,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         send_desktop_msg(
             title=exceptNotifier["SUBJECT"][:20], message=exceptNotifier["BODY"][:200]
         )
 
 
 # if __name__ == "__main__":
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/discord_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/discord_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import datetime
 import traceback
 from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptDiscord(BaseException):
     """Override excepthook to send error message to Discord.
 
@@ -68,29 +68,44 @@
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
                 )
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
             except Exception as e:
-                print(e)
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_discord_msg(_DISCORD_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through discord app's webhook url.
 
         :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
@@ -127,15 +142,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
 
 
 class SendDiscord:
     """Sending message to Discord
@@ -149,15 +164,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
 
 
 # if __name__ == "__main__":
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/kakao_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/kakao_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import datetime
 import requests
 import traceback
 from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptKakao(BaseException):
     """Override excepthook to send error message to Kakaotalk.
 
@@ -69,29 +70,44 @@
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
                 )
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], advice_msg)
             except Exception as e:
-                print(e)
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], advice_msg)
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_kakao_msg(_KAKAO_TOKEN_PATH: str, msg: str) -> dict:
         """Send message to chat room through kakaotalk app's REST API.
 
         :param _KAKAO_TOKEN_PATH: Kakaotalk token path
@@ -133,15 +149,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] ** Success! ** Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
 
 
 class SendKakao:
@@ -156,15 +172,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] ** Notice! ** Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         with open(environ["_KAKAO_TOKEN_PATH"], "r") as kakao:
             tokens = json.load(kakao)
 
         send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/line_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/line_notifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import requests
 import traceback
 from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.line_sender import send_line_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptLine(BaseException):
     """Override excepthook to send error message to Line.
 
@@ -69,15 +69,15 @@
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
@@ -85,14 +85,30 @@
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
             except Exception as e:
                 pass
 
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
+            except Exception as e:
+                pass
+
     @staticmethod
     def send_line_msg(_LINE_NOTIFY_API_TOKEN: str, msg: str) -> dict:
         """Send message to chat room through Line app's REST API.
 
         :param _LINE_NOTIFY_API_TOKEN: Line notify API token
         :type _LINE_NOTIFY_API_TOKEN: str
         :param msg: Message text
@@ -120,15 +136,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 class SendLine:
@@ -143,15 +159,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 # if __name__ == "__main__":
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/mail_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/teams_notifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
-import smtplib
+import json
 import datetime
+import requests
 import traceback
+from os import environ
 from email.message import EmailMessage
+from ExceptNotifier.base.teams_sender import send_teams_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptMail(BaseException):
-    """Override excepthook to send error message to Gmail.
+class ExceptTeams(BaseException):
+    """Override excepthook to send error message to Microsoft Teams.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
+        start_time = datetime.datetime.now()
+
         exceptNotifier = {
-            "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
-            "FROM": os.environ["_GMAIL_SENDER_ADDR"],
-            "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected",
-            "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier.\n\n{excType}: %{etype.__doc__}\n\n {value} \n\n",
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
         }
-        SMTP_SERVER = "smtp.gmail.com"
         for line in traceback.extract_tb(tb):
             exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
             )
@@ -51,184 +51,136 @@
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        start_time = datetime.datetime.now()
 
-        exceptNotifier["BODY"] += f"\nTime Stamp: {start_time.strftime(DATE_FORMAT)}"
-        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
+        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
         for frame in stack:
             exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
                 frame.f_code.co_name,
                 frame.f_code.co_filename,
                 frame.f_lineno,
             )
             for key, val in frame.f_locals.items():
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        print(exceptNotifier["BODY"])
-        exceptNotifier["ALL"] = "From: %s\nTo: %s\nSubject: %s\n\n%s" % (
-            exceptNotifier["FROM"],
-            exceptNotifier["TO"],
-            exceptNotifier["SUBJECT"],
-            exceptNotifier["BODY"],
-        )
-        smtp = smtplib.SMTP_SSL(SMTP_SERVER, 465)
-        smtp.login(
-            os.environ["_GMAIL_SENDER_ADDR"],
-            os.environ["_GMAIL_APP_PASSWORD_OF_SENDER"],
-        )
-        smtp.sendmail(
-            exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
-        )
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message,
-            )  # NO-QA
-            exceptNotifier = {
-                "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
-                "FROM": os.environ["_GMAIL_SENDER_ADDR"],
-                "SUBJECT": "[Except AI Debugging] Error! chatGPT Debugging guide.",
-                "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}",
-            }
-            smtp.sendmail(
-                exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
-            )
-        except Exception as e:
-            pass
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        smtp.quit()
+        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        if environ.get("_OPEN_AI_API") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                pass
 
     @staticmethod
-    def send_gmail_msg(
-        from_email_addr: str,
-        to_email_addr: str,
-        from_email_app_password: str,
-        subject_msg: str,
-        body_msg: str,
-    ) -> dict:
-        """Send mail through gmail smtp server
-
-        :param from_email_addr: Gmail address who send message
-        :type from_email_addr: str
-        :param to_email_addr: Gmail address who receive message
-        :type to_email_addr: str
-        :param from_email_app_password: Google app password
-        :type from_email_app_password: str
-        :param subject_msg: Mail title
-        :type subject_msg: str
-        :param body_msg: Mail body
-        :type body_msg: str
-        :return: Response according to sending request
+    def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
+        """Send message to chat room through microsoft teams app's webhook url.
+
+        :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
+        :type _TEAMS_WEBHOOK_URL: str
+        :param msg: Message text
+        :type msg: str
+        :return: Response according to REST API request
         :rtype: dict
         """
 
-        SMTP_SERVER = "smtp.gmail.com"
-        SMTP_PORT = 465
-        smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
-        EMAIL_ADDR = from_email_addr
-        EMAIL_PASSWORD = from_email_app_password
-        smtp.login(EMAIL_ADDR, EMAIL_PASSWORD)
-        message = EmailMessage()
-        message.set_content(body_msg)
-        message["Subject"] = subject_msg
-        message["From"] = EMAIL_ADDR
-        message["To"] = to_email_addr
-        resp = smtp.send_message(message)
-        smtp.quit()
+        payload = {"text": msg}
+        headers = {"Content-Type": "application/json"}
+        resp = requests.post(
+            _TEAMS_WEBHOOK_URL, headers=headers, data=json.dumps(payload)
+        )
 
         return resp
 
 
-class SuccessMail:
-    """Sending success message to Gmail
+class SuccessTeams:
+    """Sending success message to microsoft teams
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
-        SMTP_SERVER = "smtp.gmail.com"
-        SMTP_PORT = 465
-        smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
-        smtp.login(
-            os.environ["_GMAIL_SENDER_ADDR"],
-            os.environ["_GMAIL_APP_PASSWORD_OF_SENDER"],
-        )
-        message = EmailMessage()
+        exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
-        message.set_content(
-            f"Hi there, \nThis is a success notifier.\n\n - Time: {start_time.strftime(DATE_FORMAT)} \n - Code Status: Done. \n - Detail: Python Code Ran Without Exceptions. \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        )
-        message[
-            "Subject"
-        ] = "[Success Notifier] Success! Python Code Executed Successfully"
-        message["From"] = os.environ["_GMAIL_SENDER_ADDR"]
-        message["To"] = os.environ["_GAMIL_RECIPIENT_ADDR"]
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        smtp.send_message(message)
-        smtp.quit()
+        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
 
-class SendMail:
-    """Sending message to Gmail
+class SendTeams:
+    """Sending message to microsoft teams
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
-        SMTP_SERVER = "smtp.gmail.com"
-        SMTP_PORT = 465
-        smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
-        smtp.login(
-            os.environ["_GMAIL_SENDER_ADDR"],
-            os.environ["_GMAIL_APP_PASSWORD_OF_SENDER"],
-        )
-        message = EmailMessage()
+        exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
-        message.set_content(
-            f"Hi there, \nThis is a customized notifier.\n\n - Time: {start_time.strftime(DATE_FORMAT)}\n - Code Status: Done. \n - Detail: Code Execution Reached Specified Line. \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        )
-        message[
-            "Subject"
-        ] = "[Codeline Notifier] Notice! Code Execution Reached Specified Line"
-        message["From"] = os.environ["_GMAIL_SENDER_ADDR"]
-        message["To"] = os.environ["_GAMIL_RECIPIENT_ADDR"]
-        smtp.send_message(message)
-        smtp.quit()
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
-#     # Set global variables
-# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
-#     global _GAMIL_RECIPIENT_ADDR, _GMAIL_SENDER_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER
-#     _GAMIL_RECIPIENT_ADDR = "xxx@gmail.com"
-#     _GMAIL_SENDER_ADDR = "xxxx@gmail.com"
-#     _GMAIL_APP_PASSWORD_OF_SENDER = "xxxxxxxxxxx"
-#     sys.excepthook = ExceptMail.__call__
+#     """Follow next page"""
+#     environ['_TEAMS_WEBHOOK_URL'] = "microsoft webhook _TEAMS_WEBHOOK_URL"
+# #     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     sys.excepthook = ExceptTeams.__call__
 #     try:
-#         print(1 / 0)
-#         SuccessMail().__call__()  # 1 success sender
-#     except ExceptMail as e:  # 2 except sender
+#         print(1 / 20)
+#         SuccessTeams().__call__()  # 1 success sender
+#     except ExceptTeams as e:  # 2 except sender
 #         sys.exit()
-#     SendMail().__call__()  # 3 Any line sender
+#     SendTeams().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/slack_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/slack_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import requests
 import traceback
 from os import environ
 from email.message import EmailMessage
 from ExceptNotifier import send_slack_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptSlack(BaseException):
     """Override excepthook to send error message to Slack.
 
@@ -68,29 +68,45 @@
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
                 )
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_slack_msg(environ["_SLACK_WEBHOOK_URL"], advice_msg)
             except Exception as e:
-                print(e)
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_slack_msg(environ["_SLACK_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_slack_msg(_SLACK_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through slack app's api.
 
         :param _SLACK_WEBHOOK_URL: _SLACK_WEBHOOK_URL from slack app
@@ -118,15 +134,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifie github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
 
 
 class SendSlack:
     """Sending message to Slack
@@ -140,15 +156,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
 #     # Get your slack bot and enter _SLACK_WEBHOOK_URL
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/sms_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/sms_notifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import traceback
 from os import environ
 from twilio.rest import Client
 from email.message import EmailMessage
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
-
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptSMS(BaseException):
     """Override excepthook to send error message to SMS.
 
@@ -75,15 +75,16 @@
         send_sms_msg(
             environ["_TWILIO_SID"],
             environ["_TWILIO_TOKEN"],
             environ["_SENDER_PHONE_NUMBER"],
             environ["_RECIPIENT_PHONE_NUMBER"],
             data["text"],
         )
-        if environ.get('_OPEN_AI_API') is not None:
+
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
@@ -95,15 +96,36 @@
                     environ["_TWILIO_SID"],
                     environ["_TWILIO_TOKEN"],
                     environ["_SENDER_PHONE_NUMBER"],
                     environ["_RECIPIENT_PHONE_NUMBER"],
                     advice_msg,
                 )
             except Exception as e:
-                print(e)
+                pass
+
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_sms_msg(
+                    environ["_TWILIO_SID"],
+                    environ["_TWILIO_TOKEN"],
+                    environ["_SENDER_PHONE_NUMBER"],
+                    environ["_RECIPIENT_PHONE_NUMBER"],
+                    advice_msg,
+                )
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_sms_msg(
         _TWILIO_SID: str,
         _TWILIO_TOKEN: str,
         _SENDER_PHONE_NUMBER: str,
@@ -146,15 +168,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] ** Success! ** Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_sms_msg(
             environ["_TWILIO_SID"],
             environ["_TWILIO_TOKEN"],
             environ["_SENDER_PHONE_NUMBER"],
@@ -175,15 +197,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] ** Notice! ** Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_sms_msg(
             environ["_TWILIO_SID"],
             environ["_TWILIO_TOKEN"],
             environ["_SENDER_PHONE_NUMBER"],
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/teams_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/wechat_notifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import json
-import datetime
 import requests
 import traceback
+import datetime
 from os import environ
 from email.message import EmailMessage
-from ExceptNotifier.base.teams_sender import send_teams_msg
+from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptTeams(BaseException):
-    """Override excepthook to send error message to Microsoft Teams.
+class ExceptWechat(BaseException):
+    """Override excepthook to send error message to Wechat.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
@@ -50,121 +51,129 @@
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-
-        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
             exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
                 frame.f_code.co_name,
                 frame.f_code.co_filename,
                 frame.f_lineno,
             )
             for key, val in frame.f_locals.items():
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-
-        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
                 )
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
-                send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+                send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                pass
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
             except Exception as e:
-                print(e)
                 pass
 
     @staticmethod
-    def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
-        """Send message to chat room through microsoft teams app's webhook url.
+    def send_wechat_msg(_WECHAT_WEBHOOK_URL: str, msg: str) -> None:
+        """Send message to wechat.
 
-        :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
-        :type _TEAMS_WEBHOOK_URL: str
-        :param msg: Message text
+        :param _WECHAT_WEBHOOK_URL: Wechat Webhook URL https://work.weixin.qq.com/api/doc/90000/90136/91770
+        :type _WECHAT_WEBHOOK_URL: str
+        :param msg: Message to send
         :type msg: str
-        :return: Response according to REST API request
-        :rtype: dict
         """
-
-        payload = {"text": msg}
-        headers = {"Content-Type": "application/json"}
-        resp = requests.post(
-            _TEAMS_WEBHOOK_URL, headers=headers, data=json.dumps(payload)
-        )
-
-        return resp
+        msg_template = {"msgtype": "text", "text": {"content": ""}}
+        msg_template["text"]["content"] = "\n".join(msg)
+        requests.post(_WECHAT_WEBHOOK_URL, json=msg_template)
 
 
-class SuccessTeams:
-    """Sending success message to microsoft teams
+class SuccessWechat:
+    """Sending success message to wechat
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
 
-class SendTeams:
-    """Sending message to microsoft teams
+class SendWechat:
+    """Sending message to wechat
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
-#     """Follow next page"""
-#     environ['_TEAMS_WEBHOOK_URL'] = "microsoft webhook _TEAMS_WEBHOOK_URL"
-# #     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# #     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
-#     sys.excepthook = ExceptTeams.__call__
+#     """Get your wechat webhook URL.
+#     https://work.weixin.qq.com/api/doc/90000/90136/91770"""
+#     environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
+#     # environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     # environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     sys.excepthook = ExceptWechat.__call__
 #     try:
-#         print(1 / 20)
-#         SuccessTeams().__call__()  # 1 success sender
-#     except ExceptTeams as e:  # 2 except sender
+#         print(1 / 0)
+#         SuccessWechat().__call__()  # 1 success sender
+#     except ExceptWechat as e:  # 2 except sender
 #         sys.exit()
-#     SendTeams().__call__()  # 3 customized sender
+#     SendWechat().__call__()  # 3 customized sender
+#     send = SendWechat()  # You can use it like this, too.
+#     send() # 3 cusotomized sender
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/pycore/telegram_notifier.py` & `exceptnotifier-0.2.5/ExceptNotifier/pycore/telegram_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import requests
 import traceback
 import datetime
 from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.bard_receiver import receive_bard_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptTelegram(BaseException):
     """Override excepthook to send error message to Telegram.
 
@@ -65,30 +66,45 @@
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
-        if environ.get('_OPEN_AI_API') is not None:
+        if environ.get("_OPEN_AI_API") is not None:
             try:
                 error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
                 advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                     line[0],
                     line[2],
                     line[1],
                     line[3],
                 )
                 advice_msg += receive_openai_advice(
                     environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
                 )  # NO-QA
                 send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
 
             except Exception as e:
-                print(e)
+                pass
+        if environ.get("_BARD_API_KEY") is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_bard_advice(
+                    environ["_BARD_API_KEY"], error_message
+                )  # NO-QA
+                send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
+
+            except Exception as e:
                 pass
 
     @staticmethod
     def send_telegram_msg(_TELEGRAM_TOKEN: str, msg: str) -> dict:
         """Send message via telegram bot.
 
         :param _TELEGRAM_TOKEN: Telegram secure bot Token
@@ -121,15 +137,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 class SendTelegram:
@@ -144,15 +160,15 @@
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
             "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 # if __name__ == "__main__":
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.2.5/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.2.5/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.4
+Version: 0.2.5
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,39 +16,40 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Development Status :: 2 - Pre-Alpha <br>
+
+Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
-Before QA<br> 
 
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
-<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
+<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-blue"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
+<a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/ExceptNotifier?color=blue"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
-
+<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black"></a>
+<a href="https://www.buymeacoffee.com/parkminwoo"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" height="20px"></a>
 </p>
 
 ![](./assets/imgs/main3.png)
-##### Provides a notification from the application shown in the captured screen.
+##### Provides a notification from the application shown in the captured screen. 
 
-# Python Package: ExceptNotifier
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
- The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
+# Python Package: ExceptNotifier [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com) [](https://img.shields.io/badge/License-MIT-blue.svg) [![Documentation Status](https://readthedocs.org/projects/exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/en/latest/)
+
+ The ExceptNotifier Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
-With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
+With ExceptNotifier, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
 ![](./assets/imgs/core02.png)
 
 <Br>
 
 
 # Supporting Applications
@@ -63,24 +64,28 @@
 - [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
 - [Wecaht](https://www.wechat.com/)
 - SMS Sending using [Twilio](https://www.twilio.com/en-us)
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 - [Opea AI API](https://openai.com/blog/openai-api)
         - If you have OpenAI API Key and model name, you can get information and code examples for debugging in any application.
-
-
+- [Google Bard](https://bard.google.com/) Python package [BardAPI](https://github.com/dsdanielpark/BARD_API)
+        - Starting from Exceptnotifier version 0.2.5
+        - Using the Python package [Bard API](https://github.com/dsdanielpark/BARD_API), if you declare the __Secure-1PSID value as a global variable , you can receive debugging hints and explanations about errors in your code through Google Bard.
 <br>
 
-# Quick Start
-```bash
-$ pip install ExceptNotifier
+# Install
+The latest stable release (and required dependencies) can be installed from PyPI:
 ```
-```bash
-$ pip install exceptnotifier
+pip install ExceptNotifier
+```
+
+You may instead want to use the development version from Github:
+```
+pip install git+https://github.com/dsdanielpark/ExceptNotifier.git
 ```
 
 <br><br><br>
 
 # Contents
 
 - [App Setup Overview](#app-setup-overview)
@@ -142,22 +147,25 @@
 |Discord|`_DISCORD_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptDiscord](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) |
 |AWS Chime|`_CHIME_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptChime](./tutorials/ExceptChime/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) |
 |G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) |
 |SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/ExceptTeams/GUIDE.md)|
-|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)|
+|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
 | OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/APIOpenAI/GUIDE.md)|
+| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://bard.google.com/)|
+
+- Starting from v0.2.5, you can receive debugging hints and examples through Google Bard using the same syntax as the OpenAI API. However, due to time constraints, examples will only be added for Telegram and Discord.
 
 <br>
 
 # Tutorial
 I will update tutorial ASAP. `README.md` is sufficient, but read the application's official documentation if necessary. However, we are preparing a more detailed and friendly tutorial.
 
 1. Main-tutorials: [Notebook](https://github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
@@ -390,26 +398,32 @@
 As all classes function the same, the example will only use one image, like in Telegram.
 ![](./assets/imgs/fig44.png)
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
 - b. Type /newbot to create a new bot <br>
 - c. Give your bot a name & a username <br>
 - d. Copy your new Telegram bot’s token <br>
 - e. You have to click `Start_bot` and must enter anything to your bot.
-   - Before use Notifier, Please use this to check if you follow guide. The Telegram bot may have a slight delay and it responded within 2-3 minutes.
+   - Before use Notifier, Please use this to check if you follow guide. The Telegram bot may have a slight delay and it responded within 2-3 minutes. <br>
+
+
+![](./assets/imgs/telegram.gif)
+
 *API TEST*
 ```python
 from ExceptNotifier import send_telegram_msg
 
 _TELEGRAM_TOKEN = "xxxxx:xxxxx-xxxx"
 send_telegram_msg(_TELEGRAM_TOKEN, 'msg')
 ```
 
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
 <br><br>
  
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 ### a. Notifier without OpenAI API
 *Notifier*
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys, os
 sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx"
@@ -468,14 +482,17 @@
 send_gmail_msg(
     _GMAIL_SENDER_ADDR,
     _GAMIL_RECIPIENT_ADDR,
     _GMAIL_APP_PASSWORD_OF_SENDER,
     subject_msg,
     body_msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail
 sys.excepthook = ExceptMail.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -552,20 +569,26 @@
 
 ## *Discord*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) 
 - a. Select the channel to receive notifications.
 - b. Click `Edit Channel` in the upper right corner of the chat window.
 - c. Click `Integrations` - `Webhook` - `New Webhook`.
 - d. Then click `Copy Webhook`.
+ 
+![](./assets/imgs/discord.gif)
+
 *API TEST*
 ```python
 from ExceptNotifier import send_discord_msg
 
 send_discord_msg(_DISCORD_WEBHOOK_URL, "Any Test Message") 
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import ExceptDiscord, SuccessDiscord, SendDiscord
 sys.excepthook = ExceptDiscord.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -588,21 +611,24 @@
 ## *Chime*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)
 
 - a. Select the Chat room to receive notifications.
 - b. Click `Room Setting` in the upper right corner.
 - c. Click `Manage Webhook and bot`
 - d. Create Add Webhook, set it up, then click `Copy Webhook`.
+ 
 *API TEST*
 ```python
 from ExceptNotifier import send_chime_msg
 
 send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message")
-
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import SuccessChime, ExceptChime, SendChime
 sys.excepthook = ExceptChime.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -623,20 +649,25 @@
 
 ## *Slack*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) 
 - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App`
 - c. Add webhook: Click `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace
 - d. Copy `Webhook URL`
+ 
 *API TEST*
 ```python
 from ExceptNotifier import send_slack_msg
 
 send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message")
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptSlack, SuccessSlack, SendSlack
 sys.excepthook = ExceptSlack.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -663,15 +694,16 @@
 
 *API TEST*
 ```python
 from ExceptNotifier import send_line_msg
 
 send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message")
 ```
-
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptLine, SuccessLine, SendLine
 sys.excepthook = ExceptLine.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -711,14 +743,16 @@
     _TWILIO_SID,
     _TWILIO_TOKEN,
     _SENDER_PHONE_NUMBER,
     _RECIPIENT_PHONE_NUMBER,
     "Any Test Message")
 ```
 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS
 sys.excepthook = ExceptSMS.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -753,14 +787,16 @@
 ```python
 from ExceptNotifier import send_teams_msg
 
 _TEAMS_WEBHOOK_URL = 'xxxx'
 
 send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message")
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptTeams, SuccessTeams, SendTeams
 sys.excepthook = ExceptTeams.__call__
 
@@ -777,14 +813,18 @@
 
 SendTeams().__call__()        #3 customized sender        
 ```
 
 <Br>
 
 ## *Kakaotalk*
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)
+
+
 - a. Sign up at the following site: [https://developers.kakao.com/](https://developers.kakao.com/)
 - b. Click `My Application` on the top bar.
 - c. Click `Add an application`, set a name, and create it.
 - d. Click `Kakao Login` in the left menu, then change the State of `Kakao Login Activation` to ON on the resulting page.
 - e. In `My Application > Product Settings > Kakao Login`, be sure to set `Redirect URI` as follows: [https://example.com/oauth](https://example.com/oauth)
 - f. In the left Consent Items menu, set `Send message in KakaoTalk` to optional agreement.
 - g. Copy the `REST API Key` in `My Application > App Settings > Summary`.
@@ -795,14 +835,17 @@
 ```python
 from ExceptNotifier import send_kakao_msg
 
 _KAKAO_TOKEN_PATH = 'xxx/xx/xxx.json'
 
 send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code. 
+
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptKakao, SuccessKakao, SendKakao
 sys.excepthook = ExceptKakao.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -817,21 +860,24 @@
     sys.exit()
 
 SendKakao().__call__()        #3 customized sender         
 ```
 
 
 ## *Wechat*
-a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770) <br>
 *API TEST*
 ```python
 from ExceptNotifier import send_wechat_msg
 
 send_wechat_msg(_WECHAT_WEBHOOK_URL, msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat
 
 # Define the next two variables optionally when using OpenAI's API.
 # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"    
@@ -847,15 +893,15 @@
 
 SendWechat().__call__()        #3 customized sender       
 ```
 
 <Br>
 
 ## *Beep*
-No setup is required. Use as follows.
+No setup is required. Use as follows. <br>
 *TEST*
 ```python
 from ExceptNotifier import beep
 
 beep(sec=1, freq=1000) 
 ```
 *Notifier*
@@ -877,15 +923,15 @@
 
 ```
 
 <Br>
 
 
 ## *Desktop*
-No setup is required. Use as follows.
+No setup is required. Use as follows. <br>
 *TEST*
 ```python
 from ExceptNotifier import send_desktop_msg
 
 title_msg = "Test Title"
 body_msg = "Test Body"
 DISP_TIME = 5
@@ -910,30 +956,60 @@
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
 
 <Br><br><br>
-# License
-MIT
+ 
+# Documentation [![Documentation Status](https://readthedocs.org/projects/exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/en/latest/)
+ 
+Official Document: https://exceptnotifier.readthedocs.io/en/latest/ <br> 
+Documentation can be automatically generated by [Sphinx](https://www.sphinx-doc.org/en/master/usage/quickstart.html). But, I do not use [Google style](https://google.github.io/styleguide/pyguide.html#383-functions-and-methods) because it requires [the Napoleon extension](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) for Sphinx. I will use [m2r](https://github.com/miyakogi/m2r) to convert the README.md file to .rst so that it can be included.
+
+Having generated it with Sphinx, we can also host the documentation freely at [ReadTheDocs.org](https://citation-graph.readthedocs.io/en/latest/). 
+ 
+# License 
+ExceptNotifier: MIT <br>
+Licenses apply the each [dependencies package](https://choosealicense.com/licenses/), and the created posts follow [CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/).
 
 # Bugs and Issues
-[Open a new issue](https://github.com/dsdanielpark/ExceptNotifier/issues)
+Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
+[[Open a new issue]](https://github.com/dsdanielpark/ExceptNotifier/issues) 
  
 # Contributing Guide
 I will announce contributing rules when the code development status changes to beta soon. Until then, please create an issue for feature requests and bug reports. I would greatly appreciate it if you use it a lot and give your opinions generously. Thank you sincerely.
 
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
 
 # Contacts
-Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
-Email parkminwoo1991@gmail.com <br>
+:mortar_board: Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
+:envelope: Email: parkminwoo1991@gmail.com <br>
 - Developer note: [Link](./documents/DEV_NOTE.md)
+#### Dev Note
+1. Applying ExceptNotifier in Python
+
+    In Python, we use [sys.excepthook](https://docs.python.org/ko/3/library/sys.html#sys.excepthook) to call the exceptnotifier by taking advantage of the interpreter calling sys.excepthook with three arguments (exception class, exception instance, traceback object) when an exception occurs. Since sys.excepthook is the highest-level exception handler that occurs just before the system shuts down, exceptnotifier is implemented as a class that inherits from baseexception and overrides sys.excepthook. For overriding exceptions that cannot be raised or exceptions raised in threads, please refer to the sys.unraisablehook() function and the threading.excepthook() function, respectively.
+
+2. Application of ExceptNotifier in iPython
+
+    Strictly, iPython is a package, not a programming language like Python, but it has been classified to aid understanding.
+    IPython (Interactive Python) is a package consisting of a command shell for interactive computing for multiple programming languages.
+
+    It is a very useful package that allows you to compile Python bit by bit in an interactive session through the concept of an interactive shell, but in iPython, control by sys.excepthook occurs just before the prompt is returned, so it is impossible to receive a traceback object using sys.excepthook and send an error message to each messenger app. Additionally, because it was necessary to inherit from baseexception, it was necessary to override other functions in iPython.
+
+    Therefore, at first, we considered the [magics](https://ipython.readthedocs.io/en/stable/interactive/magics.html) in cell, but the problem of having to import the magic function every time in the cell can be cumbersome to use, so we decided to use the [set_custom_exc](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.interactiveshell.html) in iPython, which can work even by overriding it once. The set_custom_exc allows you to set a custom exception handler that is called when an exception in the exc_tuple occurs in the main loop (especially the run_code() method), and is designed so that the handle can return a structured traceback or None. Therefore, we can receive the traceback and send it to each messenger app. The order of top-level exception handling in iPython is different. You can use by `calling` raise in the `except` statement.
+
+3. Using Environment Variables (environ)
+    In Python's except statement, it was designed to inherit exceptionbase, so we thought about how to pass variables into the class and decided to set variables through os.environ to use them by distributing them as a package. Additionally, since the user's webhook URL or API key will not change, we named the variables in uppercase and set special names to prevent contamination from duplicate variables. Since the variables are used within the class, we added an underscore before the variable name.
+
+4. About example code
+
+    For explanation, in Python, the example uses the overrided `sys.excepthook` in the except statement, like `except ExceptTelegram as e:`. However, you can use it simply by overriding `sys.excepthook` once and calling `raise` in the `except` statement. In IPython, you can use `set_custom_exc` to override the `Exception` with a user-defined function once, and then call `raise` in the `except` statement to repeatedly take the desired ExceptNotifier action. Also, although the example uses` ExceptTelegram.__call__` or `SuccessTelegram().__call__()`, these are expressions to aid understanding, and you can change them to a more concise form if you prefer.
 
 #### Could you kindly add this badge to your repository?
 ```
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ```
 
 I would appreciate it if you could share the document widely by specifying that the source is the ExceptNotifier official github.
```

#### html2text {}

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.4 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.5 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
 :: English Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 2 - Pre-Alpha
+LICENSE Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
-Before QA
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-[PyPI package] [PyPI] [Downloads] [Code_style:_black] [https://img.shields.io/
-                         badge/License-MIT-yellow.svg]
+[PyPI package] [PyPI] [Downloads] [commit update] [Code_style:_black] [https://
+img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black] [https:/
+        /www.buymeacoffee.com/assets/img/custom_images/orange_img.png]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
 shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
 /hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
-(https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
-flexible approach to receiving notifications by enhancing Python's try-except
-statement. This package enables you to receive alerts through various messaging
-applications or emails.
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
+(https://hits.seeyoufarm.com) [](https://img.shields.io/badge/License-MIT-
+blue.svg) [![Documentation Status](https://readthedocs.org/projects/
+exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/
+en/latest/) The ExceptNotifier Python package offers a flexible approach to
+receiving notifications by enhancing Python's try-except statement. This
+package enables you to receive alerts through various messaging applications or
+emails.
 
-With `ExceptNotifier`, you can obtain detailed compilation errors, including
+With ExceptNotifier, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
 accessible, streamlining your debugging process. ![](./assets/imgs/core02.png)
 # Supporting Applications Applicable to both [IPython](https://ipython.org/
 ) and [Python](https://www.python.org/), but needs to be ported differently
@@ -45,17 +48,24 @@
 [Microsoft Teams](https://www.microsoft.com/en/microsoft-teams/download-app) -
 [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
 - [Wecaht](https://www.wechat.com/) - SMS Sending using [Twilio](https://
 www.twilio.com/en-us) - Desktop Notification using [Plyer](https://github.com/
 kivy/plyer) - Beep Sound from [system](https://docs.python.org/3/library/
 winsound.html) - [Opea AI API](https://openai.com/blog/openai-api) - If you
 have OpenAI API Key and model name, you can get information and code examples
-for debugging in any application.
-# Quick Start ```bash $ pip install ExceptNotifier ``` ```bash $ pip install
-exceptnotifier ```
+for debugging in any application. - [Google Bard](https://bard.google.com/
+) Python package [BardAPI](https://github.com/dsdanielpark/BARD_API) - Starting
+from Exceptnotifier version 0.2.5 - Using the Python package [Bard API](https:/
+/github.com/dsdanielpark/BARD_API), if you declare the __Secure-1PSID value as
+a global variable , you can receive debugging hints and explanations about
+errors in your code through Google Bard.
+# Install The latest stable release (and required dependencies) can be
+installed from PyPI: ``` pip install ExceptNotifier ``` You may instead want to
+use the development version from Github: ``` pip install git+https://
+github.com/dsdanielpark/ExceptNotifier.git ```
 
 
 # Contents - [App Setup Overview](#app-setup-overview) - [Tutorial](#tutorial)
 - [Python Core](#python-core) * [Except`Notifier`](#exceptnotifier) + [AI
 Debbugging Infomation Notification](#ai-debbugging-infomation-notification) *
 [Success`Notifier`](#successnotifier) * [Send`Notifier`](#sendnotifier) *
 [Sender](#sender)
@@ -113,22 +123,28 @@
 `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not
 free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./
 tutorials/ExceptTeams/GUIDE.md)|
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|
-[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you add the following two
-variables to the required variables for each application in the table above,
-you can receive error location and explanation, as well as examples, from
-OpenAI's model | API | Required Variables | Free or Paid | Ease of Setup | Time
-Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |
-OpenAI API |`Required variables for each application`+
+[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
+If you add the following two variables to the required variables for each
+application in the table above, you can receive error location and explanation,
+as well as examples, from OpenAI's model | API | Required Variables | Free or
+Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:
+--:|:--:|:--:|:---:| | OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
-APIOpenAI/GUIDE.md)|
+APIOpenAI/GUIDE.md)| | Google Bard API |`Required variables for each
+application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://
+bard.google.com/)| - Starting from v0.2.5, you can receive debugging hints and
+examples through Google Bard using the same syntax as the OpenAI API. However,
+due to time constraints, examples will only be added for Telegram and Discord.
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
 [folder](https://github.com/DSDanielPark/ExceptNotifier/tree/main/tutorial).
 The tutorial is synchronized with the Python file name provided by
@@ -227,36 +243,38 @@
 fig44.png) - a. Open your telegram app and search for BotFather. (A built-in
 Telegram bot that helps users create custom Telegram bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 - e. You have to click `Start_bot` and must enter anything to your bot. -
 Before use Notifier, Please use this to check if you follow guide. The Telegram
-bot may have a slight delay and it responded within 2-3 minutes. *API TEST*
-```python from ExceptNotifier import send_telegram_msg _TELEGRAM_TOKEN =
-"xxxxx:xxxxx-xxxx" send_telegram_msg(_TELEGRAM_TOKEN, 'msg') ``` For more
-infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
-
-
-### a. Notifier without OpenAI API *Notifier* ```python from ExceptNotifier
-import ExceptTelegram, SuccessTelegram, SendTelegram import sys, os
-sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx"
-try: print(1/0) SuccessTelegram().__call__() #1. success sender except
+bot may have a slight delay and it responded within 2-3 minutes.
+![](./assets/imgs/telegram.gif) *API TEST* ```python from ExceptNotifier import
+send_telegram_msg _TELEGRAM_TOKEN = "xxxxx:xxxxx-xxxx" send_telegram_msg
+(_TELEGRAM_TOKEN, 'msg') ``` For more infomation, visit [Telegram Bot Father
+API](https://core.telegram.org/bots/api)
+
+##### This is a Python (*.py) example. If you are using IPython, please click
+the Google Colab icon above to view the example code. ### a. Notifier without
+OpenAI API *Notifier* ```python from ExceptNotifier import ExceptTelegram,
+SuccessTelegram, SendTelegram import sys, os sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0)
+SuccessTelegram().__call__() #1. success sender except ExceptTelegram as e: #2.
+except sender sys.exit() SendTelegram().__call__() #3. customized sender ```
+### b. Notifier with OpenAI API - If you just set `_OPEN_AI_API` and
+`_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL
+will automatically send debugging information as a message. Currently, it is
+mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that
+other models can be used later. *Notifier* ```python from ExceptNotifier import
+ExceptTelegram, SuccessTelegram, SendTelegram import sys, os sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.envirion
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try:
+print(1/0) SuccessTelegram().__call__() #1. success sender except
 ExceptTelegram as e: #2. except sender sys.exit() SendTelegram().__call__() #3.
-customized sender ``` ### b. Notifier with OpenAI API - If you just set
-`_OPEN_AI_API` and `_OPEN_AI_MODEL` environment variables in all application
-use case, AI MODEL will automatically send debugging information as a message.
-Currently, it is mainly based on the `GPT-3.5-TURBO` model, but we plan to
-update it so that other models can be used later. *Notifier* ```python from
-ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import sys,
-os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
-"xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion
-['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
-success sender except ExceptTelegram as e: #2. except sender sys.exit()
-SendTelegram().__call__() #3. customized sender ```
+customized sender ```
 ## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
 email is sent along with the error message. Additionally, you can send emails
 from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
@@ -264,19 +282,21 @@
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
 *API TEST* ```python from ExceptNotifier import send_gmail_msg
 _GMAIL_SENDER_ADDR = 'xxxx@gmail.com' _GAMIL_RECIPIENT_ADDR = 'xxxx@gmail.com'
 _GMAIL_APP_PASSWORD_OF_SENDER = 'xxxx' subject_msg = "Test Title" body_msg =
 "Test Body" send_gmail_msg( _GMAIL_SENDER_ADDR, _GAMIL_RECIPIENT_ADDR,
-_GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg) ``` *Notifier* ```python
-import sys, os from ExceptNotifier import ExceptMail, SuccessMail, SendMail
-sys.excepthook = ExceptMail.__call__ # Define the next two variables optionally
-when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" #
-os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ['_GAMIL_RECIPIENT_ADDR'] =
+_GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg) ``` ##### This is a
+Python (*.py) example. If you are using IPython, please click the Google Colab
+icon above to view the example code. *Notifier* ```python import sys, os from
+ExceptNotifier import ExceptMail, SuccessMail, SendMail sys.excepthook =
+ExceptMail.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_GAMIL_RECIPIENT_ADDR'] =
 'xxxxxxx@gmail.com' os.environ['_GMAIL_SENDER_ADDR'] = 'yyyyyy@gmail.com'
 os.environ['_GMAIL_APP_PASSWORD_OF_SENDER'] = 'zzzzzz' try: main() # Your Code
 Here SuccessMail().__call__() # No Exception -> Send Success mail. except
 ExceptMail: # Exception -> Send Fail mail. pass SendMail().__call__() # When
 Process Ended -> Any Line mail. ```   See Example... ```python import sys, os
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail # Define the next
 two variables optionally when using OpenAI's API. # os.environ
@@ -296,166 +316,251 @@
 ['_GMAIL_APP_PASSWORD_OF_SENDER'] = 'zzzzzz' try: 'your code' SuccessMail
 ().__call__() except ExceptMail: pass SendMail().__call__() ```
 ## *Discord* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) - a. Select the channel to
 receive notifications. - b. Click `Edit Channel` in the upper right corner of
 the chat window. - c. Click `Integrations` - `Webhook` - `New Webhook`. - d.
-Then click `Copy Webhook`. *API TEST* ```python from ExceptNotifier import
-send_discord_msg send_discord_msg(_DISCORD_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys, os from ExceptNotifier import ExceptDiscord,
-SuccessDiscord, SendDiscord sys.excepthook = ExceptDiscord.__call__ # Define
-the next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_DISCORD_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxx" try: print(1/20)
-SuccessDiscord().__call__() #1 success sender except ExceptDiscord as e: #2
-except sender sys.exit() SendDiscord().__call__() #3 customized sender ```
+Then click `Copy Webhook`. ![](./assets/imgs/discord.gif) *API TEST* ```python
+from ExceptNotifier import send_discord_msg send_discord_msg
+(_DISCORD_WEBHOOK_URL, "Any Test Message") ``` ##### This is a Python (*.py)
+example. If you are using IPython, please click the Google Colab icon above to
+view the example code. *Notifier* ```python import sys, os from ExceptNotifier
+import ExceptDiscord, SuccessDiscord, SendDiscord sys.excepthook =
+ExceptDiscord.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_DISCORD_WEBHOOK_URL'] =
+"xxxxxxxxxxxxxxxxx" try: print(1/20) SuccessDiscord().__call__() #1 success
+sender except ExceptDiscord as e: #2 except sender sys.exit() SendDiscord
+().__call__() #3 customized sender ```
 ## *Chime* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing) - a. Select the Chat room to
 receive notifications. - b. Click `Room Setting` in the upper right corner. -
 c. Click `Manage Webhook and bot` - d. Create Add Webhook, set it up, then
 click `Copy Webhook`. *API TEST* ```python from ExceptNotifier import
-send_chime_msg send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys, os from ExceptNotifier import SuccessChime,
-ExceptChime, SendChime sys.excepthook = ExceptChime.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx" try: print(1/0)
-SuccessChime().__call__() #1 success sender except ExceptChime as e: #2 except
-sender sys.exit() SendChime().__call__() #3 customized sender ```
+send_chime_msg send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message") ``` #####
+This is a Python (*.py) example. If you are using IPython, please click the
+Google Colab icon above to view the example code. *Notifier* ```python import
+sys, os from ExceptNotifier import SuccessChime, ExceptChime, SendChime
+sys.excepthook = ExceptChime.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
+['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx" try: print(1/0) SuccessChime
+().__call__() #1 success sender except ExceptChime as e: #2 except sender
+sys.exit() SendChime().__call__() #3 customized sender ```
 ## *Slack* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/1-
 dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App` - c. Add webhook: Click
 `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace -
 d. Copy `Webhook URL` *API TEST* ```python from ExceptNotifier import
-send_slack_msg send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys from ExceptNotifier import ExceptSlack,
-SuccessSlack, SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_SLACK_WEBHOOK_URL'] = 'https://hooks.slack.com/services/
-xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlack().__call__() #1 success
-sender except ExceptSlack as e: #2 except sender sys.exit() SendSlack
-().__call__() #3 customized sender ```
+send_slack_msg send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message") ``` #####
+This is a Python (*.py) example. If you are using IPython, please click the
+Google Colab icon above to view the example code. *Notifier* ```python import
+sys from ExceptNotifier import ExceptSlack, SuccessSlack, SendSlack
+sys.excepthook = ExceptSlack.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
+['_SLACK_WEBHOOK_URL'] = 'https://hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx'
+try: print(1/0) SuccessSlack().__call__() #1 success sender except ExceptSlack
+as e: #2 except sender sys.exit() SendSlack().__call__() #3 customized sender
+```
 ## *Line* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) - a. Register [https://notify-
 bot.line.me/](https://notify-bot.line.me/) - b. Go to mypage [https://notify-
 bot.line.me/my/](https://notify-bot.line.me/my/) - c. Click `Generate Token`,
 enter Service Name and click `1-on-1 chat with LINE` (anything you like) - d.
 Copy Token. *API TEST* ```python from ExceptNotifier import send_line_msg
-send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message") ``` *Notifier*
-```python import sys from ExceptNotifier import ExceptLine, SuccessLine,
-SendLine sys.excepthook = ExceptLine.__call__ # Define the next two variables
-optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
-['_LINE_NOTIFY_API_TOKEN'] = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
-().__call__() #1 success sender except ExceptLine as e: #2 except sender
-sys.exit() SendLine().__call__() #3 customized sender ```
+send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message") ``` ##### This is a
+Python (*.py) example. If you are using IPython, please click the Google Colab
+icon above to view the example code. *Notifier* ```python import sys from
+ExceptNotifier import ExceptLine, SuccessLine, SendLine sys.excepthook =
+ExceptLine.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_LINE_NOTIFY_API_TOKEN'] =
+'xxxxxxxxxxx' try: print(1/20) SuccessLine().__call__() #1 success sender
+except ExceptLine as e: #2 except sender sys.exit() SendLine().__call__() #3
+customized sender ```
 ## *SMS* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing) - a. Sign up for Twilio. [https:
 //www.twilio.com/en-us](https://www.twilio.com/en-us) - b. Click Console in the
 upper right corner. - c. Copy the variables provided in the console. *API TEST*
 ```python from ExceptNotifier import send_sms_msg _TWILIO_SID = 'xxxx'
 _TWILIO_TOKEN = "xxxx" _SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER =
 "xxxx" send_sms_msg( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER,
-_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` *Notifier* ```python import
-sys from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
-ExceptSMS.__call__ # Define the next two variables optionally when using
-OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
-['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TWILIO_SID'] = 'xxxx' os.environ
-['_TWILIO_TOKEN'] = 'yyyyyy' os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa",
-os.environ['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS
-().__call__() #1 success sender except ExceptSMS as e: #2 except sender
-sys.exit() SendSMS().__call__() #3 customized sender ```
+_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` ##### This is a Python (*.py)
+example. If you are using IPython, please click the Google Colab icon above to
+view the example code. *Notifier* ```python import sys from ExceptNotifier
+import ExceptSMS, SuccessSMS, SendSMS sys.excepthook = ExceptSMS.__call__ #
+Define the next two variables optionally when using OpenAI's API. # os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_TWILIO_SID'] = 'xxxx' os.environ['_TWILIO_TOKEN'] = 'yyyyyy'
+os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa", os.environ
+['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS().__call__() #1
+success sender except ExceptSMS as e: #2 except sender sys.exit() SendSMS
+().__call__() #3 customized sender ```
 ## *Teams* - a. Create the channel that you want to notify. - b. `App` -
 `Search: webhook` - `Incoming Webhook` [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
 the webhook incoming application is available. - c. Go to the team channel to
 receive notifications, and click `Connectors` in Settings. - d. `Connectors`
 After configuring webhook incoming in Connector, copy the webhook URL. *API
 TEST* ```python from ExceptNotifier import send_teams_msg _TEAMS_WEBHOOK_URL =
-'xxxx' send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message") ``` *Notifier*
-```python import sys from ExceptNotifier import ExceptTeams, SuccessTeams,
-SendTeams sys.excepthook = ExceptTeams.__call__ # Define the next two variables
-optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
-['_TEAMS_WEBHOOK_URL'] = 'microsoft webhook _TEAMS_WEBHOOK_URL' try: print(1/
-20) SuccessTeams().__call__() #1 success sender except ExceptTeams as e: #2
-except sender sys.exit() SendTeams().__call__() #3 customized sender ```
-## *Kakaotalk* - a. Sign up at the following site: [https://
-developers.kakao.com/](https://developers.kakao.com/) - b. Click `My
+'xxxx' send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message") ``` ##### This is
+a Python (*.py) example. If you are using IPython, please click the Google
+Colab icon above to view the example code. *Notifier* ```python import sys from
+ExceptNotifier import ExceptTeams, SuccessTeams, SendTeams sys.excepthook =
+ExceptTeams.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TEAMS_WEBHOOK_URL'] = 'microsoft
+webhook _TEAMS_WEBHOOK_URL' try: print(1/20) SuccessTeams().__call__() #1
+success sender except ExceptTeams as e: #2 except sender sys.exit() SendTeams
+().__call__() #3 customized sender ```
+## *Kakaotalk* [![Open In Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-
+lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing) - a. Sign up at the following site:
+[https://developers.kakao.com/](https://developers.kakao.com/) - b. Click `My
 Application` on the top bar. - c. Click `Add an application`, set a name, and
 create it. - d. Click `Kakao Login` in the left menu, then change the State of
 `Kakao Login Activation` to ON on the resulting page. - e. In `My Application >
 Product Settings > Kakao Login`, be sure to set `Redirect URI` as follows:
 [https://example.com/oauth](https://example.com/oauth) - f. In the left Consent
 Items menu, set `Send message in KakaoTalk` to optional agreement. - g. Copy
 the `REST API Key` in `My Application > App Settings > Summary`. - h. If you
 have successfully completed all of the above steps, go to the following
 document and follow the instructions: ./tutorials/kakao_token_generator.ipynb
 *API TEST* ```python from ExceptNotifier import send_kakao_msg
 _KAKAO_TOKEN_PATH = 'xxx/xx/xxx.json' send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
-``` *Notifier* ```python import sys from ExceptNotifier import ExceptKakao,
-SuccessKakao, SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_KAKAO_TOKEN_PATH'] = 'xxxx/xxx/xxx.json'' try: print(1/0)
-SuccessKakao().__call__() #1 success sender except ExceptKakao as e: #2 except
-sender sys.exit() SendKakao().__call__() #3 customized sender ``` ## *Wechat*
-a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/
-90136/91770) *API TEST* ```python from ExceptNotifier import send_wechat_msg
-send_wechat_msg(_WECHAT_WEBHOOK_URL, msg) ``` *Notifier* ```python import sys
-from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat # Define the
-next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx" sys.excepthook =
-ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__() #1 success
-sender except ExceptWechat as e: #2 except sender sys.exit() SendWechat
-().__call__() #3 customized sender ```
-## *Beep* No setup is required. Use as follows. *TEST* ```python from
-ExceptNotifier import beep beep(sec=1, freq=1000) ``` *Notifier* ```python from
-Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep() os.environ
-['BEEP_TIME'] = 1 sys.excepthook = ExceptBeep.__call__ try: print(1/20)
-SuccessBeep().__call__() #1 success beep-beep except ExceptBeep as e: #2 except
-beep-beep sys.exit() SendBeep().__call__() #3 customized beep-beep beep() ```
-## *Desktop* No setup is required. Use as follows. *TEST* ```python from
-ExceptNotifier import send_desktop_msg title_msg = "Test Title" body_msg =
-"Test Body" DISP_TIME = 5 send_desktop_msg(title_msg, body_msg, DISP_TIME) ```
-*Notifier* ```python from ExceptNotifier import ExceptDesktop, SuccessDesktop,
-SendDesktop sys.excepthook = ExceptDesktop.__call__ # Define the next two
-variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-try: print(1/0) SuccessDesktop().__call__() #1 success sender except
-ExceptDesktop as e: #2 except sender sys.exit() SendDesktop().__call__() #3
-customized sender ```
+``` ##### This is a Python (*.py) example. If you are using IPython, please
+click the Google Colab icon above to view the example code. *Notifier*
+```python import sys from ExceptNotifier import ExceptKakao, SuccessKakao,
+SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ['_KAKAO_TOKEN_PATH']
+= 'xxxx/xxx/xxx.json'' try: print(1/0) SuccessKakao().__call__() #1 success
+sender except ExceptKakao as e: #2 except sender sys.exit() SendKakao
+().__call__() #3 customized sender ``` ## *Wechat* a. Get Webhook URL by
+visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+*API TEST* ```python from ExceptNotifier import send_wechat_msg send_wechat_msg
+(_WECHAT_WEBHOOK_URL, msg) ``` ##### This is a Python (*.py) example. If you
+are using IPython, please click the Google Colab icon above to view the example
+code. *Notifier* ```python import sys from ExceptNotifier import ExceptWechat,
+SuccessWechat, SendWechat # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__
+() #1 success sender except ExceptWechat as e: #2 except sender sys.exit()
+SendWechat().__call__() #3 customized sender ```
+## *Beep* No setup is required. Use as follows.
+*TEST* ```python from ExceptNotifier import beep beep(sec=1, freq=1000) ```
+*Notifier* ```python from Exceptnotifier import ExceptBeep, SuccessBeep,
+SendBeep(), beep() os.environ['BEEP_TIME'] = 1 sys.excepthook =
+ExceptBeep.__call__ try: print(1/20) SuccessBeep().__call__() #1 success beep-
+beep except ExceptBeep as e: #2 except beep-beep sys.exit() SendBeep().__call__
+() #3 customized beep-beep beep() ```
+## *Desktop* No setup is required. Use as follows.
+*TEST* ```python from ExceptNotifier import send_desktop_msg title_msg = "Test
+Title" body_msg = "Test Body" DISP_TIME = 5 send_desktop_msg(title_msg,
+body_msg, DISP_TIME) ``` *Notifier* ```python from ExceptNotifier import
+ExceptDesktop, SuccessDesktop, SendDesktop sys.excepthook =
+ExceptDesktop.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1
+success sender except ExceptDesktop as e: #2 except sender sys.exit()
+SendDesktop().__call__() #3 customized sender ```
 
 
 
-# License MIT # Bugs and Issues [Open a new issue](https://github.com/
+# Documentation [![Documentation Status](https://readthedocs.org/projects/
+exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/
+en/latest/) Official Document: https://exceptnotifier.readthedocs.io/en/latest/
+
+Documentation can be automatically generated by [Sphinx](https://www.sphinx-
+doc.org/en/master/usage/quickstart.html). But, I do not use [Google style]
+(https://google.github.io/styleguide/pyguide.html#383-functions-and-methods)
+because it requires [the Napoleon extension](https://sphinxcontrib-
+napoleon.readthedocs.io/en/latest/example_google.html) for Sphinx. I will use
+[m2r](https://github.com/miyakogi/m2r) to convert the README.md file to .rst so
+that it can be included. Having generated it with Sphinx, we can also host the
+documentation freely at [ReadTheDocs.org](https://citation-
+graph.readthedocs.io/en/latest/). # License ExceptNotifier: MIT
+Licenses apply the each [dependencies package](https://choosealicense.com/
+licenses/), and the created posts follow [CC BY-NC-SA](https://
+creativecommons.org/licenses/by-nc-sa/4.0/). # Bugs and Issues Sincerely
+grateful for any reports on new features or bugs. Your valuable feedback on the
+code is highly appreciated. [[Open a new issue]](https://github.com/
 dsdanielpark/ExceptNotifier/issues) # Contributing Guide I will announce
 contributing rules when the code development status changes to beta soon. Until
 then, please create an issue for feature requests and bug reports. I would
 greatly appreciate it if you use it a lot and give your opinions generously.
 Thank you sincerely. # Code of Conduct Everyone participating in the
 `ExceptNotifier` project, and in particular in the issue tracker, pull
 requests, and social media activity, is expected to treat other people with
 respect and more generally to follow the guidelines articulated in [the Python
-Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts
-Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark)
-Email parkminwoo1991@gmail.com
-- Developer note: [Link](./documents/DEV_NOTE.md) #### Could you kindly add
-this badge to your repository? ``` ![Except-Notifier](https://img.shields.io/
-badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if you could share
-the document widely by specifying that the source is the ExceptNotifier
-official github. ##### The package is currently in the development and QA
-stages, and the development stage will be updated at the top of this page. If
-it is determined that the product is stable through feature improvement,
-addition, and issue resolution, the development stage will reach stage 5. If no
-new updates or issues arise, it will be adjusted upward to stage 6 or higher.
+Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts :
+mortar_board: Core maintainer: [Daniel Park, South Korea](https://github.com/
+DSDanielPark)
+:envelope: Email: parkminwoo1991@gmail.com
+- Developer note: [Link](./documents/DEV_NOTE.md) #### Dev Note 1. Applying
+ExceptNotifier in Python In Python, we use [sys.excepthook](https://
+docs.python.org/ko/3/library/sys.html#sys.excepthook) to call the
+exceptnotifier by taking advantage of the interpreter calling sys.excepthook
+with three arguments (exception class, exception instance, traceback object)
+when an exception occurs. Since sys.excepthook is the highest-level exception
+handler that occurs just before the system shuts down, exceptnotifier is
+implemented as a class that inherits from baseexception and overrides
+sys.excepthook. For overriding exceptions that cannot be raised or exceptions
+raised in threads, please refer to the sys.unraisablehook() function and the
+threading.excepthook() function, respectively. 2. Application of ExceptNotifier
+in iPython Strictly, iPython is a package, not a programming language like
+Python, but it has been classified to aid understanding. IPython (Interactive
+Python) is a package consisting of a command shell for interactive computing
+for multiple programming languages. It is a very useful package that allows you
+to compile Python bit by bit in an interactive session through the concept of
+an interactive shell, but in iPython, control by sys.excepthook occurs just
+before the prompt is returned, so it is impossible to receive a traceback
+object using sys.excepthook and send an error message to each messenger app.
+Additionally, because it was necessary to inherit from baseexception, it was
+necessary to override other functions in iPython. Therefore, at first, we
+considered the [magics](https://ipython.readthedocs.io/en/stable/interactive/
+magics.html) in cell, but the problem of having to import the magic function
+every time in the cell can be cumbersome to use, so we decided to use the
+[set_custom_exc](https://ipython.readthedocs.io/en/stable/api/generated/
+IPython.core.interactiveshell.html) in iPython, which can work even by
+overriding it once. The set_custom_exc allows you to set a custom exception
+handler that is called when an exception in the exc_tuple occurs in the main
+loop (especially the run_code() method), and is designed so that the handle can
+return a structured traceback or None. Therefore, we can receive the traceback
+and send it to each messenger app. The order of top-level exception handling in
+iPython is different. You can use by `calling` raise in the `except` statement.
+3. Using Environment Variables (environ) In Python's except statement, it was
+designed to inherit exceptionbase, so we thought about how to pass variables
+into the class and decided to set variables through os.environ to use them by
+distributing them as a package. Additionally, since the user's webhook URL or
+API key will not change, we named the variables in uppercase and set special
+names to prevent contamination from duplicate variables. Since the variables
+are used within the class, we added an underscore before the variable name. 4.
+About example code For explanation, in Python, the example uses the overrided
+`sys.excepthook` in the except statement, like `except ExceptTelegram as e:`.
+However, you can use it simply by overriding `sys.excepthook` once and calling
+`raise` in the `except` statement. In IPython, you can use `set_custom_exc` to
+override the `Exception` with a user-defined function once, and then call
+`raise` in the `except` statement to repeatedly take the desired ExceptNotifier
+action. Also, although the example uses` ExceptTelegram.__call__` or
+`SuccessTelegram().__call__()`, these are expressions to aid understanding, and
+you can change them to a more concise form if you prefer. #### Could you kindly
+add this badge to your repository? ``` ![Except-Notifier](https://
+img.shields.io/badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if
+you could share the document widely by specifying that the source is the
+ExceptNotifier official github. ##### The package is currently in the
+development and QA stages, and the development stage will be updated at the top
+of this page. If it is determined that the product is stable through feature
+improvement, addition, and issue resolution, the development stage will reach
+stage 5. If no new updates or issues arise, it will be adjusted upward to stage
+6 or higher.
```

### Comparing `exceptnotifier-0.2.4/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.2.5/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ExceptNotifier.egg-info/PKG-INFO
 ExceptNotifier.egg-info/SOURCES.txt
 ExceptNotifier.egg-info/dependency_links.txt
 ExceptNotifier.egg-info/entry_points.txt
 ExceptNotifier.egg-info/requires.txt
 ExceptNotifier.egg-info/top_level.txt
 ExceptNotifier/base/__init__.py
+ExceptNotifier/base/bard_receiver.py
 ExceptNotifier/base/beep_sender.py
 ExceptNotifier/base/chime_sender.py
 ExceptNotifier/base/desktop_sender.py
 ExceptNotifier/base/discord_sender.py
 ExceptNotifier/base/kakao_sender.py
 ExceptNotifier/base/line_sender.py
 ExceptNotifier/base/mail_sender.py
```

### Comparing `exceptnotifier-0.2.4/LICENSE` & `exceptnotifier-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.4/PKG-INFO` & `exceptnotifier-0.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.4
+Version: 0.2.5
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,39 +16,40 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Development Status :: 2 - Pre-Alpha <br>
+
+Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
-Before QA<br> 
 
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
-<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
+<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-blue"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
+<a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/ExceptNotifier?color=blue"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
-
+<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black"></a>
+<a href="https://www.buymeacoffee.com/parkminwoo"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" height="20px"></a>
 </p>
 
 ![](./assets/imgs/main3.png)
-##### Provides a notification from the application shown in the captured screen.
+##### Provides a notification from the application shown in the captured screen. 
 
-# Python Package: ExceptNotifier
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
- The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
+# Python Package: ExceptNotifier [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com) [](https://img.shields.io/badge/License-MIT-blue.svg) [![Documentation Status](https://readthedocs.org/projects/exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/en/latest/)
+
+ The ExceptNotifier Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
-With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
+With ExceptNotifier, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
 ![](./assets/imgs/core02.png)
 
 <Br>
 
 
 # Supporting Applications
@@ -63,24 +64,28 @@
 - [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
 - [Wecaht](https://www.wechat.com/)
 - SMS Sending using [Twilio](https://www.twilio.com/en-us)
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 - [Opea AI API](https://openai.com/blog/openai-api)
         - If you have OpenAI API Key and model name, you can get information and code examples for debugging in any application.
-
-
+- [Google Bard](https://bard.google.com/) Python package [BardAPI](https://github.com/dsdanielpark/BARD_API)
+        - Starting from Exceptnotifier version 0.2.5
+        - Using the Python package [Bard API](https://github.com/dsdanielpark/BARD_API), if you declare the __Secure-1PSID value as a global variable , you can receive debugging hints and explanations about errors in your code through Google Bard.
 <br>
 
-# Quick Start
-```bash
-$ pip install ExceptNotifier
+# Install
+The latest stable release (and required dependencies) can be installed from PyPI:
 ```
-```bash
-$ pip install exceptnotifier
+pip install ExceptNotifier
+```
+
+You may instead want to use the development version from Github:
+```
+pip install git+https://github.com/dsdanielpark/ExceptNotifier.git
 ```
 
 <br><br><br>
 
 # Contents
 
 - [App Setup Overview](#app-setup-overview)
@@ -142,22 +147,25 @@
 |Discord|`_DISCORD_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptDiscord](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) |
 |AWS Chime|`_CHIME_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptChime](./tutorials/ExceptChime/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) |
 |G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) |
 |SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/ExceptTeams/GUIDE.md)|
-|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)|
+|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
 | OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/APIOpenAI/GUIDE.md)|
+| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://bard.google.com/)|
+
+- Starting from v0.2.5, you can receive debugging hints and examples through Google Bard using the same syntax as the OpenAI API. However, due to time constraints, examples will only be added for Telegram and Discord.
 
 <br>
 
 # Tutorial
 I will update tutorial ASAP. `README.md` is sufficient, but read the application's official documentation if necessary. However, we are preparing a more detailed and friendly tutorial.
 
 1. Main-tutorials: [Notebook](https://github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
@@ -390,26 +398,32 @@
 As all classes function the same, the example will only use one image, like in Telegram.
 ![](./assets/imgs/fig44.png)
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
 - b. Type /newbot to create a new bot <br>
 - c. Give your bot a name & a username <br>
 - d. Copy your new Telegram bot’s token <br>
 - e. You have to click `Start_bot` and must enter anything to your bot.
-   - Before use Notifier, Please use this to check if you follow guide. The Telegram bot may have a slight delay and it responded within 2-3 minutes.
+   - Before use Notifier, Please use this to check if you follow guide. The Telegram bot may have a slight delay and it responded within 2-3 minutes. <br>
+
+
+![](./assets/imgs/telegram.gif)
+
 *API TEST*
 ```python
 from ExceptNotifier import send_telegram_msg
 
 _TELEGRAM_TOKEN = "xxxxx:xxxxx-xxxx"
 send_telegram_msg(_TELEGRAM_TOKEN, 'msg')
 ```
 
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
 <br><br>
  
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 ### a. Notifier without OpenAI API
 *Notifier*
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys, os
 sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx"
@@ -468,14 +482,17 @@
 send_gmail_msg(
     _GMAIL_SENDER_ADDR,
     _GAMIL_RECIPIENT_ADDR,
     _GMAIL_APP_PASSWORD_OF_SENDER,
     subject_msg,
     body_msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail
 sys.excepthook = ExceptMail.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -552,20 +569,26 @@
 
 ## *Discord*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) 
 - a. Select the channel to receive notifications.
 - b. Click `Edit Channel` in the upper right corner of the chat window.
 - c. Click `Integrations` - `Webhook` - `New Webhook`.
 - d. Then click `Copy Webhook`.
+ 
+![](./assets/imgs/discord.gif)
+
 *API TEST*
 ```python
 from ExceptNotifier import send_discord_msg
 
 send_discord_msg(_DISCORD_WEBHOOK_URL, "Any Test Message") 
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import ExceptDiscord, SuccessDiscord, SendDiscord
 sys.excepthook = ExceptDiscord.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -588,21 +611,24 @@
 ## *Chime*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)
 
 - a. Select the Chat room to receive notifications.
 - b. Click `Room Setting` in the upper right corner.
 - c. Click `Manage Webhook and bot`
 - d. Create Add Webhook, set it up, then click `Copy Webhook`.
+ 
 *API TEST*
 ```python
 from ExceptNotifier import send_chime_msg
 
 send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message")
-
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import SuccessChime, ExceptChime, SendChime
 sys.excepthook = ExceptChime.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -623,20 +649,25 @@
 
 ## *Slack*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) 
 - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App`
 - c. Add webhook: Click `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace
 - d. Copy `Webhook URL`
+ 
 *API TEST*
 ```python
 from ExceptNotifier import send_slack_msg
 
 send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message")
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptSlack, SuccessSlack, SendSlack
 sys.excepthook = ExceptSlack.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -663,15 +694,16 @@
 
 *API TEST*
 ```python
 from ExceptNotifier import send_line_msg
 
 send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message")
 ```
-
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptLine, SuccessLine, SendLine
 sys.excepthook = ExceptLine.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -711,14 +743,16 @@
     _TWILIO_SID,
     _TWILIO_TOKEN,
     _SENDER_PHONE_NUMBER,
     _RECIPIENT_PHONE_NUMBER,
     "Any Test Message")
 ```
 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS
 sys.excepthook = ExceptSMS.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -753,14 +787,16 @@
 ```python
 from ExceptNotifier import send_teams_msg
 
 _TEAMS_WEBHOOK_URL = 'xxxx'
 
 send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message")
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptTeams, SuccessTeams, SendTeams
 sys.excepthook = ExceptTeams.__call__
 
@@ -777,14 +813,18 @@
 
 SendTeams().__call__()        #3 customized sender        
 ```
 
 <Br>
 
 ## *Kakaotalk*
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)
+
+
 - a. Sign up at the following site: [https://developers.kakao.com/](https://developers.kakao.com/)
 - b. Click `My Application` on the top bar.
 - c. Click `Add an application`, set a name, and create it.
 - d. Click `Kakao Login` in the left menu, then change the State of `Kakao Login Activation` to ON on the resulting page.
 - e. In `My Application > Product Settings > Kakao Login`, be sure to set `Redirect URI` as follows: [https://example.com/oauth](https://example.com/oauth)
 - f. In the left Consent Items menu, set `Send message in KakaoTalk` to optional agreement.
 - g. Copy the `REST API Key` in `My Application > App Settings > Summary`.
@@ -795,14 +835,17 @@
 ```python
 from ExceptNotifier import send_kakao_msg
 
 _KAKAO_TOKEN_PATH = 'xxx/xx/xxx.json'
 
 send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code. 
+
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptKakao, SuccessKakao, SendKakao
 sys.excepthook = ExceptKakao.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -817,21 +860,24 @@
     sys.exit()
 
 SendKakao().__call__()        #3 customized sender         
 ```
 
 
 ## *Wechat*
-a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770) <br>
 *API TEST*
 ```python
 from ExceptNotifier import send_wechat_msg
 
 send_wechat_msg(_WECHAT_WEBHOOK_URL, msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat
 
 # Define the next two variables optionally when using OpenAI's API.
 # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"    
@@ -847,15 +893,15 @@
 
 SendWechat().__call__()        #3 customized sender       
 ```
 
 <Br>
 
 ## *Beep*
-No setup is required. Use as follows.
+No setup is required. Use as follows. <br>
 *TEST*
 ```python
 from ExceptNotifier import beep
 
 beep(sec=1, freq=1000) 
 ```
 *Notifier*
@@ -877,15 +923,15 @@
 
 ```
 
 <Br>
 
 
 ## *Desktop*
-No setup is required. Use as follows.
+No setup is required. Use as follows. <br>
 *TEST*
 ```python
 from ExceptNotifier import send_desktop_msg
 
 title_msg = "Test Title"
 body_msg = "Test Body"
 DISP_TIME = 5
@@ -910,30 +956,60 @@
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
 
 <Br><br><br>
-# License
-MIT
+ 
+# Documentation [![Documentation Status](https://readthedocs.org/projects/exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/en/latest/)
+ 
+Official Document: https://exceptnotifier.readthedocs.io/en/latest/ <br> 
+Documentation can be automatically generated by [Sphinx](https://www.sphinx-doc.org/en/master/usage/quickstart.html). But, I do not use [Google style](https://google.github.io/styleguide/pyguide.html#383-functions-and-methods) because it requires [the Napoleon extension](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) for Sphinx. I will use [m2r](https://github.com/miyakogi/m2r) to convert the README.md file to .rst so that it can be included.
+
+Having generated it with Sphinx, we can also host the documentation freely at [ReadTheDocs.org](https://citation-graph.readthedocs.io/en/latest/). 
+ 
+# License 
+ExceptNotifier: MIT <br>
+Licenses apply the each [dependencies package](https://choosealicense.com/licenses/), and the created posts follow [CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/).
 
 # Bugs and Issues
-[Open a new issue](https://github.com/dsdanielpark/ExceptNotifier/issues)
+Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
+[[Open a new issue]](https://github.com/dsdanielpark/ExceptNotifier/issues) 
  
 # Contributing Guide
 I will announce contributing rules when the code development status changes to beta soon. Until then, please create an issue for feature requests and bug reports. I would greatly appreciate it if you use it a lot and give your opinions generously. Thank you sincerely.
 
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
 
 # Contacts
-Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
-Email parkminwoo1991@gmail.com <br>
+:mortar_board: Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
+:envelope: Email: parkminwoo1991@gmail.com <br>
 - Developer note: [Link](./documents/DEV_NOTE.md)
+#### Dev Note
+1. Applying ExceptNotifier in Python
+
+    In Python, we use [sys.excepthook](https://docs.python.org/ko/3/library/sys.html#sys.excepthook) to call the exceptnotifier by taking advantage of the interpreter calling sys.excepthook with three arguments (exception class, exception instance, traceback object) when an exception occurs. Since sys.excepthook is the highest-level exception handler that occurs just before the system shuts down, exceptnotifier is implemented as a class that inherits from baseexception and overrides sys.excepthook. For overriding exceptions that cannot be raised or exceptions raised in threads, please refer to the sys.unraisablehook() function and the threading.excepthook() function, respectively.
+
+2. Application of ExceptNotifier in iPython
+
+    Strictly, iPython is a package, not a programming language like Python, but it has been classified to aid understanding.
+    IPython (Interactive Python) is a package consisting of a command shell for interactive computing for multiple programming languages.
+
+    It is a very useful package that allows you to compile Python bit by bit in an interactive session through the concept of an interactive shell, but in iPython, control by sys.excepthook occurs just before the prompt is returned, so it is impossible to receive a traceback object using sys.excepthook and send an error message to each messenger app. Additionally, because it was necessary to inherit from baseexception, it was necessary to override other functions in iPython.
+
+    Therefore, at first, we considered the [magics](https://ipython.readthedocs.io/en/stable/interactive/magics.html) in cell, but the problem of having to import the magic function every time in the cell can be cumbersome to use, so we decided to use the [set_custom_exc](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.interactiveshell.html) in iPython, which can work even by overriding it once. The set_custom_exc allows you to set a custom exception handler that is called when an exception in the exc_tuple occurs in the main loop (especially the run_code() method), and is designed so that the handle can return a structured traceback or None. Therefore, we can receive the traceback and send it to each messenger app. The order of top-level exception handling in iPython is different. You can use by `calling` raise in the `except` statement.
+
+3. Using Environment Variables (environ)
+    In Python's except statement, it was designed to inherit exceptionbase, so we thought about how to pass variables into the class and decided to set variables through os.environ to use them by distributing them as a package. Additionally, since the user's webhook URL or API key will not change, we named the variables in uppercase and set special names to prevent contamination from duplicate variables. Since the variables are used within the class, we added an underscore before the variable name.
+
+4. About example code
+
+    For explanation, in Python, the example uses the overrided `sys.excepthook` in the except statement, like `except ExceptTelegram as e:`. However, you can use it simply by overriding `sys.excepthook` once and calling `raise` in the `except` statement. In IPython, you can use `set_custom_exc` to override the `Exception` with a user-defined function once, and then call `raise` in the `except` statement to repeatedly take the desired ExceptNotifier action. Also, although the example uses` ExceptTelegram.__call__` or `SuccessTelegram().__call__()`, these are expressions to aid understanding, and you can change them to a more concise form if you prefer.
 
 #### Could you kindly add this badge to your repository?
 ```
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ```
 
 I would appreciate it if you could share the document widely by specifying that the source is the ExceptNotifier official github.
```

#### html2text {}

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.4 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.5 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
 :: English Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 2 - Pre-Alpha
+LICENSE Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
-Before QA
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-[PyPI package] [PyPI] [Downloads] [Code_style:_black] [https://img.shields.io/
-                         badge/License-MIT-yellow.svg]
+[PyPI package] [PyPI] [Downloads] [commit update] [Code_style:_black] [https://
+img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black] [https:/
+        /www.buymeacoffee.com/assets/img/custom_images/orange_img.png]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
 shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
 /hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
-(https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
-flexible approach to receiving notifications by enhancing Python's try-except
-statement. This package enables you to receive alerts through various messaging
-applications or emails.
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
+(https://hits.seeyoufarm.com) [](https://img.shields.io/badge/License-MIT-
+blue.svg) [![Documentation Status](https://readthedocs.org/projects/
+exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/
+en/latest/) The ExceptNotifier Python package offers a flexible approach to
+receiving notifications by enhancing Python's try-except statement. This
+package enables you to receive alerts through various messaging applications or
+emails.
 
-With `ExceptNotifier`, you can obtain detailed compilation errors, including
+With ExceptNotifier, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
 accessible, streamlining your debugging process. ![](./assets/imgs/core02.png)
 # Supporting Applications Applicable to both [IPython](https://ipython.org/
 ) and [Python](https://www.python.org/), but needs to be ported differently
@@ -45,17 +48,24 @@
 [Microsoft Teams](https://www.microsoft.com/en/microsoft-teams/download-app) -
 [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
 - [Wecaht](https://www.wechat.com/) - SMS Sending using [Twilio](https://
 www.twilio.com/en-us) - Desktop Notification using [Plyer](https://github.com/
 kivy/plyer) - Beep Sound from [system](https://docs.python.org/3/library/
 winsound.html) - [Opea AI API](https://openai.com/blog/openai-api) - If you
 have OpenAI API Key and model name, you can get information and code examples
-for debugging in any application.
-# Quick Start ```bash $ pip install ExceptNotifier ``` ```bash $ pip install
-exceptnotifier ```
+for debugging in any application. - [Google Bard](https://bard.google.com/
+) Python package [BardAPI](https://github.com/dsdanielpark/BARD_API) - Starting
+from Exceptnotifier version 0.2.5 - Using the Python package [Bard API](https:/
+/github.com/dsdanielpark/BARD_API), if you declare the __Secure-1PSID value as
+a global variable , you can receive debugging hints and explanations about
+errors in your code through Google Bard.
+# Install The latest stable release (and required dependencies) can be
+installed from PyPI: ``` pip install ExceptNotifier ``` You may instead want to
+use the development version from Github: ``` pip install git+https://
+github.com/dsdanielpark/ExceptNotifier.git ```
 
 
 # Contents - [App Setup Overview](#app-setup-overview) - [Tutorial](#tutorial)
 - [Python Core](#python-core) * [Except`Notifier`](#exceptnotifier) + [AI
 Debbugging Infomation Notification](#ai-debbugging-infomation-notification) *
 [Success`Notifier`](#successnotifier) * [Send`Notifier`](#sendnotifier) *
 [Sender](#sender)
@@ -113,22 +123,28 @@
 `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not
 free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./
 tutorials/ExceptTeams/GUIDE.md)|
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|
-[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you add the following two
-variables to the required variables for each application in the table above,
-you can receive error location and explanation, as well as examples, from
-OpenAI's model | API | Required Variables | Free or Paid | Ease of Setup | Time
-Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |
-OpenAI API |`Required variables for each application`+
+[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
+If you add the following two variables to the required variables for each
+application in the table above, you can receive error location and explanation,
+as well as examples, from OpenAI's model | API | Required Variables | Free or
+Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:
+--:|:--:|:--:|:---:| | OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
-APIOpenAI/GUIDE.md)|
+APIOpenAI/GUIDE.md)| | Google Bard API |`Required variables for each
+application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://
+bard.google.com/)| - Starting from v0.2.5, you can receive debugging hints and
+examples through Google Bard using the same syntax as the OpenAI API. However,
+due to time constraints, examples will only be added for Telegram and Discord.
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
 [folder](https://github.com/DSDanielPark/ExceptNotifier/tree/main/tutorial).
 The tutorial is synchronized with the Python file name provided by
@@ -227,36 +243,38 @@
 fig44.png) - a. Open your telegram app and search for BotFather. (A built-in
 Telegram bot that helps users create custom Telegram bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 - e. You have to click `Start_bot` and must enter anything to your bot. -
 Before use Notifier, Please use this to check if you follow guide. The Telegram
-bot may have a slight delay and it responded within 2-3 minutes. *API TEST*
-```python from ExceptNotifier import send_telegram_msg _TELEGRAM_TOKEN =
-"xxxxx:xxxxx-xxxx" send_telegram_msg(_TELEGRAM_TOKEN, 'msg') ``` For more
-infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
-
-
-### a. Notifier without OpenAI API *Notifier* ```python from ExceptNotifier
-import ExceptTelegram, SuccessTelegram, SendTelegram import sys, os
-sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx"
-try: print(1/0) SuccessTelegram().__call__() #1. success sender except
+bot may have a slight delay and it responded within 2-3 minutes.
+![](./assets/imgs/telegram.gif) *API TEST* ```python from ExceptNotifier import
+send_telegram_msg _TELEGRAM_TOKEN = "xxxxx:xxxxx-xxxx" send_telegram_msg
+(_TELEGRAM_TOKEN, 'msg') ``` For more infomation, visit [Telegram Bot Father
+API](https://core.telegram.org/bots/api)
+
+##### This is a Python (*.py) example. If you are using IPython, please click
+the Google Colab icon above to view the example code. ### a. Notifier without
+OpenAI API *Notifier* ```python from ExceptNotifier import ExceptTelegram,
+SuccessTelegram, SendTelegram import sys, os sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0)
+SuccessTelegram().__call__() #1. success sender except ExceptTelegram as e: #2.
+except sender sys.exit() SendTelegram().__call__() #3. customized sender ```
+### b. Notifier with OpenAI API - If you just set `_OPEN_AI_API` and
+`_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL
+will automatically send debugging information as a message. Currently, it is
+mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that
+other models can be used later. *Notifier* ```python from ExceptNotifier import
+ExceptTelegram, SuccessTelegram, SendTelegram import sys, os sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.envirion
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try:
+print(1/0) SuccessTelegram().__call__() #1. success sender except
 ExceptTelegram as e: #2. except sender sys.exit() SendTelegram().__call__() #3.
-customized sender ``` ### b. Notifier with OpenAI API - If you just set
-`_OPEN_AI_API` and `_OPEN_AI_MODEL` environment variables in all application
-use case, AI MODEL will automatically send debugging information as a message.
-Currently, it is mainly based on the `GPT-3.5-TURBO` model, but we plan to
-update it so that other models can be used later. *Notifier* ```python from
-ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import sys,
-os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
-"xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion
-['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
-success sender except ExceptTelegram as e: #2. except sender sys.exit()
-SendTelegram().__call__() #3. customized sender ```
+customized sender ```
 ## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
 email is sent along with the error message. Additionally, you can send emails
 from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
@@ -264,19 +282,21 @@
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
 *API TEST* ```python from ExceptNotifier import send_gmail_msg
 _GMAIL_SENDER_ADDR = 'xxxx@gmail.com' _GAMIL_RECIPIENT_ADDR = 'xxxx@gmail.com'
 _GMAIL_APP_PASSWORD_OF_SENDER = 'xxxx' subject_msg = "Test Title" body_msg =
 "Test Body" send_gmail_msg( _GMAIL_SENDER_ADDR, _GAMIL_RECIPIENT_ADDR,
-_GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg) ``` *Notifier* ```python
-import sys, os from ExceptNotifier import ExceptMail, SuccessMail, SendMail
-sys.excepthook = ExceptMail.__call__ # Define the next two variables optionally
-when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" #
-os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ['_GAMIL_RECIPIENT_ADDR'] =
+_GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg) ``` ##### This is a
+Python (*.py) example. If you are using IPython, please click the Google Colab
+icon above to view the example code. *Notifier* ```python import sys, os from
+ExceptNotifier import ExceptMail, SuccessMail, SendMail sys.excepthook =
+ExceptMail.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_GAMIL_RECIPIENT_ADDR'] =
 'xxxxxxx@gmail.com' os.environ['_GMAIL_SENDER_ADDR'] = 'yyyyyy@gmail.com'
 os.environ['_GMAIL_APP_PASSWORD_OF_SENDER'] = 'zzzzzz' try: main() # Your Code
 Here SuccessMail().__call__() # No Exception -> Send Success mail. except
 ExceptMail: # Exception -> Send Fail mail. pass SendMail().__call__() # When
 Process Ended -> Any Line mail. ```   See Example... ```python import sys, os
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail # Define the next
 two variables optionally when using OpenAI's API. # os.environ
@@ -296,166 +316,251 @@
 ['_GMAIL_APP_PASSWORD_OF_SENDER'] = 'zzzzzz' try: 'your code' SuccessMail
 ().__call__() except ExceptMail: pass SendMail().__call__() ```
 ## *Discord* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) - a. Select the channel to
 receive notifications. - b. Click `Edit Channel` in the upper right corner of
 the chat window. - c. Click `Integrations` - `Webhook` - `New Webhook`. - d.
-Then click `Copy Webhook`. *API TEST* ```python from ExceptNotifier import
-send_discord_msg send_discord_msg(_DISCORD_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys, os from ExceptNotifier import ExceptDiscord,
-SuccessDiscord, SendDiscord sys.excepthook = ExceptDiscord.__call__ # Define
-the next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_DISCORD_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxx" try: print(1/20)
-SuccessDiscord().__call__() #1 success sender except ExceptDiscord as e: #2
-except sender sys.exit() SendDiscord().__call__() #3 customized sender ```
+Then click `Copy Webhook`. ![](./assets/imgs/discord.gif) *API TEST* ```python
+from ExceptNotifier import send_discord_msg send_discord_msg
+(_DISCORD_WEBHOOK_URL, "Any Test Message") ``` ##### This is a Python (*.py)
+example. If you are using IPython, please click the Google Colab icon above to
+view the example code. *Notifier* ```python import sys, os from ExceptNotifier
+import ExceptDiscord, SuccessDiscord, SendDiscord sys.excepthook =
+ExceptDiscord.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_DISCORD_WEBHOOK_URL'] =
+"xxxxxxxxxxxxxxxxx" try: print(1/20) SuccessDiscord().__call__() #1 success
+sender except ExceptDiscord as e: #2 except sender sys.exit() SendDiscord
+().__call__() #3 customized sender ```
 ## *Chime* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing) - a. Select the Chat room to
 receive notifications. - b. Click `Room Setting` in the upper right corner. -
 c. Click `Manage Webhook and bot` - d. Create Add Webhook, set it up, then
 click `Copy Webhook`. *API TEST* ```python from ExceptNotifier import
-send_chime_msg send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys, os from ExceptNotifier import SuccessChime,
-ExceptChime, SendChime sys.excepthook = ExceptChime.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx" try: print(1/0)
-SuccessChime().__call__() #1 success sender except ExceptChime as e: #2 except
-sender sys.exit() SendChime().__call__() #3 customized sender ```
+send_chime_msg send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message") ``` #####
+This is a Python (*.py) example. If you are using IPython, please click the
+Google Colab icon above to view the example code. *Notifier* ```python import
+sys, os from ExceptNotifier import SuccessChime, ExceptChime, SendChime
+sys.excepthook = ExceptChime.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
+['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx" try: print(1/0) SuccessChime
+().__call__() #1 success sender except ExceptChime as e: #2 except sender
+sys.exit() SendChime().__call__() #3 customized sender ```
 ## *Slack* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/1-
 dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App` - c. Add webhook: Click
 `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace -
 d. Copy `Webhook URL` *API TEST* ```python from ExceptNotifier import
-send_slack_msg send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys from ExceptNotifier import ExceptSlack,
-SuccessSlack, SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_SLACK_WEBHOOK_URL'] = 'https://hooks.slack.com/services/
-xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlack().__call__() #1 success
-sender except ExceptSlack as e: #2 except sender sys.exit() SendSlack
-().__call__() #3 customized sender ```
+send_slack_msg send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message") ``` #####
+This is a Python (*.py) example. If you are using IPython, please click the
+Google Colab icon above to view the example code. *Notifier* ```python import
+sys from ExceptNotifier import ExceptSlack, SuccessSlack, SendSlack
+sys.excepthook = ExceptSlack.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
+['_SLACK_WEBHOOK_URL'] = 'https://hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx'
+try: print(1/0) SuccessSlack().__call__() #1 success sender except ExceptSlack
+as e: #2 except sender sys.exit() SendSlack().__call__() #3 customized sender
+```
 ## *Line* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) - a. Register [https://notify-
 bot.line.me/](https://notify-bot.line.me/) - b. Go to mypage [https://notify-
 bot.line.me/my/](https://notify-bot.line.me/my/) - c. Click `Generate Token`,
 enter Service Name and click `1-on-1 chat with LINE` (anything you like) - d.
 Copy Token. *API TEST* ```python from ExceptNotifier import send_line_msg
-send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message") ``` *Notifier*
-```python import sys from ExceptNotifier import ExceptLine, SuccessLine,
-SendLine sys.excepthook = ExceptLine.__call__ # Define the next two variables
-optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
-['_LINE_NOTIFY_API_TOKEN'] = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
-().__call__() #1 success sender except ExceptLine as e: #2 except sender
-sys.exit() SendLine().__call__() #3 customized sender ```
+send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message") ``` ##### This is a
+Python (*.py) example. If you are using IPython, please click the Google Colab
+icon above to view the example code. *Notifier* ```python import sys from
+ExceptNotifier import ExceptLine, SuccessLine, SendLine sys.excepthook =
+ExceptLine.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_LINE_NOTIFY_API_TOKEN'] =
+'xxxxxxxxxxx' try: print(1/20) SuccessLine().__call__() #1 success sender
+except ExceptLine as e: #2 except sender sys.exit() SendLine().__call__() #3
+customized sender ```
 ## *SMS* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing) - a. Sign up for Twilio. [https:
 //www.twilio.com/en-us](https://www.twilio.com/en-us) - b. Click Console in the
 upper right corner. - c. Copy the variables provided in the console. *API TEST*
 ```python from ExceptNotifier import send_sms_msg _TWILIO_SID = 'xxxx'
 _TWILIO_TOKEN = "xxxx" _SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER =
 "xxxx" send_sms_msg( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER,
-_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` *Notifier* ```python import
-sys from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
-ExceptSMS.__call__ # Define the next two variables optionally when using
-OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
-['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TWILIO_SID'] = 'xxxx' os.environ
-['_TWILIO_TOKEN'] = 'yyyyyy' os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa",
-os.environ['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS
-().__call__() #1 success sender except ExceptSMS as e: #2 except sender
-sys.exit() SendSMS().__call__() #3 customized sender ```
+_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` ##### This is a Python (*.py)
+example. If you are using IPython, please click the Google Colab icon above to
+view the example code. *Notifier* ```python import sys from ExceptNotifier
+import ExceptSMS, SuccessSMS, SendSMS sys.excepthook = ExceptSMS.__call__ #
+Define the next two variables optionally when using OpenAI's API. # os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_TWILIO_SID'] = 'xxxx' os.environ['_TWILIO_TOKEN'] = 'yyyyyy'
+os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa", os.environ
+['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS().__call__() #1
+success sender except ExceptSMS as e: #2 except sender sys.exit() SendSMS
+().__call__() #3 customized sender ```
 ## *Teams* - a. Create the channel that you want to notify. - b. `App` -
 `Search: webhook` - `Incoming Webhook` [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
 the webhook incoming application is available. - c. Go to the team channel to
 receive notifications, and click `Connectors` in Settings. - d. `Connectors`
 After configuring webhook incoming in Connector, copy the webhook URL. *API
 TEST* ```python from ExceptNotifier import send_teams_msg _TEAMS_WEBHOOK_URL =
-'xxxx' send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message") ``` *Notifier*
-```python import sys from ExceptNotifier import ExceptTeams, SuccessTeams,
-SendTeams sys.excepthook = ExceptTeams.__call__ # Define the next two variables
-optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
-['_TEAMS_WEBHOOK_URL'] = 'microsoft webhook _TEAMS_WEBHOOK_URL' try: print(1/
-20) SuccessTeams().__call__() #1 success sender except ExceptTeams as e: #2
-except sender sys.exit() SendTeams().__call__() #3 customized sender ```
-## *Kakaotalk* - a. Sign up at the following site: [https://
-developers.kakao.com/](https://developers.kakao.com/) - b. Click `My
+'xxxx' send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message") ``` ##### This is
+a Python (*.py) example. If you are using IPython, please click the Google
+Colab icon above to view the example code. *Notifier* ```python import sys from
+ExceptNotifier import ExceptTeams, SuccessTeams, SendTeams sys.excepthook =
+ExceptTeams.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TEAMS_WEBHOOK_URL'] = 'microsoft
+webhook _TEAMS_WEBHOOK_URL' try: print(1/20) SuccessTeams().__call__() #1
+success sender except ExceptTeams as e: #2 except sender sys.exit() SendTeams
+().__call__() #3 customized sender ```
+## *Kakaotalk* [![Open In Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-
+lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing) - a. Sign up at the following site:
+[https://developers.kakao.com/](https://developers.kakao.com/) - b. Click `My
 Application` on the top bar. - c. Click `Add an application`, set a name, and
 create it. - d. Click `Kakao Login` in the left menu, then change the State of
 `Kakao Login Activation` to ON on the resulting page. - e. In `My Application >
 Product Settings > Kakao Login`, be sure to set `Redirect URI` as follows:
 [https://example.com/oauth](https://example.com/oauth) - f. In the left Consent
 Items menu, set `Send message in KakaoTalk` to optional agreement. - g. Copy
 the `REST API Key` in `My Application > App Settings > Summary`. - h. If you
 have successfully completed all of the above steps, go to the following
 document and follow the instructions: ./tutorials/kakao_token_generator.ipynb
 *API TEST* ```python from ExceptNotifier import send_kakao_msg
 _KAKAO_TOKEN_PATH = 'xxx/xx/xxx.json' send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
-``` *Notifier* ```python import sys from ExceptNotifier import ExceptKakao,
-SuccessKakao, SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_KAKAO_TOKEN_PATH'] = 'xxxx/xxx/xxx.json'' try: print(1/0)
-SuccessKakao().__call__() #1 success sender except ExceptKakao as e: #2 except
-sender sys.exit() SendKakao().__call__() #3 customized sender ``` ## *Wechat*
-a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/
-90136/91770) *API TEST* ```python from ExceptNotifier import send_wechat_msg
-send_wechat_msg(_WECHAT_WEBHOOK_URL, msg) ``` *Notifier* ```python import sys
-from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat # Define the
-next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx" sys.excepthook =
-ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__() #1 success
-sender except ExceptWechat as e: #2 except sender sys.exit() SendWechat
-().__call__() #3 customized sender ```
-## *Beep* No setup is required. Use as follows. *TEST* ```python from
-ExceptNotifier import beep beep(sec=1, freq=1000) ``` *Notifier* ```python from
-Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep() os.environ
-['BEEP_TIME'] = 1 sys.excepthook = ExceptBeep.__call__ try: print(1/20)
-SuccessBeep().__call__() #1 success beep-beep except ExceptBeep as e: #2 except
-beep-beep sys.exit() SendBeep().__call__() #3 customized beep-beep beep() ```
-## *Desktop* No setup is required. Use as follows. *TEST* ```python from
-ExceptNotifier import send_desktop_msg title_msg = "Test Title" body_msg =
-"Test Body" DISP_TIME = 5 send_desktop_msg(title_msg, body_msg, DISP_TIME) ```
-*Notifier* ```python from ExceptNotifier import ExceptDesktop, SuccessDesktop,
-SendDesktop sys.excepthook = ExceptDesktop.__call__ # Define the next two
-variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-try: print(1/0) SuccessDesktop().__call__() #1 success sender except
-ExceptDesktop as e: #2 except sender sys.exit() SendDesktop().__call__() #3
-customized sender ```
+``` ##### This is a Python (*.py) example. If you are using IPython, please
+click the Google Colab icon above to view the example code. *Notifier*
+```python import sys from ExceptNotifier import ExceptKakao, SuccessKakao,
+SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ['_KAKAO_TOKEN_PATH']
+= 'xxxx/xxx/xxx.json'' try: print(1/0) SuccessKakao().__call__() #1 success
+sender except ExceptKakao as e: #2 except sender sys.exit() SendKakao
+().__call__() #3 customized sender ``` ## *Wechat* a. Get Webhook URL by
+visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+*API TEST* ```python from ExceptNotifier import send_wechat_msg send_wechat_msg
+(_WECHAT_WEBHOOK_URL, msg) ``` ##### This is a Python (*.py) example. If you
+are using IPython, please click the Google Colab icon above to view the example
+code. *Notifier* ```python import sys from ExceptNotifier import ExceptWechat,
+SuccessWechat, SendWechat # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__
+() #1 success sender except ExceptWechat as e: #2 except sender sys.exit()
+SendWechat().__call__() #3 customized sender ```
+## *Beep* No setup is required. Use as follows.
+*TEST* ```python from ExceptNotifier import beep beep(sec=1, freq=1000) ```
+*Notifier* ```python from Exceptnotifier import ExceptBeep, SuccessBeep,
+SendBeep(), beep() os.environ['BEEP_TIME'] = 1 sys.excepthook =
+ExceptBeep.__call__ try: print(1/20) SuccessBeep().__call__() #1 success beep-
+beep except ExceptBeep as e: #2 except beep-beep sys.exit() SendBeep().__call__
+() #3 customized beep-beep beep() ```
+## *Desktop* No setup is required. Use as follows.
+*TEST* ```python from ExceptNotifier import send_desktop_msg title_msg = "Test
+Title" body_msg = "Test Body" DISP_TIME = 5 send_desktop_msg(title_msg,
+body_msg, DISP_TIME) ``` *Notifier* ```python from ExceptNotifier import
+ExceptDesktop, SuccessDesktop, SendDesktop sys.excepthook =
+ExceptDesktop.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1
+success sender except ExceptDesktop as e: #2 except sender sys.exit()
+SendDesktop().__call__() #3 customized sender ```
 
 
 
-# License MIT # Bugs and Issues [Open a new issue](https://github.com/
+# Documentation [![Documentation Status](https://readthedocs.org/projects/
+exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/
+en/latest/) Official Document: https://exceptnotifier.readthedocs.io/en/latest/
+
+Documentation can be automatically generated by [Sphinx](https://www.sphinx-
+doc.org/en/master/usage/quickstart.html). But, I do not use [Google style]
+(https://google.github.io/styleguide/pyguide.html#383-functions-and-methods)
+because it requires [the Napoleon extension](https://sphinxcontrib-
+napoleon.readthedocs.io/en/latest/example_google.html) for Sphinx. I will use
+[m2r](https://github.com/miyakogi/m2r) to convert the README.md file to .rst so
+that it can be included. Having generated it with Sphinx, we can also host the
+documentation freely at [ReadTheDocs.org](https://citation-
+graph.readthedocs.io/en/latest/). # License ExceptNotifier: MIT
+Licenses apply the each [dependencies package](https://choosealicense.com/
+licenses/), and the created posts follow [CC BY-NC-SA](https://
+creativecommons.org/licenses/by-nc-sa/4.0/). # Bugs and Issues Sincerely
+grateful for any reports on new features or bugs. Your valuable feedback on the
+code is highly appreciated. [[Open a new issue]](https://github.com/
 dsdanielpark/ExceptNotifier/issues) # Contributing Guide I will announce
 contributing rules when the code development status changes to beta soon. Until
 then, please create an issue for feature requests and bug reports. I would
 greatly appreciate it if you use it a lot and give your opinions generously.
 Thank you sincerely. # Code of Conduct Everyone participating in the
 `ExceptNotifier` project, and in particular in the issue tracker, pull
 requests, and social media activity, is expected to treat other people with
 respect and more generally to follow the guidelines articulated in [the Python
-Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts
-Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark)
-Email parkminwoo1991@gmail.com
-- Developer note: [Link](./documents/DEV_NOTE.md) #### Could you kindly add
-this badge to your repository? ``` ![Except-Notifier](https://img.shields.io/
-badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if you could share
-the document widely by specifying that the source is the ExceptNotifier
-official github. ##### The package is currently in the development and QA
-stages, and the development stage will be updated at the top of this page. If
-it is determined that the product is stable through feature improvement,
-addition, and issue resolution, the development stage will reach stage 5. If no
-new updates or issues arise, it will be adjusted upward to stage 6 or higher.
+Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts :
+mortar_board: Core maintainer: [Daniel Park, South Korea](https://github.com/
+DSDanielPark)
+:envelope: Email: parkminwoo1991@gmail.com
+- Developer note: [Link](./documents/DEV_NOTE.md) #### Dev Note 1. Applying
+ExceptNotifier in Python In Python, we use [sys.excepthook](https://
+docs.python.org/ko/3/library/sys.html#sys.excepthook) to call the
+exceptnotifier by taking advantage of the interpreter calling sys.excepthook
+with three arguments (exception class, exception instance, traceback object)
+when an exception occurs. Since sys.excepthook is the highest-level exception
+handler that occurs just before the system shuts down, exceptnotifier is
+implemented as a class that inherits from baseexception and overrides
+sys.excepthook. For overriding exceptions that cannot be raised or exceptions
+raised in threads, please refer to the sys.unraisablehook() function and the
+threading.excepthook() function, respectively. 2. Application of ExceptNotifier
+in iPython Strictly, iPython is a package, not a programming language like
+Python, but it has been classified to aid understanding. IPython (Interactive
+Python) is a package consisting of a command shell for interactive computing
+for multiple programming languages. It is a very useful package that allows you
+to compile Python bit by bit in an interactive session through the concept of
+an interactive shell, but in iPython, control by sys.excepthook occurs just
+before the prompt is returned, so it is impossible to receive a traceback
+object using sys.excepthook and send an error message to each messenger app.
+Additionally, because it was necessary to inherit from baseexception, it was
+necessary to override other functions in iPython. Therefore, at first, we
+considered the [magics](https://ipython.readthedocs.io/en/stable/interactive/
+magics.html) in cell, but the problem of having to import the magic function
+every time in the cell can be cumbersome to use, so we decided to use the
+[set_custom_exc](https://ipython.readthedocs.io/en/stable/api/generated/
+IPython.core.interactiveshell.html) in iPython, which can work even by
+overriding it once. The set_custom_exc allows you to set a custom exception
+handler that is called when an exception in the exc_tuple occurs in the main
+loop (especially the run_code() method), and is designed so that the handle can
+return a structured traceback or None. Therefore, we can receive the traceback
+and send it to each messenger app. The order of top-level exception handling in
+iPython is different. You can use by `calling` raise in the `except` statement.
+3. Using Environment Variables (environ) In Python's except statement, it was
+designed to inherit exceptionbase, so we thought about how to pass variables
+into the class and decided to set variables through os.environ to use them by
+distributing them as a package. Additionally, since the user's webhook URL or
+API key will not change, we named the variables in uppercase and set special
+names to prevent contamination from duplicate variables. Since the variables
+are used within the class, we added an underscore before the variable name. 4.
+About example code For explanation, in Python, the example uses the overrided
+`sys.excepthook` in the except statement, like `except ExceptTelegram as e:`.
+However, you can use it simply by overriding `sys.excepthook` once and calling
+`raise` in the `except` statement. In IPython, you can use `set_custom_exc` to
+override the `Exception` with a user-defined function once, and then call
+`raise` in the `except` statement to repeatedly take the desired ExceptNotifier
+action. Also, although the example uses` ExceptTelegram.__call__` or
+`SuccessTelegram().__call__()`, these are expressions to aid understanding, and
+you can change them to a more concise form if you prefer. #### Could you kindly
+add this badge to your repository? ``` ![Except-Notifier](https://
+img.shields.io/badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if
+you could share the document widely by specifying that the source is the
+ExceptNotifier official github. ##### The package is currently in the
+development and QA stages, and the development stage will be updated at the top
+of this page. If it is determined that the product is stable through feature
+improvement, addition, and issue resolution, the development stage will reach
+stage 5. If no new updates or issues arise, it will be adjusted upward to stage
+6 or higher.
```

### Comparing `exceptnotifier-0.2.4/README.md` & `exceptnotifier-0.2.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-Development Status :: 2 - Pre-Alpha <br>
+
+Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
-Before QA<br> 
 
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
-<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
+<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-blue"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
+<a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/ExceptNotifier?color=blue"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
-
+<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black"></a>
+<a href="https://www.buymeacoffee.com/parkminwoo"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" height="20px"></a>
 </p>
 
 ![](./assets/imgs/main3.png)
-##### Provides a notification from the application shown in the captured screen.
+##### Provides a notification from the application shown in the captured screen. 
 
-# Python Package: ExceptNotifier
-[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
- The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
+# Python Package: ExceptNotifier [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com) [](https://img.shields.io/badge/License-MIT-blue.svg) [![Documentation Status](https://readthedocs.org/projects/exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/en/latest/)
+
+ The ExceptNotifier Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
-With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
+With ExceptNotifier, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
 ![](./assets/imgs/core02.png)
 
 <Br>
 
 
 # Supporting Applications
@@ -41,24 +42,28 @@
 - [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
 - [Wecaht](https://www.wechat.com/)
 - SMS Sending using [Twilio](https://www.twilio.com/en-us)
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 - [Opea AI API](https://openai.com/blog/openai-api)
         - If you have OpenAI API Key and model name, you can get information and code examples for debugging in any application.
-
-
+- [Google Bard](https://bard.google.com/) Python package [BardAPI](https://github.com/dsdanielpark/BARD_API)
+        - Starting from Exceptnotifier version 0.2.5
+        - Using the Python package [Bard API](https://github.com/dsdanielpark/BARD_API), if you declare the __Secure-1PSID value as a global variable , you can receive debugging hints and explanations about errors in your code through Google Bard.
 <br>
 
-# Quick Start
-```bash
-$ pip install ExceptNotifier
+# Install
+The latest stable release (and required dependencies) can be installed from PyPI:
 ```
-```bash
-$ pip install exceptnotifier
+pip install ExceptNotifier
+```
+
+You may instead want to use the development version from Github:
+```
+pip install git+https://github.com/dsdanielpark/ExceptNotifier.git
 ```
 
 <br><br><br>
 
 # Contents
 
 - [App Setup Overview](#app-setup-overview)
@@ -120,22 +125,25 @@
 |Discord|`_DISCORD_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptDiscord](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) |
 |AWS Chime|`_CHIME_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptChime](./tutorials/ExceptChime/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) |
 |G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) |
 |SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/ExceptTeams/GUIDE.md)|
-|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)|
+|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
 | OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/APIOpenAI/GUIDE.md)|
+| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://bard.google.com/)|
+
+- Starting from v0.2.5, you can receive debugging hints and examples through Google Bard using the same syntax as the OpenAI API. However, due to time constraints, examples will only be added for Telegram and Discord.
 
 <br>
 
 # Tutorial
 I will update tutorial ASAP. `README.md` is sufficient, but read the application's official documentation if necessary. However, we are preparing a more detailed and friendly tutorial.
 
 1. Main-tutorials: [Notebook](https://github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
@@ -368,26 +376,32 @@
 As all classes function the same, the example will only use one image, like in Telegram.
 ![](./assets/imgs/fig44.png)
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
 - b. Type /newbot to create a new bot <br>
 - c. Give your bot a name & a username <br>
 - d. Copy your new Telegram bot’s token <br>
 - e. You have to click `Start_bot` and must enter anything to your bot.
-   - Before use Notifier, Please use this to check if you follow guide. The Telegram bot may have a slight delay and it responded within 2-3 minutes.
+   - Before use Notifier, Please use this to check if you follow guide. The Telegram bot may have a slight delay and it responded within 2-3 minutes. <br>
+
+
+![](./assets/imgs/telegram.gif)
+
 *API TEST*
 ```python
 from ExceptNotifier import send_telegram_msg
 
 _TELEGRAM_TOKEN = "xxxxx:xxxxx-xxxx"
 send_telegram_msg(_TELEGRAM_TOKEN, 'msg')
 ```
 
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
 <br><br>
  
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 ### a. Notifier without OpenAI API
 *Notifier*
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys, os
 sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx"
@@ -446,14 +460,17 @@
 send_gmail_msg(
     _GMAIL_SENDER_ADDR,
     _GAMIL_RECIPIENT_ADDR,
     _GMAIL_APP_PASSWORD_OF_SENDER,
     subject_msg,
     body_msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail
 sys.excepthook = ExceptMail.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -530,20 +547,26 @@
 
 ## *Discord*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) 
 - a. Select the channel to receive notifications.
 - b. Click `Edit Channel` in the upper right corner of the chat window.
 - c. Click `Integrations` - `Webhook` - `New Webhook`.
 - d. Then click `Copy Webhook`.
+ 
+![](./assets/imgs/discord.gif)
+
 *API TEST*
 ```python
 from ExceptNotifier import send_discord_msg
 
 send_discord_msg(_DISCORD_WEBHOOK_URL, "Any Test Message") 
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import ExceptDiscord, SuccessDiscord, SendDiscord
 sys.excepthook = ExceptDiscord.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -566,21 +589,24 @@
 ## *Chime*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)
 
 - a. Select the Chat room to receive notifications.
 - b. Click `Room Setting` in the upper right corner.
 - c. Click `Manage Webhook and bot`
 - d. Create Add Webhook, set it up, then click `Copy Webhook`.
+ 
 *API TEST*
 ```python
 from ExceptNotifier import send_chime_msg
 
 send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message")
-
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys, os
 from ExceptNotifier import SuccessChime, ExceptChime, SendChime
 sys.excepthook = ExceptChime.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -601,20 +627,25 @@
 
 ## *Slack*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) 
 - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App`
 - c. Add webhook: Click `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace
 - d. Copy `Webhook URL`
+ 
 *API TEST*
 ```python
 from ExceptNotifier import send_slack_msg
 
 send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message")
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptSlack, SuccessSlack, SendSlack
 sys.excepthook = ExceptSlack.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -641,15 +672,16 @@
 
 *API TEST*
 ```python
 from ExceptNotifier import send_line_msg
 
 send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message")
 ```
-
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptLine, SuccessLine, SendLine
 sys.excepthook = ExceptLine.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -689,14 +721,16 @@
     _TWILIO_SID,
     _TWILIO_TOKEN,
     _SENDER_PHONE_NUMBER,
     _RECIPIENT_PHONE_NUMBER,
     "Any Test Message")
 ```
 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS
 sys.excepthook = ExceptSMS.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -731,14 +765,16 @@
 ```python
 from ExceptNotifier import send_teams_msg
 
 _TEAMS_WEBHOOK_URL = 'xxxx'
 
 send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message")
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptTeams, SuccessTeams, SendTeams
 sys.excepthook = ExceptTeams.__call__
 
@@ -755,14 +791,18 @@
 
 SendTeams().__call__()        #3 customized sender        
 ```
 
 <Br>
 
 ## *Kakaotalk*
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)
+
+
 - a. Sign up at the following site: [https://developers.kakao.com/](https://developers.kakao.com/)
 - b. Click `My Application` on the top bar.
 - c. Click `Add an application`, set a name, and create it.
 - d. Click `Kakao Login` in the left menu, then change the State of `Kakao Login Activation` to ON on the resulting page.
 - e. In `My Application > Product Settings > Kakao Login`, be sure to set `Redirect URI` as follows: [https://example.com/oauth](https://example.com/oauth)
 - f. In the left Consent Items menu, set `Send message in KakaoTalk` to optional agreement.
 - g. Copy the `REST API Key` in `My Application > App Settings > Summary`.
@@ -773,14 +813,17 @@
 ```python
 from ExceptNotifier import send_kakao_msg
 
 _KAKAO_TOKEN_PATH = 'xxx/xx/xxx.json'
 
 send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code. 
+
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptKakao, SuccessKakao, SendKakao
 sys.excepthook = ExceptKakao.__call__
 
 # Define the next two variables optionally when using OpenAI's API.
@@ -795,21 +838,24 @@
     sys.exit()
 
 SendKakao().__call__()        #3 customized sender         
 ```
 
 
 ## *Wechat*
-a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770) <br>
 *API TEST*
 ```python
 from ExceptNotifier import send_wechat_msg
 
 send_wechat_msg(_WECHAT_WEBHOOK_URL, msg)
 ```
+ 
+##### This is a Python (*.py) example. If you are using IPython, please click the Google Colab icon above to view the example code.
+ 
 *Notifier*
 ```python
 import sys
 from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat
 
 # Define the next two variables optionally when using OpenAI's API.
 # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"    
@@ -825,15 +871,15 @@
 
 SendWechat().__call__()        #3 customized sender       
 ```
 
 <Br>
 
 ## *Beep*
-No setup is required. Use as follows.
+No setup is required. Use as follows. <br>
 *TEST*
 ```python
 from ExceptNotifier import beep
 
 beep(sec=1, freq=1000) 
 ```
 *Notifier*
@@ -855,15 +901,15 @@
 
 ```
 
 <Br>
 
 
 ## *Desktop*
-No setup is required. Use as follows.
+No setup is required. Use as follows. <br>
 *TEST*
 ```python
 from ExceptNotifier import send_desktop_msg
 
 title_msg = "Test Title"
 body_msg = "Test Body"
 DISP_TIME = 5
@@ -888,30 +934,60 @@
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
 
 <Br><br><br>
-# License
-MIT
+ 
+# Documentation [![Documentation Status](https://readthedocs.org/projects/exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/en/latest/)
+ 
+Official Document: https://exceptnotifier.readthedocs.io/en/latest/ <br> 
+Documentation can be automatically generated by [Sphinx](https://www.sphinx-doc.org/en/master/usage/quickstart.html). But, I do not use [Google style](https://google.github.io/styleguide/pyguide.html#383-functions-and-methods) because it requires [the Napoleon extension](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) for Sphinx. I will use [m2r](https://github.com/miyakogi/m2r) to convert the README.md file to .rst so that it can be included.
+
+Having generated it with Sphinx, we can also host the documentation freely at [ReadTheDocs.org](https://citation-graph.readthedocs.io/en/latest/). 
+ 
+# License 
+ExceptNotifier: MIT <br>
+Licenses apply the each [dependencies package](https://choosealicense.com/licenses/), and the created posts follow [CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/).
 
 # Bugs and Issues
-[Open a new issue](https://github.com/dsdanielpark/ExceptNotifier/issues)
+Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
+[[Open a new issue]](https://github.com/dsdanielpark/ExceptNotifier/issues) 
  
 # Contributing Guide
 I will announce contributing rules when the code development status changes to beta soon. Until then, please create an issue for feature requests and bug reports. I would greatly appreciate it if you use it a lot and give your opinions generously. Thank you sincerely.
 
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
 
 # Contacts
-Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
-Email parkminwoo1991@gmail.com <br>
+:mortar_board: Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
+:envelope: Email: parkminwoo1991@gmail.com <br>
 - Developer note: [Link](./documents/DEV_NOTE.md)
+#### Dev Note
+1. Applying ExceptNotifier in Python
+
+    In Python, we use [sys.excepthook](https://docs.python.org/ko/3/library/sys.html#sys.excepthook) to call the exceptnotifier by taking advantage of the interpreter calling sys.excepthook with three arguments (exception class, exception instance, traceback object) when an exception occurs. Since sys.excepthook is the highest-level exception handler that occurs just before the system shuts down, exceptnotifier is implemented as a class that inherits from baseexception and overrides sys.excepthook. For overriding exceptions that cannot be raised or exceptions raised in threads, please refer to the sys.unraisablehook() function and the threading.excepthook() function, respectively.
+
+2. Application of ExceptNotifier in iPython
+
+    Strictly, iPython is a package, not a programming language like Python, but it has been classified to aid understanding.
+    IPython (Interactive Python) is a package consisting of a command shell for interactive computing for multiple programming languages.
+
+    It is a very useful package that allows you to compile Python bit by bit in an interactive session through the concept of an interactive shell, but in iPython, control by sys.excepthook occurs just before the prompt is returned, so it is impossible to receive a traceback object using sys.excepthook and send an error message to each messenger app. Additionally, because it was necessary to inherit from baseexception, it was necessary to override other functions in iPython.
+
+    Therefore, at first, we considered the [magics](https://ipython.readthedocs.io/en/stable/interactive/magics.html) in cell, but the problem of having to import the magic function every time in the cell can be cumbersome to use, so we decided to use the [set_custom_exc](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.interactiveshell.html) in iPython, which can work even by overriding it once. The set_custom_exc allows you to set a custom exception handler that is called when an exception in the exc_tuple occurs in the main loop (especially the run_code() method), and is designed so that the handle can return a structured traceback or None. Therefore, we can receive the traceback and send it to each messenger app. The order of top-level exception handling in iPython is different. You can use by `calling` raise in the `except` statement.
+
+3. Using Environment Variables (environ)
+    In Python's except statement, it was designed to inherit exceptionbase, so we thought about how to pass variables into the class and decided to set variables through os.environ to use them by distributing them as a package. Additionally, since the user's webhook URL or API key will not change, we named the variables in uppercase and set special names to prevent contamination from duplicate variables. Since the variables are used within the class, we added an underscore before the variable name.
+
+4. About example code
+
+    For explanation, in Python, the example uses the overrided `sys.excepthook` in the except statement, like `except ExceptTelegram as e:`. However, you can use it simply by overriding `sys.excepthook` once and calling `raise` in the `except` statement. In IPython, you can use `set_custom_exc` to override the `Exception` with a user-defined function once, and then call `raise` in the `except` statement to repeatedly take the desired ExceptNotifier action. Also, although the example uses` ExceptTelegram.__call__` or `SuccessTelegram().__call__()`, these are expressions to aid understanding, and you can change them to a more concise form if you prefer.
 
 #### Could you kindly add this badge to your repository?
 ```
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ```
 
 I would appreciate it if you could share the document widely by specifying that the source is the ExceptNotifier official github.
```

#### html2text {}

```diff
@@ -1,25 +1,28 @@
-Development Status :: 2 - Pre-Alpha
+ Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
-Before QA
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-[PyPI package] [PyPI] [Downloads] [Code_style:_black] [https://img.shields.io/
-                         badge/License-MIT-yellow.svg]
+[PyPI package] [PyPI] [Downloads] [commit update] [Code_style:_black] [https://
+img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black] [https:/
+        /www.buymeacoffee.com/assets/img/custom_images/orange_img.png]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
 shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
 /hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
-(https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
-flexible approach to receiving notifications by enhancing Python's try-except
-statement. This package enables you to receive alerts through various messaging
-applications or emails.
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
+(https://hits.seeyoufarm.com) [](https://img.shields.io/badge/License-MIT-
+blue.svg) [![Documentation Status](https://readthedocs.org/projects/
+exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/
+en/latest/) The ExceptNotifier Python package offers a flexible approach to
+receiving notifications by enhancing Python's try-except statement. This
+package enables you to receive alerts through various messaging applications or
+emails.
 
-With `ExceptNotifier`, you can obtain detailed compilation errors, including
+With ExceptNotifier, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
 accessible, streamlining your debugging process. ![](./assets/imgs/core02.png)
 # Supporting Applications Applicable to both [IPython](https://ipython.org/
 ) and [Python](https://www.python.org/), but needs to be ported differently
@@ -31,17 +34,24 @@
 [Microsoft Teams](https://www.microsoft.com/en/microsoft-teams/download-app) -
 [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
 - [Wecaht](https://www.wechat.com/) - SMS Sending using [Twilio](https://
 www.twilio.com/en-us) - Desktop Notification using [Plyer](https://github.com/
 kivy/plyer) - Beep Sound from [system](https://docs.python.org/3/library/
 winsound.html) - [Opea AI API](https://openai.com/blog/openai-api) - If you
 have OpenAI API Key and model name, you can get information and code examples
-for debugging in any application.
-# Quick Start ```bash $ pip install ExceptNotifier ``` ```bash $ pip install
-exceptnotifier ```
+for debugging in any application. - [Google Bard](https://bard.google.com/
+) Python package [BardAPI](https://github.com/dsdanielpark/BARD_API) - Starting
+from Exceptnotifier version 0.2.5 - Using the Python package [Bard API](https:/
+/github.com/dsdanielpark/BARD_API), if you declare the __Secure-1PSID value as
+a global variable , you can receive debugging hints and explanations about
+errors in your code through Google Bard.
+# Install The latest stable release (and required dependencies) can be
+installed from PyPI: ``` pip install ExceptNotifier ``` You may instead want to
+use the development version from Github: ``` pip install git+https://
+github.com/dsdanielpark/ExceptNotifier.git ```
 
 
 # Contents - [App Setup Overview](#app-setup-overview) - [Tutorial](#tutorial)
 - [Python Core](#python-core) * [Except`Notifier`](#exceptnotifier) + [AI
 Debbugging Infomation Notification](#ai-debbugging-infomation-notification) *
 [Success`Notifier`](#successnotifier) * [Send`Notifier`](#sendnotifier) *
 [Sender](#sender)
@@ -99,22 +109,28 @@
 `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not
 free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./
 tutorials/ExceptTeams/GUIDE.md)|
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|
-[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you add the following two
-variables to the required variables for each application in the table above,
-you can receive error location and explanation, as well as examples, from
-OpenAI's model | API | Required Variables | Free or Paid | Ease of Setup | Time
-Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |
-OpenAI API |`Required variables for each application`+
+[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
+If you add the following two variables to the required variables for each
+application in the table above, you can receive error location and explanation,
+as well as examples, from OpenAI's model | API | Required Variables | Free or
+Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:
+--:|:--:|:--:|:---:| | OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
-APIOpenAI/GUIDE.md)|
+APIOpenAI/GUIDE.md)| | Google Bard API |`Required variables for each
+application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://
+bard.google.com/)| - Starting from v0.2.5, you can receive debugging hints and
+examples through Google Bard using the same syntax as the OpenAI API. However,
+due to time constraints, examples will only be added for Telegram and Discord.
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
 [folder](https://github.com/DSDanielPark/ExceptNotifier/tree/main/tutorial).
 The tutorial is synchronized with the Python file name provided by
@@ -213,36 +229,38 @@
 fig44.png) - a. Open your telegram app and search for BotFather. (A built-in
 Telegram bot that helps users create custom Telegram bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 - e. You have to click `Start_bot` and must enter anything to your bot. -
 Before use Notifier, Please use this to check if you follow guide. The Telegram
-bot may have a slight delay and it responded within 2-3 minutes. *API TEST*
-```python from ExceptNotifier import send_telegram_msg _TELEGRAM_TOKEN =
-"xxxxx:xxxxx-xxxx" send_telegram_msg(_TELEGRAM_TOKEN, 'msg') ``` For more
-infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
-
-
-### a. Notifier without OpenAI API *Notifier* ```python from ExceptNotifier
-import ExceptTelegram, SuccessTelegram, SendTelegram import sys, os
-sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx"
-try: print(1/0) SuccessTelegram().__call__() #1. success sender except
+bot may have a slight delay and it responded within 2-3 minutes.
+![](./assets/imgs/telegram.gif) *API TEST* ```python from ExceptNotifier import
+send_telegram_msg _TELEGRAM_TOKEN = "xxxxx:xxxxx-xxxx" send_telegram_msg
+(_TELEGRAM_TOKEN, 'msg') ``` For more infomation, visit [Telegram Bot Father
+API](https://core.telegram.org/bots/api)
+
+##### This is a Python (*.py) example. If you are using IPython, please click
+the Google Colab icon above to view the example code. ### a. Notifier without
+OpenAI API *Notifier* ```python from ExceptNotifier import ExceptTelegram,
+SuccessTelegram, SendTelegram import sys, os sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0)
+SuccessTelegram().__call__() #1. success sender except ExceptTelegram as e: #2.
+except sender sys.exit() SendTelegram().__call__() #3. customized sender ```
+### b. Notifier with OpenAI API - If you just set `_OPEN_AI_API` and
+`_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL
+will automatically send debugging information as a message. Currently, it is
+mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that
+other models can be used later. *Notifier* ```python from ExceptNotifier import
+ExceptTelegram, SuccessTelegram, SendTelegram import sys, os sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.envirion
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try:
+print(1/0) SuccessTelegram().__call__() #1. success sender except
 ExceptTelegram as e: #2. except sender sys.exit() SendTelegram().__call__() #3.
-customized sender ``` ### b. Notifier with OpenAI API - If you just set
-`_OPEN_AI_API` and `_OPEN_AI_MODEL` environment variables in all application
-use case, AI MODEL will automatically send debugging information as a message.
-Currently, it is mainly based on the `GPT-3.5-TURBO` model, but we plan to
-update it so that other models can be used later. *Notifier* ```python from
-ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import sys,
-os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
-"xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion
-['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
-success sender except ExceptTelegram as e: #2. except sender sys.exit()
-SendTelegram().__call__() #3. customized sender ```
+customized sender ```
 ## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
 email is sent along with the error message. Additionally, you can send emails
 from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
@@ -250,19 +268,21 @@
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
 *API TEST* ```python from ExceptNotifier import send_gmail_msg
 _GMAIL_SENDER_ADDR = 'xxxx@gmail.com' _GAMIL_RECIPIENT_ADDR = 'xxxx@gmail.com'
 _GMAIL_APP_PASSWORD_OF_SENDER = 'xxxx' subject_msg = "Test Title" body_msg =
 "Test Body" send_gmail_msg( _GMAIL_SENDER_ADDR, _GAMIL_RECIPIENT_ADDR,
-_GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg) ``` *Notifier* ```python
-import sys, os from ExceptNotifier import ExceptMail, SuccessMail, SendMail
-sys.excepthook = ExceptMail.__call__ # Define the next two variables optionally
-when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" #
-os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ['_GAMIL_RECIPIENT_ADDR'] =
+_GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg) ``` ##### This is a
+Python (*.py) example. If you are using IPython, please click the Google Colab
+icon above to view the example code. *Notifier* ```python import sys, os from
+ExceptNotifier import ExceptMail, SuccessMail, SendMail sys.excepthook =
+ExceptMail.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_GAMIL_RECIPIENT_ADDR'] =
 'xxxxxxx@gmail.com' os.environ['_GMAIL_SENDER_ADDR'] = 'yyyyyy@gmail.com'
 os.environ['_GMAIL_APP_PASSWORD_OF_SENDER'] = 'zzzzzz' try: main() # Your Code
 Here SuccessMail().__call__() # No Exception -> Send Success mail. except
 ExceptMail: # Exception -> Send Fail mail. pass SendMail().__call__() # When
 Process Ended -> Any Line mail. ```   See Example... ```python import sys, os
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail # Define the next
 two variables optionally when using OpenAI's API. # os.environ
@@ -282,166 +302,251 @@
 ['_GMAIL_APP_PASSWORD_OF_SENDER'] = 'zzzzzz' try: 'your code' SuccessMail
 ().__call__() except ExceptMail: pass SendMail().__call__() ```
 ## *Discord* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) - a. Select the channel to
 receive notifications. - b. Click `Edit Channel` in the upper right corner of
 the chat window. - c. Click `Integrations` - `Webhook` - `New Webhook`. - d.
-Then click `Copy Webhook`. *API TEST* ```python from ExceptNotifier import
-send_discord_msg send_discord_msg(_DISCORD_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys, os from ExceptNotifier import ExceptDiscord,
-SuccessDiscord, SendDiscord sys.excepthook = ExceptDiscord.__call__ # Define
-the next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_DISCORD_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxx" try: print(1/20)
-SuccessDiscord().__call__() #1 success sender except ExceptDiscord as e: #2
-except sender sys.exit() SendDiscord().__call__() #3 customized sender ```
+Then click `Copy Webhook`. ![](./assets/imgs/discord.gif) *API TEST* ```python
+from ExceptNotifier import send_discord_msg send_discord_msg
+(_DISCORD_WEBHOOK_URL, "Any Test Message") ``` ##### This is a Python (*.py)
+example. If you are using IPython, please click the Google Colab icon above to
+view the example code. *Notifier* ```python import sys, os from ExceptNotifier
+import ExceptDiscord, SuccessDiscord, SendDiscord sys.excepthook =
+ExceptDiscord.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_DISCORD_WEBHOOK_URL'] =
+"xxxxxxxxxxxxxxxxx" try: print(1/20) SuccessDiscord().__call__() #1 success
+sender except ExceptDiscord as e: #2 except sender sys.exit() SendDiscord
+().__call__() #3 customized sender ```
 ## *Chime* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing) - a. Select the Chat room to
 receive notifications. - b. Click `Room Setting` in the upper right corner. -
 c. Click `Manage Webhook and bot` - d. Create Add Webhook, set it up, then
 click `Copy Webhook`. *API TEST* ```python from ExceptNotifier import
-send_chime_msg send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys, os from ExceptNotifier import SuccessChime,
-ExceptChime, SendChime sys.excepthook = ExceptChime.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx" try: print(1/0)
-SuccessChime().__call__() #1 success sender except ExceptChime as e: #2 except
-sender sys.exit() SendChime().__call__() #3 customized sender ```
+send_chime_msg send_chime_msg(_CHIME_WEBHOOK_URL, "Any Test Message") ``` #####
+This is a Python (*.py) example. If you are using IPython, please click the
+Google Colab icon above to view the example code. *Notifier* ```python import
+sys, os from ExceptNotifier import SuccessChime, ExceptChime, SendChime
+sys.excepthook = ExceptChime.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
+['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx" try: print(1/0) SuccessChime
+().__call__() #1 success sender except ExceptChime as e: #2 except sender
+sys.exit() SendChime().__call__() #3 customized sender ```
 ## *Slack* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/1-
 dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App` - c. Add webhook: Click
 `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace -
 d. Copy `Webhook URL` *API TEST* ```python from ExceptNotifier import
-send_slack_msg send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message") ```
-*Notifier* ```python import sys from ExceptNotifier import ExceptSlack,
-SuccessSlack, SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_SLACK_WEBHOOK_URL'] = 'https://hooks.slack.com/services/
-xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlack().__call__() #1 success
-sender except ExceptSlack as e: #2 except sender sys.exit() SendSlack
-().__call__() #3 customized sender ```
+send_slack_msg send_slack_msg(_SLACK_WEBHOOK_URL, "Any Test Message") ``` #####
+This is a Python (*.py) example. If you are using IPython, please click the
+Google Colab icon above to view the example code. *Notifier* ```python import
+sys from ExceptNotifier import ExceptSlack, SuccessSlack, SendSlack
+sys.excepthook = ExceptSlack.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
+['_SLACK_WEBHOOK_URL'] = 'https://hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx'
+try: print(1/0) SuccessSlack().__call__() #1 success sender except ExceptSlack
+as e: #2 except sender sys.exit() SendSlack().__call__() #3 customized sender
+```
 ## *Line* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) - a. Register [https://notify-
 bot.line.me/](https://notify-bot.line.me/) - b. Go to mypage [https://notify-
 bot.line.me/my/](https://notify-bot.line.me/my/) - c. Click `Generate Token`,
 enter Service Name and click `1-on-1 chat with LINE` (anything you like) - d.
 Copy Token. *API TEST* ```python from ExceptNotifier import send_line_msg
-send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message") ``` *Notifier*
-```python import sys from ExceptNotifier import ExceptLine, SuccessLine,
-SendLine sys.excepthook = ExceptLine.__call__ # Define the next two variables
-optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
-['_LINE_NOTIFY_API_TOKEN'] = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
-().__call__() #1 success sender except ExceptLine as e: #2 except sender
-sys.exit() SendLine().__call__() #3 customized sender ```
+send_line_msg(_LINE_NOTIFY_API_TOKEN:, "Any Test Message") ``` ##### This is a
+Python (*.py) example. If you are using IPython, please click the Google Colab
+icon above to view the example code. *Notifier* ```python import sys from
+ExceptNotifier import ExceptLine, SuccessLine, SendLine sys.excepthook =
+ExceptLine.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_LINE_NOTIFY_API_TOKEN'] =
+'xxxxxxxxxxx' try: print(1/20) SuccessLine().__call__() #1 success sender
+except ExceptLine as e: #2 except sender sys.exit() SendLine().__call__() #3
+customized sender ```
 ## *SMS* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing) - a. Sign up for Twilio. [https:
 //www.twilio.com/en-us](https://www.twilio.com/en-us) - b. Click Console in the
 upper right corner. - c. Copy the variables provided in the console. *API TEST*
 ```python from ExceptNotifier import send_sms_msg _TWILIO_SID = 'xxxx'
 _TWILIO_TOKEN = "xxxx" _SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER =
 "xxxx" send_sms_msg( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER,
-_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` *Notifier* ```python import
-sys from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
-ExceptSMS.__call__ # Define the next two variables optionally when using
-OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
-['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TWILIO_SID'] = 'xxxx' os.environ
-['_TWILIO_TOKEN'] = 'yyyyyy' os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa",
-os.environ['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS
-().__call__() #1 success sender except ExceptSMS as e: #2 except sender
-sys.exit() SendSMS().__call__() #3 customized sender ```
+_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` ##### This is a Python (*.py)
+example. If you are using IPython, please click the Google Colab icon above to
+view the example code. *Notifier* ```python import sys from ExceptNotifier
+import ExceptSMS, SuccessSMS, SendSMS sys.excepthook = ExceptSMS.__call__ #
+Define the next two variables optionally when using OpenAI's API. # os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_TWILIO_SID'] = 'xxxx' os.environ['_TWILIO_TOKEN'] = 'yyyyyy'
+os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa", os.environ
+['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS().__call__() #1
+success sender except ExceptSMS as e: #2 except sender sys.exit() SendSMS
+().__call__() #3 customized sender ```
 ## *Teams* - a. Create the channel that you want to notify. - b. `App` -
 `Search: webhook` - `Incoming Webhook` [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
 the webhook incoming application is available. - c. Go to the team channel to
 receive notifications, and click `Connectors` in Settings. - d. `Connectors`
 After configuring webhook incoming in Connector, copy the webhook URL. *API
 TEST* ```python from ExceptNotifier import send_teams_msg _TEAMS_WEBHOOK_URL =
-'xxxx' send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message") ``` *Notifier*
-```python import sys from ExceptNotifier import ExceptTeams, SuccessTeams,
-SendTeams sys.excepthook = ExceptTeams.__call__ # Define the next two variables
-optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
-['_TEAMS_WEBHOOK_URL'] = 'microsoft webhook _TEAMS_WEBHOOK_URL' try: print(1/
-20) SuccessTeams().__call__() #1 success sender except ExceptTeams as e: #2
-except sender sys.exit() SendTeams().__call__() #3 customized sender ```
-## *Kakaotalk* - a. Sign up at the following site: [https://
-developers.kakao.com/](https://developers.kakao.com/) - b. Click `My
+'xxxx' send_teams_msg(_TEAMS_WEBHOOK_URL, "Any Test Message") ``` ##### This is
+a Python (*.py) example. If you are using IPython, please click the Google
+Colab icon above to view the example code. *Notifier* ```python import sys from
+ExceptNotifier import ExceptTeams, SuccessTeams, SendTeams sys.excepthook =
+ExceptTeams.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TEAMS_WEBHOOK_URL'] = 'microsoft
+webhook _TEAMS_WEBHOOK_URL' try: print(1/20) SuccessTeams().__call__() #1
+success sender except ExceptTeams as e: #2 except sender sys.exit() SendTeams
+().__call__() #3 customized sender ```
+## *Kakaotalk* [![Open In Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-
+lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing) - a. Sign up at the following site:
+[https://developers.kakao.com/](https://developers.kakao.com/) - b. Click `My
 Application` on the top bar. - c. Click `Add an application`, set a name, and
 create it. - d. Click `Kakao Login` in the left menu, then change the State of
 `Kakao Login Activation` to ON on the resulting page. - e. In `My Application >
 Product Settings > Kakao Login`, be sure to set `Redirect URI` as follows:
 [https://example.com/oauth](https://example.com/oauth) - f. In the left Consent
 Items menu, set `Send message in KakaoTalk` to optional agreement. - g. Copy
 the `REST API Key` in `My Application > App Settings > Summary`. - h. If you
 have successfully completed all of the above steps, go to the following
 document and follow the instructions: ./tutorials/kakao_token_generator.ipynb
 *API TEST* ```python from ExceptNotifier import send_kakao_msg
 _KAKAO_TOKEN_PATH = 'xxx/xx/xxx.json' send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
-``` *Notifier* ```python import sys from ExceptNotifier import ExceptKakao,
-SuccessKakao, SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next
-two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_KAKAO_TOKEN_PATH'] = 'xxxx/xxx/xxx.json'' try: print(1/0)
-SuccessKakao().__call__() #1 success sender except ExceptKakao as e: #2 except
-sender sys.exit() SendKakao().__call__() #3 customized sender ``` ## *Wechat*
-a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/
-90136/91770) *API TEST* ```python from ExceptNotifier import send_wechat_msg
-send_wechat_msg(_WECHAT_WEBHOOK_URL, msg) ``` *Notifier* ```python import sys
-from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat # Define the
-next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx" sys.excepthook =
-ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__() #1 success
-sender except ExceptWechat as e: #2 except sender sys.exit() SendWechat
-().__call__() #3 customized sender ```
-## *Beep* No setup is required. Use as follows. *TEST* ```python from
-ExceptNotifier import beep beep(sec=1, freq=1000) ``` *Notifier* ```python from
-Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep() os.environ
-['BEEP_TIME'] = 1 sys.excepthook = ExceptBeep.__call__ try: print(1/20)
-SuccessBeep().__call__() #1 success beep-beep except ExceptBeep as e: #2 except
-beep-beep sys.exit() SendBeep().__call__() #3 customized beep-beep beep() ```
-## *Desktop* No setup is required. Use as follows. *TEST* ```python from
-ExceptNotifier import send_desktop_msg title_msg = "Test Title" body_msg =
-"Test Body" DISP_TIME = 5 send_desktop_msg(title_msg, body_msg, DISP_TIME) ```
-*Notifier* ```python from ExceptNotifier import ExceptDesktop, SuccessDesktop,
-SendDesktop sys.excepthook = ExceptDesktop.__call__ # Define the next two
-variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-try: print(1/0) SuccessDesktop().__call__() #1 success sender except
-ExceptDesktop as e: #2 except sender sys.exit() SendDesktop().__call__() #3
-customized sender ```
+``` ##### This is a Python (*.py) example. If you are using IPython, please
+click the Google Colab icon above to view the example code. *Notifier*
+```python import sys from ExceptNotifier import ExceptKakao, SuccessKakao,
+SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next two variables
+optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
+turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ['_KAKAO_TOKEN_PATH']
+= 'xxxx/xxx/xxx.json'' try: print(1/0) SuccessKakao().__call__() #1 success
+sender except ExceptKakao as e: #2 except sender sys.exit() SendKakao
+().__call__() #3 customized sender ``` ## *Wechat* a. Get Webhook URL by
+visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+*API TEST* ```python from ExceptNotifier import send_wechat_msg send_wechat_msg
+(_WECHAT_WEBHOOK_URL, msg) ``` ##### This is a Python (*.py) example. If you
+are using IPython, please click the Google Colab icon above to view the example
+code. *Notifier* ```python import sys from ExceptNotifier import ExceptWechat,
+SuccessWechat, SendWechat # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__
+() #1 success sender except ExceptWechat as e: #2 except sender sys.exit()
+SendWechat().__call__() #3 customized sender ```
+## *Beep* No setup is required. Use as follows.
+*TEST* ```python from ExceptNotifier import beep beep(sec=1, freq=1000) ```
+*Notifier* ```python from Exceptnotifier import ExceptBeep, SuccessBeep,
+SendBeep(), beep() os.environ['BEEP_TIME'] = 1 sys.excepthook =
+ExceptBeep.__call__ try: print(1/20) SuccessBeep().__call__() #1 success beep-
+beep except ExceptBeep as e: #2 except beep-beep sys.exit() SendBeep().__call__
+() #3 customized beep-beep beep() ```
+## *Desktop* No setup is required. Use as follows.
+*TEST* ```python from ExceptNotifier import send_desktop_msg title_msg = "Test
+Title" body_msg = "Test Body" DISP_TIME = 5 send_desktop_msg(title_msg,
+body_msg, DISP_TIME) ``` *Notifier* ```python from ExceptNotifier import
+ExceptDesktop, SuccessDesktop, SendDesktop sys.excepthook =
+ExceptDesktop.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1
+success sender except ExceptDesktop as e: #2 except sender sys.exit()
+SendDesktop().__call__() #3 customized sender ```
 
 
 
-# License MIT # Bugs and Issues [Open a new issue](https://github.com/
+# Documentation [![Documentation Status](https://readthedocs.org/projects/
+exceptnotifier/badge/?version=latest)](https://exceptnotifier.readthedocs.io/
+en/latest/) Official Document: https://exceptnotifier.readthedocs.io/en/latest/
+
+Documentation can be automatically generated by [Sphinx](https://www.sphinx-
+doc.org/en/master/usage/quickstart.html). But, I do not use [Google style]
+(https://google.github.io/styleguide/pyguide.html#383-functions-and-methods)
+because it requires [the Napoleon extension](https://sphinxcontrib-
+napoleon.readthedocs.io/en/latest/example_google.html) for Sphinx. I will use
+[m2r](https://github.com/miyakogi/m2r) to convert the README.md file to .rst so
+that it can be included. Having generated it with Sphinx, we can also host the
+documentation freely at [ReadTheDocs.org](https://citation-
+graph.readthedocs.io/en/latest/). # License ExceptNotifier: MIT
+Licenses apply the each [dependencies package](https://choosealicense.com/
+licenses/), and the created posts follow [CC BY-NC-SA](https://
+creativecommons.org/licenses/by-nc-sa/4.0/). # Bugs and Issues Sincerely
+grateful for any reports on new features or bugs. Your valuable feedback on the
+code is highly appreciated. [[Open a new issue]](https://github.com/
 dsdanielpark/ExceptNotifier/issues) # Contributing Guide I will announce
 contributing rules when the code development status changes to beta soon. Until
 then, please create an issue for feature requests and bug reports. I would
 greatly appreciate it if you use it a lot and give your opinions generously.
 Thank you sincerely. # Code of Conduct Everyone participating in the
 `ExceptNotifier` project, and in particular in the issue tracker, pull
 requests, and social media activity, is expected to treat other people with
 respect and more generally to follow the guidelines articulated in [the Python
-Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts
-Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark)
-Email parkminwoo1991@gmail.com
-- Developer note: [Link](./documents/DEV_NOTE.md) #### Could you kindly add
-this badge to your repository? ``` ![Except-Notifier](https://img.shields.io/
-badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if you could share
-the document widely by specifying that the source is the ExceptNotifier
-official github. ##### The package is currently in the development and QA
-stages, and the development stage will be updated at the top of this page. If
-it is determined that the product is stable through feature improvement,
-addition, and issue resolution, the development stage will reach stage 5. If no
-new updates or issues arise, it will be adjusted upward to stage 6 or higher.
+Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts :
+mortar_board: Core maintainer: [Daniel Park, South Korea](https://github.com/
+DSDanielPark)
+:envelope: Email: parkminwoo1991@gmail.com
+- Developer note: [Link](./documents/DEV_NOTE.md) #### Dev Note 1. Applying
+ExceptNotifier in Python In Python, we use [sys.excepthook](https://
+docs.python.org/ko/3/library/sys.html#sys.excepthook) to call the
+exceptnotifier by taking advantage of the interpreter calling sys.excepthook
+with three arguments (exception class, exception instance, traceback object)
+when an exception occurs. Since sys.excepthook is the highest-level exception
+handler that occurs just before the system shuts down, exceptnotifier is
+implemented as a class that inherits from baseexception and overrides
+sys.excepthook. For overriding exceptions that cannot be raised or exceptions
+raised in threads, please refer to the sys.unraisablehook() function and the
+threading.excepthook() function, respectively. 2. Application of ExceptNotifier
+in iPython Strictly, iPython is a package, not a programming language like
+Python, but it has been classified to aid understanding. IPython (Interactive
+Python) is a package consisting of a command shell for interactive computing
+for multiple programming languages. It is a very useful package that allows you
+to compile Python bit by bit in an interactive session through the concept of
+an interactive shell, but in iPython, control by sys.excepthook occurs just
+before the prompt is returned, so it is impossible to receive a traceback
+object using sys.excepthook and send an error message to each messenger app.
+Additionally, because it was necessary to inherit from baseexception, it was
+necessary to override other functions in iPython. Therefore, at first, we
+considered the [magics](https://ipython.readthedocs.io/en/stable/interactive/
+magics.html) in cell, but the problem of having to import the magic function
+every time in the cell can be cumbersome to use, so we decided to use the
+[set_custom_exc](https://ipython.readthedocs.io/en/stable/api/generated/
+IPython.core.interactiveshell.html) in iPython, which can work even by
+overriding it once. The set_custom_exc allows you to set a custom exception
+handler that is called when an exception in the exc_tuple occurs in the main
+loop (especially the run_code() method), and is designed so that the handle can
+return a structured traceback or None. Therefore, we can receive the traceback
+and send it to each messenger app. The order of top-level exception handling in
+iPython is different. You can use by `calling` raise in the `except` statement.
+3. Using Environment Variables (environ) In Python's except statement, it was
+designed to inherit exceptionbase, so we thought about how to pass variables
+into the class and decided to set variables through os.environ to use them by
+distributing them as a package. Additionally, since the user's webhook URL or
+API key will not change, we named the variables in uppercase and set special
+names to prevent contamination from duplicate variables. Since the variables
+are used within the class, we added an underscore before the variable name. 4.
+About example code For explanation, in Python, the example uses the overrided
+`sys.excepthook` in the except statement, like `except ExceptTelegram as e:`.
+However, you can use it simply by overriding `sys.excepthook` once and calling
+`raise` in the `except` statement. In IPython, you can use `set_custom_exc` to
+override the `Exception` with a user-defined function once, and then call
+`raise` in the `except` statement to repeatedly take the desired ExceptNotifier
+action. Also, although the example uses` ExceptTelegram.__call__` or
+`SuccessTelegram().__call__()`, these are expressions to aid understanding, and
+you can change them to a more concise form if you prefer. #### Could you kindly
+add this badge to your repository? ``` ![Except-Notifier](https://
+img.shields.io/badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if
+you could share the document widely by specifying that the source is the
+ExceptNotifier official github. ##### The package is currently in the
+development and QA stages, and the development stage will be updated at the top
+of this page. If it is determined that the product is stable through feature
+improvement, addition, and issue resolution, the development stage will reach
+stage 5. If no new updates or issues arise, it will be adjusted upward to stage
+6 or higher.
```

### Comparing `exceptnotifier-0.2.4/setup.py` & `exceptnotifier-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.2.4",
+    version="0.2.5",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```


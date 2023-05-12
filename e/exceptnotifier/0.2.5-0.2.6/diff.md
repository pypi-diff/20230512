# Comparing `tmp/exceptnotifier-0.2.5.tar.gz` & `tmp/exceptnotifier-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.2.5.tar", last modified: Fri May 12 10:20:32 2023, max compression
+gzip compressed data, was "exceptnotifier-0.2.6.tar", last modified: Fri May 12 10:55:29 2023, max compression
```

## Comparing `exceptnotifier-0.2.5.tar` & `exceptnotifier-0.2.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.401742 exceptnotifier-0.2.5/
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.256895 exceptnotifier-0.2.5/ExceptNotifier/
--rw-rw-rw-   0        0        0     4847 2023-05-12 10:19:31.000000 exceptnotifier-0.2.5/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.318189 exceptnotifier-0.2.5/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1382 2023-05-12 10:19:43.000000 exceptnotifier-0.2.5/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/base/bard_receiver.py
--rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.5/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.5/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.5/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0     1009 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.5/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.5/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.5/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.5/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.5/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.5/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.5/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.5/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.5/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.5/ExceptNotifier/base/whatsapp_sender.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.351176 exceptnotifier-0.2.5/ExceptNotifier/ipycore/
--rw-rw-rw-   0        0        0     1472 2023-05-12 10:19:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/__init__.py
--rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/beep_notifier_ipython.py
--rw-rw-rw-   0        0        0     2578 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/chime_notifier_ipython.py
--rw-rw-rw-   0        0        0     2947 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/desktop_notifier_ipython.py
--rw-rw-rw-   0        0        0     2590 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/discord_notifier_ipython.py
--rw-rw-rw-   0        0        0     2570 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/kakao_notifier_ipython.py
--rw-rw-rw-   0        0        0     2584 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/line_notifier_ipython.py
--rw-rw-rw-   0        0        0     4013 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/mail_notifier_ipython.py
--rw-rw-rw-   0        0        0     2577 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/slack_notifier_ipython.py
--rw-rw-rw-   0        0        0     3049 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/sms_notifier_ipython.py
--rw-rw-rw-   0        0        0     2581 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/teams_notifier_ipython.py
--rw-rw-rw-   0        0        0     2583 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/telegram_notifier_ipython.py
--rw-rw-rw-   0        0        0     2591 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/ipycore/wechat_notifier_ipython.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.384815 exceptnotifier-0.2.5/ExceptNotifier/pycore/
--rw-rw-rw-   0        0        0     2009 2023-05-12 10:20:13.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-05-12 05:17:37.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/beep_notifier.py
--rw-rw-rw-   0        0        0     7700 2023-05-12 10:13:08.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/chime_notifier.py
--rw-rw-rw-   0        0        0     7277 2023-05-12 10:13:17.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/desktop_notifier.py
--rw-rw-rw-   0        0        0     8013 2023-05-12 10:13:29.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/discord_notifier.py
--rw-rw-rw-   0        0        0     8080 2023-05-12 10:13:41.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/kakao_notifier.py
--rw-rw-rw-   0        0        0     7652 2023-05-12 10:13:54.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/line_notifier.py
--rw-rw-rw-   0        0        0    10267 2023-05-12 10:16:36.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/mail_notifier.py
--rw-rw-rw-   0        0        0     7606 2023-05-12 10:14:40.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/slack_notifier.py
--rw-rw-rw-   0        0        0     9034 2023-05-12 10:16:08.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/sms_notifier.py
--rw-rw-rw-   0        0        0     7588 2023-05-12 10:16:16.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/teams_notifier.py
--rw-rw-rw-   0        0        0     7815 2023-05-12 10:16:22.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/telegram_notifier.py
--rw-rw-rw-   0        0        0     7607 2023-05-12 10:16:28.000000 exceptnotifier-0.2.5/ExceptNotifier/pycore/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.394182 exceptnotifier-0.2.5/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      265 2023-05-12 10:19:40.000000 exceptnotifier-0.2.5/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.5/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:20:32.279040 exceptnotifier-0.2.5/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    42887 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2307 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 10:20:32.000000 exceptnotifier-0.2.5/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.5/LICENSE
--rw-rw-rw-   0        0        0    42887 2023-05-12 10:20:32.400730 exceptnotifier-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    41839 2023-05-11 20:54:05.000000 exceptnotifier-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 10:20:32.402739 exceptnotifier-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-05-12 10:18:36.000000 exceptnotifier-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.282724 exceptnotifier-0.2.6/
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.150112 exceptnotifier-0.2.6/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4847 2023-05-12 10:35:56.000000 exceptnotifier-0.2.6/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.211428 exceptnotifier-0.2.6/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1382 2023-05-12 10:54:50.000000 exceptnotifier-0.2.6/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-05-12 10:41:13.000000 exceptnotifier-0.2.6/ExceptNotifier/base/bard_receiver.py
+-rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.6/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.6/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.6/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1009 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.6/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.6/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.6/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.6/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.6/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.6/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.6/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.6/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.6/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.6/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.238352 exceptnotifier-0.2.6/ExceptNotifier/ipycore/
+-rw-rw-rw-   0        0        0     1472 2023-05-12 10:36:00.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2578 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2947 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2590 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2570 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2584 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     4013 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2577 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     3049 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2581 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2583 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2591 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/ipycore/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.271804 exceptnotifier-0.2.6/ExceptNotifier/pycore/
+-rw-rw-rw-   0        0        0     2009 2023-05-12 10:54:52.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-05-12 05:17:37.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/beep_notifier.py
+-rw-rw-rw-   0        0        0     7700 2023-05-12 10:13:08.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/chime_notifier.py
+-rw-rw-rw-   0        0        0     7277 2023-05-12 10:13:17.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/desktop_notifier.py
+-rw-rw-rw-   0        0        0     8013 2023-05-12 10:13:29.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/discord_notifier.py
+-rw-rw-rw-   0        0        0     8080 2023-05-12 10:13:41.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/kakao_notifier.py
+-rw-rw-rw-   0        0        0     7652 2023-05-12 10:13:54.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/line_notifier.py
+-rw-rw-rw-   0        0        0    10267 2023-05-12 10:16:36.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/mail_notifier.py
+-rw-rw-rw-   0        0        0     7606 2023-05-12 10:14:40.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/slack_notifier.py
+-rw-rw-rw-   0        0        0     9034 2023-05-12 10:16:08.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/sms_notifier.py
+-rw-rw-rw-   0        0        0     7588 2023-05-12 10:16:16.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/teams_notifier.py
+-rw-rw-rw-   0        0        0     7815 2023-05-12 10:16:22.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/telegram_notifier.py
+-rw-rw-rw-   0        0        0     7607 2023-05-12 10:16:28.000000 exceptnotifier-0.2.6/ExceptNotifier/pycore/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.276465 exceptnotifier-0.2.6/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      265 2023-05-12 10:36:03.000000 exceptnotifier-0.2.6/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.6/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:55:29.171651 exceptnotifier-0.2.6/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    45493 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 10:55:29.000000 exceptnotifier-0.2.6/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0    45493 2023-05-12 10:55:29.281288 exceptnotifier-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    44445 2023-05-12 10:55:07.000000 exceptnotifier-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:55:29.282724 exceptnotifier-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-05-12 10:35:52.000000 exceptnotifier-0.2.6/setup.py
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/__init__.py` & `exceptnotifier-0.2.6/ExceptNotifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,9 +127,9 @@
     "ExceptMailIpython",
     "ExceptSlackIpython",
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
 ]
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     "send_whatsapp_msg",
     "send_sms_msg",
     "beep",
     "receive_openai_advice",
     "get_resp_openai_advice",
 ]
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/bard_receiver.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/bard_receiver.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
     :type _OPEN_AI_API: str
     :param error_message: Error message
     :type error_message: str
     :return: Returns a description and example of the code, the location of the error, and a debugging code example.
     :rtype: str
     """
     os.environ["_BARD_API_KEY"] = _BARD_API_KEY
-    input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix exampel. error== {error_message}"
+    if os.environ["_BARD_ADVICE_LANG"]=='ko':
+        input_text = f"다음 error를 어떻게 고칠 수 있을까? 다음 에러에 대해서 설명해주고, 어떤 위치에서 어떤 코드가 잘못 되었는지 말해줘. 그리고 이 코드를 고칠 수 있는 예시 코드를 보여줘 error=={error_message}"
+    elif os.environ["_BARD_ADVICE_LANG"]=='jp':
+        input_text = f"次のエラーをどのように修正できますか？次のエラーについて説明し、どの場所でどのコードが間違っているかを教えてください。そして、このコードを修正できるサンプルコードを見せてください。 error=={error_message}"
+    else:
+        input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix example. error=={error_message}"
+    
     response = bardapi.core.Bard().get_answer(input_text)
     advice_msg = response["content"]
 
     return advice_msg
 
 
 # if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/discord_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/wechat_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.2.6/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/__init__.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
 ]
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/beep_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/beep_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/chime_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/chime_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/desktop_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/desktop_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/discord_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/discord_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/kakao_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/kakao_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/line_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/line_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/mail_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/mail_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/slack_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/slack_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/sms_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/sms_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/teams_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/teams_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/telegram_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/telegram_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/ipycore/wechat_notifier_ipython.py` & `exceptnotifier-0.2.6/ExceptNotifier/ipycore/wechat_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/__init__.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     "ExceptWechat",
     "SendWechat",
     "SuccessDesktop",
     "ExceptDesktop",
     "SendDesktop",
 ]
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/beep_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/chime_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/chime_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/desktop_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/desktop_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/discord_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/discord_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/kakao_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/kakao_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/line_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/line_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/mail_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/slack_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/sms_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/teams_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/telegram_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/pycore/wechat_notifier.py` & `exceptnotifier-0.2.6/ExceptNotifier/pycore/wechat_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.2.6/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: exceptnotifier
-Version: 0.2.5
-Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
-Home-page: https://github.com/dsdanielpark/ExceptNotifier
-Author: daniel park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
 
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
@@ -107,14 +85,15 @@
   * [Sender in Ipython](#sender-in-ipython)
 <br>
 
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
+    + [c. Notifier with Google Bard API](#b-notifier-with-google-bard-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
   * [*Slack*](#slack)
   * [*Line*](#line)
   * [*SMS*](#sms)
   * [*Teams*](#teams)
@@ -154,18 +133,19 @@
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
-| OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/APIOpenAI/GUIDE.md)|
-| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://bard.google.com/)|
+| OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/OpenAI/GUIDE.md)|
+| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`,'_BARD_ADVICE_LANG'|Free|Easy|1min|[Google Bard](./documents/GoogleBard/GUIDE.md)|
 
 - Starting from v0.2.5, you can receive debugging hints and examples through Google Bard using the same syntax as the OpenAI API. However, due to time constraints, examples will only be added for Telegram and Discord.
+- Starting from v0.2.6, you can receive debugging hints in Korean or Japanese by setting `_BARD_ADVICE_LANG` to 'ko' or 'jp'.
 
 <br>
 
 # Tutorial
 I will update tutorial ASAP. `README.md` is sufficient, but read the application's official documentation if necessary. However, we are preparing a more detailed and friendly tutorial.
 
 1. Main-tutorials: [Notebook](https://github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
@@ -203,33 +183,55 @@
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
 ![](./assets/imgs/ex02_1.png)
 
+#### Using Open AI - Chat GPT 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
 from ExceptNotifier import ExceptTelegram
 sys.excepthook = ExceptTelegram.__call__
 
-os.envirion['_TELEGRAM_TOKEN'] = "xxxx"
-os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo"
-os.envirion['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_TELEGRAM_TOKEN'] = "xxxx"
+os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"
+os.environ['_OPEN_AI_API']="sk-xxxxxx"
 
 try:
     print(1/0)
 except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
     sys.exit()
 ```
 
+#### Using Google - Bard 
+You can receive debugging information from Google Bard via the python package [Bard API](https://github.com/dsdanielpark/BARD_API). you'll need to configure a variable:
+`_BARD_API_KEY`<br>
+(Optional) Google Bard officially supports Korean, so you can set the language of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to korean, debugging hints for code in Korean are provided. Just set a variable `_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
+
+```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
+import sys, os
+sys.excepthook = ExceptTelegram.__call__
+os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+os.environ['_BARD_API_KEY']="xxxxxxxxx"
+# os.environ['_BARD_ADVICE_LANG']="ko"
+
+try:
+    print(1/0)  
+    SuccessTelegram().__call__() #1. success sender          
+except ExceptTelegram as e:      #2. except sender            
+    sys.exit()
+
+SendTelegram().__call__()        #3. customized sender     
+```
 
 ## Success`Notifier`
 ![](./assets/imgs/ex03.png)
 
 - Format: Success`[appName]`
 - Type: Class <br>
 *ExampleClass* <br>
@@ -383,17 +385,23 @@
 
 send_telegram_msg(_TELEGRAM_TOKEN, "This is test message")
 ```
 
 <br>
 
 # Applied in each application
+
+## Open AI - Chat GPT
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
+## Google - Bard
+You can receive debugging information from Google Bard via the python package [Bard API](https://github.com/dsdanielpark/BARD_API) when using the Except statement. The syntax remains the same, but you'll need to configure a variable:
+`_BARD_API_KEY`<br><br>
+(Optional) Google Bard officially supports Korean, so you can set the language of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to korean, debugging hints for code in Korean are provided. Just set a variable `_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
 
 <br>
 
 ## *Telegram*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) 
 As all classes function the same, the example will only use one image, like in Telegram.
 ![](./assets/imgs/fig44.png)
@@ -443,29 +451,51 @@
 - If you just set `_OPEN_AI_API` and `_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL will automatically send debugging information as a message. Currently, it is mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that other models can be used later.
 *Notifier*
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys, os
 sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx"
-os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo"
-os.envirion['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"
+os.environ['_OPEN_AI_API']="sk-xxxxxx"
 
 try:
     print(1/0)  
     SuccessTelegram().__call__() #1. success sender          
 
 except ExceptTelegram as e:      #2. except sender            
     sys.exit()
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
+
+### c. Notifier with Google Bard API
+- Just set `_BARD_API_KEY`. If you would like to receive guidance in Korean, you can optionally set the following. Set `_BARD_ADVICE_LANG` as `ko` or `jp`.
+*Notifier*
+```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
+import sys, os
+sys.excepthook = ExceptTelegram.__call__
+os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+os.environ['_BARD_API_KEY']="xxxxxxxxx"
+# os.environ['_BARD_ADVICE_LANG']="ko"
+
+try:
+    print(1/0)  
+    SuccessTelegram().__call__() #1. success sender          
+except ExceptTelegram as e:      #2. except sender            
+    sys.exit()
+
+SendTelegram().__call__()        #3. customized sender     
+```
+<br>
+
 ## *Mail*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)
 
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en).
```

#### html2text {}

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.5 Summary: With
-Python's try-except to receive notifications about Errors or Successes in your
-code through messenger app or email. Home-page: https://github.com/
-dsdanielpark/ExceptNotifier Author: daniel park Author-email:
-parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
-Alarm,Error notifications,Customizable notifications,Traceback
-management,Single line alarm Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 3 - Alpha
+ Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
 [PyPI package] [PyPI] [Downloads] [commit update] [Code_style:_black] [https://
 img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black] [https:/
         /www.buymeacoffee.com/assets/img/custom_images/orange_img.png]
@@ -71,19 +57,20 @@
 [Sender](#sender)
 - [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
 (#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
 in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
 in Ipython](#sender-in-ipython)
 - [Applied in each application](#applied-in-each-application) * [*Telegram*]
 (#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
-+ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail)
-* [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*]
-(#line) * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) *
-[*Wechat*](#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing
-Guide](#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
++ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) + [c. Notifier
+with Google Bard API](#b-notifier-with-google-bard-api) * [*Mail*](#mail) *
+[*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line)
+* [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*]
+(#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide]
+(#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
 conduct) - [Contacts](#contacts)
 
 
 
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - As you already know, API Keys or security tokens must be
@@ -132,19 +119,21 @@
 colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 If you add the following two variables to the required variables for each
 application in the table above, you can receive error location and explanation,
 as well as examples, from OpenAI's model | API | Required Variables | Free or
 Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:
 --:|:--:|:--:|:---:| | OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
-APIOpenAI/GUIDE.md)| | Google Bard API |`Required variables for each
-application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://
-bard.google.com/)| - Starting from v0.2.5, you can receive debugging hints and
-examples through Google Bard using the same syntax as the OpenAI API. However,
-due to time constraints, examples will only be added for Telegram and Discord.
+OpenAI/GUIDE.md)| | Google Bard API |`Required variables for each application`+
+`_BARD_API_KEY`,'_BARD_ADVICE_LANG'|Free|Easy|1min|[Google Bard](./documents/
+GoogleBard/GUIDE.md)| - Starting from v0.2.5, you can receive debugging hints
+and examples through Google Bard using the same syntax as the OpenAI API.
+However, due to time constraints, examples will only be added for Telegram and
+Discord. - Starting from v0.2.6, you can receive debugging hints in Korean or
+Japanese by setting `_BARD_ADVICE_LANG` to 'ko' or 'jp'.
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
 [folder](https://github.com/DSDanielPark/ExceptNotifier/tree/main/tutorial).
 The tutorial is synchronized with the Python file name provided by
@@ -160,24 +149,36 @@
 
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex02_1.png) You can receive debugging
-information from ChatGPT via OpenAI's API when using the Except statement. The
-syntax remains the same, but you'll need to configure these two variables:
-`_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
-ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
-os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
-ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
-Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
-Type: Class
+Notification ![](./assets/imgs/ex02_1.png) #### Using Open AI - Chat GPT You
+can receive debugging information from ChatGPT via OpenAI's API when using the
+Except statement. The syntax remains the same, but you'll need to configure
+these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import
+sys, os from ExceptNotifier import ExceptTelegram sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.environ['_OPEN_AI_API']="sk-xxxxxx" try:
+print(1/0) except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
+sys.exit() ``` #### Using Google - Bard You can receive debugging information
+from Google Bard via the python package [Bard API](https://github.com/
+dsdanielpark/BARD_API). you'll need to configure a variable: `_BARD_API_KEY`
+(Optional) Google Bard officially supports Korean, so you can set the language
+of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to
+korean, debugging hints for code in Korean are provided. Just set a variable
+`_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'. ```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import
+sys, os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN']
+= "xxxxxxxxx" os.environ['_BARD_API_KEY']="xxxxxxxxx" # os.environ
+['_BARD_ADVICE_LANG']="ko" try: print(1/0) SuccessTelegram().__call__() #1.
+success sender except ExceptTelegram as e: #2. except sender sys.exit()
+SendTelegram().__call__() #3. customized sender ``` ## Success`Notifier` ![](./
+assets/imgs/ex03.png) - Format: Success`[appName]` - Type: Class
 *ExampleClass*
 By placing the try except in python at the end of the try statement,
 applications can be notified that the try statement worked normally. ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail,
 SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope,
 SuccessBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SuccessTelgeram sys.excepthook = ExceptTelegram.__call__ os.environ
@@ -228,18 +229,26 @@
 Ipython ![](./assets/imgs/ex09.png) - Same syntax in Python. See Python Core
 above. ```python import sys import os from ExceptNotifier import SendTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx" SendTelegram().__call__() # Sending
 telegram message ``` ## Sender in Ipython ![](./assets/imgs/ex10.png) - Same
 syntax in Python. See Python Core above. ```python from ExceptNotifier import
 send_telegram_msg _TELEGRAM_TOKEN = "xxxxx" send_telegram_msg(_TELEGRAM_TOKEN,
 "This is test message") ```
-# Applied in each application You can receive debugging information from
-ChatGPT via OpenAI's API when using the Except statement. The syntax remains
-the same, but you'll need to configure these two variables:
-`_OPEN_AI_MODEL`,`_OPEN_AI_API`
+# Applied in each application ## Open AI - Chat GPT You can receive debugging
+information from ChatGPT via OpenAI's API when using the Except statement. The
+syntax remains the same, but you'll need to configure these two variables:
+`_OPEN_AI_MODEL`,`_OPEN_AI_API` ## Google - Bard You can receive debugging
+information from Google Bard via the python package [Bard API](https://
+github.com/dsdanielpark/BARD_API) when using the Except statement. The syntax
+remains the same, but you'll need to configure a variable: `_BARD_API_KEY`
+
+(Optional) Google Bard officially supports Korean, so you can set the language
+of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to
+korean, debugging hints for code in Korean are provided. Just set a variable
+`_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
 ## *Telegram* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) As all classes function the
 same, the example will only use one image, like in Telegram. ![](./assets/imgs/
 fig44.png) - a. Open your telegram app and search for BotFather. (A built-in
 Telegram bot that helps users create custom Telegram bots)
 - b. Type /newbot to create a new bot
@@ -262,19 +271,28 @@
 except sender sys.exit() SendTelegram().__call__() #3. customized sender ```
 ### b. Notifier with OpenAI API - If you just set `_OPEN_AI_API` and
 `_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL
 will automatically send debugging information as a message. Currently, it is
 mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that
 other models can be used later. *Notifier* ```python from ExceptNotifier import
 ExceptTelegram, SuccessTelegram, SendTelegram import sys, os sys.excepthook =
-ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.envirion
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try:
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.environ['_OPEN_AI_API']="sk-xxxxxx" try:
 print(1/0) SuccessTelegram().__call__() #1. success sender except
 ExceptTelegram as e: #2. except sender sys.exit() SendTelegram().__call__() #3.
 customized sender ```
+### c. Notifier with Google Bard API - Just set `_BARD_API_KEY`. If you would
+like to receive guidance in Korean, you can optionally set the following. Set
+`_BARD_ADVICE_LANG` as `ko` or `jp`. *Notifier* ```python from ExceptNotifier
+import ExceptTelegram, SuccessTelegram, SendTelegram import sys, os
+sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
+"xxxxxxxxx" os.environ['_BARD_API_KEY']="xxxxxxxxx" # os.environ
+['_BARD_ADVICE_LANG']="ko" try: print(1/0) SuccessTelegram().__call__() #1.
+success sender except ExceptTelegram as e: #2. except sender sys.exit()
+SendTelegram().__call__() #3. customized sender ```
 ## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
 email is sent along with the error message. Additionally, you can send emails
 from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
```

### Comparing `exceptnotifier-0.2.5/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.2.6/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/LICENSE` & `exceptnotifier-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.5/PKG-INFO` & `exceptnotifier-0.2.6/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.5
+Version: 0.2.6
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -107,14 +107,15 @@
   * [Sender in Ipython](#sender-in-ipython)
 <br>
 
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
+    + [c. Notifier with Google Bard API](#b-notifier-with-google-bard-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
   * [*Slack*](#slack)
   * [*Line*](#line)
   * [*SMS*](#sms)
   * [*Teams*](#teams)
@@ -154,18 +155,19 @@
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
-| OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/APIOpenAI/GUIDE.md)|
-| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://bard.google.com/)|
+| OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/OpenAI/GUIDE.md)|
+| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`,'_BARD_ADVICE_LANG'|Free|Easy|1min|[Google Bard](./documents/GoogleBard/GUIDE.md)|
 
 - Starting from v0.2.5, you can receive debugging hints and examples through Google Bard using the same syntax as the OpenAI API. However, due to time constraints, examples will only be added for Telegram and Discord.
+- Starting from v0.2.6, you can receive debugging hints in Korean or Japanese by setting `_BARD_ADVICE_LANG` to 'ko' or 'jp'.
 
 <br>
 
 # Tutorial
 I will update tutorial ASAP. `README.md` is sufficient, but read the application's official documentation if necessary. However, we are preparing a more detailed and friendly tutorial.
 
 1. Main-tutorials: [Notebook](https://github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
@@ -203,33 +205,55 @@
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
 ![](./assets/imgs/ex02_1.png)
 
+#### Using Open AI - Chat GPT 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
 from ExceptNotifier import ExceptTelegram
 sys.excepthook = ExceptTelegram.__call__
 
-os.envirion['_TELEGRAM_TOKEN'] = "xxxx"
-os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo"
-os.envirion['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_TELEGRAM_TOKEN'] = "xxxx"
+os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"
+os.environ['_OPEN_AI_API']="sk-xxxxxx"
 
 try:
     print(1/0)
 except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
     sys.exit()
 ```
 
+#### Using Google - Bard 
+You can receive debugging information from Google Bard via the python package [Bard API](https://github.com/dsdanielpark/BARD_API). you'll need to configure a variable:
+`_BARD_API_KEY`<br>
+(Optional) Google Bard officially supports Korean, so you can set the language of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to korean, debugging hints for code in Korean are provided. Just set a variable `_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
+
+```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
+import sys, os
+sys.excepthook = ExceptTelegram.__call__
+os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+os.environ['_BARD_API_KEY']="xxxxxxxxx"
+# os.environ['_BARD_ADVICE_LANG']="ko"
+
+try:
+    print(1/0)  
+    SuccessTelegram().__call__() #1. success sender          
+except ExceptTelegram as e:      #2. except sender            
+    sys.exit()
+
+SendTelegram().__call__()        #3. customized sender     
+```
 
 ## Success`Notifier`
 ![](./assets/imgs/ex03.png)
 
 - Format: Success`[appName]`
 - Type: Class <br>
 *ExampleClass* <br>
@@ -383,17 +407,23 @@
 
 send_telegram_msg(_TELEGRAM_TOKEN, "This is test message")
 ```
 
 <br>
 
 # Applied in each application
+
+## Open AI - Chat GPT
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
+## Google - Bard
+You can receive debugging information from Google Bard via the python package [Bard API](https://github.com/dsdanielpark/BARD_API) when using the Except statement. The syntax remains the same, but you'll need to configure a variable:
+`_BARD_API_KEY`<br><br>
+(Optional) Google Bard officially supports Korean, so you can set the language of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to korean, debugging hints for code in Korean are provided. Just set a variable `_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
 
 <br>
 
 ## *Telegram*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) 
 As all classes function the same, the example will only use one image, like in Telegram.
 ![](./assets/imgs/fig44.png)
@@ -443,29 +473,51 @@
 - If you just set `_OPEN_AI_API` and `_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL will automatically send debugging information as a message. Currently, it is mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that other models can be used later.
 *Notifier*
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys, os
 sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx"
-os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo"
-os.envirion['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"
+os.environ['_OPEN_AI_API']="sk-xxxxxx"
 
 try:
     print(1/0)  
     SuccessTelegram().__call__() #1. success sender          
 
 except ExceptTelegram as e:      #2. except sender            
     sys.exit()
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
+
+### c. Notifier with Google Bard API
+- Just set `_BARD_API_KEY`. If you would like to receive guidance in Korean, you can optionally set the following. Set `_BARD_ADVICE_LANG` as `ko` or `jp`.
+*Notifier*
+```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
+import sys, os
+sys.excepthook = ExceptTelegram.__call__
+os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+os.environ['_BARD_API_KEY']="xxxxxxxxx"
+# os.environ['_BARD_ADVICE_LANG']="ko"
+
+try:
+    print(1/0)  
+    SuccessTelegram().__call__() #1. success sender          
+except ExceptTelegram as e:      #2. except sender            
+    sys.exit()
+
+SendTelegram().__call__()        #3. customized sender     
+```
+<br>
+
 ## *Mail*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)
 
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.5 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.6 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -71,19 +71,20 @@
 [Sender](#sender)
 - [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
 (#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
 in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
 in Ipython](#sender-in-ipython)
 - [Applied in each application](#applied-in-each-application) * [*Telegram*]
 (#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
-+ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail)
-* [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*]
-(#line) * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) *
-[*Wechat*](#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing
-Guide](#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
++ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) + [c. Notifier
+with Google Bard API](#b-notifier-with-google-bard-api) * [*Mail*](#mail) *
+[*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line)
+* [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*]
+(#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide]
+(#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
 conduct) - [Contacts](#contacts)
 
 
 
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - As you already know, API Keys or security tokens must be
@@ -132,19 +133,21 @@
 colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 If you add the following two variables to the required variables for each
 application in the table above, you can receive error location and explanation,
 as well as examples, from OpenAI's model | API | Required Variables | Free or
 Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:
 --:|:--:|:--:|:---:| | OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
-APIOpenAI/GUIDE.md)| | Google Bard API |`Required variables for each
-application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://
-bard.google.com/)| - Starting from v0.2.5, you can receive debugging hints and
-examples through Google Bard using the same syntax as the OpenAI API. However,
-due to time constraints, examples will only be added for Telegram and Discord.
+OpenAI/GUIDE.md)| | Google Bard API |`Required variables for each application`+
+`_BARD_API_KEY`,'_BARD_ADVICE_LANG'|Free|Easy|1min|[Google Bard](./documents/
+GoogleBard/GUIDE.md)| - Starting from v0.2.5, you can receive debugging hints
+and examples through Google Bard using the same syntax as the OpenAI API.
+However, due to time constraints, examples will only be added for Telegram and
+Discord. - Starting from v0.2.6, you can receive debugging hints in Korean or
+Japanese by setting `_BARD_ADVICE_LANG` to 'ko' or 'jp'.
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
 [folder](https://github.com/DSDanielPark/ExceptNotifier/tree/main/tutorial).
 The tutorial is synchronized with the Python file name provided by
@@ -160,24 +163,36 @@
 
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex02_1.png) You can receive debugging
-information from ChatGPT via OpenAI's API when using the Except statement. The
-syntax remains the same, but you'll need to configure these two variables:
-`_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
-ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
-os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
-ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
-Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
-Type: Class
+Notification ![](./assets/imgs/ex02_1.png) #### Using Open AI - Chat GPT You
+can receive debugging information from ChatGPT via OpenAI's API when using the
+Except statement. The syntax remains the same, but you'll need to configure
+these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import
+sys, os from ExceptNotifier import ExceptTelegram sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.environ['_OPEN_AI_API']="sk-xxxxxx" try:
+print(1/0) except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
+sys.exit() ``` #### Using Google - Bard You can receive debugging information
+from Google Bard via the python package [Bard API](https://github.com/
+dsdanielpark/BARD_API). you'll need to configure a variable: `_BARD_API_KEY`
+(Optional) Google Bard officially supports Korean, so you can set the language
+of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to
+korean, debugging hints for code in Korean are provided. Just set a variable
+`_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'. ```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import
+sys, os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN']
+= "xxxxxxxxx" os.environ['_BARD_API_KEY']="xxxxxxxxx" # os.environ
+['_BARD_ADVICE_LANG']="ko" try: print(1/0) SuccessTelegram().__call__() #1.
+success sender except ExceptTelegram as e: #2. except sender sys.exit()
+SendTelegram().__call__() #3. customized sender ``` ## Success`Notifier` ![](./
+assets/imgs/ex03.png) - Format: Success`[appName]` - Type: Class
 *ExampleClass*
 By placing the try except in python at the end of the try statement,
 applications can be notified that the try statement worked normally. ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail,
 SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope,
 SuccessBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SuccessTelgeram sys.excepthook = ExceptTelegram.__call__ os.environ
@@ -228,18 +243,26 @@
 Ipython ![](./assets/imgs/ex09.png) - Same syntax in Python. See Python Core
 above. ```python import sys import os from ExceptNotifier import SendTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx" SendTelegram().__call__() # Sending
 telegram message ``` ## Sender in Ipython ![](./assets/imgs/ex10.png) - Same
 syntax in Python. See Python Core above. ```python from ExceptNotifier import
 send_telegram_msg _TELEGRAM_TOKEN = "xxxxx" send_telegram_msg(_TELEGRAM_TOKEN,
 "This is test message") ```
-# Applied in each application You can receive debugging information from
-ChatGPT via OpenAI's API when using the Except statement. The syntax remains
-the same, but you'll need to configure these two variables:
-`_OPEN_AI_MODEL`,`_OPEN_AI_API`
+# Applied in each application ## Open AI - Chat GPT You can receive debugging
+information from ChatGPT via OpenAI's API when using the Except statement. The
+syntax remains the same, but you'll need to configure these two variables:
+`_OPEN_AI_MODEL`,`_OPEN_AI_API` ## Google - Bard You can receive debugging
+information from Google Bard via the python package [Bard API](https://
+github.com/dsdanielpark/BARD_API) when using the Except statement. The syntax
+remains the same, but you'll need to configure a variable: `_BARD_API_KEY`
+
+(Optional) Google Bard officially supports Korean, so you can set the language
+of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to
+korean, debugging hints for code in Korean are provided. Just set a variable
+`_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
 ## *Telegram* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) As all classes function the
 same, the example will only use one image, like in Telegram. ![](./assets/imgs/
 fig44.png) - a. Open your telegram app and search for BotFather. (A built-in
 Telegram bot that helps users create custom Telegram bots)
 - b. Type /newbot to create a new bot
@@ -262,19 +285,28 @@
 except sender sys.exit() SendTelegram().__call__() #3. customized sender ```
 ### b. Notifier with OpenAI API - If you just set `_OPEN_AI_API` and
 `_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL
 will automatically send debugging information as a message. Currently, it is
 mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that
 other models can be used later. *Notifier* ```python from ExceptNotifier import
 ExceptTelegram, SuccessTelegram, SendTelegram import sys, os sys.excepthook =
-ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.envirion
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try:
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.environ['_OPEN_AI_API']="sk-xxxxxx" try:
 print(1/0) SuccessTelegram().__call__() #1. success sender except
 ExceptTelegram as e: #2. except sender sys.exit() SendTelegram().__call__() #3.
 customized sender ```
+### c. Notifier with Google Bard API - Just set `_BARD_API_KEY`. If you would
+like to receive guidance in Korean, you can optionally set the following. Set
+`_BARD_ADVICE_LANG` as `ko` or `jp`. *Notifier* ```python from ExceptNotifier
+import ExceptTelegram, SuccessTelegram, SendTelegram import sys, os
+sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
+"xxxxxxxxx" os.environ['_BARD_API_KEY']="xxxxxxxxx" # os.environ
+['_BARD_ADVICE_LANG']="ko" try: print(1/0) SuccessTelegram().__call__() #1.
+success sender except ExceptTelegram as e: #2. except sender sys.exit()
+SendTelegram().__call__() #3. customized sender ```
 ## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
 email is sent along with the error message. Additionally, you can send emails
 from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
```

### Comparing `exceptnotifier-0.2.5/README.md` & `exceptnotifier-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: exceptnotifier
+Version: 0.2.6
+Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
+Home-page: https://github.com/dsdanielpark/ExceptNotifier
+Author: daniel park
+Author-email: parkminwoo1991@gmail.com
+Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
 
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
@@ -85,14 +107,15 @@
   * [Sender in Ipython](#sender-in-ipython)
 <br>
 
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
+    + [c. Notifier with Google Bard API](#b-notifier-with-google-bard-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
   * [*Slack*](#slack)
   * [*Line*](#line)
   * [*SMS*](#sms)
   * [*Teams*](#teams)
@@ -132,18 +155,19 @@
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
-| OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/APIOpenAI/GUIDE.md)|
-| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://bard.google.com/)|
+| OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/OpenAI/GUIDE.md)|
+| Google Bard API |`Required variables for each application`+ `_BARD_API_KEY`,'_BARD_ADVICE_LANG'|Free|Easy|1min|[Google Bard](./documents/GoogleBard/GUIDE.md)|
 
 - Starting from v0.2.5, you can receive debugging hints and examples through Google Bard using the same syntax as the OpenAI API. However, due to time constraints, examples will only be added for Telegram and Discord.
+- Starting from v0.2.6, you can receive debugging hints in Korean or Japanese by setting `_BARD_ADVICE_LANG` to 'ko' or 'jp'.
 
 <br>
 
 # Tutorial
 I will update tutorial ASAP. `README.md` is sufficient, but read the application's official documentation if necessary. However, we are preparing a more detailed and friendly tutorial.
 
 1. Main-tutorials: [Notebook](https://github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
@@ -181,33 +205,55 @@
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
 ![](./assets/imgs/ex02_1.png)
 
+#### Using Open AI - Chat GPT 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
 from ExceptNotifier import ExceptTelegram
 sys.excepthook = ExceptTelegram.__call__
 
-os.envirion['_TELEGRAM_TOKEN'] = "xxxx"
-os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo"
-os.envirion['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_TELEGRAM_TOKEN'] = "xxxx"
+os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"
+os.environ['_OPEN_AI_API']="sk-xxxxxx"
 
 try:
     print(1/0)
 except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
     sys.exit()
 ```
 
+#### Using Google - Bard 
+You can receive debugging information from Google Bard via the python package [Bard API](https://github.com/dsdanielpark/BARD_API). you'll need to configure a variable:
+`_BARD_API_KEY`<br>
+(Optional) Google Bard officially supports Korean, so you can set the language of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to korean, debugging hints for code in Korean are provided. Just set a variable `_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
+
+```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
+import sys, os
+sys.excepthook = ExceptTelegram.__call__
+os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+os.environ['_BARD_API_KEY']="xxxxxxxxx"
+# os.environ['_BARD_ADVICE_LANG']="ko"
+
+try:
+    print(1/0)  
+    SuccessTelegram().__call__() #1. success sender          
+except ExceptTelegram as e:      #2. except sender            
+    sys.exit()
+
+SendTelegram().__call__()        #3. customized sender     
+```
 
 ## Success`Notifier`
 ![](./assets/imgs/ex03.png)
 
 - Format: Success`[appName]`
 - Type: Class <br>
 *ExampleClass* <br>
@@ -361,17 +407,23 @@
 
 send_telegram_msg(_TELEGRAM_TOKEN, "This is test message")
 ```
 
 <br>
 
 # Applied in each application
+
+## Open AI - Chat GPT
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
+## Google - Bard
+You can receive debugging information from Google Bard via the python package [Bard API](https://github.com/dsdanielpark/BARD_API) when using the Except statement. The syntax remains the same, but you'll need to configure a variable:
+`_BARD_API_KEY`<br><br>
+(Optional) Google Bard officially supports Korean, so you can set the language of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to korean, debugging hints for code in Korean are provided. Just set a variable `_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
 
 <br>
 
 ## *Telegram*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) 
 As all classes function the same, the example will only use one image, like in Telegram.
 ![](./assets/imgs/fig44.png)
@@ -421,29 +473,51 @@
 - If you just set `_OPEN_AI_API` and `_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL will automatically send debugging information as a message. Currently, it is mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that other models can be used later.
 *Notifier*
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys, os
 sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx"
-os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo"
-os.envirion['_OPEN_AI_API']="sk-xxxxxx"
+os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo"
+os.environ['_OPEN_AI_API']="sk-xxxxxx"
 
 try:
     print(1/0)  
     SuccessTelegram().__call__() #1. success sender          
 
 except ExceptTelegram as e:      #2. except sender            
     sys.exit()
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
+
+### c. Notifier with Google Bard API
+- Just set `_BARD_API_KEY`. If you would like to receive guidance in Korean, you can optionally set the following. Set `_BARD_ADVICE_LANG` as `ko` or `jp`.
+*Notifier*
+```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
+import sys, os
+sys.excepthook = ExceptTelegram.__call__
+os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+os.environ['_BARD_API_KEY']="xxxxxxxxx"
+# os.environ['_BARD_ADVICE_LANG']="ko"
+
+try:
+    print(1/0)  
+    SuccessTelegram().__call__() #1. success sender          
+except ExceptTelegram as e:      #2. except sender            
+    sys.exit()
+
+SendTelegram().__call__()        #3. customized sender     
+```
+<br>
+
 ## *Mail*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)
 
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en).
```

#### html2text {}

```diff
@@ -1,8 +1,22 @@
- Development Status :: 3 - Alpha
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.6 Summary: With
+Python's try-except to receive notifications about Errors or Successes in your
+code through messenger app or email. Home-page: https://github.com/
+dsdanielpark/ExceptNotifier Author: daniel park Author-email:
+parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
+Alarm,Error notifications,Customizable notifications,Traceback
+management,Single line alarm Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research Classifier: Natural Language
+:: English Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
 [PyPI package] [PyPI] [Downloads] [commit update] [Code_style:_black] [https://
 img.shields.io/github/license/dsdanielpark/ExceptNotifier?color=black] [https:/
         /www.buymeacoffee.com/assets/img/custom_images/orange_img.png]
@@ -57,19 +71,20 @@
 [Sender](#sender)
 - [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
 (#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
 in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
 in Ipython](#sender-in-ipython)
 - [Applied in each application](#applied-in-each-application) * [*Telegram*]
 (#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
-+ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail)
-* [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*]
-(#line) * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) *
-[*Wechat*](#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing
-Guide](#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
++ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) + [c. Notifier
+with Google Bard API](#b-notifier-with-google-bard-api) * [*Mail*](#mail) *
+[*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line)
+* [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*]
+(#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide]
+(#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
 conduct) - [Contacts](#contacts)
 
 
 
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - As you already know, API Keys or security tokens must be
@@ -118,19 +133,21 @@
 colab.research.google.com/drive/1E5Q-lnWStG1MqtnGCr5pzInlfWt2uc2S?usp=sharing)|
 If you add the following two variables to the required variables for each
 application in the table above, you can receive error location and explanation,
 as well as examples, from OpenAI's model | API | Required Variables | Free or
 Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:
 --:|:--:|:--:|:---:| | OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
-APIOpenAI/GUIDE.md)| | Google Bard API |`Required variables for each
-application`+ `_BARD_API_KEY`|Free|Easy|1min|[Google Bard](https://
-bard.google.com/)| - Starting from v0.2.5, you can receive debugging hints and
-examples through Google Bard using the same syntax as the OpenAI API. However,
-due to time constraints, examples will only be added for Telegram and Discord.
+OpenAI/GUIDE.md)| | Google Bard API |`Required variables for each application`+
+`_BARD_API_KEY`,'_BARD_ADVICE_LANG'|Free|Easy|1min|[Google Bard](./documents/
+GoogleBard/GUIDE.md)| - Starting from v0.2.5, you can receive debugging hints
+and examples through Google Bard using the same syntax as the OpenAI API.
+However, due to time constraints, examples will only be added for Telegram and
+Discord. - Starting from v0.2.6, you can receive debugging hints in Korean or
+Japanese by setting `_BARD_ADVICE_LANG` to 'ko' or 'jp'.
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
 [folder](https://github.com/DSDanielPark/ExceptNotifier/tree/main/tutorial).
 The tutorial is synchronized with the Python file name provided by
@@ -146,24 +163,36 @@
 
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex02_1.png) You can receive debugging
-information from ChatGPT via OpenAI's API when using the Except statement. The
-syntax remains the same, but you'll need to configure these two variables:
-`_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
-ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
-os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
-ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
-Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
-Type: Class
+Notification ![](./assets/imgs/ex02_1.png) #### Using Open AI - Chat GPT You
+can receive debugging information from ChatGPT via OpenAI's API when using the
+Except statement. The syntax remains the same, but you'll need to configure
+these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import
+sys, os from ExceptNotifier import ExceptTelegram sys.excepthook =
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.environ['_OPEN_AI_API']="sk-xxxxxx" try:
+print(1/0) except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
+sys.exit() ``` #### Using Google - Bard You can receive debugging information
+from Google Bard via the python package [Bard API](https://github.com/
+dsdanielpark/BARD_API). you'll need to configure a variable: `_BARD_API_KEY`
+(Optional) Google Bard officially supports Korean, so you can set the language
+of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to
+korean, debugging hints for code in Korean are provided. Just set a variable
+`_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'. ```python
+from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import
+sys, os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN']
+= "xxxxxxxxx" os.environ['_BARD_API_KEY']="xxxxxxxxx" # os.environ
+['_BARD_ADVICE_LANG']="ko" try: print(1/0) SuccessTelegram().__call__() #1.
+success sender except ExceptTelegram as e: #2. except sender sys.exit()
+SendTelegram().__call__() #3. customized sender ``` ## Success`Notifier` ![](./
+assets/imgs/ex03.png) - Format: Success`[appName]` - Type: Class
 *ExampleClass*
 By placing the try except in python at the end of the try statement,
 applications can be notified that the try statement worked normally. ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail,
 SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope,
 SuccessBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SuccessTelgeram sys.excepthook = ExceptTelegram.__call__ os.environ
@@ -214,18 +243,26 @@
 Ipython ![](./assets/imgs/ex09.png) - Same syntax in Python. See Python Core
 above. ```python import sys import os from ExceptNotifier import SendTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx" SendTelegram().__call__() # Sending
 telegram message ``` ## Sender in Ipython ![](./assets/imgs/ex10.png) - Same
 syntax in Python. See Python Core above. ```python from ExceptNotifier import
 send_telegram_msg _TELEGRAM_TOKEN = "xxxxx" send_telegram_msg(_TELEGRAM_TOKEN,
 "This is test message") ```
-# Applied in each application You can receive debugging information from
-ChatGPT via OpenAI's API when using the Except statement. The syntax remains
-the same, but you'll need to configure these two variables:
-`_OPEN_AI_MODEL`,`_OPEN_AI_API`
+# Applied in each application ## Open AI - Chat GPT You can receive debugging
+information from ChatGPT via OpenAI's API when using the Except statement. The
+syntax remains the same, but you'll need to configure these two variables:
+`_OPEN_AI_MODEL`,`_OPEN_AI_API` ## Google - Bard You can receive debugging
+information from Google Bard via the python package [Bard API](https://
+github.com/dsdanielpark/BARD_API) when using the Except statement. The syntax
+remains the same, but you'll need to configure a variable: `_BARD_API_KEY`
+
+(Optional) Google Bard officially supports Korean, so you can set the language
+of Bard Advice to Korean. Additionally, if `_BARD_ADVICE_LANG` is set to
+korean, debugging hints for code in Korean are provided. Just set a variable
+`_BARD_ADVICE_LANG` as 'ko'. Japanese is also supported. Set as 'jp'.
 ## *Telegram* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) As all classes function the
 same, the example will only use one image, like in Telegram. ![](./assets/imgs/
 fig44.png) - a. Open your telegram app and search for BotFather. (A built-in
 Telegram bot that helps users create custom Telegram bots)
 - b. Type /newbot to create a new bot
@@ -248,19 +285,28 @@
 except sender sys.exit() SendTelegram().__call__() #3. customized sender ```
 ### b. Notifier with OpenAI API - If you just set `_OPEN_AI_API` and
 `_OPEN_AI_MODEL` environment variables in all application use case, AI MODEL
 will automatically send debugging information as a message. Currently, it is
 mainly based on the `GPT-3.5-TURBO` model, but we plan to update it so that
 other models can be used later. *Notifier* ```python from ExceptNotifier import
 ExceptTelegram, SuccessTelegram, SendTelegram import sys, os sys.excepthook =
-ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.envirion
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try:
+ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] = "xxxx" os.environ
+['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.environ['_OPEN_AI_API']="sk-xxxxxx" try:
 print(1/0) SuccessTelegram().__call__() #1. success sender except
 ExceptTelegram as e: #2. except sender sys.exit() SendTelegram().__call__() #3.
 customized sender ```
+### c. Notifier with Google Bard API - Just set `_BARD_API_KEY`. If you would
+like to receive guidance in Korean, you can optionally set the following. Set
+`_BARD_ADVICE_LANG` as `ko` or `jp`. *Notifier* ```python from ExceptNotifier
+import ExceptTelegram, SuccessTelegram, SendTelegram import sys, os
+sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
+"xxxxxxxxx" os.environ['_BARD_API_KEY']="xxxxxxxxx" # os.environ
+['_BARD_ADVICE_LANG']="ko" try: print(1/0) SuccessTelegram().__call__() #1.
+success sender except ExceptTelegram as e: #2. except sender sys.exit()
+SendTelegram().__call__() #3. customized sender ```
 ## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
 email is sent along with the error message. Additionally, you can send emails
 from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
```

### Comparing `exceptnotifier-0.2.5/setup.py` & `exceptnotifier-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.2.5",
+    version="0.2.6",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```


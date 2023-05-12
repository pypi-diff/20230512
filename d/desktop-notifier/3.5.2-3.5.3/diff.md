# Comparing `tmp/desktop-notifier-3.5.2.tar.gz` & `tmp/desktop-notifier-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.5.2.tar", last modified: Wed May  3 22:25:39 2023, max compression
+gzip compressed data, was "desktop-notifier-3.5.3.tar", last modified: Fri May 12 08:35:11 2023, max compression
```

## Comparing `desktop-notifier-3.5.2.tar` & `desktop-notifier-3.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.005712 desktop-notifier-3.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-03 22:25:25.000000 desktop-notifier-3.5.2/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:25:39.009713 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 22:25:39.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 22:25:38.000000 desktop-notifier-3.5.2/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-12 08:34:55.000000 desktop-notifier-3.5.3/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:11.687101 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 08:35:11.000000 desktop-notifier-3.5.3/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.5.2/LICENSE` & `desktop-notifier-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/PKG-INFO` & `desktop-notifier-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.2
+Version: 3.5.3
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.2/README.md` & `desktop-notifier-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/pyproject.toml` & `desktop-notifier-3.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
```

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/base.py` & `desktop-notifier-3.5.3/src/desktop_notifier/base.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/dbus.py` & `desktop-notifier-3.5.3/src/desktop_notifier/dbus.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/dummy.py` & `desktop-notifier-3.5.3/src/desktop_notifier/dummy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/macos.py` & `desktop-notifier-3.5.3/src/desktop_notifier/macos.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 UNUserNotificationCenter backend for macOS.
 
 * Introduced in macOS 10.14.
 * Cross-platform with iOS and iPadOS.
 * Only available from signed app bundles if called from the main executable or from a
   signed Python framework (for example from python.org).
 * Requires a running CFRunLoop to invoke callbacks.
-
 """
 
-from __future__ import annotations
-
 # system imports
 import uuid
 import logging
 import enum
 import asyncio
 from concurrent.futures import Future
 from urllib.parse import urlparse, unquote
-from typing import cast
+from typing import cast, Optional
 
 # external imports
 from packaging.version import Version
 from rubicon.objc import NSObject, ObjCClass, objc_method, py_from_ns
 from rubicon.objc.runtime import load_library, objc_id, objc_block
 
 # local imports
@@ -155,15 +152,15 @@
         Urgency.Normal: UNNotificationInterruptionLevel.Active,
         Urgency.Critical: UNNotificationInterruptionLevel.TimeSensitive,
     }
 
     def __init__(
         self,
         app_name: str = "Python",
-        notification_limit: int | None = None,
+        notification_limit: Optional[int] = None,
     ) -> None:
         super().__init__(app_name, notification_limit)
         self.nc = UNUserNotificationCenter.currentNotificationCenter()
         self.nc_delegate = NotificationCenterDelegate.alloc().init()
         self.nc_delegate.interface = self
         self.nc.delegate = self.nc_delegate
 
@@ -225,29 +222,29 @@
         settings.release()  # type:ignore
 
         return authorized
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Notification | None,
+        notification_to_replace: Optional[Notification],
     ) -> str:
         """
         Uses UNUserNotificationCenter to schedule a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
 
         if notification_to_replace:
             platform_nid = str(notification_to_replace.identifier)
         else:
             platform_nid = str(uuid.uuid4())
 
-        # On macOS, we need need to register a new notification category for every
+        # On macOS, we need to register a new notification category for every
         # unique set of buttons.
         category_id = await self._create_category_for_notification(notification)
 
         # Create the native notification and notification request.
         content = UNMutableNotificationContent.alloc().init()
         content.title = notification.title
         content.body = notification.message
@@ -310,15 +307,15 @@
             else:
                 raise RuntimeError(error.localizedDescription)  # type:ignore
 
         return platform_nid
 
     async def _create_category_for_notification(
         self, notification: Notification
-    ) -> str | None:
+    ) -> Optional[str]:
         """
         Registers a new notification category with UNNotificationCenter for the given
         notification or retrieves an existing one if it exists for our set of buttons.
 
         :param notification: Notification instance.
         :returns: The identifier of the existing or created notification category.
         """
```

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/macos_legacy.py` & `desktop-notifier-3.5.3/src/desktop_notifier/macos_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 * Should be used for macOS 10.13 and earlier.
 * Deprecated but still available in macOS 11.0.
 * Requires a running CFRunLoop to invoke callbacks.
 
 """
 
-from __future__ import annotations
-
 # system imports
 import uuid
 import platform
 import logging
-from typing import cast
+from typing import cast, Optional
 
 # external imports
 from rubicon.objc import NSObject, ObjCClass, objc_method, py_from_ns
 from rubicon.objc.runtime import load_library
 
 # local imports
 from .base import Notification, DesktopNotifierBase
@@ -85,15 +83,15 @@
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center.
     """
 
     def __init__(
         self,
         app_name: str = "Python",
-        notification_limit: int | None = None,
+        notification_limit: Optional[int] = None,
     ) -> None:
         super().__init__(app_name, notification_limit)
 
         self.nc = NSUserNotificationCenter.defaultUserNotificationCenter
         self.nc_delegate = NotificationCenterDelegate.alloc().init()
         self.nc_delegate.interface = self
         self.nc.delegate = self.nc_delegate
@@ -111,15 +109,15 @@
         Whether we have authorisation to send notifications.
         """
         return True
 
     async def _send(
         self,
         notification: Notification,
-        notification_to_replace: Notification | None,
+        notification_to_replace: Optional[Notification],
     ) -> str:
         """
         Uses NSUserNotificationCenter to schedule a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
```

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/macos_support.py` & `desktop-notifier-3.5.3/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/main.py` & `desktop-notifier-3.5.3/src/desktop_notifier/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,36 @@
             self._did_request_authorisation = True
             return await self._impl.request_authorisation()
 
     async def has_authorisation(self) -> bool:
         """Returns whether we have authorisation to send notifications."""
         return await self._impl.has_authorisation()
 
+    async def send_notification(self, notification: Notification) -> Notification:
+        """
+        Sends a desktop notification.
+
+        This method takes a fully constructed :class:`Notification` instance as input.
+        Use :meth:`send` to provide separate notification properties such as ``title``,
+        ``message``, etc., instead.
+
+        :param notification: The notification to send.
+        """
+        with self._lock:
+            # Ask for authorisation if not already done. On some platforms, this will
+            # trigger a system dialog to ask the user for permission.
+            if not self._did_request_authorisation:
+                await self.request_authorisation()
+
+            # We attempt to send the notification regardless of authorization.
+            # The user may have changed settings in the meantime.
+            await self._impl.send(notification)
+
+            return notification
+
     async def send(
         self,
         title: str,
         message: str,
         urgency: Urgency = Urgency.Normal,
         icon: Path | str | None = None,
         buttons: Sequence[Button] = (),
@@ -288,25 +310,15 @@
             on_dismissed,
             attachment,
             sound,
             thread,
             timeout,
         )
 
-        with self._lock:
-            # Ask for authorisation if not already done. On some platforms, this will
-            # trigger a system dialog to ask the user for permission.
-            if not self._did_request_authorisation:
-                await self.request_authorisation()
-
-            # We attempt to send the notification regardless of authorization.
-            # The user may have changed settings in the meantime.
-            await self._impl.send(notification)
-
-            return notification
+        return await self.send_notification(notification)
 
     def send_sync(
         self,
         title: str,
         message: str,
         urgency: Urgency = Urgency.Normal,
         icon: Path | str | None = None,
```

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/resources/python.png` & `desktop-notifier-3.5.3/src/desktop_notifier/resources/python.png`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier/winrt.py` & `desktop-notifier-3.5.3/src/desktop_notifier/winrt.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier.egg-info/PKG-INFO` & `desktop-notifier-3.5.3/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.2
+Version: 3.5.3
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.2/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop-notifier-3.5.3/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*


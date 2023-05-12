# Comparing `tmp/sonofflan-0.3.1.tar.gz` & `tmp/sonofflan-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonofflan-0.3.1.tar", max compression
+gzip compressed data, was "sonofflan-0.3.2.tar", max compression
```

## Comparing `sonofflan-0.3.1.tar` & `sonofflan-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1458 2022-11-21 17:52:10.623161 sonofflan-0.3.1/LICENSE
--rw-r--r--   0        0        0      488 2023-03-03 17:40:42.230068 sonofflan-0.3.1/README.md
--rw-r--r--   0        0        0      902 2023-03-03 17:40:42.373402 sonofflan-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-28 12:04:41.616281 sonofflan-0.3.1/sonofflan/__init__.py
--rw-r--r--   0        0        0     6582 2023-02-27 10:28:28.454057 sonofflan-0.3.1/sonofflan/__main__.py
--rw-r--r--   0        0        0     5521 2023-02-01 18:08:26.738912 sonofflan-0.3.1/sonofflan/browser.py
--rw-r--r--   0        0        0     3643 2022-11-29 20:41:55.723131 sonofflan-0.3.1/sonofflan/config.py
--rw-r--r--   0        0        0     1718 2022-11-29 20:43:10.176848 sonofflan-0.3.1/sonofflan/crypto.py
--rw-r--r--   0        0        0     1075 2023-02-01 17:49:54.112559 sonofflan-0.3.1/sonofflan/devices/__init__.py
--rw-r--r--   0        0        0     6046 2023-03-03 17:28:39.151166 sonofflan-0.3.1/sonofflan/devices/device.py
--rw-r--r--   0        0        0     2957 2023-02-27 10:28:21.314009 sonofflan-0.3.1/sonofflan/devices/plug.py
--rw-r--r--   0        0        0     1939 2023-02-01 18:03:45.853996 sonofflan-0.3.1/sonofflan/devices/powerplug.py
--rw-r--r--   0        0        0     3216 2022-11-28 17:19:41.600376 sonofflan-0.3.1/sonofflan/devices/strip.py
--rw-r--r--   0        0        0     1719 2022-12-01 17:11:19.286906 sonofflan-0.3.1/sonofflan/devices/thermoplug.py
--rw-r--r--   0        0        0     1317 2023-02-01 17:40:10.765696 sonofflan-0.3.1/sonofflan/errors.py
--rw-r--r--   0        0        0      288 2022-11-24 18:38:28.778014 sonofflan-0.3.1/sonofflan/utils.py
--rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 sonofflan-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1458 2022-11-21 17:52:10.623161 sonofflan-0.3.2/LICENSE
+-rw-r--r--   0        0        0      488 2023-05-12 15:14:40.556172 sonofflan-0.3.2/README.md
+-rw-r--r--   0        0        0      902 2023-05-12 15:14:14.942222 sonofflan-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-28 12:04:41.616281 sonofflan-0.3.2/sonofflan/__init__.py
+-rw-r--r--   0        0        0     6582 2023-02-27 10:28:28.454057 sonofflan-0.3.2/sonofflan/__main__.py
+-rw-r--r--   0        0        0     5557 2023-05-12 15:10:55.961242 sonofflan-0.3.2/sonofflan/browser.py
+-rw-r--r--   0        0        0     3643 2022-11-29 20:41:55.723131 sonofflan-0.3.2/sonofflan/config.py
+-rw-r--r--   0        0        0     1718 2022-11-29 20:43:10.176848 sonofflan-0.3.2/sonofflan/crypto.py
+-rw-r--r--   0        0        0     1075 2023-02-01 17:49:54.112559 sonofflan-0.3.2/sonofflan/devices/__init__.py
+-rw-r--r--   0        0        0     6046 2023-03-03 17:28:39.151166 sonofflan-0.3.2/sonofflan/devices/device.py
+-rw-r--r--   0        0        0     2957 2023-02-27 10:28:21.314009 sonofflan-0.3.2/sonofflan/devices/plug.py
+-rw-r--r--   0        0        0     1939 2023-02-01 18:03:45.853996 sonofflan-0.3.2/sonofflan/devices/powerplug.py
+-rw-r--r--   0        0        0     3216 2022-11-28 17:19:41.600376 sonofflan-0.3.2/sonofflan/devices/strip.py
+-rw-r--r--   0        0        0     1719 2022-12-01 17:11:19.286906 sonofflan-0.3.2/sonofflan/devices/thermoplug.py
+-rw-r--r--   0        0        0     1317 2023-02-01 17:40:10.765696 sonofflan-0.3.2/sonofflan/errors.py
+-rw-r--r--   0        0        0      288 2022-11-24 18:38:28.778014 sonofflan-0.3.2/sonofflan/utils.py
+-rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 sonofflan-0.3.2/PKG-INFO
```

### Comparing `sonofflan-0.3.1/LICENSE` & `sonofflan-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/pyproject.toml` & `sonofflan-0.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sonofflan"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library to interact with Sonoff devices through LAN mode (without eWeLink cloud)"
 authors = ["Danilo Treffiletti <urban82@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 keywords = ["sonoff", "ewelink", "itead"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `sonofflan-0.3.1/sonofflan/__main__.py` & `sonofflan-0.3.2/sonofflan/__main__.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/browser.py` & `sonofflan-0.3.2/sonofflan/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self._browser = AsyncServiceBrowser(self._zeroconf.zeroconf, SERVICE_TYPE, handlers=[self._update])
 
     async def shutdown(self) -> None:
         """Shutdown the browser"""
 
         self._logger.debug("Stopping...")
         await self._browser.async_cancel()
+        await self._queue.put(None)
         self._logger.debug("Stopped")
 
     async def wait_event(self) -> Event:
         """Get one event from the queue"""
         return await self._queue.get()
 
     def event_processed(self) -> None:
```

### Comparing `sonofflan-0.3.1/sonofflan/config.py` & `sonofflan-0.3.2/sonofflan/config.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/crypto.py` & `sonofflan-0.3.2/sonofflan/crypto.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/devices/__init__.py` & `sonofflan-0.3.2/sonofflan/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/devices/device.py` & `sonofflan-0.3.2/sonofflan/devices/device.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/devices/plug.py` & `sonofflan-0.3.2/sonofflan/devices/plug.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/devices/powerplug.py` & `sonofflan-0.3.2/sonofflan/devices/powerplug.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/devices/strip.py` & `sonofflan-0.3.2/sonofflan/devices/strip.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/devices/thermoplug.py` & `sonofflan-0.3.2/sonofflan/devices/thermoplug.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/sonofflan/errors.py` & `sonofflan-0.3.2/sonofflan/errors.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.1/PKG-INFO` & `sonofflan-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonofflan
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to interact with Sonoff devices through LAN mode (without eWeLink cloud)
 License: BSD-3-Clause
 Keywords: sonoff,ewelink,itead
 Author: Danilo Treffiletti
 Author-email: urban82@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,15 @@
 Library to interact with Sonoff devices through LAN mode (without eWeLink cloud) with firmware
 version 3+ (tested up to version 3.7.0).
 
 Author: Danilo Treffiletti <urban82@gmail.com>
 
 License: BSD-3
 
-Version: 0.3.1
+Version: 0.3.2
 
 ## Install
 
 ### Requirements
 * Python 3.9+
 
 ## Usage
```


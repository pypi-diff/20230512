# Comparing `tmp/lmcloud-0.3.0.tar.gz` & `tmp/lmcloud-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.0.tar", last modified: Fri May 12 09:07:56 2023, max compression
+gzip compressed data, was "lmcloud-0.3.1.tar", last modified: Fri May 12 18:52:48 2023, max compression
```

## Comparing `lmcloud-0.3.0.tar` & `lmcloud-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:07:56.473077 lmcloud-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-12 09:07:38.000000 lmcloud-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 09:07:56.473077 lmcloud-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-12 09:07:38.000000 lmcloud-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:07:56.473077 lmcloud-0.3.0/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    23461 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:07:56.473077 lmcloud-0.3.0/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:07:56.473077 lmcloud-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 09:07:38.000000 lmcloud-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:52:48.583556 lmcloud-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-12 18:52:33.000000 lmcloud-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 18:52:48.579556 lmcloud-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-12 18:52:33.000000 lmcloud-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:52:48.579556 lmcloud-0.3.1/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23578 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-12 18:52:33.000000 lmcloud-0.3.1/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:52:48.579556 lmcloud-0.3.1/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 18:52:48.000000 lmcloud-0.3.1/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 18:52:48.000000 lmcloud-0.3.1/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:52:48.000000 lmcloud-0.3.1/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 18:52:48.000000 lmcloud-0.3.1/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 18:52:48.000000 lmcloud-0.3.1/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:52:48.583556 lmcloud-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 18:52:33.000000 lmcloud-0.3.1/setup.py
```

### Comparing `lmcloud-0.3.0/LICENSE` & `lmcloud-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.0/PKG-INFO` & `lmcloud-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.0/README.md` & `lmcloud-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.0/lmcloud/const.py` & `lmcloud-0.3.1/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.0/lmcloud/helpers.py` & `lmcloud-0.3.1/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.0/lmcloud/lmbluetooth.py` & `lmcloud-0.3.1/lmcloud/lmbluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.0/lmcloud/lmcloud.py` & `lmcloud-0.3.1/lmcloud/lmcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
         await self.update_local_machine_status()
         return self
 
 
     @classmethod
-    async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False):
+    async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False, bluetooth_scanner=None):
         '''
         Also initialize a local API client
         '''
 
         self = cls()
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
@@ -170,15 +170,16 @@
             asyncio.create_task(self._lm_local_api.websocket_connect())
 
         # init bluetooth if set
         if use_bluetooth:
             try:
                 self._lm_bluetooth = await LMBluetooth.create(username=credentials["username"], 
                                                         serial_number=self.machine_info[SERIAL_NUMBER],
-                                                        token=self.machine_info[KEY])
+                                                        token=self.machine_info[KEY],
+                                                        bluetooth_scanner=bluetooth_scanner)
             except BluetoothDeviceNotFound as e:
                 _logger.warn(f"Could not find bluetooth device. Bluetooth commands will not be available and commands will all be sent through cloud.")
                 _logger.debug(f"Full error: {e}")
             except BleakError as e:
                 _logger.warn(f"Bleak encountered an error while trying to connect to bluetooth device. \
                              Maybe no bluetooth adapter is available? Bluetooth commands will not be available and commands will all be sent through cloud.")
                 _logger.debug(f"Full error: {e}")
```

### Comparing `lmcloud-0.3.0/lmcloud/lmlocalapi.py` & `lmcloud-0.3.1/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.0/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.1/lmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.0/setup.py` & `lmcloud-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.0",
+    version="0.3.1",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```


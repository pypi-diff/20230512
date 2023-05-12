# Comparing `tmp/lmcloud-0.2.3.tar.gz` & `tmp/lmcloud-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.2.3.tar", last modified: Thu Apr 27 06:16:08 2023, max compression
+gzip compressed data, was "lmcloud-0.3.0.tar", last modified: Fri May 12 09:07:56 2023, max compression
```

## Comparing `lmcloud-0.2.3.tar` & `lmcloud-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:16:08.068407 lmcloud-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 06:15:47.000000 lmcloud-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-27 06:16:08.068407 lmcloud-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-27 06:15:47.000000 lmcloud-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:16:08.068407 lmcloud-0.2.3/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:16:08.068407 lmcloud-0.2.3/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:16:08.068407 lmcloud-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-27 06:15:47.000000 lmcloud-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:07:56.473077 lmcloud-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-12 09:07:38.000000 lmcloud-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 09:07:56.473077 lmcloud-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-12 09:07:38.000000 lmcloud-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:07:56.473077 lmcloud-0.3.0/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23461 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-12 09:07:38.000000 lmcloud-0.3.0/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:07:56.473077 lmcloud-0.3.0/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 09:07:56.000000 lmcloud-0.3.0/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:07:56.473077 lmcloud-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 09:07:38.000000 lmcloud-0.3.0/setup.py
```

### Comparing `lmcloud-0.2.3/LICENSE` & `lmcloud-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.3/PKG-INFO` & `lmcloud-0.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-Metadata-Version: 2.1
-Name: lmcloud
-Version: 0.2.3
-Summary: A Python implementation of the new La Marzocco API
-Home-page: https://github.com/zweckj/lmcloud
-Author: Josef Zweck
-Author-email: 24647999+zweckj@users.noreply.github.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# La Marzocco REST API
-This is a library to interface with La Marzocco's Home machine REST APIs.
+# La Marzocco Client
+This is a library to interface with La Marzocco's "new" Home machines (currently only the Micra).
 
 It's in experimentals stages and meant mainly to connect to the Micra, as for the other IoT enabled machines you can use the [lmdirect](https://github.com/rccoleman/lmdirect) library.
 
 # Libraries in this project
-- `lmlocalapi` calls the new local API the Micra exposes, using the Bearer token from the customer cloud endpoint. However, this API currently only supports getting the config, and some status objects (like shottimer) over websockets, but does not support setting anything (to my knowledge). Local settings appear to only happen through Bluetooth connections. If La Marzocco updates the firmware or more endpoints are found this library will be updated to reflect those additional endpoints.
+- `lmlocalapi` calls the new local API the Micra exposes, using the Bearer token from the customer cloud endpoint. However, this API currently only supports getting the config, and some status objects (like shottimer) over websockets, but does not support setting anything (to my knowledge). Local settings appear to only happen through [Bluetooth connections](#lmbluetooth). If La Marzocco updates the firmware or more endpoints are found this library will be updated to reflect those additional endpoints.
 - `lmcloud` interacts with `gw.lamarzocco.com` to send commands. lmcloud can be initialized to only issue remote commands, or to initialize an instance of `lmlocalapi` for getting the current machine settings. This helps to avoid flooding the cloud API and is faster overall.
+- `lmbluetooth` provides a bluetooth client to send settings to the machine via bluetooth
 
 Because of that reason the config object `self._config` in the lmcloud instance without utilizing the local API will always at least be 10 seconds old. This is to avoid automatic property checks (e.g. from HomeAssistant) to spam the cloud API. If you really require a most recent config you can call the method `get_config()`.
 
 # Setup
 
 ## lmcloud
 To run `lmcloud` you will first need to create a dict, containing `clientId`, `clientSecret`, `username` and `password`.
@@ -93,7 +76,24 @@
 ```python
 lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_websockets=True)
 
 while True:
     print(lm._lm_local_api.active_brew) # is a brew running at the moment
     print(lm._lm_local_api.active_brew_duration) # the current shot timer returned by the machine
 ```
+
+
+## lmbluetooth
+Some commands, like turning the machine on and off are always sent through bluetooth whenever possible. The available bluetooth characteristics are described in [bluetooth_characteristics](docs/bluetooth_characteristics.md).
+The class `LMBluetooth` discovers any bluetooth devices with `Micra` in the name and connects to it. Then we can send local bluetooth commands.
+
+To use Bluetooth you can either init LMCloud with
+```python
+    lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_bluetooth=True)
+```
+
+or even init the Bluetooth client standalony
+```python
+    lm_bt = await LMBluetooth.create(username, serial_number, token)
+```
+
+The token is the same token you need to initialize the local API, which you need to get from LM's cloud once. The serial number is your machine's serial number and the username is the email of your LaMarzocco account.
```

### Comparing `lmcloud-0.2.3/lmcloud/const.py` & `lmcloud-0.3.0/lmcloud/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,8 +24,13 @@
 PRE_INFUSION_SETTINGS = "PREINFUSIONSETTINGS"
 WEEKLY_SCHEDULING_CONFIG = "WEEKLYSCHEDULINGCONFIG"
 BACKFLUSH_ENABLED = "ISBACKFLUSHENABLED"
 COFFEE_TEMP = "TEMP_COFFEE"
 STEAM_TEMP = "TEMP_STEAM"
 TANK_LEVEL = "LEVEL_TANK"
 ACTIVE_BREW = "ACTIVE_BREW"
-ACTIVE_BREW_DURATION = "ACTIVE_BREW_DURATION"
+ACTIVE_BREW_DURATION = "ACTIVE_BREW_DURATION"
+
+
+# bluetooth
+SETTINGS_CHARACTERISTIC = "050b7847-e12b-09a8-b04b-8e0922a9abab"
+AUTH_CHARACTERISTIC = "090b7847-e12b-09a8-b04b-8e0922a9abab"
```

### Comparing `lmcloud-0.2.3/lmcloud/helpers.py` & `lmcloud-0.3.0/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.3/lmcloud/lmcloud.py` & `lmcloud-0.3.0/lmcloud/lmcloud.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .const import *
 from .exceptions import *
 from .lmlocalapi import LMLocalAPI
+from .lmbluetooth import LMBluetooth
 from .helpers import *
 from authlib.integrations.base_client.errors import OAuthError
 from authlib.integrations.httpx_client import AsyncOAuth2Client
-from requests.exceptions import RequestException
 from datetime import datetime
+from bleak import BleakError
 import logging
 import asyncio
 
 _logger = logging.getLogger(__name__)
 
 class LMCloud:  
 
@@ -31,28 +32,34 @@
     
     @property 
     def firmware_version(self):
         return self._firmware["machine_firmware"]["version"]
 
     @property
     def config(self):
-        """ Return the config with capitalized keys to be consistent across local/remote APIs """
+        """ 
+        Return the config with capitalized keys to be consistent across local/remote APIs 
+        """
+
         return {k.upper():v for k,v in self._config.items()}
     
     @property
     def status(self):
         return self._status
     
     @property
     def statistics(self):
         return self._statistics
     
     @property 
     def current_status(self):
-        """ Build object which holds status for lamarzocco Home Assistant Integration"""
+        """ 
+        Build object which holds status for lamarzocco Home Assistant Integration
+        """
+
         return {
             "power": True if self.config[MACHINE_MODE] == "BrewingMode" else False,
             "enable_prebrewing": True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "Enabled" else False,
             "enable_preinfusion": True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "TypeB" else False,
             "steam_boiler_enable": next(item for item in self.config[BOILERS] if item["id"] == STEAM_BOILER_NAME)["isEnabled"],
             "global_auto": self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"],
             "coffee_temp": self.status[COFFEE_TEMP],
@@ -118,53 +125,77 @@
     ***********  Functions ********************
     *******************************************
     '''
 
     def __init__(self):
         _logger.setLevel(logging.DEBUG)
         self._lm_local_api      = None
+        self._lm_bluetooth      = None
         self. _config           = {}
         self. _status           = {}
         self. _statistics       = {}
         self._use_websocket     = False
 
-    '''
-    Initialize a cloud only client
-    '''
+
     @classmethod
     async def create(cls, credentials):
+        '''
+        Initialize a cloud only client
+        '''
+
         self = cls()
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
         await self.update_local_machine_status()
         return self
 
-    '''
-    Also initialize a local API client
-    '''
+
     @classmethod
-    async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False):
+    async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False):
+        '''
+        Also initialize a local API client
+        '''
+
         self = cls()
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
         self._lm_local_api = LMLocalAPI(local_ip=ip, local_port=port, local_bearer=self.machine_info[KEY])
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
+
+        # init websockets if set
         if use_websocket:
             self._use_websocket = True
             asyncio.create_task(self._lm_local_api.websocket_connect())
+
+        # init bluetooth if set
+        if use_bluetooth:
+            try:
+                self._lm_bluetooth = await LMBluetooth.create(username=credentials["username"], 
+                                                        serial_number=self.machine_info[SERIAL_NUMBER],
+                                                        token=self.machine_info[KEY])
+            except BluetoothDeviceNotFound as e:
+                _logger.warn(f"Could not find bluetooth device. Bluetooth commands will not be available and commands will all be sent through cloud.")
+                _logger.debug(f"Full error: {e}")
+            except BleakError as e:
+                _logger.warn(f"Bleak encountered an error while trying to connect to bluetooth device. \
+                             Maybe no bluetooth adapter is available? Bluetooth commands will not be available and commands will all be sent through cloud.")
+                _logger.debug(f"Full error: {e}")
+
         await self.update_local_machine_status(in_init=True)
         return self
         
-    '''
-    Establish connection by building the OAuth client and requesting the token
-    '''
+
     async def _connect(self, credentials):
+        '''
+        Establish connection by building the OAuth client and requesting the token
+        '''
+
         client = AsyncOAuth2Client(
             client_id=credentials["client_id"],
             client_secret=credentials["client_secret"],
             token_endpoint=TOKEN_URL
         )
 
         headers = {
@@ -181,41 +212,46 @@
             )
             return client
     
         except OAuthError as err:
             raise AuthFail("Authorization failure") from err
         
 
-    '''
-    Get configuration from cloud
-    '''
     async def get_config(self):
+        '''
+        Get configuration from cloud
+        '''
+        
         url = f"{self._gw_url_with_serial}/configuration"
         try:
             config = await self._rest_api_call(url=url, verb="GET")
             return config
         except Exception as e:
             _logger.error(f"Could not get config from cloud. Full error: {e}")
             return self._config
         
-    '''
-    Load the config into variables in this class
-    '''
+
     async def _update_config_obj(self, force_update=False):
+        '''
+        Load the config into variables in this class
+        '''
+
         if self._config:
             # wait at least 10 seconds between config updates to not flood the remote API
             if (datetime.now() - self._last_config_update).total_seconds() < POLLING_DELAY_S or force_update:
                 return
         self._config = await self.get_config()
         self._last_config_update = datetime.now()
 
-    '''
-    Get status from cloud
-    '''
+
     async def get_status(self):
+        '''
+        Get status from cloud
+        '''
+
         url = f"{self._gw_url_with_serial}/status"
         try:
             status = await self._rest_api_call(url=url, verb="GET")
             return status
         except Exception as e:
             _logger.error(f"Could not get config from cloud. Full error: {e}")
             return self._status
@@ -224,23 +260,25 @@
         if self._status:
             # wait at least 10 seconds between config updates to not flood the remote API
             if (datetime.now() - self._last_status_update).total_seconds() < POLLING_DELAY_S or force_update:
                 return
         self._status = await self.get_status()
         self._last_status_update = datetime.now() 
 
-    '''
-    update config object
-    '''
+
     async def update_local_machine_status(self, in_init=False):
+        '''
+        update config object
+        '''
+
         if self._lm_local_api:
             try:
                 conf = await self._lm_local_api.local_get_config()
                 self._config = {k.upper():v for k,v in conf.items()}
-            except RequestException as e:
+            except Exception as e:
                 _logger.warn(f"Could not connect to local API although initialized. Full error: {e}")
                 await self._update_config_obj()
 
             if self._lm_local_api._timestamp_last_websocket_msg == None or (datetime.now() - self._lm_local_api._timestamp_last_websocket_msg).total_seconds() > 30: 
                 if self._use_websocket and not in_init: # during init we don't want to log this warning
                     _logger.warn("Could not get local machine status. Falling back to cloud status.")
                 await self._update_status_obj()
@@ -251,18 +289,20 @@
                 self._status = self._lm_local_api._status # reference to the same object tp get websocket updates
         else:
             await self._update_config_obj()     
             await self._update_status_obj()
 
         await self._update_statistics_obj()
 
-    '''
-    Get statistics
-    '''
+
     async def get_statistics(self):
+        '''
+        Get statistics
+        '''
+
         url = f"{self._gw_url_with_serial}/statistics/counters"
         try:
             statistics = await self._rest_api_call(url=url, verb="GET")
             return statistics
         except Exception as e:
             _logger.error(f"Could not get config from cloud. Full error: {e}")
             return self._statistics   
@@ -273,18 +313,20 @@
             # wait at least 10 seconds between config updates to not flood the remote API
             if (datetime.now() - self._last_statistics_update).total_seconds() < POLLING_DELAY_STATISTICS_S or force_update:
                 return
         self._statistics = await self.get_statistics()
         self._last_statistics_update = datetime.now() 
 
 
-    '''
-    Wrapper for the API call
-    '''
+
     async def _rest_api_call(self, url, verb="GET", data=None):
+        '''
+        Wrapper for the API call
+        '''
+
         # make sure oauth token is still valid
         if self.client.token.is_expired():
             await self.client.refresh_token(TOKEN_URL)
 
         # make API call
         if verb == "GET":
             response = await self.client.get(url)
@@ -298,115 +340,154 @@
             return response.json()["data"]
         else:
             msg = f"Request to endpoint {response.url} failed with status code {response.status_code}"
             _logger.warn(f"{msg}. Details: {response.text}")
             raise RequestNotSuccessful(msg)
         
 
-    '''
-    Get Basic machine info from the customer endpoint
-    '''
+    async def _send_bluetooth_command(self, func, param):
+        '''
+        Wrapper for bluetooth commands
+        '''
+        try:
+            await func(param)
+            return True
+        except BleakError as e:
+            _logger.warn("Could not send command to bluetooth device, even though initalized. Falling back to cloud...")
+            _logger.debug(f"Full error: {e}")
+            return False
+        
+
     async def _get_machine_info(self):
+        '''
+        Get Basic machine info from the customer endpoint
+        '''
+
         data = await self._rest_api_call(url=CUSTOMER_URL, verb="GET")
 
         machine_info = {}
         fleet = data["fleet"][0]
         machine_info[KEY] = fleet["communicationKey"]
         machine_info[SERIAL_NUMBER] = fleet["machine"]["serialNumber"]
         machine_info[MACHINE_NAME] = fleet["name"]
         machine_info[MODEL_NAME] = fleet["machine"]["model"]["name"]
         return machine_info
     
-    '''
-    Get Firmware details
-    '''
+
     async def get_firmware(self):
+        '''
+        Get Firmware details
+        '''
+
         url = f"{self._gw_url_with_serial}/firmwarev2/"
         return await self._rest_api_call(url=url, verb="GET")
 
-
-    '''
-    Machine power wrapper with bool input
-    '''
+   
     async def set_power(self, enabled: bool):
-        power_status = "ON" if enabled else "STANDBY"
-        return await self._set_power(power_status)
+        '''
+        Turn power of machine on or off
+        '''
+
+        if self._lm_bluetooth:
+            bt_ok = await self._send_bluetooth_command(self._lm_bluetooth.set_power, enabled)
+            response = "Ok"
 
-    '''
-    Turn power of machine on or off
-    '''
-    async def _set_power(self, power_status: str):
-        power_status = str.upper(power_status)
-        if not power_status in ["ON", "STANDBY"]:
-            msg = "Power status can only be on or standby"
-            self._logger.debug(msg)
-            raise ValueError(msg)
-        else:
+        if not self._lm_bluetooth or not bt_ok:
+            power_status = "ON" if enabled else "STANDBY"
             data = {"status": power_status}
             url = f"{self._gw_url_with_serial}/status"
             response = await self._rest_api_call(url=url, verb="POST", data=data)
-            self._config[MACHINE_MODE] = "BrewingMode" if power_status == "ON" else "StandBy"
-            return response
 
-    '''
-    Turn Steamboiler on or off
-    '''
+        self._config[MACHINE_MODE] = "BrewingMode" if enabled else "StandBy"
+        return response
+
+
     async def set_steam(self, steam_state:bool):
+        '''
+        Turn Steamboiler on or off
+        '''
+
         if not type(steam_state) == bool:
             msg = "Steam state must be boolean"
             _logger.debug(msg)
             raise TypeError(msg)
         else:
-            data = {"identifier": STEAM_BOILER_NAME, "state": steam_state}
-            url = f"{self._gw_url_with_serial}/enable-boiler"
-            response = await self._rest_api_call(url=url, verb="POST", data=data)
+            if self._lm_bluetooth:
+                bt_ok = await self._send_bluetooth_command(self._lm_bluetooth.set_steam, steam_state)
+                response = "Ok"
+
+            if not self._lm_bluetooth or not bt_ok:
+                data = {"identifier": STEAM_BOILER_NAME, "state": steam_state}
+                url = f"{self._gw_url_with_serial}/enable-boiler"
+                response = await self._rest_api_call(url=url, verb="POST", data=data)
+            
             idx = [STEAM_BOILER_NAME in i['id'] for i in self.config[BOILERS]].index(True)
             self._config[BOILERS][idx]["isEnabled"] = steam_state
             return response
 
-    '''
-    Set steamboiler temperature (in Celsius)
-    '''
+
     async def set_steam_temp(self, temperature:int):
+        '''
+        Set steamboiler temperature (in Celsius)
+        '''
+
         if not type(temperature) == int:
             msg = "Steam temp must be integer"
             _logger.debug(msg)
             raise TypeError(msg)
+        
         elif not temperature == 131 and not temperature == 128 and not temperature == 126:
             msg = "Steam temp must be one of 126, 128, 131 (°C)"
             _logger.debug(msg)
             raise ValueError(msg)
+        
         else:
-            data = { "identifier": STEAM_BOILER_NAME, "value": temperature}
-            url = f"{self._gw_url_with_serial}/target-boiler"
-            response = await self._rest_api_call(url=url, verb="POST", data=data)
+            if self._lm_bluetooth:
+                bt_ok = await self._send_bluetooth_command(self._lm_bluetooth.set_steam_temp, temperature)
+                response = "Ok"
+                    
+            if not self._lm_bluetooth or not bt_ok:
+                data = { "identifier": STEAM_BOILER_NAME, "value": temperature}
+                url = f"{self._gw_url_with_serial}/target-boiler"
+                response = await self._rest_api_call(url=url, verb="POST", data=data)
+
             self._config[BOILER_TARGET_TEMP][STEAM_BOILER_NAME] = temperature
             return response
 
-    '''
-    Set coffee boiler temperature (in Celsius)
-    '''
+
     async def set_coffee_temp(self, temperature):
+        '''
+        Set coffee boiler temperature (in Celsius)
+        '''
 
         if temperature > 104 or temperature < 85:
             msg = "Coffee temp must be between 85 and 104 (°C)"
             _logger.debug(msg)
             raise ValueError(msg)
-        else:
+        else: 
             temperature = round(temperature, 1)
-            data = { "identifier": COFFEE_BOILER_NAME, "value": temperature}
-            url = f"{self._gw_url_with_serial}/target-boiler"
-            response = await self._rest_api_call(url=url, verb="POST", data=data)
+
+            if self._lm_bluetooth:
+                bt_ok = await self._send_bluetooth_command(self._lm_bluetooth.set_coffee_temp, temperature)
+                response = "Ok"
+            
+            if not self._lm_bluetooth or not bt_ok:
+                data = { "identifier": COFFEE_BOILER_NAME, "value": temperature}
+                url = f"{self._gw_url_with_serial}/target-boiler"
+                response = await self._rest_api_call(url=url, verb="POST", data=data)
+
             self._config[BOILER_TARGET_TEMP][COFFEE_BOILER_NAME] = temperature
             return response
 
-    '''
-    Enable/Disable Pre-Brew or Pre-Infusion (mutually exclusive)
-    '''
+
     async def _set_pre_brew_infusion(self, mode):
+        '''
+        Enable/Disable Pre-Brew or Pre-Infusion (mutually exclusive)
+        '''
+
         if mode != "Disabled" and mode != "TypeB" and mode != "Enabled":
             msg = "Pre-Infusion/Pre-Brew can only be TypeB (PreInfusion), Enabled (Pre-Brew) or Disabled"
             _logger.debug(msg)
             raise ValueError(msg)
         elif mode == "TypedB" and not (await self.get_plumbin_enabled()):
             msg = "Pre-Infusion can only be enabled when plumbin is enabled"
             _logger.debug(msg)
@@ -414,33 +495,38 @@
         else:
             url = f"{self._gw_url_with_serial}/enable-preinfusion"
             data = {"mode": mode}
             response = await self._rest_api_call(url=url, verb="POST", data=data)
             self._config[PRE_INFUSION_SETTINGS]["mode"] = mode
             return response
 
-    '''
-    Enable/Disable Pre-brew (Mode = Enabled)
-    '''
     async def set_prebrew(self, enabled: bool):
+        '''
+        Enable/Disable Pre-brew (Mode = Enabled)
+        '''
+
         mode = "Enabled" if enabled else "Disabled"
         return await self._set_pre_brew_infusion(mode)
 
-    '''
-    Enable/Disable Pre-Infusion (Mode = TypeB)
-    '''
+
     async def set_preinfusion(self, enabled: bool):
+        '''
+        Enable/Disable Pre-Infusion (Mode = TypeB)
+        '''
+
         mode = "TypeB" if enabled else "Disabled"
         return await self._set_pre_brew_infusion(mode)
 
-    '''
-    Set Pre-Brew details
-    Also used for preinfusion (prebrewOnTime=0, prebrewOnTime=ms)
-    '''
+
     async def configure_prebrew(self, prebrewOnTime=5000, prebrewOffTime=5000):
+        '''
+        Set Pre-Brew details
+        Also used for preinfusion (prebrewOnTime=0, prebrewOnTime=ms)
+        '''
+
         if type(prebrewOnTime) != int or type(prebrewOffTime) != int:
             msg = "Prebrew times must be in ms (integer)"
             _logger.debug(msg)
             raise TypeError(msg)
         else:
             if prebrewOnTime % 100 != 0 or prebrewOffTime % 100 != 0:
                 msg = "Prebrew times must be multiple of 100"
@@ -455,80 +541,84 @@
             }
             response = await self._rest_api_call(url=url, verb="POST", data=data)
 
             self._config[PRE_INFUSION_SETTINGS]["Group1"][0]["preWetTime"] = prebrewOnTime % 1000
             self._config[PRE_INFUSION_SETTINGS]["Group1"][0]["preWetHoldTime"] = prebrewOffTime % 1000
             return response
 
-    '''
-    Enable or disable plumbin mode
-    '''
+
     async def enable_plumbin(self, enable:bool):
+        '''
+        Enable or disable plumbin mode
+        '''
+
         if not type(enable) == bool:
             msg = "Enable param must be boolean"
             _logger.debug(msg)
             raise TypeError(msg)
         else:
             data = {"enable": enable}
             url = f"{self._gw_url_with_serial}/enable-plumbin"
             response = await self._rest_api_call(url=url, verb="POST", data=data)
             self._config[PLUMBED_IN] = enable
             return response
 
-    '''
-    Set auto-on/off schedule
-
 
-    schedule object:
-    [
-        {
-            "day": "MONDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        },
-        {
-            "day": "TUESDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        },
-        {
-            "day": "WEDNESDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        },
-        {
-            "day": "THURSDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        },
-        {
-            "day": "FRIDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        },
-        {
-            "day": "SATURDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        },
-        {
-            "day": "SUNDAY",
-            "enable": false,
-            "off": "00:00",
-            "on": "00:00"
-        }
-    ]
-    '''
     async def configure_schedule(self, enable: bool, schedule: list):
+        '''
+        Set auto-on/off schedule
+
+
+        schedule object:
+        [
+            {
+                "day": "MONDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            },
+            {
+                "day": "TUESDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            },
+            {
+                "day": "WEDNESDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            },
+            {
+                "day": "THURSDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            },
+            {
+                "day": "FRIDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            },
+            {
+                "day": "SATURDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            },
+            {
+                "day": "SUNDAY",
+                "enable": false,
+                "off": "00:00",
+                "on": "00:00"
+            }
+        ]
+        '''
+
         url = f"{self._gw_url_with_serial}/scheduling"
         data = {"enable": enable, "days": schedule}
         response = await self._rest_api_call(url=url, verb="POST", data=data)
         self._config[WEEKLY_SCHEDULING_CONFIG] = schedule_in_to_out(enable, schedule)
         return response
 
     async def set_auto_on_off(self, day_of_week, hour_on, minute_on, hour_off, minute_off):
@@ -542,16 +632,18 @@
     async def set_auto_on_off_enable(self, day_of_week, enable):
         schedule = await self.get_schedule()
         idx = [index for (index, d) in enumerate(schedule) if d["day"] == day_of_week.upper()][0]
         schedule[idx]["enable"] = enable
         return await self.configure_schedule(self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"], schedule)
 
 
-    '''
-    Send command to start backflushing
-    '''
+
     async def start_backflush(self):
+        '''
+        Send command to start backflushing
+        '''
+
         url = f"{self._gw_url_with_serial}/enable-backflush"
         data = {"enable": True}
         response = await self._rest_api_call(url=url, verb="POST", data=data)
         self._config[BACKFLUSH_ENABLED] = True
         return response
```

### Comparing `lmcloud-0.2.3/lmcloud/lmlocalapi.py` & `lmcloud-0.3.0/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.3/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,22 +12,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# La Marzocco REST API
-This is a library to interface with La Marzocco's Home machine REST APIs.
+# La Marzocco Client
+This is a library to interface with La Marzocco's "new" Home machines (currently only the Micra).
 
 It's in experimentals stages and meant mainly to connect to the Micra, as for the other IoT enabled machines you can use the [lmdirect](https://github.com/rccoleman/lmdirect) library.
 
 # Libraries in this project
-- `lmlocalapi` calls the new local API the Micra exposes, using the Bearer token from the customer cloud endpoint. However, this API currently only supports getting the config, and some status objects (like shottimer) over websockets, but does not support setting anything (to my knowledge). Local settings appear to only happen through Bluetooth connections. If La Marzocco updates the firmware or more endpoints are found this library will be updated to reflect those additional endpoints.
+- `lmlocalapi` calls the new local API the Micra exposes, using the Bearer token from the customer cloud endpoint. However, this API currently only supports getting the config, and some status objects (like shottimer) over websockets, but does not support setting anything (to my knowledge). Local settings appear to only happen through [Bluetooth connections](#lmbluetooth). If La Marzocco updates the firmware or more endpoints are found this library will be updated to reflect those additional endpoints.
 - `lmcloud` interacts with `gw.lamarzocco.com` to send commands. lmcloud can be initialized to only issue remote commands, or to initialize an instance of `lmlocalapi` for getting the current machine settings. This helps to avoid flooding the cloud API and is faster overall.
+- `lmbluetooth` provides a bluetooth client to send settings to the machine via bluetooth
 
 Because of that reason the config object `self._config` in the lmcloud instance without utilizing the local API will always at least be 10 seconds old. This is to avoid automatic property checks (e.g. from HomeAssistant) to spam the cloud API. If you really require a most recent config you can call the method `get_config()`.
 
 # Setup
 
 ## lmcloud
 To run `lmcloud` you will first need to create a dict, containing `clientId`, `clientSecret`, `username` and `password`.
@@ -93,7 +94,24 @@
 ```python
 lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_websockets=True)
 
 while True:
     print(lm._lm_local_api.active_brew) # is a brew running at the moment
     print(lm._lm_local_api.active_brew_duration) # the current shot timer returned by the machine
 ```
+
+
+## lmbluetooth
+Some commands, like turning the machine on and off are always sent through bluetooth whenever possible. The available bluetooth characteristics are described in [bluetooth_characteristics](docs/bluetooth_characteristics.md).
+The class `LMBluetooth` discovers any bluetooth devices with `Micra` in the name and connects to it. Then we can send local bluetooth commands.
+
+To use Bluetooth you can either init LMCloud with
+```python
+    lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_bluetooth=True)
+```
+
+or even init the Bluetooth client standalony
+```python
+    lm_bt = await LMBluetooth.create(username, serial_number, token)
+```
+
+The token is the same token you need to initialize the local API, which you need to get from LM's cloud once. The serial number is your machine's serial number and the username is the email of your LaMarzocco account.
```

### Comparing `lmcloud-0.2.3/setup.py` & `lmcloud-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.2.3",
+    version="0.3.0",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
@@ -19,12 +19,12 @@
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=setuptools.find_packages(),
-    install_requires=["httpx>=0.16.1", "authlib>=0.15.5,<1.0", "aiohttp>=3.8.4", "websockets>=11.0.2"],
+    install_requires=["httpx>=0.16.1", "authlib>=0.15.5,<1.0", "aiohttp>=3.8.4", "websockets>=11.0.2", "bleak>=0.20.2"],
     package_data={
         "license": ["LICENSE"],
     },
 )
```


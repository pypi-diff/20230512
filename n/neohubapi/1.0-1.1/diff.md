# Comparing `tmp/neohubapi-1.0.tar.gz` & `tmp/neohubapi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neohubapi-1.0.tar", last modified: Sun Dec 25 11:09:55 2022, max compression
+gzip compressed data, was "neohubapi-1.1.tar", last modified: Thu May 11 23:08:53 2023, max compression
```

## Comparing `neohubapi-1.0.tar` & `neohubapi-1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2022-12-25 11:09:55.105943 neohubapi-1.0/
--rw-r--r--   0 andrius   (1000) andrius   (1000)      135 2020-12-27 20:17:35.000000 neohubapi-1.0/.gitignore
--rw-r--r--   0 andrius   (1000) andrius   (1000)      330 2022-12-01 20:33:25.000000 neohubapi-1.0/.gitlab-ci.yml
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2022-12-25 11:09:55.095943 neohubapi-1.0/LICENSES/
--rw-r--r--   0 andrius   (1000) andrius   (1000)    16814 2020-10-16 22:01:40.000000 neohubapi-1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     6916 2020-11-20 18:38:22.000000 neohubapi-1.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     7431 2020-10-16 15:56:35.000000 neohubapi-1.0/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     1108 2020-10-16 22:01:40.000000 neohubapi-1.0/LICENSES/MIT.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)     2511 2022-12-25 11:09:55.095943 neohubapi-1.0/PKG-INFO
--rw-r--r--   0 andrius   (1000) andrius   (1000)     2024 2022-12-25 11:05:45.000000 neohubapi-1.0/README.md
--rwxr-xr-x   0 andrius   (1000) andrius   (1000)      938 2021-01-19 21:53:09.000000 neohubapi-1.0/example.py
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2022-12-25 11:09:55.095943 neohubapi-1.0/neohubapi/
--rw-r--r--   0 andrius   (1000) andrius   (1000)      181 2021-02-06 14:30:21.000000 neohubapi-1.0/neohubapi/__init__.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)     1229 2021-06-23 10:58:50.000000 neohubapi-1.0/neohubapi/enums.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)    20343 2022-12-01 20:29:03.000000 neohubapi-1.0/neohubapi/neohub.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)     6118 2022-07-09 08:47:41.000000 neohubapi-1.0/neohubapi/neostat.py
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2022-12-25 11:09:55.095943 neohubapi-1.0/neohubapi.egg-info/
--rw-r--r--   0 andrius   (1000) andrius   (1000)     2511 2022-12-25 11:09:54.000000 neohubapi-1.0/neohubapi.egg-info/PKG-INFO
--rw-r--r--   0 andrius   (1000) andrius   (1000)      475 2022-12-25 11:09:54.000000 neohubapi-1.0/neohubapi.egg-info/SOURCES.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2022-12-25 11:09:54.000000 neohubapi-1.0/neohubapi.egg-info/dependency_links.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)       26 2022-12-25 11:09:54.000000 neohubapi-1.0/neohubapi.egg-info/requires.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)       10 2022-12-25 11:09:54.000000 neohubapi-1.0/neohubapi.egg-info/top_level.txt
--rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2020-12-27 19:07:42.000000 neohubapi-1.0/neohubapi.egg-info/zip-safe
--rw-r--r--   0 andrius   (1000) andrius   (1000)       29 2022-12-01 20:29:12.000000 neohubapi-1.0/pytest.ini
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2022-12-25 11:09:55.095943 neohubapi-1.0/scripts/
--rwxr-xr-x   0 andrius   (1000) andrius   (1000)    11176 2021-02-06 14:30:21.000000 neohubapi-1.0/scripts/neohub_cli.py
--rw-r--r--   0 andrius   (1000) andrius   (1000)       38 2022-12-25 11:09:55.105943 neohubapi-1.0/setup.cfg
--rwxr-xr-x   0 andrius   (1000) andrius   (1000)     1012 2022-12-25 11:06:29.000000 neohubapi-1.0/setup.py
-drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2022-12-25 11:09:55.095943 neohubapi-1.0/tests/
--rw-r--r--   0 andrius   (1000) andrius   (1000)     3279 2022-12-01 20:29:03.000000 neohubapi-1.0/tests/test_neohub.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-05-11 23:08:53.450853 neohubapi-1.1/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      135 2020-12-27 20:17:35.000000 neohubapi-1.1/.gitignore
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      330 2022-12-01 20:33:25.000000 neohubapi-1.1/.gitlab-ci.yml
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-05-11 23:08:53.450853 neohubapi-1.1/LICENSES/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)    16814 2020-10-16 22:01:40.000000 neohubapi-1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     6916 2020-11-20 18:38:22.000000 neohubapi-1.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     7431 2020-10-16 15:56:35.000000 neohubapi-1.1/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     1108 2020-10-16 22:01:40.000000 neohubapi-1.1/LICENSES/MIT.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     2511 2023-05-11 23:08:53.450853 neohubapi-1.1/PKG-INFO
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     2024 2022-12-25 11:05:45.000000 neohubapi-1.1/README.md
+-rwxr-xr-x   0 andrius   (1000) andrius   (1000)      938 2021-01-19 21:53:09.000000 neohubapi-1.1/example.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-05-11 23:08:53.450853 neohubapi-1.1/neohubapi/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      181 2021-02-06 14:30:21.000000 neohubapi-1.1/neohubapi/__init__.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     1229 2021-06-23 10:58:50.000000 neohubapi-1.1/neohubapi/enums.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)    21105 2023-05-04 17:42:39.000000 neohubapi-1.1/neohubapi/neohub.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     6118 2022-07-09 08:47:41.000000 neohubapi-1.1/neohubapi/neostat.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-05-11 23:08:53.450853 neohubapi-1.1/neohubapi.egg-info/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     2511 2023-05-11 23:08:52.000000 neohubapi-1.1/neohubapi.egg-info/PKG-INFO
+-rw-r--r--   0 andrius   (1000) andrius   (1000)      475 2023-05-11 23:08:53.000000 neohubapi-1.1/neohubapi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2023-05-11 23:08:52.000000 neohubapi-1.1/neohubapi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       26 2023-05-11 23:08:52.000000 neohubapi-1.1/neohubapi.egg-info/requires.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       10 2023-05-11 23:08:52.000000 neohubapi-1.1/neohubapi.egg-info/top_level.txt
+-rw-r--r--   0 andrius   (1000) andrius   (1000)        1 2020-12-27 19:07:42.000000 neohubapi-1.1/neohubapi.egg-info/zip-safe
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       29 2022-12-01 20:29:12.000000 neohubapi-1.1/pytest.ini
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-05-11 23:08:53.450853 neohubapi-1.1/scripts/
+-rwxr-xr-x   0 andrius   (1000) andrius   (1000)    11176 2021-02-06 14:30:21.000000 neohubapi-1.1/scripts/neohub_cli.py
+-rw-r--r--   0 andrius   (1000) andrius   (1000)       38 2023-05-11 23:08:53.450853 neohubapi-1.1/setup.cfg
+-rwxr-xr-x   0 andrius   (1000) andrius   (1000)     1012 2023-05-11 23:02:37.000000 neohubapi-1.1/setup.py
+drwxr-xr-x   0 andrius   (1000) andrius   (1000)        0 2023-05-11 23:08:53.450853 neohubapi-1.1/tests/
+-rw-r--r--   0 andrius   (1000) andrius   (1000)     3279 2022-12-01 20:29:03.000000 neohubapi-1.1/tests/test_neohub.py
```

### Comparing `neohubapi-1.0/LICENSES/CC-BY-4.0.txt` & `neohubapi-1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/LICENSES/CC0-1.0.txt` & `neohubapi-1.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/LICENSES/LGPL-3.0-or-later.txt` & `neohubapi-1.1/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/LICENSES/MIT.txt` & `neohubapi-1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/PKG-INFO` & `neohubapi-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neohubapi
-Version: 1.0
+Version: 1.1
 Summary: Async library to communicate with Heatmiser NeoHub 2 API.
 Home-page: https://gitlab.com/neohubapi/neohubapi/
 Author: Andrius Štikonas
 Author-email: andrius@stikonas.eu
 Keywords: neohub,heatmiser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `neohubapi-1.0/README.md` & `neohubapi-1.1/README.md`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/example.py` & `neohubapi-1.1/example.py`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/neohubapi/enums.py` & `neohubapi-1.1/neohubapi/enums.py`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/neohubapi/neohub.py` & `neohubapi-1.1/neohubapi/neohub.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,24 +431,41 @@
 
     async def get_live_data(self):
         """
         Returns live data from hub and all devices
         """
 
         message = {"GET_LIVE_DATA": 0}
-
         hub_data = await self._send(message)
+
+        # We need the engineers data to get things like Device Type, Sensor Mode etc.
+        get_eng_data_msg = {"GET_ENGINEERS": 0}
+        eng_hub_data = await self._send(get_eng_data_msg)
+
         devices = hub_data.devices
         delattr(hub_data, "devices")
 
+        # Combine the live data and engineers data to produce a full dataset to work from.
+        # Start by working through each device in the devices
+        for device in devices:
+
+            # Find matching device ID in Engineers data
+            for key, value in eng_hub_data.__dict__.items():
+                if device.DEVICE_ID == value.DEVICE_ID:
+
+                    # Now add the engineers data dictionary entries to the existing device dictionary.
+                    for x in value.__dict__.items():
+                        setattr(device, x[0], x[1])
+
         thermostat_list = list(filter(lambda device: hasattr(device, 'THERMOSTAT') and device.THERMOSTAT, devices))
         timeclock_list = list(filter(lambda device: hasattr(device, 'TIMECLOCK') and device.TIMECLOCK, devices))
 
         thermostats = []
         timeclocks = []
+
         for thermostat in thermostat_list:
             thermostats.append(NeoStat(self, thermostat))
 
         for timeclock in timeclock_list:
             timeclocks.append(NeoStat(self, timeclock))
 
         devices = {}
```

### Comparing `neohubapi-1.0/neohubapi/neostat.py` & `neohubapi-1.1/neohubapi/neostat.py`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/neohubapi.egg-info/PKG-INFO` & `neohubapi-1.1/neohubapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neohubapi
-Version: 1.0
+Version: 1.1
 Summary: Async library to communicate with Heatmiser NeoHub 2 API.
 Home-page: https://gitlab.com/neohubapi/neohubapi/
 Author: Andrius Štikonas
 Author-email: andrius@stikonas.eu
 Keywords: neohub,heatmiser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `neohubapi-1.0/scripts/neohub_cli.py` & `neohubapi-1.1/scripts/neohub_cli.py`

 * *Files identical despite different names*

### Comparing `neohubapi-1.0/setup.py` & `neohubapi-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="neohubapi",
-    version="1.0",
+    version="1.1",
     description="Async library to communicate with Heatmiser NeoHub 2 API.",
     url="https://gitlab.com/neohubapi/neohubapi/",
     author="Andrius Štikonas",
     author_email="andrius@stikonas.eu",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
```

### Comparing `neohubapi-1.0/tests/test_neohub.py` & `neohubapi-1.1/tests/test_neohub.py`

 * *Files identical despite different names*


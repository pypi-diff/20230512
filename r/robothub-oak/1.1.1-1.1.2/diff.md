# Comparing `tmp/robothub_oak-1.1.1.tar.gz` & `tmp/robothub_oak-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub_oak-1.1.1.tar", last modified: Tue May  9 09:53:21 2023, max compression
+gzip compressed data, was "robothub_oak-1.1.2.tar", last modified: Thu May 11 21:58:52 2023, max compression
```

## Comparing `robothub_oak-1.1.1.tar` & `robothub_oak-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.139706 robothub_oak-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.147706 robothub_oak-1.1.1/src/robothub_oak/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/src/robothub_oak/components/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/device.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13350 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8615 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.147706 robothub_oak-1.1.1/src/robothub_oak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/tests/test_hub_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.798801 robothub_oak-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 21:58:52.798801 robothub_oak-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 21:58:52.798801 robothub_oak-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.786801 robothub_oak-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.790801 robothub_oak-1.1.2/src/robothub_oak/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.794801 robothub_oak-1.1.2/src/robothub_oak/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/device.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13350 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8584 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.794801 robothub_oak-1.1.2/src/robothub_oak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.794801 robothub_oak-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/tests/test_hub_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/tests/test_manager.py
```

### Comparing `robothub_oak-1.1.1/LICENSE` & `robothub_oak-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/PKG-INFO` & `robothub_oak-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub_oak
-Version: 1.1.1
+Version: 1.1.2
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.1.1/README.md` & `robothub_oak-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/setup.py` & `robothub_oak-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub_oak',
-    version='1.1.1',
+    version='1.1.2',
     description='RobotHub-OAK integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub robot hub connect agent depthai oak sdk',
     author='Luxonis',
```

### Comparing `robothub_oak-1.1.1/src/robothub_oak/callbacks.py` & `robothub_oak-1.1.2/src/robothub_oak/callbacks.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/commands.py` & `robothub_oak-1.1.2/src/robothub_oak/commands.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/components/camera.py` & `robothub_oak-1.1.2/src/robothub_oak/components/camera.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/components/neural_network.py` & `robothub_oak-1.1.2/src/robothub_oak/components/neural_network.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/components/stereo.py` & `robothub_oak-1.1.2/src/robothub_oak/components/stereo.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/device.py` & `robothub_oak-1.1.2/src/robothub_oak/device.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/hub_camera.py` & `robothub_oak-1.1.2/src/robothub_oak/hub_camera.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak/manager.py` & `robothub_oak-1.1.2/src/robothub_oak/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,46 +210,46 @@
         :param mxid: The mxid of the device.
         :param ip_address: The IP address of the device.
         :return: The device.
         """
         assert id or name or mxid or ip_address, 'Must specify at least one of id, name, mxid or ip_address'
 
         device = Device(id=id, name=name, mxid=mxid, ip_address=ip_address)
-        device_name = device.get_device_name()
 
         # Check if device already exists
         for d in DEVICE_MANAGER.devices:
-            if d == device_name:
+            if d == device:
                 return d
 
         # Add device to device manager if it doesn't exist
         DEVICE_MANAGER.add_device(device)
         return device
 
     @staticmethod
     def get_all_devices() -> List[Device]:
         """
         Returns all devices.
 
         :return: All devices.
         """
-        devices = []
         for obj in robothub.DEVICES:
             device_dict = defaultdict(lambda: None, obj.oak)
-            device = Device(mxid=device_dict['serialNumber'],
-                            name=device_dict['productName'],
-                            id=device_dict['name'],
-                            ip_address=device_dict['ipAddress'])
+            device = DEVICE_MANAGER.get_device(
+                mxid=device_dict['serialNumber'],
+                name=device_dict['productName'],
+                id=device_dict['name'],
+                ip_address=device_dict['ipAddress']
+            )
 
             exists = False
             for d in DEVICE_MANAGER.devices:
                 if d == device:
                     exists = True
-                    break
+                    continue
 
             if not exists:
-                devices.append(device)
+                DEVICE_MANAGER.add_device(device)
 
-        return devices
+        return DEVICE_MANAGER.devices
 
 
 DEVICE_MANAGER = DeviceManager()  # Global device manager
```

### Comparing `robothub_oak-1.1.1/src/robothub_oak/packets.py` & `robothub_oak-1.1.2/src/robothub_oak/packets.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.1/src/robothub_oak.egg-info/PKG-INFO` & `robothub_oak-1.1.2/src/robothub_oak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub-oak
-Version: 1.1.1
+Version: 1.1.2
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.1.1/src/robothub_oak.egg-info/SOURCES.txt` & `robothub_oak-1.1.2/src/robothub_oak.egg-info/SOURCES.txt`

 * *Files identical despite different names*


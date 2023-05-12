# Comparing `tmp/neuromeka-clients-0.1.4.tar.gz` & `tmp/neuromeka-clients-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuromeka-clients-0.1.4.tar", last modified: Fri Apr 21 04:20:16 2023, max compression
+gzip compressed data, was "neuromeka-clients-0.1.5.tar", last modified: Fri May 12 07:39:29 2023, max compression
```

## Comparing `neuromeka-clients-0.1.4.tar` & `neuromeka-clients-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/
--rw-rw-rw-   0        0        0     1076 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2168 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.105648 neuromeka-clients-0.1.4/neuromeka/
--rw-rw-rw-   0        0        0      148 2023-04-18 02:59:59.000000 neuromeka-clients-0.1.4/neuromeka/__init__.py
--rw-rw-rw-   0        0        0     7442 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/ecat.py
--rw-rw-rw-   0        0        0    14598 2023-04-18 04:44:44.000000 neuromeka-clients-0.1.4/neuromeka/eye.py
--rw-rw-rw-   0        0        0    10651 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/indy.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.115649 neuromeka-clients-0.1.4/neuromeka/indy_dcp/
--rw-rw-rw-   0        0        0        0 2020-01-22 08:47:24.000000 neuromeka-clients-0.1.4/neuromeka/indy_dcp/__init__.py
--rw-rw-rw-   0        0        0    21703 2020-04-14 06:11:08.000000 neuromeka-clients-0.1.4/neuromeka/indy_dcp/indy_program_maker.py
--rw-rw-rw-   0        0        0    61482 2020-07-10 04:18:53.000000 neuromeka-clients-0.1.4/neuromeka/indy_dcp/indydcp_client.py
--rw-rw-rw-   0        0        0     7436 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/neuromeka/moby.py
--rw-rw-rw-   0        0        0     3379 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/motor.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.225648 neuromeka-clients-0.1.4/neuromeka/proto/
--rw-rw-rw-   0        0        0    65863 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2.py
--rw-rw-rw-   0        0        0    61370 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0     5567 2023-04-18 02:59:14.000000 neuromeka-clients-0.1.4/neuromeka/proto/EyeTask_pb2.py
--rw-rw-rw-   0        0        0     6780 2023-04-18 02:59:14.000000 neuromeka-clients-0.1.4/neuromeka/proto/EyeTask_pb2_grpc.py
--rw-rw-rw-   0        0        0    61466 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2.py
--rw-rw-rw-   0        0        0   128168 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2_grpc.py
--rw-rw-rw-   0        0        0    74574 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2.py
--rw-rw-rw-   0        0        0    52785 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0    41733 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2.py
--rw-rw-rw-   0        0        0    39460 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0        0 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/__init__.py
--rw-rw-rw-   0        0        0      519 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/grpc_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/
--rw-rw-rw-   0        0        0     2168 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      930 2023-04-21 04:20:16.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-04-21 04:20:07.000000 neuromeka-clients-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:39:29.415920 neuromeka-clients-0.1.5/
+-rw-rw-rw-   0        0        0     1076 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2316 2023-05-12 07:39:29.415920 neuromeka-clients-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 07:39:29.347620 neuromeka-clients-0.1.5/neuromeka/
+-rw-rw-rw-   0        0        0      246 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/__init__.py
+-rw-rw-rw-   0        0        0     7442 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/ecat.py
+-rw-rw-rw-   0        0        0    14598 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/eye.py
+-rw-rw-rw-   0        0        0    10651 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/indy.py
+-rw-rw-rw-   0        0        0    40863 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/indy_client3.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:39:29.347620 neuromeka-clients-0.1.5/neuromeka/indy_dcp/
+-rw-rw-rw-   0        0        0        0 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/indy_dcp/__init__.py
+-rw-rw-rw-   0        0        0    21703 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/indy_dcp/indy_program_maker.py
+-rw-rw-rw-   0        0        0    61482 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/indy_dcp/indydcp_client.py
+-rw-rw-rw-   0        0        0     7436 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/moby.py
+-rw-rw-rw-   0        0        0     3379 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/motor.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:39:29.402824 neuromeka-clients-0.1.5/neuromeka/proto/
+-rw-rw-rw-   0        0        0    65863 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/EtherCATCommgRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    61370 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5567 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/EyeTask_pb2.py
+-rw-rw-rw-   0        0        0     6780 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/EyeTask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    61466 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/IndygRPCTask_pb2.py
+-rw-rw-rw-   0        0        0   128168 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/IndygRPCTask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    74574 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/MobygRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    52785 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/MobygRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0    41733 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/MotorControlgRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    39460 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/__init__.py
+-rw-rw-rw-   0        0        0   333650 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/control_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/control_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12892 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/control_pb2.py
+-rw-rw-rw-   0        0        0   139890 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/control_pb2_grpc.py
+-rw-rw-rw-   0        0        0      519 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/grpc_wrapper.py
+-rw-rw-rw-   0        0        0    73456 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/shared_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.5/neuromeka/proto/shared_msgs_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:39:29.413810 neuromeka-clients-0.1.5/neuromeka_clients.egg-info/
+-rw-rw-rw-   0        0        0     2316 2023-05-12 07:39:29.000000 neuromeka-clients-0.1.5/neuromeka_clients.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1175 2023-05-12 07:39:29.000000 neuromeka-clients-0.1.5/neuromeka_clients.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:39:29.000000 neuromeka-clients-0.1.5/neuromeka_clients.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-12 07:39:29.000000 neuromeka-clients-0.1.5/neuromeka_clients.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 07:39:29.000000 neuromeka-clients-0.1.5/neuromeka_clients.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 07:39:29.415920 neuromeka-clients-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2023-05-12 07:39:17.000000 neuromeka-clients-0.1.5/setup.py
```

### Comparing `neuromeka-clients-0.1.4/LICENSE` & `neuromeka-clients-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/PKG-INFO` & `neuromeka-clients-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromeka-clients
-Version: 0.1.4
+Version: 0.1.5
 Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Neuromeka Clients
+![PyPI](https://img.shields.io/pypi/v/neuromeka-clients)
 
 This package provides client protocols for users to interact with Neuromeka's products, including Indy, Moby, Ecat, and Motor.
 
 ## Installation
 
 You can install the package from PyPI:
 
@@ -30,26 +31,28 @@
 pip install neuromeka-clients
 ```
 
 ## Usage
 The package contatins the following client classes:
 
 * IndyClient in indy.py
+* IndyClient3 in indy_client3.py
 * MobyClient in moby.py
 * EcatClient in ecat.py
 * MotorClient in motor.py
 
 To use a client class, simply import it and create an instance:
 
 ```python
-from neuromeka import EcatClient, MobyClient, IndyClient, MotorClient
+from neuromeka import EcatClient, MobyClient, IndyClient, IndyClient3, MotorClient
 
 ecat = EcatClient("192.168.214.20")
-moby = IndyClient("192.168.214.20")
+moby = MobyClient("192.168.214.20")
 indy = IndyClient("192.168.0.11")
+indyclient3 = IndyClient3("192.168.0.11")
 motor = MotorClient("192.168.0.20")
 ```
 
 Replace EcatClient with the desired client class and the IP address with the appropriate address for your device.
 
 ## Dependencies
 This package requires the following dependencies:
```

### Comparing `neuromeka-clients-0.1.4/README.md` & `neuromeka-clients-0.1.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Neuromeka Clients
+![PyPI](https://img.shields.io/pypi/v/neuromeka-clients)
 
 This package provides client protocols for users to interact with Neuromeka's products, including Indy, Moby, Ecat, and Motor.
 
 ## Installation
 
 You can install the package from PyPI:
 
@@ -10,26 +11,28 @@
 pip install neuromeka-clients
 ```
 
 ## Usage
 The package contatins the following client classes:
 
 * IndyClient in indy.py
+* IndyClient3 in indy_client3.py
 * MobyClient in moby.py
 * EcatClient in ecat.py
 * MotorClient in motor.py
 
 To use a client class, simply import it and create an instance:
 
 ```python
-from neuromeka import EcatClient, MobyClient, IndyClient, MotorClient
+from neuromeka import EcatClient, MobyClient, IndyClient, IndyClient3, MotorClient
 
 ecat = EcatClient("192.168.214.20")
-moby = IndyClient("192.168.214.20")
+moby = MobyClient("192.168.214.20")
 indy = IndyClient("192.168.0.11")
+indyclient3 = IndyClient3("192.168.0.11")
 motor = MotorClient("192.168.0.20")
 ```
 
 Replace EcatClient with the desired client class and the IP address with the appropriate address for your device.
 
 ## Dependencies
 This package requires the following dependencies:
```

### Comparing `neuromeka-clients-0.1.4/neuromeka/ecat.py` & `neuromeka-clients-0.1.5/neuromeka/ecat.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/eye.py` & `neuromeka-clients-0.1.5/neuromeka/eye.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/indy.py` & `neuromeka-clients-0.1.5/neuromeka/indy.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/indy_dcp/indy_program_maker.py` & `neuromeka-clients-0.1.5/neuromeka/indy_dcp/indy_program_maker.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/indy_dcp/indydcp_client.py` & `neuromeka-clients-0.1.5/neuromeka/indy_dcp/indydcp_client.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/moby.py` & `neuromeka-clients-0.1.5/neuromeka/moby.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/motor.py` & `neuromeka-clients-0.1.5/neuromeka/motor.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2.py` & `neuromeka-clients-0.1.5/neuromeka/proto/EtherCATCommgRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.5/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/EyeTask_pb2.py` & `neuromeka-clients-0.1.5/neuromeka/proto/EyeTask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/EyeTask_pb2_grpc.py` & `neuromeka-clients-0.1.5/neuromeka/proto/EyeTask_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2.py` & `neuromeka-clients-0.1.5/neuromeka/proto/IndygRPCTask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2_grpc.py` & `neuromeka-clients-0.1.5/neuromeka/proto/IndygRPCTask_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2.py` & `neuromeka-clients-0.1.5/neuromeka/proto/MobygRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.5/neuromeka/proto/MobygRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2.py` & `neuromeka-clients-0.1.5/neuromeka/proto/MotorControlgRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.5/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka/proto/grpc_wrapper.py` & `neuromeka-clients-0.1.5/neuromeka/proto/grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.4/neuromeka_clients.egg-info/PKG-INFO` & `neuromeka-clients-0.1.5/neuromeka_clients.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromeka-clients
-Version: 0.1.4
+Version: 0.1.5
 Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Neuromeka Clients
+![PyPI](https://img.shields.io/pypi/v/neuromeka-clients)
 
 This package provides client protocols for users to interact with Neuromeka's products, including Indy, Moby, Ecat, and Motor.
 
 ## Installation
 
 You can install the package from PyPI:
 
@@ -30,26 +31,28 @@
 pip install neuromeka-clients
 ```
 
 ## Usage
 The package contatins the following client classes:
 
 * IndyClient in indy.py
+* IndyClient3 in indy_client3.py
 * MobyClient in moby.py
 * EcatClient in ecat.py
 * MotorClient in motor.py
 
 To use a client class, simply import it and create an instance:
 
 ```python
-from neuromeka import EcatClient, MobyClient, IndyClient, MotorClient
+from neuromeka import EcatClient, MobyClient, IndyClient, IndyClient3, MotorClient
 
 ecat = EcatClient("192.168.214.20")
-moby = IndyClient("192.168.214.20")
+moby = MobyClient("192.168.214.20")
 indy = IndyClient("192.168.0.11")
+indyclient3 = IndyClient3("192.168.0.11")
 motor = MotorClient("192.168.0.20")
 ```
 
 Replace EcatClient with the desired client class and the IP address with the appropriate address for your device.
 
 ## Dependencies
 This package requires the following dependencies:
```

### Comparing `neuromeka-clients-0.1.4/neuromeka_clients.egg-info/SOURCES.txt` & `neuromeka-clients-0.1.5/neuromeka_clients.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 neuromeka/__init__.py
 neuromeka/ecat.py
 neuromeka/eye.py
 neuromeka/indy.py
+neuromeka/indy_client3.py
 neuromeka/moby.py
 neuromeka/motor.py
 neuromeka/indy_dcp/__init__.py
 neuromeka/indy_dcp/indy_program_maker.py
 neuromeka/indy_dcp/indydcp_client.py
 neuromeka/proto/EtherCATCommgRPCServer_pb2.py
 neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
@@ -17,13 +18,19 @@
 neuromeka/proto/IndygRPCTask_pb2.py
 neuromeka/proto/IndygRPCTask_pb2_grpc.py
 neuromeka/proto/MobygRPCServer_pb2.py
 neuromeka/proto/MobygRPCServer_pb2_grpc.py
 neuromeka/proto/MotorControlgRPCServer_pb2.py
 neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
 neuromeka/proto/__init__.py
+neuromeka/proto/control_msgs_pb2.py
+neuromeka/proto/control_msgs_pb2_grpc.py
+neuromeka/proto/control_pb2.py
+neuromeka/proto/control_pb2_grpc.py
 neuromeka/proto/grpc_wrapper.py
+neuromeka/proto/shared_msgs_pb2.py
+neuromeka/proto/shared_msgs_pb2_grpc.py
 neuromeka_clients.egg-info/PKG-INFO
 neuromeka_clients.egg-info/SOURCES.txt
 neuromeka_clients.egg-info/dependency_links.txt
 neuromeka_clients.egg-info/requires.txt
 neuromeka_clients.egg-info/top_level.txt
```

### Comparing `neuromeka-clients-0.1.4/setup.py` & `neuromeka-clients-0.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="neuromeka-clients",
-    version="0.1.4",
+    version="0.1.5",
     author="Neuromeka",
     author_email="youngjin.heo@neuromeka.com",
     description="Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neuromeka-robotics/neuromeka-clients",
     packages=find_packages(),
```


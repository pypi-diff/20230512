# Comparing `tmp/vive-tracker-apiserver-0.0.3.tar.gz` & `tmp/vive-tracker-apiserver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vive-tracker-apiserver/vive-tracker-apiserver/dist/.tmp-751skjc5/vive-tracker-apiserver-0.0.3.tar", last modified: Thu May 11 09:36:49 2023, max compression
+gzip compressed data, was "/home/runner/work/vive-tracker-apiserver/vive-tracker-apiserver/dist/.tmp-va3axard/vive-tracker-apiserver-0.0.4.tar", last modified: Fri May 12 11:11:09 2023, max compression
```

## Comparing `vive-tracker-apiserver-0.0.3.tar` & `vive-tracker-apiserver-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/tests/test_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/test_visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/common/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/grpc/tracker_packet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/vr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:32.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/vr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 09:36:49.000000 vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/tests/test_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/test_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/common/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/grpc/tracker_packet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/vr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:10:52.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/vr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 11:11:09.000000 vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/top_level.txt
```

### Comparing `vive-tracker-apiserver-0.0.3/PKG-INFO` & `vive-tracker-apiserver-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vive-tracker-apiserver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vive Tracker APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Vive Tracker APIServer
```

### Comparing `vive-tracker-apiserver-0.0.3/README.md` & `vive-tracker-apiserver-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/setup.py` & `vive-tracker-apiserver-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./vive_tracker_apiserver.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="vive-tracker-apiserver",
-    version="0.0.3",
+    version="0.0.4",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="Vive Tracker APIServer",
     packages=find_packages() + ["vive_tracker_apiserver.third_party.triad_openvr." + pkg for pkg in find_packages('vive_tracker_apiserver.third_party.triad_openvr')],
     python_requires=">=3.7",
     install_requires=requires,
     long_description=open('README.md', encoding='utf-8').read(),
```

### Comparing `vive-tracker-apiserver-0.0.3/tests/test_minimal.py` & `vive-tracker-apiserver-0.0.4/tests/test_minimal.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/tests/test_tracker.py` & `vive-tracker-apiserver-0.0.4/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/__main__.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/__main__.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/app.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/app.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/main.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/main.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/apiserver/server.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/apiserver/server.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/client/Client.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/client/Client.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/configure.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/configure.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/test_server.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/test_server.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/cmd/test_visualize.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/cmd/test_visualize.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/common/Config.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/common/Config.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/grpc/tracker_packet_pb2.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/grpc/tracker_packet_pb2.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/PKG-INFO` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vive-tracker-apiserver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vive Tracker APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Vive Tracker APIServer
```

### Comparing `vive-tracker-apiserver-0.0.3/vive_tracker_apiserver.egg-info/SOURCES.txt` & `vive-tracker-apiserver-0.0.4/vive_tracker_apiserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


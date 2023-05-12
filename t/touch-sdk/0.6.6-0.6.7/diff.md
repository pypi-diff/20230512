# Comparing `tmp/touch_sdk-0.6.6.tar.gz` & `tmp/touch_sdk-0.6.7.tar.gz`

## Comparing `touch_sdk-0.6.6.tar` & `touch_sdk-0.6.7.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.DS_Store
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.gitlab-ci.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.pylintrc
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/version.sh
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/basic.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/basic_threaded.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/custom_data.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/magnetometer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/osc.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/plotter.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/pressure.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/raycasting.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/sensors.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/basic.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/pressure.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/gatt_scanner.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/uuids.py
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/watch.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/watch_connector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/vec_pb2.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_input_pb2.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_output_pb2.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.gitignore
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/LICENSE
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/.pylintrc
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/version.sh
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/basic.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/basic_threaded.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/custom_data.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/magnetometer.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/osc.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/plotter.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/pressure.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/raycasting.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/examples/sensors.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/basic.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/pressure.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/gatt_scanner.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/uuids.py
+-rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/watch.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/watch_connector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/vec_pb2.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_input_pb2.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_output_pb2.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/.gitignore
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 touch_sdk-0.6.7/PKG-INFO
```

### Comparing `touch_sdk-0.6.6/examples/basic.py` & `touch_sdk-0.6.7/examples/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/examples/basic_threaded.py` & `touch_sdk-0.6.7/examples/basic_threaded.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/examples/magnetometer.py` & `touch_sdk-0.6.7/examples/magnetometer.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/examples/plotter.py` & `touch_sdk-0.6.7/examples/plotter.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/examples/raycasting.py` & `touch_sdk-0.6.7/examples/raycasting.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/examples/sensors.py` & `touch_sdk-0.6.7/examples/sensors.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/basic.py` & `touch_sdk-0.6.7/src/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/gatt_scanner.py` & `touch_sdk-0.6.7/src/touch_sdk/gatt_scanner.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/utils.py` & `touch_sdk-0.6.7/src/touch_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/watch.py` & `touch_sdk-0.6.7/src/touch_sdk/watch.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/watch_connector.py` & `touch_sdk-0.6.7/src/touch_sdk/watch_connector.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/protobuf/vec_pb2.py` & `touch_sdk-0.6.7/src/touch_sdk/protobuf/vec_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_input_pb2.py` & `touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_input_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_output_pb2.py` & `touch_sdk-0.6.7/src/touch_sdk/protobuf/watch_output_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.6/LICENSE` & `touch_sdk-0.6.7/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ISC License
 
-Copyright (c) 2022 Port 6 Oy
+Copyright (c) 2022–2023 Doublepoint
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `touch_sdk-0.6.6/README.md` & `touch_sdk-0.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Touch SDK py
 
 ![PyPI](https://img.shields.io/pypi/v/touch-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/touch-sdk)
 ![PyPI - License](https://img.shields.io/pypi/l/touch-sdk)
 ![Discord](https://img.shields.io/discord/869474617729875998)
 
-Connects to Port 6 Touch SDK compatible Bluetooth devices – like [this Wear OS app](https://play.google.com/store/apps/details?id=io.port6.watchbridge).
+Connects to Doublepoint Touch SDK compatible Bluetooth devices – like [this Wear OS app](https://play.google.com/store/apps/details?id=io.port6.watchbridge).
 
 There is also a [web SDK](https://www.npmjs.com/package/touch-sdk) and a [Unity SDK](https://openupm.com/packages/io.port6.sdk/).
 
-See [port6.io/sdk](https://port6.io/sdk/) for more info.
+See [doublepoint.com/product](https://doublepoint.com/product) for more info.
 
 ## Installation
 
 ```sh
 pip install touch-sdk
 ```
```

### Comparing `touch_sdk-0.6.6/pyproject.toml` & `touch_sdk-0.6.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "touch-sdk"
-version = "0.6.6"
-description = "Port 6 Touch SDK"
+version = "0.6.7"
+description = "Doublepoint Touch SDK"
 license = "ISC"
 authors = [
-    { name="Port 6", email="developer@port6.io" },
+    { name="Doublepoint", email="developer@doublepoint.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["bluetooth"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -27,9 +27,9 @@
 dependencies = [
     "bleak~=0.20.1",
     "protobuf~=3.20.0",
     "asyncio-atexit~=1.0.1",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/port6io/touch-sdk-py#readme"
-"Bug Tracker" = "https://github.com/port6io/touch-sdk-py/issues"
+"Homepage" = "https://github.com/doublepointlab/touch-sdk-py#readme"
+"Bug Tracker" = "https://github.com/doublepointlab/touch-sdk-py/issues"
```

### Comparing `touch_sdk-0.6.6/PKG-INFO` & `touch_sdk-0.6.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: touch-sdk
-Version: 0.6.6
-Summary: Port 6 Touch SDK
-Project-URL: Homepage, https://github.com/port6io/touch-sdk-py#readme
-Project-URL: Bug Tracker, https://github.com/port6io/touch-sdk-py/issues
-Author-email: Port 6 <developer@port6.io>
+Version: 0.6.7
+Summary: Doublepoint Touch SDK
+Project-URL: Homepage, https://github.com/doublepointlab/touch-sdk-py#readme
+Project-URL: Bug Tracker, https://github.com/doublepointlab/touch-sdk-py/issues
+Author-email: Doublepoint <developer@doublepoint.com>
 License-Expression: ISC
 License-File: LICENSE
 Keywords: bluetooth
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: Android
@@ -26,19 +26,19 @@
 # Touch SDK py
 
 ![PyPI](https://img.shields.io/pypi/v/touch-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/touch-sdk)
 ![PyPI - License](https://img.shields.io/pypi/l/touch-sdk)
 ![Discord](https://img.shields.io/discord/869474617729875998)
 
-Connects to Port 6 Touch SDK compatible Bluetooth devices – like [this Wear OS app](https://play.google.com/store/apps/details?id=io.port6.watchbridge).
+Connects to Doublepoint Touch SDK compatible Bluetooth devices – like [this Wear OS app](https://play.google.com/store/apps/details?id=io.port6.watchbridge).
 
 There is also a [web SDK](https://www.npmjs.com/package/touch-sdk) and a [Unity SDK](https://openupm.com/packages/io.port6.sdk/).
 
-See [port6.io/sdk](https://port6.io/sdk/) for more info.
+See [doublepoint.com/product](https://doublepoint.com/product) for more info.
 
 ## Installation
 
 ```sh
 pip install touch-sdk
 ```
```


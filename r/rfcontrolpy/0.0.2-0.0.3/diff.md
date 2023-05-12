# Comparing `tmp/rfcontrolpy-0.0.2.tar.gz` & `tmp/rfcontrolpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcontrolpy-0.0.2.tar", last modified: Wed Jan 18 02:13:18 2023, max compression
+gzip compressed data, was "rfcontrolpy-0.0.3.tar", last modified: Fri May 12 14:57:19 2023, max compression
```

## Comparing `rfcontrolpy-0.0.2.tar` & `rfcontrolpy-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:13:18.659487 rfcontrolpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-18 02:13:18.659487 rfcontrolpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:13:18.655487 rfcontrolpy-0.0.2/rfcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:13:18.659487 rfcontrolpy-0.0.2/rfcontrol/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/dimmer1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/dimmer2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/generic2.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/pir3.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/skelleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch25.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/switch8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/weather19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-18 02:13:08.000000 rfcontrolpy-0.0.2/rfcontrol/protocols/weather7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 02:13:18.659487 rfcontrolpy-0.0.2/rfcontrolpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-18 02:13:18.000000 rfcontrolpy-0.0.2/rfcontrolpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-18 02:13:18.000000 rfcontrolpy-0.0.2/rfcontrolpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 02:13:18.000000 rfcontrolpy-0.0.2/rfcontrolpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-18 02:13:18.000000 rfcontrolpy-0.0.2/rfcontrolpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 02:13:18.659487 rfcontrolpy-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.435018 rfcontrolpy-0.0.3/rfcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/rfcontrol/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/generic2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/pir3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/weather19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/weather7.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    97702 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/tests/test_helpers.py
```

### Comparing `rfcontrolpy-0.0.2/LICENSE` & `rfcontrolpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/pyproject.toml` & `rfcontrolpy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rfcontrolpy"
-version = "0.0.2"
+version = "0.0.3"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `rfcontrolpy-0.0.2/rfcontrol/helpers.py` & `rfcontrolpy-0.0.3/rfcontrol/helpers.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/dimmer1.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer1.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/dimmer2.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/generic.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/generic.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/generic2.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/generic2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/pir3.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/pir3.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/skelleton.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/_skeleton.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""
+Use this skeleton protocol to implement new protocols
+"""
 import logging
 
 from rfcontrol.helpers import binary2pulses, pulses2binary
 from rfcontrol.protocols import RFControlProtocolTypes
 
 logger = logging.getLogger(__name__)
 
 # Mapping for decoding.
 pulses2binary_mapping = []
 
 # Mapping for encoding
 binary2pulses_mapping = {}
 
-name = "dimmer1"
+name = "skeleton"
 type = RFControlProtocolTypes.DIMMER
 brands = []
 pulse_lengths = []
 pulse_count = 0
 
 
 def decode(pulses):
```

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch1.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch1.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch10.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch10.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch11.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch11.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch2.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch25.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch25.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch3.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch3.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch4.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch4.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch5.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch5.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch6.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch6.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch7.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch7.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/switch8.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/switch8.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/weather19.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/weather19.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrol/protocols/weather7.py` & `rfcontrolpy-0.0.3/rfcontrol/protocols/weather7.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.2/rfcontrolpy.egg-info/SOURCES.txt` & `rfcontrolpy-0.0.3/rfcontrolpy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE
+MANIFEST.in
+README.md
 pyproject.toml
 rfcontrol/__init__.py
 rfcontrol/controller.py
 rfcontrol/helpers.py
+rfcontrol/py.typed
 rfcontrol/protocols/__init__.py
+rfcontrol/protocols/_skeleton.py
 rfcontrol/protocols/dimmer1.py
 rfcontrol/protocols/dimmer2.py
 rfcontrol/protocols/generic.py
 rfcontrol/protocols/generic2.py
 rfcontrol/protocols/pir3.py
-rfcontrol/protocols/skelleton.py
 rfcontrol/protocols/switch1.py
 rfcontrol/protocols/switch10.py
 rfcontrol/protocols/switch11.py
 rfcontrol/protocols/switch2.py
 rfcontrol/protocols/switch25.py
 rfcontrol/protocols/switch3.py
 rfcontrol/protocols/switch4.py
@@ -22,8 +25,10 @@
 rfcontrol/protocols/switch7.py
 rfcontrol/protocols/switch8.py
 rfcontrol/protocols/weather19.py
 rfcontrol/protocols/weather7.py
 rfcontrolpy.egg-info/PKG-INFO
 rfcontrolpy.egg-info/SOURCES.txt
 rfcontrolpy.egg-info/dependency_links.txt
-rfcontrolpy.egg-info/top_level.txt
+rfcontrolpy.egg-info/top_level.txt
+tests/test_controller.py
+tests/test_helpers.py
```


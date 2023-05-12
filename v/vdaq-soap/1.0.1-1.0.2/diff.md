# Comparing `tmp/vdaq_soap-1.0.1.tar.gz` & `tmp/vdaq_soap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdaq_soap-1.0.1.tar", last modified: Fri May 12 07:06:20 2023, max compression
+gzip compressed data, was "vdaq_soap-1.0.2.tar", last modified: Fri May 12 07:49:51 2023, max compression
```

## Comparing `vdaq_soap-1.0.1.tar` & `vdaq_soap-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 07:06:20.287526 vdaq_soap-1.0.1/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-05-12 07:06:20.287025 vdaq_soap-1.0.1/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.1/README.md
--rw-r--r--   0 lacasta    (503) staff       (20)      951 2023-05-12 06:54:51.000000 vdaq_soap-1.0.1/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-12 07:06:20.287650 vdaq_soap-1.0.1/setup.cfg
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 07:06:20.284011 vdaq_soap-1.0.1/vdaq_soap/
--rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-05-12 06:54:51.000000 vdaq_soap-1.0.1/vdaq_soap/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.1/vdaq_soap/analyzeHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.1/vdaq_soap/analyzeMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.1/vdaq_soap/data_utils.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    25156 2023-05-12 06:55:29.000000 vdaq_soap-1.0.1/vdaq_soap/soapCheckMadDaq.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2980 2023-05-12 06:51:08.000000 vdaq_soap-1.0.1/vdaq_soap/soapHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3073 2023-05-12 06:55:33.000000 vdaq_soap-1.0.1/vdaq_soap/soapMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3099 2023-05-12 07:05:33.000000 vdaq_soap-1.0.1/vdaq_soap/soapTestChannel.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 07:06:20.286606 vdaq_soap-1.0.1/vdaq_soap.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-05-12 07:06:20.000000 vdaq_soap-1.0.1/vdaq_soap.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-05-12 07:06:20.000000 vdaq_soap-1.0.1/vdaq_soap.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-12 07:06:20.000000 vdaq_soap-1.0.1/vdaq_soap.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      258 2023-05-12 07:06:20.000000 vdaq_soap-1.0.1/vdaq_soap.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-05-12 07:06:20.000000 vdaq_soap-1.0.1/vdaq_soap.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-12 07:06:20.000000 vdaq_soap-1.0.1/vdaq_soap.egg-info/top_level.txt
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 07:49:51.985803 vdaq_soap-1.0.2/
+-rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-05-12 07:49:51.985341 vdaq_soap-1.0.2/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.2/README.md
+-rw-r--r--   0 lacasta    (503) staff       (20)      951 2023-05-12 07:48:01.000000 vdaq_soap-1.0.2/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-12 07:49:51.985946 vdaq_soap-1.0.2/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 07:49:51.981998 vdaq_soap-1.0.2/vdaq_soap/
+-rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-05-12 07:48:01.000000 vdaq_soap-1.0.2/vdaq_soap/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.2/vdaq_soap/analyzeHoldDelay.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.2/vdaq_soap/analyzeMbias.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.2/vdaq_soap/data_utils.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    25156 2023-05-12 06:55:29.000000 vdaq_soap-1.0.2/vdaq_soap/soapCheckMadDaq.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2980 2023-05-12 06:51:08.000000 vdaq_soap-1.0.2/vdaq_soap/soapHoldDelay.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3073 2023-05-12 06:55:33.000000 vdaq_soap-1.0.2/vdaq_soap/soapMbias.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3105 2023-05-12 07:44:42.000000 vdaq_soap-1.0.2/vdaq_soap/soapTestChannel.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-12 07:49:51.984559 vdaq_soap-1.0.2/vdaq_soap.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-05-12 07:49:51.000000 vdaq_soap-1.0.2/vdaq_soap.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-05-12 07:49:51.000000 vdaq_soap-1.0.2/vdaq_soap.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-12 07:49:51.000000 vdaq_soap-1.0.2/vdaq_soap.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      258 2023-05-12 07:49:51.000000 vdaq_soap-1.0.2/vdaq_soap.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-05-12 07:49:51.000000 vdaq_soap-1.0.2/vdaq_soap.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-12 07:49:51.000000 vdaq_soap-1.0.2/vdaq_soap.egg-info/top_level.txt
```

### Comparing `vdaq_soap-1.0.1/PKG-INFO` & `vdaq_soap-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdaq_soap
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of python scripts to control VDaq.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `vdaq_soap-1.0.1/pyproject.toml` & `vdaq_soap-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vdaq_soap"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to control VDaq."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vdaq_soap-1.0.1/vdaq_soap/analyzeHoldDelay.py` & `vdaq_soap-1.0.2/vdaq_soap/analyzeHoldDelay.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.1/vdaq_soap/analyzeMbias.py` & `vdaq_soap-1.0.2/vdaq_soap/analyzeMbias.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.1/vdaq_soap/data_utils.py` & `vdaq_soap-1.0.2/vdaq_soap/data_utils.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.1/vdaq_soap/soapCheckMadDaq.py` & `vdaq_soap-1.0.2/vdaq_soap/soapCheckMadDaq.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.1/vdaq_soap/soapHoldDelay.py` & `vdaq_soap-1.0.2/vdaq_soap/soapHoldDelay.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.1/vdaq_soap/soapMbias.py` & `vdaq_soap-1.0.2/vdaq_soap/soapMbias.py`

 * *Files identical despite different names*

### Comparing `vdaq_soap-1.0.1/vdaq_soap/soapTestChannel.py` & `vdaq_soap-1.0.2/vdaq_soap/soapTestChannel.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,16 @@
                         type=int, help="The soap port")
     parser.add_argument("--mid", dest="mid", default="11",
                         type=str, help="The slot ID")
     parser.add_argument("--channel", dest="channel", default=32,
                         type=int, help="The test channel")
     parser.add_argument("--mbias", dest="mbias", default=300,
                         type=int, help="Chip Main bias")
-    parser.add_argument("--hold_delay", dest="mbias", default=175,
-                        type=int, help="Chip Main bias")
+    parser.add_argument("--hold_delay", dest="hold_delay", default=175,
+                        type=int, help="Chip hold delay")
     parser.add_argument("--polarity", dest="polarity", default=0,
                         type=int, help="Signal polarity")
     parser.add_argument("--nsec", dest="nsec", default=10,
                         type=int, help="Chip Main bias")
     parser.add_argument("--thrs", default=0.0, type=float,
                         help="Min E to show in histogram")
```

### Comparing `vdaq_soap-1.0.1/vdaq_soap.egg-info/PKG-INFO` & `vdaq_soap-1.0.2/vdaq_soap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdaq-soap
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of python scripts to control VDaq.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```


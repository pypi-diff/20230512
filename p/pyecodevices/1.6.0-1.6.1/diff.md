# Comparing `tmp/pyecodevices-1.6.0.tar.gz` & `tmp/pyecodevices-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecodevices-1.6.0.tar", last modified: Mon Apr 24 21:11:23 2023, max compression
+gzip compressed data, was "pyecodevices-1.6.1.tar", last modified: Fri May 12 07:13:42 2023, max compression
```

## Comparing `pyecodevices-1.6.0.tar` & `pyecodevices-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2023-04-24 21:11:23.467012 pyecodevices-1.6.0/
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1065 2021-01-24 13:39:26.000000 pyecodevices-1.6.0/LICENSE
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1679 2023-04-24 21:11:23.463678 pyecodevices-1.6.0/PKG-INFO
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1248 2021-04-14 17:00:11.000000 pyecodevices-1.6.0/README.md
-drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2023-04-24 21:11:23.463678 pyecodevices-1.6.0/pyecodevices/
--rw-r--r--   0 matthieu  (1000) wheel      (998)     8098 2023-04-24 21:10:34.000000 pyecodevices-1.6.0/pyecodevices/__init__.py
-drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2023-04-24 21:11:23.463678 pyecodevices-1.6.0/pyecodevices.egg-info/
--rw-r--r--   0 matthieu  (1000) wheel      (998)     1679 2023-04-24 21:11:23.000000 pyecodevices-1.6.0/pyecodevices.egg-info/PKG-INFO
--rw-r--r--   0 matthieu  (1000) wheel      (998)      195 2023-04-24 21:11:23.000000 pyecodevices-1.6.0/pyecodevices.egg-info/SOURCES.txt
--rw-r--r--   0 matthieu  (1000) wheel      (998)        1 2023-04-24 21:11:23.000000 pyecodevices-1.6.0/pyecodevices.egg-info/dependency_links.txt
--rw-r--r--   0 matthieu  (1000) wheel      (998)       13 2023-04-24 21:11:23.000000 pyecodevices-1.6.0/pyecodevices.egg-info/top_level.txt
--rw-r--r--   0 matthieu  (1000) wheel      (998)       38 2023-04-24 21:11:23.467012 pyecodevices-1.6.0/setup.cfg
--rw-r--r--   0 matthieu  (1000) wheel      (998)      647 2023-04-24 21:10:48.000000 pyecodevices-1.6.0/setup.py
+drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2023-05-12 07:13:42.241255 pyecodevices-1.6.1/
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1065 2021-01-24 13:39:26.000000 pyecodevices-1.6.1/LICENSE
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1679 2023-05-12 07:13:42.241255 pyecodevices-1.6.1/PKG-INFO
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1248 2021-04-14 17:00:11.000000 pyecodevices-1.6.1/README.md
+drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2023-05-12 07:13:42.241255 pyecodevices-1.6.1/pyecodevices/
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     8121 2023-05-12 07:11:36.000000 pyecodevices-1.6.1/pyecodevices/__init__.py
+drwxr-xr-x   0 matthieu  (1000) wheel      (998)        0 2023-05-12 07:13:42.241255 pyecodevices-1.6.1/pyecodevices.egg-info/
+-rw-r--r--   0 matthieu  (1000) wheel      (998)     1679 2023-05-12 07:13:42.000000 pyecodevices-1.6.1/pyecodevices.egg-info/PKG-INFO
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      195 2023-05-12 07:13:42.000000 pyecodevices-1.6.1/pyecodevices.egg-info/SOURCES.txt
+-rw-r--r--   0 matthieu  (1000) wheel      (998)        1 2023-05-12 07:13:42.000000 pyecodevices-1.6.1/pyecodevices.egg-info/dependency_links.txt
+-rw-r--r--   0 matthieu  (1000) wheel      (998)       13 2023-05-12 07:13:42.000000 pyecodevices-1.6.1/pyecodevices.egg-info/top_level.txt
+-rw-r--r--   0 matthieu  (1000) wheel      (998)       38 2023-05-12 07:13:42.241255 pyecodevices-1.6.1/setup.cfg
+-rw-r--r--   0 matthieu  (1000) wheel      (998)      647 2023-05-12 07:11:48.000000 pyecodevices-1.6.1/setup.py
```

### Comparing `pyecodevices-1.6.0/LICENSE` & `pyecodevices-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecodevices-1.6.0/PKG-INFO` & `pyecodevices-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecodevices
-Version: 1.6.0
+Version: 1.6.1
 Summary: Get information from GCE Eco-Devices.
 Home-page: https://github.com/aohzan/pyecodevices
 Author: Aohzan
 Author-email: aohzan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyecodevices-1.6.0/README.md` & `pyecodevices-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyecodevices-1.6.0/pyecodevices/__init__.py` & `pyecodevices-1.6.1/pyecodevices/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if response.status == 401:
             raise EcoDevicesInvalidAuthError("Authentication failed with Eco-Devices.")
 
         if response.status:
             contents = await response.text()
             response.close()
             _LOGGER.debug("Data received from the Eco-Devices: %s", contents)
-            xml_content = xmltodict.parse(contents)
+            xml_content = xmltodict.parse(contents, encoding="iso-8859-1")
             if (data := xml_content.get("response")):
                 return data
             raise EcoDevicesCannotConnectError("Eco-Devices XML request error:", data)
 
     @property
     def host(self) -> str:
         """Return the hostname."""
```

### Comparing `pyecodevices-1.6.0/pyecodevices.egg-info/PKG-INFO` & `pyecodevices-1.6.1/pyecodevices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecodevices
-Version: 1.6.0
+Version: 1.6.1
 Summary: Get information from GCE Eco-Devices.
 Home-page: https://github.com/aohzan/pyecodevices
 Author: Aohzan
 Author-email: aohzan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyecodevices-1.6.0/setup.py` & `pyecodevices-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyecodevices",
-    version="1.6.0",
+    version="1.6.1",
     author="Aohzan",
     author_email="aohzan@gmail.com",
     description="Get information from GCE Eco-Devices.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aohzan/pyecodevices",
     packages=setuptools.find_packages(),
```


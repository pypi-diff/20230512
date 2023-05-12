# Comparing `tmp/mattlib-1.1.2.tar.gz` & `tmp/mattlib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattlib-1.1.2.tar", last modified: Thu May 11 14:17:08 2023, max compression
+gzip compressed data, was "mattlib-1.1.3.tar", last modified: Fri May 12 00:07:27 2023, max compression
```

## Comparing `mattlib-1.1.2.tar` & `mattlib-1.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:08.131341 mattlib-1.1.2/
--rwxrwxrwx   0 livia     (1000) livia     (1000)    35149 2023-03-10 11:27:09.000000 mattlib-1.1.2/COPYING
--rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-11 14:17:08.132850 mattlib-1.1.2/PKG-INFO
--rwxrwxrwx   0 livia     (1000) livia     (1000)      147 2023-03-10 11:27:09.000000 mattlib-1.1.2/README.md
--rwxrwxrwx   0 livia     (1000) livia     (1000)      104 2023-03-10 11:27:09.000000 mattlib-1.1.2/pyproject.toml
--rwxrwxrwx   0 livia     (1000) livia     (1000)      807 2023-05-11 14:17:08.151507 mattlib-1.1.2/setup.cfg
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:03.131439 mattlib-1.1.2/src/
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:03.719806 mattlib-1.1.2/src/mattlib/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      733 2023-03-10 11:27:09.000000 mattlib-1.1.2/src/mattlib/API_factory.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     3228 2023-05-11 14:13:56.000000 mattlib-1.1.2/src/mattlib/BaseAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      193 2023-03-10 11:27:09.000000 mattlib-1.1.2/src/mattlib/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:04.616818 mattlib-1.1.2/src/mattlib/adobe/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     3332 2023-03-10 11:27:09.000000 mattlib-1.1.2/src/mattlib/adobe/AdobeAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       30 2023-03-10 11:27:09.000000 mattlib-1.1.2/src/mattlib/adobe/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:05.018946 mattlib-1.1.2/src/mattlib/clockify/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      751 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/clockify/ClockifyAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       26 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/clockify/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:05.551358 mattlib-1.1.2/src/mattlib/fourmatters/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     8016 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/fourmatters/virtual_machine.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     2964 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/fourmatters/virtual_network.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:05.831430 mattlib-1.1.2/src/mattlib/gcp/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/gcp/PubSub.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       21 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/gcp/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:06.831213 mattlib-1.1.2/src/mattlib/google/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1116 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/google/BaseGoogleAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1061 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/google/GCPAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1175 2023-03-10 11:27:10.000000 mattlib-1.1.2/src/mattlib/google/GoogleWorkspaceAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/google/PubSub.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1483 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/google/SQL.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      750 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/google/Storage.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      139 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/google/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:07.391332 mattlib-1.1.2/src/mattlib/microsoft/
--rwxrwxrwx   0 livia     (1000) livia     (1000)    18681 2023-03-16 17:34:31.000000 mattlib-1.1.2/src/mattlib/microsoft/AzureAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     2022 2023-05-11 14:13:25.000000 mattlib-1.1.2/src/mattlib/microsoft/BaseMicrosoftAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)     5701 2023-05-11 14:14:16.000000 mattlib-1.1.2/src/mattlib/microsoft/GraphAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       61 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/microsoft/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:07.577501 mattlib-1.1.2/src/mattlib/network/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1373 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/network/HttpListener.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       39 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/network/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:07.737650 mattlib-1.1.2/src/mattlib/salesforce/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     6366 2023-05-11 14:13:25.000000 mattlib-1.1.2/src/mattlib/salesforce/SalesForceAPI.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       41 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/salesforce/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:07.922556 mattlib-1.1.2/src/mattlib/system/
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1370 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/system/Logger.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)       27 2023-03-10 11:27:11.000000 mattlib-1.1.2/src/mattlib/system/__init__.py
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:04.222727 mattlib-1.1.2/src/mattlib.egg-info/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-11 14:17:02.000000 mattlib-1.1.2/src/mattlib.egg-info/PKG-INFO
--rwxrwxrwx   0 livia     (1000) livia     (1000)     1173 2023-05-11 14:17:03.000000 mattlib-1.1.2/src/mattlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 livia     (1000) livia     (1000)        1 2023-05-11 14:17:02.000000 mattlib-1.1.2/src/mattlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 livia     (1000) livia     (1000)       91 2023-05-11 14:17:02.000000 mattlib-1.1.2/src/mattlib.egg-info/requires.txt
--rwxrwxrwx   0 livia     (1000) livia     (1000)        8 2023-05-11 14:17:02.000000 mattlib-1.1.2/src/mattlib.egg-info/top_level.txt
-drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 14:17:08.040564 mattlib-1.1.2/test/
--rwxrwxrwx   0 livia     (1000) livia     (1000)      628 2023-03-10 11:27:11.000000 mattlib-1.1.2/test/test_salesforce.py
--rwxrwxrwx   0 livia     (1000) livia     (1000)      766 2023-03-10 11:27:11.000000 mattlib-1.1.2/test/test_vm_size.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:27.880710 mattlib-1.1.3/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    35149 2023-03-10 11:27:09.000000 mattlib-1.1.3/COPYING
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-12 00:07:27.882719 mattlib-1.1.3/PKG-INFO
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      147 2023-03-10 11:27:09.000000 mattlib-1.1.3/README.md
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      104 2023-03-10 11:27:09.000000 mattlib-1.1.3/pyproject.toml
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      807 2023-05-12 00:07:27.897829 mattlib-1.1.3/setup.cfg
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:21.097315 mattlib-1.1.3/src/
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:21.932428 mattlib-1.1.3/src/mattlib/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      733 2023-03-10 11:27:09.000000 mattlib-1.1.3/src/mattlib/API_factory.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     3173 2023-05-12 00:03:57.000000 mattlib-1.1.3/src/mattlib/BaseAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      193 2023-03-10 11:27:09.000000 mattlib-1.1.3/src/mattlib/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:23.235701 mattlib-1.1.3/src/mattlib/adobe/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     3332 2023-03-10 11:27:09.000000 mattlib-1.1.3/src/mattlib/adobe/AdobeAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       30 2023-03-10 11:27:09.000000 mattlib-1.1.3/src/mattlib/adobe/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:23.817154 mattlib-1.1.3/src/mattlib/clockify/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      751 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/clockify/ClockifyAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       26 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/clockify/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:24.120436 mattlib-1.1.3/src/mattlib/fourmatters/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     8016 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/fourmatters/virtual_machine.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2964 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/fourmatters/virtual_network.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:24.622213 mattlib-1.1.3/src/mattlib/gcp/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/gcp/PubSub.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       21 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/gcp/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:26.566177 mattlib-1.1.3/src/mattlib/google/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1116 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/google/BaseGoogleAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1061 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/google/GCPAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1175 2023-03-10 11:27:10.000000 mattlib-1.1.3/src/mattlib/google/GoogleWorkspaceAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/google/PubSub.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1483 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/google/SQL.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      750 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/google/Storage.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      139 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/google/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:27.044764 mattlib-1.1.3/src/mattlib/microsoft/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    18681 2023-03-16 17:34:31.000000 mattlib-1.1.3/src/mattlib/microsoft/AzureAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2022 2023-05-11 14:13:25.000000 mattlib-1.1.3/src/mattlib/microsoft/BaseMicrosoftAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     5700 2023-05-11 22:56:46.000000 mattlib-1.1.3/src/mattlib/microsoft/GraphAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       61 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/microsoft/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:27.220041 mattlib-1.1.3/src/mattlib/network/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1373 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/network/HttpListener.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       39 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/network/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:27.416443 mattlib-1.1.3/src/mattlib/salesforce/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     6468 2023-05-11 22:54:37.000000 mattlib-1.1.3/src/mattlib/salesforce/SalesForceAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       41 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/salesforce/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:27.635389 mattlib-1.1.3/src/mattlib/system/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1370 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/system/Logger.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       27 2023-03-10 11:27:11.000000 mattlib-1.1.3/src/mattlib/system/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:22.838704 mattlib-1.1.3/src/mattlib.egg-info/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-12 00:07:20.000000 mattlib-1.1.3/src/mattlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1173 2023-05-12 00:07:21.000000 mattlib-1.1.3/src/mattlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)        1 2023-05-12 00:07:20.000000 mattlib-1.1.3/src/mattlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       91 2023-05-12 00:07:20.000000 mattlib-1.1.3/src/mattlib.egg-info/requires.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)        8 2023-05-12 00:07:20.000000 mattlib-1.1.3/src/mattlib.egg-info/top_level.txt
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-12 00:07:27.779643 mattlib-1.1.3/test/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      628 2023-03-10 11:27:11.000000 mattlib-1.1.3/test/test_salesforce.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      766 2023-03-10 11:27:11.000000 mattlib-1.1.3/test/test_vm_size.py
```

### Comparing `mattlib-1.1.2/COPYING` & `mattlib-1.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/PKG-INFO` & `mattlib-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.1.2
+Version: 1.1.3
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.1.2/setup.cfg` & `mattlib-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mattlib
-version = 1.1.2
+version = 1.1.3
 author = 4matt
 author_email = mattzero@4matt.com.br
 description = API data extraction and formatting utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://source.cloud.google.com/mtz-repos-global/mattlib
 classifiers =
```

### Comparing `mattlib-1.1.2/src/mattlib/API_factory.py` & `mattlib-1.1.3/src/mattlib/API_factory.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/BaseAPI.py` & `mattlib-1.1.3/src/mattlib/BaseAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,10 +99,9 @@
             return self.serialize_csv_list(data)
         elif input_format == 'csv':
             return data
 
     def serialize_csv_list(self, data: List[tuple]) -> str:
         serialized_list = ''
         for pair in data:
-            escaped_data = pair[1].replace('@','\#')
-            serialized_list += pair[0] + '@' + escaped_data + ';'
-        return serialized_list.strip(';')
+            serialized_list += pair[0] + '|#' + pair[1] + '|$'
+        return serialized_list.strip('|$')
```

### Comparing `mattlib-1.1.2/src/mattlib/adobe/AdobeAPI.py` & `mattlib-1.1.3/src/mattlib/adobe/AdobeAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/clockify/ClockifyAPI.py` & `mattlib-1.1.3/src/mattlib/clockify/ClockifyAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/fourmatters/virtual_machine.py` & `mattlib-1.1.3/src/mattlib/fourmatters/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/fourmatters/virtual_network.py` & `mattlib-1.1.3/src/mattlib/fourmatters/virtual_network.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/google/BaseGoogleAPI.py` & `mattlib-1.1.3/src/mattlib/google/BaseGoogleAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/google/GCPAPI.py` & `mattlib-1.1.3/src/mattlib/google/GCPAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/google/GoogleWorkspaceAPI.py` & `mattlib-1.1.3/src/mattlib/google/GoogleWorkspaceAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/google/SQL.py` & `mattlib-1.1.3/src/mattlib/google/SQL.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/google/Storage.py` & `mattlib-1.1.3/src/mattlib/google/Storage.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/microsoft/AzureAPI.py` & `mattlib-1.1.3/src/mattlib/microsoft/AzureAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/microsoft/BaseMicrosoftAPI.py` & `mattlib-1.1.3/src/mattlib/microsoft/BaseMicrosoftAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/microsoft/GraphAPI.py` & `mattlib-1.1.3/src/mattlib/microsoft/GraphAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                         'getOneDriveUsageAccountDetail',
                         'getOneDriveActivityUserDetail',
                         'getTeamsDeviceUsageUserDetail',
                         'getTeamsUserActivityUserDetail',
                         'getEmailActivityUserDetail',
                         'getEmailAppUsageUserDetail',
                         'getSharePointActivityUserDetail',
-                        'getSharePointSiteUsageDetail',
+                        'getSharePointSiteUsageDetail'
                     ],
                     paramsData=('period',7)) -> list:
         results = []
         supported_paramsExtract = [
             'getOneDriveUsageAccountDetail',
             'getOneDriveActivityUserDetail',
             'getTeamsDeviceUsageUserDetail',
```

### Comparing `mattlib-1.1.2/src/mattlib/network/HttpListener.py` & `mattlib-1.1.3/src/mattlib/network/HttpListener.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib/salesforce/SalesForceAPI.py` & `mattlib-1.1.3/src/mattlib/salesforce/SalesForceAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
     def user(self, fields=None):
         if not fields:
             fields = [
                 'Id', 'FirstName', 
                 'LastName', 'Username', 'Email',
                 'IsActive', 'LastLoginDate',
-                'UserType', 'ProfileId'
+                'UserType', 'ProfileId', 'Department', 'Division',
+                'EmployeeNumber', 'IsPartner', 'UserRoleId', 'CompanyName'
             ]
         fields = ',+'.join(fields)
         query = f'SELECT+{fields}+from+User'
         request_url = f'{self.url}/services/data/v53.0/query?q={query}'
         response = self.call_api(request_url)
         return response
```

### Comparing `mattlib-1.1.2/src/mattlib/system/Logger.py` & `mattlib-1.1.3/src/mattlib/system/Logger.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/src/mattlib.egg-info/PKG-INFO` & `mattlib-1.1.3/src/mattlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.1.2
+Version: 1.1.3
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.1.2/src/mattlib.egg-info/SOURCES.txt` & `mattlib-1.1.3/src/mattlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/test/test_salesforce.py` & `mattlib-1.1.3/test/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.2/test/test_vm_size.py` & `mattlib-1.1.3/test/test_vm_size.py`

 * *Files identical despite different names*


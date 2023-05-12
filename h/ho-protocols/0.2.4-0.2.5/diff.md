# Comparing `tmp/ho-protocols-0.2.4.tar.gz` & `tmp/ho-protocols-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ho-protocols-0.2.4.tar", last modified: Thu May  4 09:12:41 2023, max compression
+gzip compressed data, was "ho-protocols-0.2.5.tar", last modified: Fri May 12 09:49:39 2023, max compression
```

## Comparing `ho-protocols-0.2.4.tar` & `ho-protocols-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.4/LICENCE
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.4/README.md
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/setup.cfg
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.4/setup.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.340732 ho-protocols-0.2.4/src/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.344732 ho-protocols-0.2.4/src/ho_protocols/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.4/src/ho_protocols/__init__.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.348732 ho-protocols-0.2.4/src/ho_protocols/alert/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.4/src/ho_protocols/alert/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/alert/alert_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/alert/alert_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/alert/bees_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/alert/bees_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/alert/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/alert/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.348732 ho-protocols-0.2.4/src/ho_protocols/cmd/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.4/src/ho_protocols/cmd/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/cmd/cmd_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/cmd/cmd_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/common_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/common_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/data_in_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/data_in_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/example_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/example_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/src/ho_protocols/live/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.4/src/ho_protocols/live/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/actuators_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/actuators_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/live_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/live_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/models_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/models_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3409 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/sensors_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     7863 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/sensors_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1483 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1972 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/live/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/src/ho_protocols/map/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.4/src/ho_protocols/map/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/map/map_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/map/map_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/src/ho_protocols/query/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.4/src/ho_protocols/query/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/query/query_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-05-04 09:12:08.000000 ho-protocols-0.2.4/src/ho_protocols/query/query_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.344732 ho-protocols-0.2.4/src/ho_protocols.egg-info/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-04 09:12:41.000000 ho-protocols-0.2.4/src/ho_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-04 09:12:41.000000 ho-protocols-0.2.4/src/ho_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-04 09:12:41.000000 ho-protocols-0.2.4/src/ho_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-04 09:12:41.000000 ho-protocols-0.2.4/src/ho_protocols.egg-info/requires.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-04 09:12:41.000000 ho-protocols-0.2.4/src/ho_protocols.egg-info/top_level.txt
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-04 09:12:41.356732 ho-protocols-0.2.4/test/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.4/test/test.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.985791 ho-protocols-0.2.5/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.5/LICENCE
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-12 09:49:39.985791 ho-protocols-0.2.5/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.5/README.md
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-12 09:49:39.985791 ho-protocols-0.2.5/setup.cfg
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.5/setup.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.969791 ho-protocols-0.2.5/src/
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.977791 ho-protocols-0.2.5/src/ho_protocols/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.5/src/ho_protocols/__init__.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.977791 ho-protocols-0.2.5/src/ho_protocols/alert/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.5/src/ho_protocols/alert/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/alert/alert_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/alert/alert_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/alert/bees_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/alert/bees_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/alert/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/alert/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.977791 ho-protocols-0.2.5/src/ho_protocols/cmd/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.5/src/ho_protocols/cmd/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/cmd/cmd_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/cmd/cmd_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/common_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/common_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/data_in_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/data_in_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/example_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/example_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.981791 ho-protocols-0.2.5/src/ho_protocols/live/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.5/src/ho_protocols/live/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/actuators_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/actuators_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/live_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/live_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/models_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/models_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3409 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/sensors_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     7863 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/sensors_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1483 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1972 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/live/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.981791 ho-protocols-0.2.5/src/ho_protocols/map/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.5/src/ho_protocols/map/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/map/map_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/map/map_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.981791 ho-protocols-0.2.5/src/ho_protocols/query/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.5/src/ho_protocols/query/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     7480 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/query/query_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    19845 2023-05-12 09:49:28.000000 ho-protocols-0.2.5/src/ho_protocols/query/query_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.977791 ho-protocols-0.2.5/src/ho_protocols.egg-info/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-12 09:49:39.000000 ho-protocols-0.2.5/src/ho_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-12 09:49:39.000000 ho-protocols-0.2.5/src/ho_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-12 09:49:39.000000 ho-protocols-0.2.5/src/ho_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-12 09:49:39.000000 ho-protocols-0.2.5/src/ho_protocols.egg-info/requires.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-12 09:49:39.000000 ho-protocols-0.2.5/src/ho_protocols.egg-info/top_level.txt
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 09:49:39.981791 ho-protocols-0.2.5/test/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.5/test/test.py
```

### Comparing `ho-protocols-0.2.4/LICENCE` & `ho-protocols-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/PKG-INFO` & `ho-protocols-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.4
+Version: 0.2.5
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.4/README.md` & `ho-protocols-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/setup.py` & `ho-protocols-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/alert/alert_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/alert/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/alert/alert_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/alert/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/alert/bees_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/alert/bees_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/alert/bees_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/alert/bees_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/alert/system_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/alert/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/alert/system_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/alert/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/cmd/cmd_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/cmd/cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/cmd/cmd_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/cmd/cmd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/common_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/common_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/data_in_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/data_in_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/data_in_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/data_in_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/example_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/example_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/example_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/actuators_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/live/actuators_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/actuators_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/live/actuators_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/live_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/live/live_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/live_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/live/live_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/models_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/live/models_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/models_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/live/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/sensors_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/live/sensors_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/sensors_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/live/sensors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/system_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/live/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/live/system_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/live/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/map/map_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/map/map_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/map/map_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/map/map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/src/ho_protocols/query/query_pb2.py` & `ho-protocols-0.2.5/src/ho_protocols/query/query_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,43 +10,59 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from ho_protocols import common_pb2 as ho__protocols_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eho_protocols/query/query.proto\x12\x08ho.query\x1a\x19ho_protocols/common.proto\"\xf0\x01\n\x0cQueryRequest\x12!\n\x06header\x18\x01 \x01(\x0b\x32\x11.ho.common.Header\x12\x37\n\x11historical_weight\x18\x02 \x01(\x0b\x32\x1a.ho.query.HistoricalWeightH\x00\x12\x39\n\x12recent_temperature\x18\x03 \x01(\x0b\x32\x1b.ho.query.RecentTemperatureH\x00\x12@\n\x16latest_hive_parameters\x18\x04 \x01(\x0b\x32\x1e.ho.query.LatestHiveParametersH\x00\x42\x07\n\x05query\"\x84\x02\n\rQueryResponse\x12!\n\x06header\x18\x01 \x01(\x0b\x32\x11.ho.common.Header\x12=\n\x11historical_weight\x18\x02 \x01(\x0b\x32 .ho.query.HistoricalWeightResultH\x00\x12?\n\x12recent_temperature\x18\x03 \x01(\x0b\x32!.ho.query.RecentTemperatureResultH\x00\x12\x46\n\x16latest_hive_parameters\x18\x04 \x01(\x0b\x32$.ho.query.LatestHiveParametersResultH\x00\x42\x08\n\x06result\"4\n\x10HistoricalWeight\x12\x10\n\x08start_ts\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_ts\x18\x02 \x01(\x03\"U\n\x16HistoricalWeightResult\x12\x12\n\nmin_weight\x18\x01 \x01(\x02\x12\x12\n\nmax_weight\x18\x02 \x01(\x02\x12\x13\n\x0bmean_weight\x18\x03 \x01(\x02\"|\n\x11RecentTemperature\x12:\n\nresolution\x18\x01 \x01(\x0e\x32&.ho.query.RecentTemperature.Resolution\"+\n\nResolution\x12\n\n\x06Minute\x10\x00\x12\x08\n\x04Hour\x10\x01\x12\x07\n\x03\x44\x61y\x10\x02\"\xb4\x01\n\x17RecentTemperatureResult\x12\x10\n\x08start_ts\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_ts\x18\x02 \x01(\x03\x12\x39\n\x07records\x18\x03 \x03(\x0b\x32(.ho.query.RecentTemperatureResult.Record\x1a<\n\x06Record\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x0b\n\x03min\x18\x02 \x01(\x02\x12\x0b\n\x03max\x18\x03 \x01(\x02\x12\x0c\n\x04mean\x18\x04 \x01(\x02\"9\n\x14LatestHiveParameters\x12\x0f\n\x07hive_id\x18\x01 \x01(\t\x12\x10\n\x08start_ts\x18\x02 \x01(\x03\"\x99\x03\n\x1aLatestHiveParametersResult\x12=\n\x07traffic\x18\x01 \x03(\x0b\x32,.ho.query.LatestHiveParametersResult.Traffic\x12\x41\n\tbroodnest\x18\x02 \x03(\x0b\x32..ho.query.LatestHiveParametersResult.Broodnest\x12\x41\n\tharvester\x18\x03 \x03(\x0b\x32..ho.query.LatestHiveParametersResult.Harvester\x1a\x38\n\x07Traffic\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x62\x65\x65s_in\x18\x02 \x03(\x02\x12\x10\n\x08\x62\x65\x65s_out\x18\x03 \x03(\x02\x1aS\n\tBroodnest\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05width\x18\x02 \x01(\x05\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x02\x12\x0b\n\x03png\x18\x05 \x01(\x0c\x1a\'\n\tHarvester\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06weight\x18\x02 \x01(\x02\x42\x02H\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eho_protocols/query/query.proto\x12\x08ho.query\x1a\x19ho_protocols/common.proto\"\x8f\x03\n\x0cQueryRequest\x12!\n\x06header\x18\x01 \x01(\x0b\x32\x11.ho.common.Header\x12\x37\n\x11historical_weight\x18\x02 \x01(\x0b\x32\x1a.ho.query.HistoricalWeightH\x00\x12\x39\n\x12recent_temperature\x18\x03 \x01(\x0b\x32\x1b.ho.query.RecentTemperatureH\x00\x12@\n\x16latest_hive_parameters\x18\x04 \x01(\x0b\x32\x1e.ho.query.LatestHiveParametersH\x00\x12+\n\x0b\x62\x65\x65_counter\x18\x05 \x01(\x0b\x32\x14.ho.query.BeeCounterH\x00\x12/\n\rhoney_storage\x18\x06 \x01(\x0b\x32\x16.ho.query.HoneyStorageH\x00\x12?\n\x15\x62roodnest_temperature\x18\x07 \x01(\x0b\x32\x1e.ho.query.BroodnestTemperatureH\x00\x42\x07\n\x05query\"\xb5\x03\n\rQueryResponse\x12!\n\x06header\x18\x01 \x01(\x0b\x32\x11.ho.common.Header\x12=\n\x11historical_weight\x18\x02 \x01(\x0b\x32 .ho.query.HistoricalWeightResultH\x00\x12?\n\x12recent_temperature\x18\x03 \x01(\x0b\x32!.ho.query.RecentTemperatureResultH\x00\x12\x46\n\x16latest_hive_parameters\x18\x04 \x01(\x0b\x32$.ho.query.LatestHiveParametersResultH\x00\x12\x31\n\x0b\x62\x65\x65_counter\x18\x05 \x01(\x0b\x32\x1a.ho.query.BeeCounterResultH\x00\x12\x35\n\rhoney_storage\x18\x06 \x01(\x0b\x32\x1c.ho.query.HoneyStorageResultH\x00\x12\x45\n\x15\x62roodnest_temperature\x18\x07 \x01(\x0b\x32$.ho.query.BroodnestTemperatureResultH\x00\x42\x08\n\x06result\"4\n\x10HistoricalWeight\x12\x10\n\x08start_ts\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_ts\x18\x02 \x01(\x03\"U\n\x16HistoricalWeightResult\x12\x12\n\nmin_weight\x18\x01 \x01(\x02\x12\x12\n\nmax_weight\x18\x02 \x01(\x02\x12\x13\n\x0bmean_weight\x18\x03 \x01(\x02\"|\n\x11RecentTemperature\x12:\n\nresolution\x18\x01 \x01(\x0e\x32&.ho.query.RecentTemperature.Resolution\"+\n\nResolution\x12\n\n\x06Minute\x10\x00\x12\x08\n\x04Hour\x10\x01\x12\x07\n\x03\x44\x61y\x10\x02\"\xb4\x01\n\x17RecentTemperatureResult\x12\x10\n\x08start_ts\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_ts\x18\x02 \x01(\x03\x12\x39\n\x07records\x18\x03 \x03(\x0b\x32(.ho.query.RecentTemperatureResult.Record\x1a<\n\x06Record\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x0b\n\x03min\x18\x02 \x01(\x02\x12\x0b\n\x03max\x18\x03 \x01(\x02\x12\x0c\n\x04mean\x18\x04 \x01(\x02\"9\n\x14LatestHiveParameters\x12\x0f\n\x07hive_id\x18\x01 \x01(\t\x12\x10\n\x08start_ts\x18\x02 \x01(\x03\"\x99\x03\n\x1aLatestHiveParametersResult\x12=\n\x07traffic\x18\x01 \x03(\x0b\x32,.ho.query.LatestHiveParametersResult.Traffic\x12\x41\n\tbroodnest\x18\x02 \x03(\x0b\x32..ho.query.LatestHiveParametersResult.Broodnest\x12\x41\n\tharvester\x18\x03 \x03(\x0b\x32..ho.query.LatestHiveParametersResult.Harvester\x1a\x38\n\x07Traffic\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x62\x65\x65s_in\x18\x02 \x03(\x02\x12\x10\n\x08\x62\x65\x65s_out\x18\x03 \x03(\x02\x1aS\n\tBroodnest\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05width\x18\x02 \x01(\x05\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\x0e\n\x06values\x18\x04 \x03(\x02\x12\x0b\n\x03png\x18\x05 \x01(\x0c\x1a\'\n\tHarvester\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06weight\x18\x02 \x01(\x02\"C\n\nBeeCounter\x12\x10\n\x08start_ts\x18\x01 \x01(\x03\x12\x0f\n\x07stop_ts\x18\x02 \x01(\x03\x12\x12\n\nwindow_sec\x18\x03 \x01(\x05\"\x7f\n\x10\x42\x65\x65\x43ounterResult\x12\x32\n\x07windows\x18\x01 \x03(\x0b\x32!.ho.query.BeeCounterResult.Window\x1a\x37\n\x06Window\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x0f\n\x07\x62\x65\x65s_in\x18\x02 \x01(\x02\x12\x10\n\x08\x62\x65\x65s_out\x18\x03 \x01(\x02\"E\n\x0cHoneyStorage\x12\x10\n\x08start_ts\x18\x01 \x01(\x03\x12\x0f\n\x07stop_ts\x18\x02 \x01(\x03\x12\x12\n\nwindow_sec\x18\x03 \x01(\x05\"\x83\x01\n\x12HoneyStorageResult\x12\x34\n\x07windows\x18\x01 \x03(\x0b\x32#.ho.query.HoneyStorageResult.Window\x1a\x37\n\x06Window\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x0f\n\x07\x62\x65\x65s_in\x18\x02 \x01(\x02\x12\x10\n\x08\x62\x65\x65s_out\x18\x03 \x01(\x02\"\x16\n\x14\x42roodnestTemperature\"6\n\x1a\x42roodnestTemperatureResult\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x0c\n\x04temp\x18\x02 \x03(\x02\x42\x02H\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ho_protocols.query.query_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
   _globals['_QUERYREQUEST']._serialized_start=72
-  _globals['_QUERYREQUEST']._serialized_end=312
-  _globals['_QUERYRESPONSE']._serialized_start=315
-  _globals['_QUERYRESPONSE']._serialized_end=575
-  _globals['_HISTORICALWEIGHT']._serialized_start=577
-  _globals['_HISTORICALWEIGHT']._serialized_end=629
-  _globals['_HISTORICALWEIGHTRESULT']._serialized_start=631
-  _globals['_HISTORICALWEIGHTRESULT']._serialized_end=716
-  _globals['_RECENTTEMPERATURE']._serialized_start=718
-  _globals['_RECENTTEMPERATURE']._serialized_end=842
-  _globals['_RECENTTEMPERATURE_RESOLUTION']._serialized_start=799
-  _globals['_RECENTTEMPERATURE_RESOLUTION']._serialized_end=842
-  _globals['_RECENTTEMPERATURERESULT']._serialized_start=845
-  _globals['_RECENTTEMPERATURERESULT']._serialized_end=1025
-  _globals['_RECENTTEMPERATURERESULT_RECORD']._serialized_start=965
-  _globals['_RECENTTEMPERATURERESULT_RECORD']._serialized_end=1025
-  _globals['_LATESTHIVEPARAMETERS']._serialized_start=1027
-  _globals['_LATESTHIVEPARAMETERS']._serialized_end=1084
-  _globals['_LATESTHIVEPARAMETERSRESULT']._serialized_start=1087
-  _globals['_LATESTHIVEPARAMETERSRESULT']._serialized_end=1496
-  _globals['_LATESTHIVEPARAMETERSRESULT_TRAFFIC']._serialized_start=1314
-  _globals['_LATESTHIVEPARAMETERSRESULT_TRAFFIC']._serialized_end=1370
-  _globals['_LATESTHIVEPARAMETERSRESULT_BROODNEST']._serialized_start=1372
-  _globals['_LATESTHIVEPARAMETERSRESULT_BROODNEST']._serialized_end=1455
-  _globals['_LATESTHIVEPARAMETERSRESULT_HARVESTER']._serialized_start=1457
-  _globals['_LATESTHIVEPARAMETERSRESULT_HARVESTER']._serialized_end=1496
+  _globals['_QUERYREQUEST']._serialized_end=471
+  _globals['_QUERYRESPONSE']._serialized_start=474
+  _globals['_QUERYRESPONSE']._serialized_end=911
+  _globals['_HISTORICALWEIGHT']._serialized_start=913
+  _globals['_HISTORICALWEIGHT']._serialized_end=965
+  _globals['_HISTORICALWEIGHTRESULT']._serialized_start=967
+  _globals['_HISTORICALWEIGHTRESULT']._serialized_end=1052
+  _globals['_RECENTTEMPERATURE']._serialized_start=1054
+  _globals['_RECENTTEMPERATURE']._serialized_end=1178
+  _globals['_RECENTTEMPERATURE_RESOLUTION']._serialized_start=1135
+  _globals['_RECENTTEMPERATURE_RESOLUTION']._serialized_end=1178
+  _globals['_RECENTTEMPERATURERESULT']._serialized_start=1181
+  _globals['_RECENTTEMPERATURERESULT']._serialized_end=1361
+  _globals['_RECENTTEMPERATURERESULT_RECORD']._serialized_start=1301
+  _globals['_RECENTTEMPERATURERESULT_RECORD']._serialized_end=1361
+  _globals['_LATESTHIVEPARAMETERS']._serialized_start=1363
+  _globals['_LATESTHIVEPARAMETERS']._serialized_end=1420
+  _globals['_LATESTHIVEPARAMETERSRESULT']._serialized_start=1423
+  _globals['_LATESTHIVEPARAMETERSRESULT']._serialized_end=1832
+  _globals['_LATESTHIVEPARAMETERSRESULT_TRAFFIC']._serialized_start=1650
+  _globals['_LATESTHIVEPARAMETERSRESULT_TRAFFIC']._serialized_end=1706
+  _globals['_LATESTHIVEPARAMETERSRESULT_BROODNEST']._serialized_start=1708
+  _globals['_LATESTHIVEPARAMETERSRESULT_BROODNEST']._serialized_end=1791
+  _globals['_LATESTHIVEPARAMETERSRESULT_HARVESTER']._serialized_start=1793
+  _globals['_LATESTHIVEPARAMETERSRESULT_HARVESTER']._serialized_end=1832
+  _globals['_BEECOUNTER']._serialized_start=1834
+  _globals['_BEECOUNTER']._serialized_end=1901
+  _globals['_BEECOUNTERRESULT']._serialized_start=1903
+  _globals['_BEECOUNTERRESULT']._serialized_end=2030
+  _globals['_BEECOUNTERRESULT_WINDOW']._serialized_start=1975
+  _globals['_BEECOUNTERRESULT_WINDOW']._serialized_end=2030
+  _globals['_HONEYSTORAGE']._serialized_start=2032
+  _globals['_HONEYSTORAGE']._serialized_end=2101
+  _globals['_HONEYSTORAGERESULT']._serialized_start=2104
+  _globals['_HONEYSTORAGERESULT']._serialized_end=2235
+  _globals['_HONEYSTORAGERESULT_WINDOW']._serialized_start=1975
+  _globals['_HONEYSTORAGERESULT_WINDOW']._serialized_end=2030
+  _globals['_BROODNESTTEMPERATURE']._serialized_start=2237
+  _globals['_BROODNESTTEMPERATURE']._serialized_end=2259
+  _globals['_BROODNESTTEMPERATURERESULT']._serialized_start=2261
+  _globals['_BROODNESTTEMPERATURERESULT']._serialized_end=2315
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ho-protocols-0.2.4/src/ho_protocols/query/query_pb2.pyi` & `ho-protocols-0.2.5/src/ho_protocols/query/query_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -23,63 +23,87 @@
 class QueryRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEADER_FIELD_NUMBER: builtins.int
     HISTORICAL_WEIGHT_FIELD_NUMBER: builtins.int
     RECENT_TEMPERATURE_FIELD_NUMBER: builtins.int
     LATEST_HIVE_PARAMETERS_FIELD_NUMBER: builtins.int
+    BEE_COUNTER_FIELD_NUMBER: builtins.int
+    HONEY_STORAGE_FIELD_NUMBER: builtins.int
+    BROODNEST_TEMPERATURE_FIELD_NUMBER: builtins.int
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
     @property
     def historical_weight(self) -> global___HistoricalWeight: ...
     @property
     def recent_temperature(self) -> global___RecentTemperature: ...
     @property
     def latest_hive_parameters(self) -> global___LatestHiveParameters: ...
+    @property
+    def bee_counter(self) -> global___BeeCounter: ...
+    @property
+    def honey_storage(self) -> global___HoneyStorage: ...
+    @property
+    def broodnest_temperature(self) -> global___BroodnestTemperature: ...
     def __init__(
         self,
         *,
         header: ho_protocols.common_pb2.Header | None = ...,
         historical_weight: global___HistoricalWeight | None = ...,
         recent_temperature: global___RecentTemperature | None = ...,
         latest_hive_parameters: global___LatestHiveParameters | None = ...,
+        bee_counter: global___BeeCounter | None = ...,
+        honey_storage: global___HoneyStorage | None = ...,
+        broodnest_temperature: global___BroodnestTemperature | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "query", b"query", "recent_temperature", b"recent_temperature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "query", b"query", "recent_temperature", b"recent_temperature"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["query", b"query"]) -> typing_extensions.Literal["historical_weight", "recent_temperature", "latest_hive_parameters"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bee_counter", b"bee_counter", "broodnest_temperature", b"broodnest_temperature", "header", b"header", "historical_weight", b"historical_weight", "honey_storage", b"honey_storage", "latest_hive_parameters", b"latest_hive_parameters", "query", b"query", "recent_temperature", b"recent_temperature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bee_counter", b"bee_counter", "broodnest_temperature", b"broodnest_temperature", "header", b"header", "historical_weight", b"historical_weight", "honey_storage", b"honey_storage", "latest_hive_parameters", b"latest_hive_parameters", "query", b"query", "recent_temperature", b"recent_temperature"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["query", b"query"]) -> typing_extensions.Literal["historical_weight", "recent_temperature", "latest_hive_parameters", "bee_counter", "honey_storage", "broodnest_temperature"] | None: ...
 
 global___QueryRequest = QueryRequest
 
 @typing_extensions.final
 class QueryResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEADER_FIELD_NUMBER: builtins.int
     HISTORICAL_WEIGHT_FIELD_NUMBER: builtins.int
     RECENT_TEMPERATURE_FIELD_NUMBER: builtins.int
     LATEST_HIVE_PARAMETERS_FIELD_NUMBER: builtins.int
+    BEE_COUNTER_FIELD_NUMBER: builtins.int
+    HONEY_STORAGE_FIELD_NUMBER: builtins.int
+    BROODNEST_TEMPERATURE_FIELD_NUMBER: builtins.int
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
     @property
     def historical_weight(self) -> global___HistoricalWeightResult: ...
     @property
     def recent_temperature(self) -> global___RecentTemperatureResult: ...
     @property
     def latest_hive_parameters(self) -> global___LatestHiveParametersResult: ...
+    @property
+    def bee_counter(self) -> global___BeeCounterResult: ...
+    @property
+    def honey_storage(self) -> global___HoneyStorageResult: ...
+    @property
+    def broodnest_temperature(self) -> global___BroodnestTemperatureResult: ...
     def __init__(
         self,
         *,
         header: ho_protocols.common_pb2.Header | None = ...,
         historical_weight: global___HistoricalWeightResult | None = ...,
         recent_temperature: global___RecentTemperatureResult | None = ...,
         latest_hive_parameters: global___LatestHiveParametersResult | None = ...,
+        bee_counter: global___BeeCounterResult | None = ...,
+        honey_storage: global___HoneyStorageResult | None = ...,
+        broodnest_temperature: global___BroodnestTemperatureResult | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "recent_temperature", b"recent_temperature", "result", b"result"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "recent_temperature", b"recent_temperature", "result", b"result"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["historical_weight", "recent_temperature", "latest_hive_parameters"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bee_counter", b"bee_counter", "broodnest_temperature", b"broodnest_temperature", "header", b"header", "historical_weight", b"historical_weight", "honey_storage", b"honey_storage", "latest_hive_parameters", b"latest_hive_parameters", "recent_temperature", b"recent_temperature", "result", b"result"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bee_counter", b"bee_counter", "broodnest_temperature", b"broodnest_temperature", "header", b"header", "historical_weight", b"historical_weight", "honey_storage", b"honey_storage", "latest_hive_parameters", b"latest_hive_parameters", "recent_temperature", b"recent_temperature", "result", b"result"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["historical_weight", "recent_temperature", "latest_hive_parameters", "bee_counter", "honey_storage", "broodnest_temperature"] | None: ...
 
 global___QueryResponse = QueryResponse
 
 @typing_extensions.final
 class HistoricalWeight(google.protobuf.message.Message):
     """### Historical weight query"""
 
@@ -298,7 +322,154 @@
         traffic: collections.abc.Iterable[global___LatestHiveParametersResult.Traffic] | None = ...,
         broodnest: collections.abc.Iterable[global___LatestHiveParametersResult.Broodnest] | None = ...,
         harvester: collections.abc.Iterable[global___LatestHiveParametersResult.Harvester] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["broodnest", b"broodnest", "harvester", b"harvester", "traffic", b"traffic"]) -> None: ...
 
 global___LatestHiveParametersResult = LatestHiveParametersResult
+
+@typing_extensions.final
+class BeeCounter(google.protobuf.message.Message):
+    """### Bee counter report"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    START_TS_FIELD_NUMBER: builtins.int
+    STOP_TS_FIELD_NUMBER: builtins.int
+    WINDOW_SEC_FIELD_NUMBER: builtins.int
+    start_ts: builtins.int
+    stop_ts: builtins.int
+    window_sec: builtins.int
+    def __init__(
+        self,
+        *,
+        start_ts: builtins.int = ...,
+        stop_ts: builtins.int = ...,
+        window_sec: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["start_ts", b"start_ts", "stop_ts", b"stop_ts", "window_sec", b"window_sec"]) -> None: ...
+
+global___BeeCounter = BeeCounter
+
+@typing_extensions.final
+class BeeCounterResult(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
+    class Window(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        TS_FIELD_NUMBER: builtins.int
+        BEES_IN_FIELD_NUMBER: builtins.int
+        BEES_OUT_FIELD_NUMBER: builtins.int
+        ts: builtins.int
+        bees_in: builtins.float
+        bees_out: builtins.float
+        def __init__(
+            self,
+            *,
+            ts: builtins.int = ...,
+            bees_in: builtins.float = ...,
+            bees_out: builtins.float = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["bees_in", b"bees_in", "bees_out", b"bees_out", "ts", b"ts"]) -> None: ...
+
+    WINDOWS_FIELD_NUMBER: builtins.int
+    @property
+    def windows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BeeCounterResult.Window]: ...
+    def __init__(
+        self,
+        *,
+        windows: collections.abc.Iterable[global___BeeCounterResult.Window] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["windows", b"windows"]) -> None: ...
+
+global___BeeCounterResult = BeeCounterResult
+
+@typing_extensions.final
+class HoneyStorage(google.protobuf.message.Message):
+    """### Honey storage report"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    START_TS_FIELD_NUMBER: builtins.int
+    STOP_TS_FIELD_NUMBER: builtins.int
+    WINDOW_SEC_FIELD_NUMBER: builtins.int
+    start_ts: builtins.int
+    stop_ts: builtins.int
+    window_sec: builtins.int
+    def __init__(
+        self,
+        *,
+        start_ts: builtins.int = ...,
+        stop_ts: builtins.int = ...,
+        window_sec: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["start_ts", b"start_ts", "stop_ts", b"stop_ts", "window_sec", b"window_sec"]) -> None: ...
+
+global___HoneyStorage = HoneyStorage
+
+@typing_extensions.final
+class HoneyStorageResult(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
+    class Window(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        TS_FIELD_NUMBER: builtins.int
+        BEES_IN_FIELD_NUMBER: builtins.int
+        BEES_OUT_FIELD_NUMBER: builtins.int
+        ts: builtins.int
+        bees_in: builtins.float
+        bees_out: builtins.float
+        def __init__(
+            self,
+            *,
+            ts: builtins.int = ...,
+            bees_in: builtins.float = ...,
+            bees_out: builtins.float = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["bees_in", b"bees_in", "bees_out", b"bees_out", "ts", b"ts"]) -> None: ...
+
+    WINDOWS_FIELD_NUMBER: builtins.int
+    @property
+    def windows(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HoneyStorageResult.Window]: ...
+    def __init__(
+        self,
+        *,
+        windows: collections.abc.Iterable[global___HoneyStorageResult.Window] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["windows", b"windows"]) -> None: ...
+
+global___HoneyStorageResult = HoneyStorageResult
+
+@typing_extensions.final
+class BroodnestTemperature(google.protobuf.message.Message):
+    """### BroodnestTemperature report"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___BroodnestTemperature = BroodnestTemperature
+
+@typing_extensions.final
+class BroodnestTemperatureResult(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    TS_FIELD_NUMBER: builtins.int
+    TEMP_FIELD_NUMBER: builtins.int
+    ts: builtins.int
+    @property
+    def temp(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        ts: builtins.int = ...,
+        temp: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["temp", b"temp", "ts", b"ts"]) -> None: ...
+
+global___BroodnestTemperatureResult = BroodnestTemperatureResult
```

### Comparing `ho-protocols-0.2.4/src/ho_protocols.egg-info/PKG-INFO` & `ho-protocols-0.2.5/src/ho_protocols.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.4
+Version: 0.2.5
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.4/src/ho_protocols.egg-info/SOURCES.txt` & `ho-protocols-0.2.5/src/ho_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.4/test/test.py` & `ho-protocols-0.2.5/test/test.py`

 * *Files identical despite different names*


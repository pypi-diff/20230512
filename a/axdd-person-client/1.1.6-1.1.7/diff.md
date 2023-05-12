# Comparing `tmp/axdd-person-client-1.1.6.tar.gz` & `tmp/axdd-person-client-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.6.tar", last modified: Tue May  9 20:54:51 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.7.tar", last modified: Fri May 12 17:49:54 2023, max compression
```

## Comparing `axdd-person-client-1.1.6.tar` & `axdd-person-client-1.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27350 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    35548 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27342 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35548 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.6/LICENSE` & `axdd-person-client-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/PKG-INFO` & `axdd-person-client-1.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.6
+Version: 1.1.7
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.6/README.md` & `axdd-person-client-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.7/axdd_person_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.6
+Version: 1.1.7
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.6/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.7/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/conf/settings.py` & `axdd-person-client-1.1.7/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/setup.py` & `axdd-person-client-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.7/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.7/uw_person_client/clients/core_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
             for hold in sqla_student.student_hold:
                 hold = self._map_hold(hold)
                 student.holds.append(hold)
 
         if include_student_degrees:
             # map degrees
             student.degrees = []
-            for degree in sqla_student.student_degree:
+            for degree in sqla_student.degree:
                 degree = self._map_degree(degree)
                 student.degrees.append(degree)
 
         return student
 
     def _map_employee(self, sqla_employee):
         employee = Employee()
```

### Comparing `axdd-person-client-1.1.6/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.7/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/components.py` & `axdd-person-client-1.1.7/uw_person_client/components.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.7/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.7/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.7/uw_person_client/databases/uwpds.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.7/uw_person_client/tests/test_core_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.6/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.7/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*


# Comparing `tmp/tds-django-4.2.0.tar.gz` & `tmp/tds-django-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tds-django-4.2.0.tar", last modified: Wed May 10 12:30:54 2023, max compression
+gzip compressed data, was "tds-django-4.2.1.tar", last modified: Fri May 12 15:14:16 2023, max compression
```

## Comparing `tds-django-4.2.0.tar` & `tds-django-4.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.394771 tds-django-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-10 12:30:41.000000 tds-django-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-10 12:30:54.394771 tds-django-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-10 12:30:41.000000 tds-django-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:30:54.394771 tds-django-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-10 12:30:41.000000 tds-django-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.390771 tds-django-4.2.0/tds_django/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5805 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7431 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/creation.py
--rw-r--r--   0 runner    (1001) docker     (122)    14532 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/features.py
--rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6969 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/introspection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/patches.py
--rw-r--r--   0 runner    (1001) docker     (122)    21732 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.394771 tds-django-4.2.0/tds_django/sql/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/clr.sql
--rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/init.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)    21250 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/tz.py
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.394771 tds-django-4.2.0/tds_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.471518 tds-django-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-12 15:14:01.000000 tds-django-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-12 15:14:16.471518 tds-django-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-12 15:14:01.000000 tds-django-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 15:14:16.471518 tds-django-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-12 15:14:01.000000 tds-django-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.467518 tds-django-4.2.1/tds_django/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6197 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7431 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14532 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6969 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/patches.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21732 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.471518 tds-django-4.2.1/tds_django/sql/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/clr.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/init.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21250 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/tz.py
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.467518 tds-django-4.2.1/tds_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/top_level.txt
```

### Comparing `tds-django-4.2.0/LICENSE` & `tds-django-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/PKG-INFO` & `tds-django-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tds-django
-Version: 4.2.0
+Version: 4.2.1
 Summary: Django backend for SQL Server using tds
 Home-page: https://github.com/ecogels/tds-django
 Author: Etienne Cogels
 Author-email: ecogels@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ecogels/tds-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tds-django-4.2.0/README.md` & `tds-django-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/setup.py` & `tds-django-4.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tds-django",
-    version="4.2.0",
+    version="4.2.1",
     author="Etienne Cogels",
     author_email="ecogels@users.noreply.github.com",
     description="Django backend for SQL Server using tds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ecogels/tds-django",
     project_urls={
```

### Comparing `tds-django-4.2.0/tds_django/base.py` & `tds-django-4.2.1/tds_django/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,22 +97,26 @@
     introspection_class = DatabaseIntrospection
     ops_class = DatabaseOperations
     validation_class = DatabaseValidation
 
     def get_connection_params(self):
         settings_dict = self.settings_dict
         # TODO warnings for user
+        # skipped: as_dict use_tz bytes_to_unicode row_strategy server(?)
+        allowed_params = 'timeout login_timeout appname tds_version use_mars auth readonly load_balancer ' \
+                         'failover_partner cafile sock validate_host enc_login_only disable_connect_retry ' \
+                         'pooling use_sso'.split()
         conn_params = {
             'dsn': settings_dict['HOST'] or 'localhost',
             'port': settings_dict['PORT'] or 1433,
             'database': settings_dict['NAME'],
             'user': settings_dict['USER'],
             'password': settings_dict['PASSWORD'],
             'autocommit': getattr(settings, 'AUTOCOMMIT', False),
-            'use_mars': False,
+            **{k: v for k, v in settings_dict.items() if k in allowed_params},
          }
         return conn_params
 
     def get_new_connection(self, conn_params):
         conn = self.Database.connect(**conn_params)
         return conn
```

### Comparing `tds-django-4.2.0/tds_django/compiler.py` & `tds-django-4.2.1/tds_django/compiler.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/creation.py` & `tds-django-4.2.1/tds_django/creation.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/features.py` & `tds-django-4.2.1/tds_django/features.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/functions.py` & `tds-django-4.2.1/tds_django/functions.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/introspection.py` & `tds-django-4.2.1/tds_django/introspection.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/operations.py` & `tds-django-4.2.1/tds_django/operations.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/patches.py` & `tds-django-4.2.1/tds_django/patches.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/schema.py` & `tds-django-4.2.1/tds_django/schema.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/sql/clr.sql` & `tds-django-4.2.1/tds_django/sql/clr.sql`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/sql/init.sql` & `tds-django-4.2.1/tds_django/sql/init.sql`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/sql/queries.py` & `tds-django-4.2.1/tds_django/sql/queries.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/tz.py` & `tds-django-4.2.1/tds_django/tz.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django/validation.py` & `tds-django-4.2.1/tds_django/validation.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.0/tds_django.egg-info/PKG-INFO` & `tds-django-4.2.1/tds_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tds-django
-Version: 4.2.0
+Version: 4.2.1
 Summary: Django backend for SQL Server using tds
 Home-page: https://github.com/ecogels/tds-django
 Author: Etienne Cogels
 Author-email: ecogels@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ecogels/tds-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tds-django-4.2.0/tds_django.egg-info/SOURCES.txt` & `tds-django-4.2.1/tds_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*


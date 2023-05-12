# Comparing `tmp/eswrap-0.4.tar.gz` & `tmp/eswrap-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.tar", last modified: Thu May 11 11:44:31 2023, max compression
+gzip compressed data, was "eswrap-0.4.1.tar", last modified: Fri May 12 06:15:04 2023, max compression
```

## Comparing `eswrap-0.4.tar` & `eswrap-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-11 11:44:18.000000 eswrap-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-11 11:44:31.900946 eswrap-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 11:44:18.000000 eswrap-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:44:31.904946 eswrap-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-11 11:44:18.000000 eswrap-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 06:15:04.396215 eswrap-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 06:14:50.000000 eswrap-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 06:15:04.396215 eswrap-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 06:14:50.000000 eswrap-0.4.1/setup.py
```

### Comparing `eswrap-0.4/LICENSE` & `eswrap-0.4.1/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4/PKG-INFO` & `eswrap-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4
+Version: 0.4.1
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # ESWRAP
```

### Comparing `eswrap-0.4/eswrap/__init__.py` & `eswrap-0.4.1/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4/eswrap/common/EsHandler.py` & `eswrap-0.4.1/eswrap/common/EsHandler.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4/eswrap/main.py` & `eswrap-0.4.1/eswrap/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,32 +18,64 @@
     version_file = os.path.join(_PKG_DIR, "VERSION")
     with open(version_file, "r") as fdsec:
         VERSION = fdsec.read()
 
 
 class EsWrap(object):
     def __init__(
-        self, host: str = "localhost", port: int = 9200, scheme: str = "http", **kwargs
+        self,
+        host: str = "localhost",
+        port: int = 9200,
+        scheme: str = "http",
+        connection_details: list[str] | list[dict] = None,
+        **kwargs,
     ):
+        """
+        connection_details should facilitate all connection options as stated in the API documentation of the
+        Elasticsearch library.
+        E.g.
+        [
+            {'host': 'localhost'},
+            {'host': 'othernode', 'port': 443, 'url_prefix': 'es', 'use_ssl': True},
+        ]
+
+        or
+
+        ['localhost:443', 'other_host:443'] with additional kwargs (if any)
+
+        or
+
+        [
+            'http://user:secret@localhost:9200/',
+            'https://user:secret@other_host:443/production'
+        ]
+        """
         self.__version = VERSION
 
-        self.connection_details = {"host": host, "port": port, "scheme": scheme}
+        if connection_details is not None:
+            self.connection_details = [{"host": host, "port": port, "scheme": scheme}]
+        else:
+            self.connection_details = connection_details
 
         self.logger = logging.getLogger(__name__)
 
-        self.__es_client = Elasticsearch([self.connection_details], **kwargs)
+        self.__es_client = Elasticsearch(self.connection_details, **kwargs)
 
         try:
             for each in self.__es_client.indices.get(index="*").keys():
                 if not each.startswith("."):
                     setattr(
-                        self, each, EsHandler(es_connection=self.__es_client, index=each)
+                        self,
+                        each,
+                        EsHandler(es_connection=self.__es_client, index=each),
                     )
         except elastic_transport.ConnectionError as err:
-            self.logger.warning(f"Cannot connect to elasticsearch, error encountered: {err}")
+            self.logger.warning(
+                f"Cannot connect to elasticsearch, error encountered: {err}"
+            )
         except Exception as err:
             self.logger.error(f"Uncaught exeption encountered: {err}")
 
     @property
     def es_client(self):
         return self.__es_client
 
@@ -66,13 +98,34 @@
                 self,
                 index_name,
                 EsHandler(es_connection=self.__es_client, index=index_name),
             )
 
         return self.es_client.index(index=index_name, document=data, id=doc_id)
 
+    def delete_index(self, index_name: str):
+
+        ret_val = self.es_client.options(ignore_status=[400, 404]).indices.delete(
+            index=index_name
+        )
+
+        try:
+            if ret_val["acknowledged"]:
+                if hasattr(self, index_name):
+                    delattr(self, index_name)
+                return True
+        except KeyError:
+            # failed somehow, assuming the given index does not exist
+            self.logger.warning(
+                f"The index {index_name} cannot not be deleted; reason -> {ret_val}"
+            )
+        except Exception as err:
+            self.logger.error(f"Uncaught exception encountered: {err}")
+
+        return False
+
     def __del__(self):
         self.__es_client.close()
 
     def __repr__(self):
         """String representation of object"""
         return "<< EsWrap:{} >>".format(self.version)
```

### Comparing `eswrap-0.4/eswrap.egg-info/PKG-INFO` & `eswrap-0.4.1/eswrap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4
+Version: 0.4.1
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # ESWRAP
```

### Comparing `eswrap-0.4/setup.py` & `eswrap-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     url="",
     license="GNU General Public License v3.0",
     author="Paul Tikken",
     author_email="paul.tikken@gmail.com",
     description="Python wrapper for simple elasticsearch queries",
     long_description=README,
     long_description_content_type="text/markdown",
-    package_data={"eswrap": ["LICENSE", "VERSION", "sources/user_agents.txt"]},
+    package_data={"eswrap": ["LICENSE", "VERSION"]},
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```


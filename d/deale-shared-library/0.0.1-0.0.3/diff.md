# Comparing `tmp/deale_shared_library-0.0.1.tar.gz` & `tmp/deale_shared_library-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deale_shared_library-0.0.1.tar", last modified: Thu May 11 08:29:51 2023, max compression
+gzip compressed data, was "deale_shared_library-0.0.3.tar", last modified: Fri May 12 08:16:17 2023, max compression
```

## Comparing `deale_shared_library-0.0.1.tar` & `deale_shared_library-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-11 08:29:51.451846 deale_shared_library-0.0.1/
--rw-r--r--   0 caaarlxs   (501) staff       (20)      347 2023-05-11 08:29:51.451725 deale_shared_library-0.0.1/PKG-INFO
--rw-r--r--   0 caaarlxs   (501) staff       (20)        2 2023-05-11 08:12:29.000000 deale_shared_library-0.0.1/README.md
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-11 08:29:51.451091 deale_shared_library-0.0.1/deale_shared_library/
--rw-r--r--   0 caaarlxs   (501) staff       (20)     1190 2023-05-11 08:05:39.000000 deale_shared_library-0.0.1/deale_shared_library/DynamoDB.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)     5412 2023-05-11 07:52:30.000000 deale_shared_library-0.0.1/deale_shared_library/DynamoDB_test.py
--rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:28.000000 deale_shared_library-0.0.1/deale_shared_library/__init__.py
-drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-11 08:29:51.451548 deale_shared_library-0.0.1/deale_shared_library.egg-info/
--rw-r--r--   0 caaarlxs   (501) staff       (20)      347 2023-05-11 08:29:51.000000 deale_shared_library-0.0.1/deale_shared_library.egg-info/PKG-INFO
--rw-r--r--   0 caaarlxs   (501) staff       (20)      298 2023-05-11 08:29:51.000000 deale_shared_library-0.0.1/deale_shared_library.egg-info/SOURCES.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)        1 2023-05-11 08:29:51.000000 deale_shared_library-0.0.1/deale_shared_library.egg-info/dependency_links.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)       21 2023-05-11 08:29:51.000000 deale_shared_library-0.0.1/deale_shared_library.egg-info/top_level.txt
--rw-r--r--   0 caaarlxs   (501) staff       (20)       38 2023-05-11 08:29:51.451890 deale_shared_library-0.0.1/setup.cfg
--rw-r--r--   0 caaarlxs   (501) staff       (20)      582 2023-05-11 08:29:39.000000 deale_shared_library-0.0.1/setup.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.510661 deale_shared_library-0.0.3/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      347 2023-05-12 08:16:17.510512 deale_shared_library-0.0.3/PKG-INFO
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        2 2023-05-11 08:12:29.000000 deale_shared_library-0.0.3/README.md
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.508822 deale_shared_library-0.0.3/deale_shared_library/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     1571 2023-05-12 08:12:54.000000 deale_shared_library-0.0.3/deale_shared_library/DynamoDB.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)     5412 2023-05-11 07:52:30.000000 deale_shared_library-0.0.3/deale_shared_library/DynamoDB_test.py
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:28.000000 deale_shared_library-0.0.3/deale_shared_library/__init__.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.510164 deale_shared_library-0.0.3/deale_shared_library.egg-info/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      347 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/PKG-INFO
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      313 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/SOURCES.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        1 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/dependency_links.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)       21 2023-05-12 08:16:17.000000 deale_shared_library-0.0.3/deale_shared_library.egg-info/top_level.txt
+-rw-r--r--   0 caaarlxs   (501) staff       (20)       38 2023-05-12 08:16:17.510705 deale_shared_library-0.0.3/setup.cfg
+-rw-r--r--   0 caaarlxs   (501) staff       (20)      582 2023-05-12 08:14:12.000000 deale_shared_library-0.0.3/setup.py
+drwxr-xr-x   0 caaarlxs   (501) staff       (20)        0 2023-05-12 08:16:17.510339 deale_shared_library-0.0.3/tests/
+-rw-r--r--   0 caaarlxs   (501) staff       (20)        0 2023-05-11 07:15:46.000000 deale_shared_library-0.0.3/tests/tests.py
```

### Comparing `deale_shared_library-0.0.1/deale_shared_library/DynamoDB.py` & `deale_shared_library-0.0.3/deale_shared_library/DynamoDB.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(self):
         """
         Initialize a DynamoDB resource for a specific AWS region.
 
         :param region_name: The name of the AWS region.
         """
         self.dynamodb = boto3.resource('dynamodb', region_name='eu-west-1')
+    
 
     def scan(self, table_name, **kwargs):
         """
         Scan a DynamoDB table.
 
         :param table_name: The name of the DynamoDB table.
         :param **kwargs: Any keyword arguments accepted by the boto3 Table.scan() method.
@@ -32,7 +33,19 @@
 
         :param table_name: The name of the DynamoDB table.
         :param **kwargs: Any keyword arguments accepted by the boto3 Table.query() method.
         :return: The response from the query operation.
         """
         table = self.dynamodb.Table(table_name)
         return table.query(**kwargs)
+    
+    def put_item(self, table_name, item):
+        """
+        Put an item into a DynamoDB table.
+
+        :param table_name: The name of the DynamoDB table.
+        :param item: The item to put into the table.
+        :return: The response from the put_item operation.
+        """
+        table = self.dynamodb.Table(table_name)
+        return table.put_item(Item=item)
+
```

### Comparing `deale_shared_library-0.0.1/deale_shared_library/DynamoDB_test.py` & `deale_shared_library-0.0.3/deale_shared_library/DynamoDB_test.py`

 * *Files identical despite different names*

### Comparing `deale_shared_library-0.0.1/setup.py` & `deale_shared_library-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
-    name='deale_shared_library',
-    version='0.0.1',
+    name="deale_shared_library",
+    version="0.0.3",
     packages=find_packages(),
-    description='A shared library for Deale microservices',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
+    description="A shared library for Deale microservices",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     install_requires=[
         # List your library dependencies here
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.8",
     ],
 )
```


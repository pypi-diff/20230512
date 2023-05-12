# Comparing `tmp/hkfdb-3.1.tar.gz` & `tmp/hkfdb-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.1.tar", last modified: Thu May 11 06:35:58 2023, max compression
+gzip compressed data, was "hkfdb-3.2.tar", last modified: Fri May 12 14:38:22 2023, max compression
```

## Comparing `hkfdb-3.1.tar` & `hkfdb-3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 06:35:58.772111 hkfdb-3.1/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-3.1/LICENSE
--rw-rw-rw-   0        0        0     1651 2023-05-11 06:35:58.772111 hkfdb-3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 06:35:58.766099 hkfdb-3.1/hkfdb/
--rw-rw-rw-   0        0        0    93289 2023-05-11 06:35:23.000000 hkfdb-3.1/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-3.1/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:35:58.771100 hkfdb-3.1/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1651 2023-05-11 06:35:58.000000 hkfdb-3.1/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-11 06:35:58.000000 hkfdb-3.1/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 06:35:58.000000 hkfdb-3.1/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-11 06:35:58.000000 hkfdb-3.1/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 06:35:58.000000 hkfdb-3.1/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 06:35:58.772111 hkfdb-3.1/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-05-11 06:35:49.000000 hkfdb-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:38:22.924455 hkfdb-3.2/
+-rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-3.2/LICENSE
+-rw-rw-rw-   0        0        0     1651 2023-05-12 14:38:22.924455 hkfdb-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 14:38:22.917452 hkfdb-3.2/hkfdb/
+-rw-rw-rw-   0        0        0    93289 2023-05-12 14:37:56.000000 hkfdb-3.2/hkfdb/Database.py
+-rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-3.2/hkfdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:38:22.923453 hkfdb-3.2/hkfdb.egg-info/
+-rw-rw-rw-   0        0        0     1651 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 14:38:22.924455 hkfdb-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-05-12 14:38:09.000000 hkfdb-3.2/setup.py
```

### Comparing `hkfdb-3.1/LICENSE` & `hkfdb-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.1/PKG-INFO` & `hkfdb-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.1
+Version: 3.2
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-3.1/README.md` & `hkfdb-3.2/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.1/hkfdb/Database.py` & `hkfdb-3.2/hkfdb/Database.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -396,22 +396,22 @@
                             index_0 = check_drop_index_row.index[0]
                             index_1 = check_drop_index_row.index[1]
                             expiry_date_0 = df.loc[index_0, 'expiry_date']
                             expiry_date_1 = df.loc[index_1, 'expiry_date']
                             close_price_0 = df.loc[index_0, 'close']
                             close_price_1 = df.loc[index_1, 'close']
                             if expiry_date_0 > expiry_date_1:
-                                drop_index_list.append(index_0)
+                                drop_index_list.append(index_1)
                                 roll_diff = close_price_0 - close_price_1
-                                df.at[index_1,'roll_diff'] = roll_diff
+                                df.at[index_0,'roll_diff'] = roll_diff
                             elif expiry_date_0 < expiry_date_1:
-                                drop_index_list.append(index_1)
+                                drop_index_list.append(index_0)
                                 roll_diff = close_price_1 - close_price_0
                                 roll_diff = close_price_0 - close_price_1
-                                df.at[index_0,'roll_diff'] = roll_diff
+                                df.at[index_1,'roll_diff'] = roll_diff
                     if len(drop_index_list) > 0:
                         df = df.drop(drop_index_list, axis=0)
                     df = df.drop('index', axis=1)
 
                 else:
                     df = df.reset_index()
```

### Comparing `hkfdb-3.1/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.2/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.1
+Version: 3.2
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-3.1/setup.py` & `hkfdb-3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.1",
+    version="3.2",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```


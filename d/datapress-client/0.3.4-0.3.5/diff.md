# Comparing `tmp/datapress-client-0.3.4.tar.gz` & `tmp/datapress-client-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapress-client-0.3.4.tar", last modified: Fri Feb 10 08:47:58 2023, max compression
+gzip compressed data, was "dist/datapress-client-0.3.5.tar", last modified: Fri May 12 15:15:29 2023, max compression
```

## Comparing `datapress-client-0.3.4.tar` & `datapress-client-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-02-10 08:47:58.555457 datapress-client-0.3.4/
--rw-r--r--   0 Ace        (501) staff       (20)      551 2022-11-03 10:54:22.000000 datapress-client-0.3.4/LICENSE
--rw-r--r--   0 Ace        (501) staff       (20)       27 2022-11-03 10:54:22.000000 datapress-client-0.3.4/MANIFEST.in
--rw-r--r--   0 Ace        (501) staff       (20)      450 2023-02-10 08:47:58.555569 datapress-client-0.3.4/PKG-INFO
--rw-r--r--   0 Ace        (501) staff       (20)       48 2022-11-03 10:54:22.000000 datapress-client-0.3.4/README.md
-drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-02-10 08:47:58.547991 datapress-client-0.3.4/datapress/
--rw-r--r--   0 Ace        (501) staff       (20)      316 2022-11-18 14:01:50.000000 datapress-client-0.3.4/datapress/__init__.py
--rw-r--r--   0 Ace        (501) staff       (20)       22 2023-02-10 08:46:52.000000 datapress-client-0.3.4/datapress/__version__.py
--rw-r--r--   0 Ace        (501) staff       (20)     2958 2022-11-11 15:15:30.000000 datapress-client-0.3.4/datapress/api.py
--rw-r--r--   0 Ace        (501) staff       (20)    11286 2022-12-22 18:21:14.000000 datapress-client-0.3.4/datapress/dataset.py
--rw-r--r--   0 Ace        (501) staff       (20)      551 2022-11-04 13:49:03.000000 datapress-client-0.3.4/datapress/extract.py
--rw-r--r--   0 Ace        (501) staff       (20)     3149 2023-02-10 08:45:38.000000 datapress-client-0.3.4/datapress/geo.py
--rw-r--r--   0 Ace        (501) staff       (20)     1118 2022-11-18 14:01:50.000000 datapress-client-0.3.4/datapress/nomis.py
--rw-r--r--   0 Ace        (501) staff       (20)     6180 2022-11-18 14:01:50.000000 datapress-client-0.3.4/datapress/ons.py
-drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-02-10 08:47:58.548431 datapress-client-0.3.4/datapress/static/
--rw-r--r--   0 Ace        (501) staff       (20)  6867558 2023-02-10 08:44:33.000000 datapress-client-0.3.4/datapress/static/lsoa_lookup.csv
--rw-r--r--   0 Ace        (501) staff       (20)      668 2022-11-14 11:26:46.000000 datapress-client-0.3.4/datapress/utils.py
-drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-02-10 08:47:58.555302 datapress-client-0.3.4/datapress_client.egg-info/
--rw-r--r--   0 Ace        (501) staff       (20)      450 2023-02-10 08:47:58.000000 datapress-client-0.3.4/datapress_client.egg-info/PKG-INFO
--rw-r--r--   0 Ace        (501) staff       (20)      497 2023-02-10 08:47:58.000000 datapress-client-0.3.4/datapress_client.egg-info/SOURCES.txt
--rw-r--r--   0 Ace        (501) staff       (20)        1 2023-02-10 08:47:58.000000 datapress-client-0.3.4/datapress_client.egg-info/dependency_links.txt
--rw-r--r--   0 Ace        (501) staff       (20)        1 2023-02-10 08:47:58.000000 datapress-client-0.3.4/datapress_client.egg-info/not-zip-safe
--rw-r--r--   0 Ace        (501) staff       (20)       55 2023-02-10 08:47:58.000000 datapress-client-0.3.4/datapress_client.egg-info/requires.txt
--rw-r--r--   0 Ace        (501) staff       (20)       10 2023-02-10 08:47:58.000000 datapress-client-0.3.4/datapress_client.egg-info/top_level.txt
--rw-r--r--   0 Ace        (501) staff       (20)       79 2023-02-10 08:47:58.555886 datapress-client-0.3.4/setup.cfg
--rw-r--r--   0 Ace        (501) staff       (20)     1203 2022-12-16 19:01:36.000000 datapress-client-0.3.4/setup.py
+drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-05-12 15:15:29.000000 datapress-client-0.3.5/
+-rw-r--r--   0 Ace        (501) staff       (20)      489 2023-05-12 15:15:29.000000 datapress-client-0.3.5/PKG-INFO
+drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress/
+-rw-r--r--   0 Ace        (501) staff       (20)     3160 2023-02-10 09:05:07.000000 datapress-client-0.3.5/datapress/geo.py
+-rw-r--r--   0 Ace        (501) staff       (20)     6180 2022-11-18 14:01:50.000000 datapress-client-0.3.5/datapress/ons.py
+-rw-r--r--   0 Ace        (501) staff       (20)      316 2022-11-18 14:01:50.000000 datapress-client-0.3.5/datapress/__init__.py
+-rw-r--r--   0 Ace        (501) staff       (20)       22 2023-05-12 15:06:58.000000 datapress-client-0.3.5/datapress/__version__.py
+-rw-r--r--   0 Ace        (501) staff       (20)    11323 2023-05-12 15:06:08.000000 datapress-client-0.3.5/datapress/dataset.py
+-rw-r--r--   0 Ace        (501) staff       (20)     2958 2023-05-09 09:37:58.000000 datapress-client-0.3.5/datapress/api.py
+-rw-r--r--   0 Ace        (501) staff       (20)     1118 2022-11-18 14:01:50.000000 datapress-client-0.3.5/datapress/nomis.py
+-rw-r--r--   0 Ace        (501) staff       (20)      668 2022-11-14 11:26:46.000000 datapress-client-0.3.5/datapress/utils.py
+drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress/static/
+-rw-r--r--   0 Ace        (501) staff       (20)  6867558 2023-02-10 08:44:33.000000 datapress-client-0.3.5/datapress/static/lsoa_lookup.csv
+-rw-r--r--   0 Ace        (501) staff       (20)      551 2022-11-04 13:49:03.000000 datapress-client-0.3.5/datapress/extract.py
+-rw-r--r--   0 Ace        (501) staff       (20)      551 2022-11-03 10:54:22.000000 datapress-client-0.3.5/LICENSE
+-rw-r--r--   0 Ace        (501) staff       (20)       27 2022-11-03 10:54:22.000000 datapress-client-0.3.5/MANIFEST.in
+-rw-r--r--   0 Ace        (501) staff       (20)       48 2022-11-03 10:54:22.000000 datapress-client-0.3.5/README.md
+-rw-r--r--   0 Ace        (501) staff       (20)     1201 2023-05-12 15:15:21.000000 datapress-client-0.3.5/setup.py
+-rw-r--r--   0 Ace        (501) staff       (20)       79 2023-05-12 15:15:29.000000 datapress-client-0.3.5/setup.cfg
+drwxr-xr-x   0 Ace        (501) staff       (20)        0 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress_client.egg-info/
+-rw-r--r--   0 Ace        (501) staff       (20)      489 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress_client.egg-info/PKG-INFO
+-rw-r--r--   0 Ace        (501) staff       (20)        1 2023-02-10 08:47:58.000000 datapress-client-0.3.5/datapress_client.egg-info/not-zip-safe
+-rw-r--r--   0 Ace        (501) staff       (20)      497 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress_client.egg-info/SOURCES.txt
+-rw-r--r--   0 Ace        (501) staff       (20)       55 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress_client.egg-info/requires.txt
+-rw-r--r--   0 Ace        (501) staff       (20)       10 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress_client.egg-info/top_level.txt
+-rw-r--r--   0 Ace        (501) staff       (20)        1 2023-05-12 15:15:29.000000 datapress-client-0.3.5/datapress_client.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `datapress-client-0.3.4/LICENSE` & `datapress-client-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/datapress/api.py` & `datapress-client-0.3.5/datapress/api.py`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/datapress/dataset.py` & `datapress-client-0.3.5/datapress/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,17 @@
         #     "key": "[path to upload]",
         #     "Policy": "[hashed policy]",
         #     "X-Amz-Signature": "[my signature]"
         #   }
         # }
 
         # Upload the file to the one-time URL
-        logger.debug('POST %s', presign['url'])
-        requests.post(presign['url'], data=presign['fields'], files={
+        url = presign['url'] + presign['fields']['bucket']
+        logger.debug('POST %s', url)
+        requests.post(url, data=presign['fields'], files={
             'file': csv_data
         })
         return presign['fields']['key']
 
     def commit_table(self, name, df):
         """
         Upload a table to DataPress.
```

### Comparing `datapress-client-0.3.4/datapress/extract.py` & `datapress-client-0.3.5/datapress/extract.py`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/datapress/geo.py` & `datapress-client-0.3.5/datapress/geo.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             type = 'CTRY11CD'
         case 'country':
             type = 'CTRY11NM'
         case 'nomis codes':
             type = 'NOMISCD'
 
     filename = os.path.join(DIRNAME, 'static', 'lsoa_lookup.csv')
-    frame = pd.read_csv(filename)
+    frame = pd.read_csv(filename, dtype=str)
     for col in frame.columns:
         list = frame[col].unique().tolist()
         if place in list:
             type_of_place = col
             break
     frame = frame[frame[type_of_place] == place]
     return frame[type].unique().tolist()
```

### Comparing `datapress-client-0.3.4/datapress/nomis.py` & `datapress-client-0.3.5/datapress/nomis.py`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/datapress/ons.py` & `datapress-client-0.3.5/datapress/ons.py`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/datapress/static/lsoa_lookup.csv` & `datapress-client-0.3.5/datapress/static/lsoa_lookup.csv`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/datapress/utils.py` & `datapress-client-0.3.5/datapress/utils.py`

 * *Files identical despite different names*

### Comparing `datapress-client-0.3.4/setup.py` & `datapress-client-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     long_description_content_type='text/markdown',
     version=about['__version__'],
     author='DataPress Ltd.',
     author_email='admin@datapress.com',
     url='https://github.com/datapressio/datapress-client',
     packages=['datapress'],
     include_package_data=True,
-    python_requires=">=3.7.*",
+    python_requires=">=3.7",
     install_requires=[
         'pandas>=1.5',
         'requests',
         'xlrd',
         'openpyxl',
         'python-dotenv',
         'odfpy',
```


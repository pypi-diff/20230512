# Comparing `tmp/easy_reed-0.9.1.tar.gz` & `tmp/easy_reed-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_reed-0.9.1.tar", last modified: Tue May  2 15:30:49 2023, max compression
+gzip compressed data, was "easy_reed-0.9.2.tar", last modified: Fri May 12 00:04:32 2023, max compression
```

## Comparing `easy_reed-0.9.1.tar` & `easy_reed-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 15:30:49.001423 easy_reed-0.9.1/
--rw-r--r--   0 reed      (1000) reed      (1000)    35128 2023-04-05 22:29:50.000000 easy_reed-0.9.1/LICENSE.txt
--rw-r--r--   0 reed      (1000) reed      (1000)     5948 2023-05-02 15:30:49.001423 easy_reed-0.9.1/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)     5653 2023-05-02 04:39:25.000000 easy_reed-0.9.1/README.md
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 15:30:49.001423 easy_reed-0.9.1/easy_reed/
--rw-r--r--   0 reed      (1000) reed      (1000)      781 2023-05-02 03:26:11.000000 easy_reed-0.9.1/easy_reed/__init__.py
--rw-r--r--   0 reed      (1000) reed      (1000)     1502 2023-05-02 03:26:49.000000 easy_reed-0.9.1/easy_reed/_logger.py
--rw-r--r--   0 reed      (1000) reed      (1000)    12104 2023-05-01 22:27:00.000000 easy_reed-0.9.1/easy_reed/config_object.py
--rw-r--r--   0 reed      (1000) reed      (1000)    11131 2023-04-26 19:15:42.000000 easy_reed-0.9.1/easy_reed/config_reader.py
--rw-r--r--   0 reed      (1000) reed      (1000)     5381 2023-05-02 03:25:44.000000 easy_reed-0.9.1/easy_reed/environment.py
--rw-r--r--   0 reed      (1000) reed      (1000)     7915 2023-04-28 16:17:58.000000 easy_reed-0.9.1/easy_reed/namespace.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 15:30:49.001423 easy_reed-0.9.1/easy_reed.egg-info/
--rw-r--r--   0 reed      (1000) reed      (1000)     5948 2023-05-02 15:30:48.000000 easy_reed-0.9.1/easy_reed.egg-info/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)      417 2023-05-02 15:30:48.000000 easy_reed-0.9.1/easy_reed.egg-info/SOURCES.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-02 15:30:48.000000 easy_reed-0.9.1/easy_reed.egg-info/dependency_links.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       10 2023-05-02 15:30:48.000000 easy_reed-0.9.1/easy_reed.egg-info/top_level.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-04-05 22:12:15.000000 easy_reed-0.9.1/pyproject.toml
--rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-02 15:30:49.001423 easy_reed-0.9.1/setup.cfg
--rw-r--r--   0 reed      (1000) reed      (1000)      685 2023-05-02 15:30:35.000000 easy_reed-0.9.1/setup.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 15:30:49.001423 easy_reed-0.9.1/test/
--rw-r--r--   0 reed      (1000) reed      (1000)     2258 2023-05-01 23:51:02.000000 easy_reed-0.9.1/test/test_config.py
--rw-r--r--   0 reed      (1000) reed      (1000)     6135 2023-04-28 19:29:10.000000 easy_reed-0.9.1/test/test_config_reader.py
--rw-r--r--   0 reed      (1000) reed      (1000)     3289 2023-04-16 19:59:10.000000 easy_reed-0.9.1/test/test_environment.py
--rw-r--r--   0 reed      (1000) reed      (1000)     2270 2023-04-28 16:17:14.000000 easy_reed-0.9.1/test/test_namespace.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-12 00:04:32.146679 easy_reed-0.9.2/
+-rw-r--r--   0 reed      (1000) reed      (1000)    35128 2023-04-05 22:29:50.000000 easy_reed-0.9.2/LICENSE.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)     5948 2023-05-12 00:04:32.146679 easy_reed-0.9.2/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)     5653 2023-05-02 04:39:25.000000 easy_reed-0.9.2/README.md
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-12 00:04:32.146679 easy_reed-0.9.2/easy_reed/
+-rw-r--r--   0 reed      (1000) reed      (1000)      781 2023-05-02 03:26:11.000000 easy_reed-0.9.2/easy_reed/__init__.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     1514 2023-05-12 00:04:14.000000 easy_reed-0.9.2/easy_reed/_logger.py
+-rw-r--r--   0 reed      (1000) reed      (1000)    12104 2023-05-01 22:27:00.000000 easy_reed-0.9.2/easy_reed/config_object.py
+-rw-r--r--   0 reed      (1000) reed      (1000)    11131 2023-04-26 19:15:42.000000 easy_reed-0.9.2/easy_reed/config_reader.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     5381 2023-05-02 03:25:44.000000 easy_reed-0.9.2/easy_reed/environment.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     7915 2023-04-28 16:17:58.000000 easy_reed-0.9.2/easy_reed/namespace.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-12 00:04:32.146679 easy_reed-0.9.2/easy_reed.egg-info/
+-rw-r--r--   0 reed      (1000) reed      (1000)     5948 2023-05-12 00:04:32.000000 easy_reed-0.9.2/easy_reed.egg-info/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)      417 2023-05-12 00:04:32.000000 easy_reed-0.9.2/easy_reed.egg-info/SOURCES.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-12 00:04:32.000000 easy_reed-0.9.2/easy_reed.egg-info/dependency_links.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       10 2023-05-12 00:04:32.000000 easy_reed-0.9.2/easy_reed.egg-info/top_level.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-04-05 22:12:15.000000 easy_reed-0.9.2/pyproject.toml
+-rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-12 00:04:32.146679 easy_reed-0.9.2/setup.cfg
+-rw-r--r--   0 reed      (1000) reed      (1000)      685 2023-05-12 00:04:19.000000 easy_reed-0.9.2/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-12 00:04:32.146679 easy_reed-0.9.2/test/
+-rw-r--r--   0 reed      (1000) reed      (1000)     2258 2023-05-01 23:51:02.000000 easy_reed-0.9.2/test/test_config.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     6135 2023-04-28 19:29:10.000000 easy_reed-0.9.2/test/test_config_reader.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     3289 2023-04-16 19:59:10.000000 easy_reed-0.9.2/test/test_environment.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     2270 2023-04-28 16:17:14.000000 easy_reed-0.9.2/test/test_namespace.py
```

### Comparing `easy_reed-0.9.1/LICENSE.txt` & `easy_reed-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/PKG-INFO` & `easy_reed-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_reed
-Version: 0.9.1
+Version: 0.9.2
 Summary: Config Library for cross module configuration
 Home-page: https://github.com/rns350/easy-reed
 Author: Reed Schick
 Author-email: rns350@nyu.edu
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `easy_reed-0.9.1/README.md` & `easy_reed-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/easy_reed/__init__.py` & `easy_reed-0.9.2/easy_reed/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/easy_reed/_logger.py` & `easy_reed-0.9.2/easy_reed/_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 # Define the log and date format for the log handlers, and create a Formatter
 log_format = f'%(levelname)s | %(asctime)s | {__name__} | line %(lineno)d | %(message)s'
 date_format = '%m/%d/%Y %I:%M:%S %p'
 formatter = logging.Formatter(fmt=log_format, datefmt=date_format)
 
 # Initialize the stream and file handlers - we will attach these to the logger
 stream_handler = logging.StreamHandler()
-file_handler = logging.FileHandler(filename=f'logs/{date.today()}-logs.txt')
+# file_handler = logging.FileHandler(filename=f'logs/{date.today()}-logs.txt')
 
 # set the formatter for the handlers to the one created above
 stream_handler.setFormatter(formatter)
-file_handler.setFormatter(formatter)
+# file_handler.setFormatter(formatter)
 
 # create the logger and add the details
 logger = logging.getLogger(__name__)
 logger.addHandler(stream_handler)
-if LOG_LOCATION != "":
-    if not os.path.exists(LOG_LOCATION):
-        os.mkdir(LOG_LOCATION)
-    logger.addHandler(file_handler)
+# if LOG_LOCATION != "":
+#     if not os.path.exists(LOG_LOCATION):
+#         os.mkdir(LOG_LOCATION)
+#     logger.addHandler(file_handler)
```

### Comparing `easy_reed-0.9.1/easy_reed/config_object.py` & `easy_reed-0.9.2/easy_reed/config_object.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/easy_reed/config_reader.py` & `easy_reed-0.9.2/easy_reed/config_reader.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/easy_reed/environment.py` & `easy_reed-0.9.2/easy_reed/environment.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/easy_reed/namespace.py` & `easy_reed-0.9.2/easy_reed/namespace.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/easy_reed.egg-info/PKG-INFO` & `easy_reed-0.9.2/easy_reed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-reed
-Version: 0.9.1
+Version: 0.9.2
 Summary: Config Library for cross module configuration
 Home-page: https://github.com/rns350/easy-reed
 Author: Reed Schick
 Author-email: rns350@nyu.edu
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `easy_reed-0.9.1/setup.py` & `easy_reed-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup_info = dict(
   name='easy_reed',
   python_requires=">=3.7",
-  version='0.9.1',
+  version='0.9.2',
   description='Config Library for cross module configuration',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author="Reed Schick",
   author_email='rns350@nyu.edu',
   url='https://github.com/rns350/easy-reed',
   packages=find_packages(
```

### Comparing `easy_reed-0.9.1/test/test_config.py` & `easy_reed-0.9.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/test/test_config_reader.py` & `easy_reed-0.9.2/test/test_config_reader.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/test/test_environment.py` & `easy_reed-0.9.2/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `easy_reed-0.9.1/test/test_namespace.py` & `easy_reed-0.9.2/test/test_namespace.py`

 * *Files identical despite different names*


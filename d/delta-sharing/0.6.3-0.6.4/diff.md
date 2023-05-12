# Comparing `tmp/delta-sharing-0.6.3.tar.gz` & `tmp/delta-sharing-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delta-sharing-0.6.3.tar", last modified: Thu Feb 16 19:04:45 2023, max compression
+gzip compressed data, was "dist/delta-sharing-0.6.4.tar", last modified: Fri May 12 09:47:27 2023, max compression
```

## Comparing `delta-sharing-0.6.3.tar` & `delta-sharing-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-02-16 19:04:45.991129 delta-sharing-0.6.3/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-02-16 19:04:45.990122 delta-sharing-0.6.3/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/README.md
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-02-16 19:04:45.987145 delta-sharing-0.6.3/delta_sharing/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1099 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/__init__.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/_yarl_patch.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/converter.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    11137 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/delta_sharing.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7819 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/protocol.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7712 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/reader.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    14850 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/delta_sharing/rest_client.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-02-16 19:01:32.000000 delta-sharing-0.6.3/delta_sharing/version.py
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-02-16 19:04:45.989638 delta-sharing-0.6.3/delta_sharing.egg-info/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-02-16 19:04:45.000000 delta-sharing-0.6.3/delta_sharing.egg-info/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)      419 2023-02-16 19:04:45.000000 delta-sharing-0.6.3/delta_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-02-16 19:04:45.000000 delta-sharing-0.6.3/delta_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-02-16 19:04:45.000000 delta-sharing-0.6.3/delta_sharing.egg-info/requires.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-02-16 19:04:45.000000 delta-sharing-0.6.3/delta_sharing.egg-info/top_level.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-02-16 19:04:45.991229 delta-sharing-0.6.3/setup.cfg
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-02-16 17:58:34.000000 delta-sharing-0.6.3/setup.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2400 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/README.md
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1099 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/__init__.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/_yarl_patch.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/converter.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    11137 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/delta_sharing.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7819 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/protocol.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7712 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/reader.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    14850 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/delta_sharing/rest_client.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-05-12 09:45:31.000000 delta-sharing-0.6.4/delta_sharing/version.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing.egg-info/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2400 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      419 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing.egg-info/requires.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/delta_sharing.egg-info/top_level.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-05-12 09:47:27.000000 delta-sharing-0.6.4/setup.cfg
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-05-12 09:10:25.000000 delta-sharing-0.6.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `delta-sharing-0.6.3/PKG-INFO` & `delta-sharing-0.6.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
 Project-URL: Issues, https://github.com/delta-io/delta-sharing/issues
+Description: # Delta Sharing
+        
+        [Delta Sharing](https://delta.io/sharing) is an open protocol for secure real-time exchange of large datasets, which enables secure data sharing across different computing platforms. It lets organizations share access to existing [Delta Lake](https://delta.io) and [Apache Parquet](https://parquet.apache.org) tables with other organizations, who can then directly read the table in Pandas, Apache Spark, or any other software that implements the open protocol.
+        
+        This is the Python client library for Delta Sharing, which lets you load shared tables as [pandas](https://pandas.pydata.org/) DataFrames or as [Apache Spark](http://spark.apache.org/) DataFrames if running in PySpark with the [Apache Spark Connector library](https://github.com/delta-io/delta-sharing#set-up-apache-spark).
+        
+        ## Installation and Usage
+        
+        1. Install using `pip install delta-sharing`.
+        2. To use the Python Connector, see [the project docs](https://github.com/delta-io/delta-sharing) for details.
+        
+        ## Documentation
+        
+        This README only contains basic information about the Delta Sharing Python Connector. Please read [the project documentation](https://github.com/delta-io/delta-sharing) for full usage details.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,22 +36,7 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: s3
 Provides-Extra: abfs
 Provides-Extra: adl
 Provides-Extra: gcs
 Provides-Extra: gs
-
-# Delta Sharing
-
-[Delta Sharing](https://delta.io/sharing) is an open protocol for secure real-time exchange of large datasets, which enables secure data sharing across different computing platforms. It lets organizations share access to existing [Delta Lake](https://delta.io) and [Apache Parquet](https://parquet.apache.org) tables with other organizations, who can then directly read the table in Pandas, Apache Spark, or any other software that implements the open protocol.
-
-This is the Python client library for Delta Sharing, which lets you load shared tables as [pandas](https://pandas.pydata.org/) DataFrames or as [Apache Spark](http://spark.apache.org/) DataFrames if running in PySpark with the [Apache Spark Connector library](https://github.com/delta-io/delta-sharing#set-up-apache-spark).
-
-## Installation and Usage
-
-1. Install using `pip install delta-sharing`.
-2. To use the Python Connector, see [the project docs](https://github.com/delta-io/delta-sharing) for details.
-
-## Documentation
-
-This README only contains basic information about the Delta Sharing Python Connector. Please read [the project documentation](https://github.com/delta-io/delta-sharing) for full usage details.
```

### Comparing `delta-sharing-0.6.3/README.md` & `delta-sharing-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/__init__.py` & `delta-sharing-0.6.4/delta_sharing/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/_yarl_patch.py` & `delta-sharing-0.6.4/delta_sharing/_yarl_patch.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/converter.py` & `delta-sharing-0.6.4/delta_sharing/converter.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/delta_sharing.py` & `delta-sharing-0.6.4/delta_sharing/delta_sharing.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/protocol.py` & `delta-sharing-0.6.4/delta_sharing/protocol.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/reader.py` & `delta-sharing-0.6.4/delta_sharing/reader.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/rest_client.py` & `delta-sharing-0.6.4/delta_sharing/rest_client.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.3/delta_sharing/version.py` & `delta-sharing-0.6.4/delta_sharing/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
```

### Comparing `delta-sharing-0.6.3/delta_sharing.egg-info/PKG-INFO` & `delta-sharing-0.6.4/delta_sharing.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
 Project-URL: Issues, https://github.com/delta-io/delta-sharing/issues
+Description: # Delta Sharing
+        
+        [Delta Sharing](https://delta.io/sharing) is an open protocol for secure real-time exchange of large datasets, which enables secure data sharing across different computing platforms. It lets organizations share access to existing [Delta Lake](https://delta.io) and [Apache Parquet](https://parquet.apache.org) tables with other organizations, who can then directly read the table in Pandas, Apache Spark, or any other software that implements the open protocol.
+        
+        This is the Python client library for Delta Sharing, which lets you load shared tables as [pandas](https://pandas.pydata.org/) DataFrames or as [Apache Spark](http://spark.apache.org/) DataFrames if running in PySpark with the [Apache Spark Connector library](https://github.com/delta-io/delta-sharing#set-up-apache-spark).
+        
+        ## Installation and Usage
+        
+        1. Install using `pip install delta-sharing`.
+        2. To use the Python Connector, see [the project docs](https://github.com/delta-io/delta-sharing) for details.
+        
+        ## Documentation
+        
+        This README only contains basic information about the Delta Sharing Python Connector. Please read [the project documentation](https://github.com/delta-io/delta-sharing) for full usage details.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,22 +36,7 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: s3
 Provides-Extra: abfs
 Provides-Extra: adl
 Provides-Extra: gcs
 Provides-Extra: gs
-
-# Delta Sharing
-
-[Delta Sharing](https://delta.io/sharing) is an open protocol for secure real-time exchange of large datasets, which enables secure data sharing across different computing platforms. It lets organizations share access to existing [Delta Lake](https://delta.io) and [Apache Parquet](https://parquet.apache.org) tables with other organizations, who can then directly read the table in Pandas, Apache Spark, or any other software that implements the open protocol.
-
-This is the Python client library for Delta Sharing, which lets you load shared tables as [pandas](https://pandas.pydata.org/) DataFrames or as [Apache Spark](http://spark.apache.org/) DataFrames if running in PySpark with the [Apache Spark Connector library](https://github.com/delta-io/delta-sharing#set-up-apache-spark).
-
-## Installation and Usage
-
-1. Install using `pip install delta-sharing`.
-2. To use the Python Connector, see [the project docs](https://github.com/delta-io/delta-sharing) for details.
-
-## Documentation
-
-This README only contains basic information about the Delta Sharing Python Connector. Please read [the project documentation](https://github.com/delta-io/delta-sharing) for full usage details.
```

### Comparing `delta-sharing-0.6.3/setup.py` & `delta-sharing-0.6.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pyspark-utilities-0.0.8.tar.gz` & `tmp/pyspark-utilities-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyspark-utilities-0.0.8.tar", last modified: Wed Nov 17 14:34:56 2021, max compression
+gzip compressed data, was "dist/pyspark-utilities-0.0.9.tar", last modified: Wed Nov 17 14:39:56 2021, max compression
```

## Comparing `pyspark-utilities-0.0.8.tar` & `pyspark-utilities-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:34:56.052798 pyspark-utilities-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      282 2021-11-17 14:34:56.052798 pyspark-utilities-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      271 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:34:56.051798 pyspark-utilities-0.0.8/pyspark_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)      282 2021-11-17 14:34:55.000000 pyspark-utilities-0.0.8/pyspark_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2021-11-17 14:34:55.000000 pyspark-utilities-0.0.8/pyspark_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-17 14:34:55.000000 pyspark-utilities-0.0.8/pyspark_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-11-17 14:34:55.000000 pyspark-utilities-0.0.8/pyspark_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-11-17 14:34:55.000000 pyspark-utilities-0.0.8/pyspark_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:34:56.052798 pyspark-utilities-0.0.8/pysparkutilities/
--rw-rw-rw-   0 root         (0) root         (0)      146 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/datastorage.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/ds_initializer.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/hdfs.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/hive.py
--rw-rw-rw-   0 root         (0) root         (0)     3143 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/presto.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/pysparkutilities/spark_initializer.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-17 14:34:56.053798 pyspark-utilities-0.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      413 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:34:56.052798 pyspark-utilities-0.0.8/test/
--rw-rw-rw-   0 root         (0) root         (0)      967 2021-11-17 14:34:47.000000 pyspark-utilities-0.0.8/test/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:39:56.495665 pyspark-utilities-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      282 2021-11-17 14:39:56.495665 pyspark-utilities-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      271 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:39:56.494665 pyspark-utilities-0.0.9/pyspark_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      282 2021-11-17 14:39:56.000000 pyspark-utilities-0.0.9/pyspark_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2021-11-17 14:39:56.000000 pyspark-utilities-0.0.9/pyspark_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-17 14:39:56.000000 pyspark-utilities-0.0.9/pyspark_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-11-17 14:39:56.000000 pyspark-utilities-0.0.9/pyspark_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2021-11-17 14:39:56.000000 pyspark-utilities-0.0.9/pyspark_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:39:56.494665 pyspark-utilities-0.0.9/pysparkutilities/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/datastorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/ds_initializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/hdfs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/hive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3143 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/presto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/pysparkutilities/spark_initializer.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-11-17 14:39:56.495665 pyspark-utilities-0.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      413 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-17 14:39:56.494665 pyspark-utilities-0.0.9/test/
+-rw-rw-rw-   0 root         (0) root         (0)      967 2021-11-17 14:39:48.000000 pyspark-utilities-0.0.9/test/test.py
```

### Comparing `pyspark-utilities-0.0.8/pysparkutilities/ds_initializer.py` & `pyspark-utilities-0.0.9/pysparkutilities/ds_initializer.py`

 * *Files identical despite different names*

### Comparing `pyspark-utilities-0.0.8/pysparkutilities/filesystem.py` & `pyspark-utilities-0.0.9/pysparkutilities/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         else:
             output_dataset = output_dest
         delimiter = self.args["delimiter"] if "delimiter" in self.args else ","
         output_file_format = self.args["outputFileFormat"] if "outputFileFormat" in self.args else "csv"
 
         if "save_dataset_with_pandas" in self.args:
 
-            df.toPandas().to_csv(output_dataset, delimiter=delimiter, index=False)
+            df.toPandas().to_csv(output_dataset, sep=delimiter, index=False)
 
         else:
 
             df.write.options(delimiter=delimiter).\
                 mode('overwrite').\
                 option("header", True).\
                 save(output_dataset, format=output_file_format)
```

### Comparing `pyspark-utilities-0.0.8/pysparkutilities/hdfs.py` & `pyspark-utilities-0.0.9/pysparkutilities/hdfs.py`

 * *Files identical despite different names*

### Comparing `pyspark-utilities-0.0.8/pysparkutilities/hive.py` & `pyspark-utilities-0.0.9/pysparkutilities/hive.py`

 * *Files identical despite different names*

### Comparing `pyspark-utilities-0.0.8/pysparkutilities/presto.py` & `pyspark-utilities-0.0.9/pysparkutilities/presto.py`

 * *Files identical despite different names*

### Comparing `pyspark-utilities-0.0.8/pysparkutilities/spark_initializer.py` & `pyspark-utilities-0.0.9/pysparkutilities/spark_initializer.py`

 * *Files identical despite different names*

### Comparing `pyspark-utilities-0.0.8/test/test.py` & `pyspark-utilities-0.0.9/test/test.py`

 * *Files identical despite different names*


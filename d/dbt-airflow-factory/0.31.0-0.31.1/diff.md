# Comparing `tmp/dbt-airflow-factory-0.31.0.tar.gz` & `tmp/dbt-airflow-factory-0.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-airflow-factory-0.31.0.tar", last modified: Mon Mar 27 10:54:32 2023, max compression
+gzip compressed data, was "dbt-airflow-factory-0.31.1.tar", last modified: Fri May 12 06:14:58 2023, max compression
```

## Comparing `dbt-airflow-factory-0.31.0.tar` & `dbt-airflow-factory-0.31.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/airflow_dag_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/bash/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/bash/bash_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/bash/bash_parameters_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/builder_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/dbt_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/ecs/ecs_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/ecs/ecs_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/ecs/ecs_parameters_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/ingestion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/k8s_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/notifications/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-03-27 10:54:32.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-27 10:54:32.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:54:32.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:54:32.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-27 10:54:32.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 10:54:32.000000 dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-27 10:54:32.133582 dbt-airflow-factory-0.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-27 10:54:31.000000 dbt-airflow-factory-0.31.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.128928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/airflow_dag_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_parameters_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/builder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/dbt_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_parameters_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/ingestion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 06:14:58.000000 dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-12 06:14:58.132928 dbt-airflow-factory-0.31.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-12 06:14:56.000000 dbt-airflow-factory-0.31.1/setup.py
```

### Comparing `dbt-airflow-factory-0.31.0/LICENSE` & `dbt-airflow-factory-0.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/PKG-INFO` & `dbt-airflow-factory-0.31.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-airflow-factory
-Version: 0.31.0
+Version: 0.31.1
 Summary: Library to convert DBT manifest metadata to Airflow tasks
 Home-page: https://github.com/getindata/dbt-airflow-factory/
 Author: Piotr Pekala
 Author-email: piotr.pekala@getindata.com
 License: Apache Software License (Apache 2.0)
 Keywords: dbt airflow manifest parser python
 Platform: UNKNOWN
```

### Comparing `dbt-airflow-factory-0.31.0/README.md` & `dbt-airflow-factory-0.31.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/airflow_dag_factory.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/airflow_dag_factory.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/bash/bash_operator.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/bash/bash_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/builder_factory.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/builder_factory.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/config_utils.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/dbt_parameters.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/dbt_parameters.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/ecs/ecs_operator.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/ecs/ecs_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/ingestion.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/ingestion.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/k8s_operator.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/k8s_parameters.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     :type envs: Optional[Dict[str, str]]
     :param secrets: Kubernetes secrets to inject in the container.
         They can be exposed as environment vars or files in a volume.
     :type secrets: List[Secret]
     :param is_delete_operator_pod: What to do when the pod reaches its final
         state, or the execution is interrupted. If True: delete the pod.
     :type is_delete_operator_pod: bool
+    :param config_file: The path to the Kubernetes config file. (templated)
+        If not specified, default value is ``~/.kube/config``
+    :type config_file: Optional[str]
     :param execution_script: Script that will be executed inside pod.
     :type execution_script: str
     :param in_cluster: Run kubernetes client with in_cluster configuration.
     :type in_cluster: bool
     :param cluster_context: Context that points to kubernetes cluster.
         Ignored when in_cluster is True. If None, current-context is used.
     :type cluster_context: str
@@ -58,15 +61,15 @@
         labels: Optional[dict] = None,
         limit: Optional[dict] = None,
         requests: Optional[dict] = None,
         annotations: Optional[dict] = None,
         envs: Optional[Dict[str, str]] = None,
         secrets: Optional[List[Secret]] = None,
         is_delete_operator_pod: bool = True,
-        config_file: str = "~/.kube/config",
+        config_file: Optional[str] = None,
         execution_script: str = "dbt --no-write-json",
         in_cluster: Optional[bool] = None,
         cluster_context: Optional[str] = None,
         startup_timeout_seconds: int = 120,
         **kwargs: Any,
     ) -> None:
         self.namespace = namespace
```

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/k8s/k8s_parameters_loader.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/notifications/handler.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/notifications/handler.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/operator.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/builder.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/builder.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/gateway.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory/tasks_builder/graph.py` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory/tasks_builder/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/PKG-INFO` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-airflow-factory
-Version: 0.31.0
+Version: 0.31.1
 Summary: Library to convert DBT manifest metadata to Airflow tasks
 Home-page: https://github.com/getindata/dbt-airflow-factory/
 Author: Piotr Pekala
 Author-email: piotr.pekala@getindata.com
 License: Apache Software License (Apache 2.0)
 Keywords: dbt airflow manifest parser python
 Platform: UNKNOWN
```

### Comparing `dbt-airflow-factory-0.31.0/dbt_airflow_factory.egg-info/SOURCES.txt` & `dbt-airflow-factory-0.31.1/dbt_airflow_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.31.0/setup.cfg` & `dbt-airflow-factory-0.31.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.31.0
+current_version = 0.31.1
 
 [bumpversion:file:setup.py]
 
 [bumpversion:file:dbt_airflow_factory/__init__.py]
 
 [flake8]
 exclude = .git,__pycache__,build,dist,docs/source/conf.py
```

### Comparing `dbt-airflow-factory-0.31.0/setup.py` & `dbt-airflow-factory-0.31.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "myst-parser>=0.16, <0.17",
         "docutils<0.17",
     ],
 }
 
 setup(
     name="dbt-airflow-factory",
-    version="0.31.0",
+    version="0.31.1",
     description="Library to convert DBT manifest metadata to Airflow tasks",
     long_description=README,
     long_description_content_type="text/markdown",
     license="Apache Software License (Apache 2.0)",
     python_requires=">=3",
     classifiers=[
         "Development Status :: 3 - Alpha",
```


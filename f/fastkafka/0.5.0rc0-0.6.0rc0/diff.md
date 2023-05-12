# Comparing `tmp/fastkafka-0.5.0rc0.tar.gz` & `tmp/fastkafka-0.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.5.0rc0.tar", last modified: Fri Apr 14 15:25:23 2023, max compression
+gzip compressed data, was "fastkafka-0.6.0rc0.tar", last modified: Fri May 12 13:45:18 2023, max compression
```

## Comparing `fastkafka-0.5.0rc0.tar` & `fastkafka-0.6.0rc0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/
--rw-r--r--   0 davor     (1000) davor     (1000)    11357 2023-01-25 09:24:15.000000 fastkafka-0.5.0rc0/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-01-25 09:24:15.000000 fastkafka-0.5.0rc0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    32079 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)    30651 2023-04-14 15:23:47.000000 fastkafka-0.5.0rc0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.768181 fastkafka-0.5.0rc0/fastkafka/
--rw-rw-r--   0 davor     (1000) davor     (1000)      432 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_application/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_application/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    29758 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_application/app.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     7432 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_application/tester.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     1574 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_cli.py
--rw-r--r--   0 davor     (1000) davor     (1000)     3879 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_cli_docs.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      852 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_cli_testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3705 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9356 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
--rw-r--r--   0 davor     (1000) davor     (1000)    16362 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2940 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/benchmarking.py
--rw-r--r--   0 davor     (1000) davor     (1000)     4686 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_components/encoder/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    13092 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     1026 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2952 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4445 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_components/logger.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12567 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/meta.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3556 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     5066 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14740 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_docusaurus_helper.py
--rw-r--r--   0 davor     (1000) davor     (1000)    50547 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    68208 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_modidx.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     6039 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_server.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_testing/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_testing/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)    19775 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    17978 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12382 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4671 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      833 2023-04-14 15:21:00.000000 fastkafka-0.5.0rc0/fastkafka/testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.768181 fastkafka-0.5.0rc0/fastkafka.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    32079 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     1310 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      146 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-01-25 09:30:21.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      598 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       10 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)     1230 2023-04-14 15:19:31.000000 fastkafka-0.5.0rc0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3663 2023-04-14 15:19:15.000000 fastkafka-0.5.0rc0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/
+-rw-r--r--   0 davor     (1000) davor     (1000)    11864 2023-05-12 12:45:54.000000 fastkafka-0.6.0rc0/CONTRIBUTING.md
+-rw-r--r--   0 davor     (1000) davor     (1000)    11357 2023-01-25 09:24:15.000000 fastkafka-0.6.0rc0/LICENSE
+-rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-01-25 09:24:15.000000 fastkafka-0.6.0rc0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    29859 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/PKG-INFO
+-rw-r--r--   0 davor     (1000) davor     (1000)    28431 2023-04-21 14:13:44.000000 fastkafka-0.6.0rc0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.190037 fastkafka-0.6.0rc0/fastkafka/
+-rw-r--r--   0 davor     (1000) davor     (1000)      525 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.190037 fastkafka-0.6.0rc0/fastkafka/_application/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_application/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    31006 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_application/app.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     7688 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_application/tester.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1631 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_cli.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     3879 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_cli_docs.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      852 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_cli_testing.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/fastkafka/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3705 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/_subprocess.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    10188 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    16654 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     2940 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     4706 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/fastkafka/_components/encoder/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/encoder/__init__.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    13910 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/encoder/avro.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     1640 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_components/encoder/json.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     2952 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/helpers.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     4446 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/logger.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12567 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/meta.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     5930 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/producer_decorator.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     8081 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     5090 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_components/test_dependencies.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    17520 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_docusaurus_helper.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    50547 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    80310 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_modidx.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     6095 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/_server.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/fastkafka/_testing/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-05-12 13:44:38.000000 fastkafka-0.6.0rc0/fastkafka/_testing/__init__.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    19995 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    20456 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/in_memory_broker.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    12364 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     4671 2023-05-12 13:44:36.000000 fastkafka-0.6.0rc0/fastkafka/_testing/test_utils.py
+-rw-r--r--   0 davor     (1000) davor     (1000)      598 2023-05-12 13:44:37.000000 fastkafka-0.6.0rc0/fastkafka/encoder.py
+-rw-r--r--   0 davor     (1000) davor     (1000)      858 2023-05-12 13:44:35.000000 fastkafka-0.6.0rc0/fastkafka/testing.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-05-12 13:45:18.190037 fastkafka-0.6.0rc0/fastkafka.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    29859 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1387 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      146 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-01-25 09:30:21.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      611 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       10 2023-05-12 13:45:18.000000 fastkafka-0.6.0rc0/fastkafka.egg-info/top_level.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)     1231 2023-05-12 12:45:54.000000 fastkafka-0.6.0rc0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-05-12 13:45:18.194037 fastkafka-0.6.0rc0/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3682 2023-05-12 13:44:07.000000 fastkafka-0.6.0rc0/setup.py
```

### Comparing `fastkafka-0.5.0rc0/LICENSE` & `fastkafka-0.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/PKG-INFO` & `fastkafka-0.6.0rc0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.5.0rc0
+Version: 0.6.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -285,15 +285,14 @@
   a new `IrisPrediction` message using this value and then returns it.
   The framework will call the `IrisPrediction.json().encode("utf-8")`
   function on the returned value and produce it to the specified topic.
 
 ``` python
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
 async def on_input_data(msg: IrisInputData):
-    global model
     species_class = ml_models["iris_predictor"].predict(
         [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
     )[0]
 
     to_predictions(species_class)
 
 
@@ -337,19 +336,15 @@
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker starting
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched start() called()
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
@@ -358,27 +353,24 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['predictions']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
+    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
 We have created a Iris classification model and encapulated it into our
 fastkafka application. The app will consume the IrisInputData from the
@@ -401,14 +393,36 @@
 The service can be started using builtin faskafka run CLI command.
 Before we can do that, we will concatenate the code snippets from above
 and save them in a file `"application.py"`
 
 ``` python
 # content of the "application.py" file
 
+from contextlib import asynccontextmanager
+
+from sklearn.datasets import load_iris
+from sklearn.linear_model import LogisticRegression
+
+from fastkafka import FastKafka
+
+ml_models = {}
+
+
+@asynccontextmanager
+async def lifespan(app: FastKafka):
+    # Load the ML model
+    X, y = load_iris(return_X_y=True)
+    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
+        X, y
+    )
+    yield
+    # Clean up the ML models and release the resources
+    ml_models.clear()
+
+
 from pydantic import BaseModel, NonNegativeFloat, Field
 
 class IrisInputData(BaseModel):
     sepal_length: NonNegativeFloat = Field(
         ..., example=0.5, description="Sepal length in cm"
     )
     sepal_width: NonNegativeFloat = Field(
@@ -441,30 +455,30 @@
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
     title="Iris predictions",
     kafka_brokers=kafka_brokers,
+    lifespan=lifespan,
 )
 
-iris_species = ["setosa", "versicolor", "virginica"]
-
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
 async def on_input_data(msg: IrisInputData):
-    global model
-    species_class = model.predict([
-          [msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]
-        ])[0]
+    species_class = ml_models["iris_predictor"].predict(
+        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
+    )[0]
 
     to_predictions(species_class)
 
 
 @kafka_app.produces(topic="predictions")
 def to_predictions(species_class: int) -> IrisPrediction:
+    iris_species = ["setosa", "versicolor", "virginica"]
+
     prediction = IrisPrediction(species=iris_species[species_class])
     return prediction
 ```
 
 To run the service, you will need a running Kafka broker on localhost as
 specified in the `kafka_brokers` parameter above. We can start the Kafka
 broker locally using the
@@ -514,81 +528,63 @@
 fastkafka run --num-workers=2 --kafka-broker localhost application:kafka_app
 ```
 
 In the above command, we use `--num-workers` option to specify how many
 workers to launch and we use `--kafka-broker` option to specify which
 kafka broker configuration to use from earlier specified `kafka_brokers`
 
-    [558863]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [558863]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
-    [558865]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [558865]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [558865]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [558865]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [558863]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [558863]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [558863]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [558863]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [558865]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [558865]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [558865]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.26.0.2', 9092)
-    [558863]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.26.0.2', 9092)
-    [558865]: [ERROR] aiokafka: Unable to update metadata from [0]
-    [558863]: [ERROR] aiokafka: Unable to update metadata from [0]
+    [801767]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [801765]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [801767]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [801765]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [801767]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [801767]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [801765]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [801765]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [801765]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [801765]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [801767]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [801767]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [801767]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
+    [801765]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
+    [801767]: [ERROR] aiokafka: Unable to update metadata from [0]
+    [801765]: [ERROR] aiokafka: Unable to update metadata from [0]
     ^C
     Starting process cleanup, this may take a few seconds...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 558863...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 558865...
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
-    [INFO] fastkafka._server: terminate_asyncio_process(): Process 558863 was already terminated.
-    [INFO] fastkafka._server: terminate_asyncio_process(): Process 558865 was already terminated.
+    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801765...
+    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801767...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
 
 You need to interupt running of the cell above by selecting
 `Runtime->Interupt execution` on the toolbar above.
 
 Finally, we can stop the local Kafka Broker:
 
 ``` python
 broker.stop()
 ```
 
     [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): entering...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 558265...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 558265 was already terminated.
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 557885...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 557885 was already terminated.
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 801303...
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 801303 was already terminated.
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 800930...
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 800930 was already terminated.
     [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): exited.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
@@ -604,15 +600,14 @@
 To generate the documentation programatically you just need to call the
 folloving command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: Old async specifications at '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml' does not exist.
     [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
     [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
     [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
@@ -621,16 +616,16 @@
 with:
 
 ``` sh
 ls -l asyncapi
 ```
 
     total 8
-    drwxrwxr-x 4 tvrtko tvrtko 4096 Apr  5 08:02 docs
-    drwxrwxr-x 2 tvrtko tvrtko 4096 Apr  5 08:02 spec
+    drwxrwxr-x 4 kumaran kumaran 4096 Mar 21 09:14 docs
+    drwxrwxr-x 2 kumaran kumaran 4096 Mar 21 09:14 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
```

### Comparing `fastkafka-0.5.0rc0/README.md` & `fastkafka-0.6.0rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: fastkafka
+Version: 0.6.0rc0
+Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
+Home-page: https://github.com/airtai/fastkafka
+Author: airt
+Author-email: info@airt.ai
+License: Apache Software License 2.0
+Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
+Project-URL: CI, https://github.com/airtai/fastkafka/actions
+Project-URL: Documentation, https://fastkafka.airt.ai/
+Project-URL: Tutorial, https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb
+Keywords: nbdev jupyter notebook python kafka
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: avro
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
 FastKafka
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <b>Effortless Kafka integration for your web services</b>
 
@@ -255,15 +285,14 @@
   a new `IrisPrediction` message using this value and then returns it.
   The framework will call the `IrisPrediction.json().encode("utf-8")`
   function on the returned value and produce it to the specified topic.
 
 ``` python
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
 async def on_input_data(msg: IrisInputData):
-    global model
     species_class = ml_models["iris_predictor"].predict(
         [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
     )[0]
 
     to_predictions(species_class)
 
 
@@ -307,19 +336,15 @@
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker starting
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched start() called()
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
@@ -328,27 +353,24 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['predictions']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
+    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
 We have created a Iris classification model and encapulated it into our
 fastkafka application. The app will consume the IrisInputData from the
@@ -371,14 +393,36 @@
 The service can be started using builtin faskafka run CLI command.
 Before we can do that, we will concatenate the code snippets from above
 and save them in a file `"application.py"`
 
 ``` python
 # content of the "application.py" file
 
+from contextlib import asynccontextmanager
+
+from sklearn.datasets import load_iris
+from sklearn.linear_model import LogisticRegression
+
+from fastkafka import FastKafka
+
+ml_models = {}
+
+
+@asynccontextmanager
+async def lifespan(app: FastKafka):
+    # Load the ML model
+    X, y = load_iris(return_X_y=True)
+    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
+        X, y
+    )
+    yield
+    # Clean up the ML models and release the resources
+    ml_models.clear()
+
+
 from pydantic import BaseModel, NonNegativeFloat, Field
 
 class IrisInputData(BaseModel):
     sepal_length: NonNegativeFloat = Field(
         ..., example=0.5, description="Sepal length in cm"
     )
     sepal_width: NonNegativeFloat = Field(
@@ -411,30 +455,30 @@
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
     title="Iris predictions",
     kafka_brokers=kafka_brokers,
+    lifespan=lifespan,
 )
 
-iris_species = ["setosa", "versicolor", "virginica"]
-
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
 async def on_input_data(msg: IrisInputData):
-    global model
-    species_class = model.predict([
-          [msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]
-        ])[0]
+    species_class = ml_models["iris_predictor"].predict(
+        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
+    )[0]
 
     to_predictions(species_class)
 
 
 @kafka_app.produces(topic="predictions")
 def to_predictions(species_class: int) -> IrisPrediction:
+    iris_species = ["setosa", "versicolor", "virginica"]
+
     prediction = IrisPrediction(species=iris_species[species_class])
     return prediction
 ```
 
 To run the service, you will need a running Kafka broker on localhost as
 specified in the `kafka_brokers` parameter above. We can start the Kafka
 broker locally using the
@@ -484,81 +528,63 @@
 fastkafka run --num-workers=2 --kafka-broker localhost application:kafka_app
 ```
 
 In the above command, we use `--num-workers` option to specify how many
 workers to launch and we use `--kafka-broker` option to specify which
 kafka broker configuration to use from earlier specified `kafka_brokers`
 
-    [558863]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [558863]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
-    [558865]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [558865]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [558865]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [558865]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [558863]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [558863]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [558863]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [558863]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [558865]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [558865]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [558865]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.26.0.2', 9092)
-    [558863]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.26.0.2', 9092)
-    [558865]: [ERROR] aiokafka: Unable to update metadata from [0]
-    [558863]: [ERROR] aiokafka: Unable to update metadata from [0]
+    [801767]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [801765]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [801767]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [801765]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [801767]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [801767]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [801765]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [801765]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [801765]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [801765]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [801767]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [801767]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [801767]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
+    [801765]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
+    [801767]: [ERROR] aiokafka: Unable to update metadata from [0]
+    [801765]: [ERROR] aiokafka: Unable to update metadata from [0]
     ^C
     Starting process cleanup, this may take a few seconds...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 558863...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 558865...
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
-    [INFO] fastkafka._server: terminate_asyncio_process(): Process 558863 was already terminated.
-    [INFO] fastkafka._server: terminate_asyncio_process(): Process 558865 was already terminated.
+    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801765...
+    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801767...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
 
 You need to interupt running of the cell above by selecting
 `Runtime->Interupt execution` on the toolbar above.
 
 Finally, we can stop the local Kafka Broker:
 
 ``` python
 broker.stop()
 ```
 
     [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): entering...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 558265...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 558265 was already terminated.
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 557885...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 557885 was already terminated.
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 801303...
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 801303 was already terminated.
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 800930...
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 800930 was already terminated.
     [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): exited.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
@@ -574,15 +600,14 @@
 To generate the documentation programatically you just need to call the
 folloving command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: Old async specifications at '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml' does not exist.
     [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
     [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
     [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
@@ -591,16 +616,16 @@
 with:
 
 ``` sh
 ls -l asyncapi
 ```
 
     total 8
-    drwxrwxr-x 4 tvrtko tvrtko 4096 Apr  5 08:02 docs
-    drwxrwxr-x 2 tvrtko tvrtko 4096 Apr  5 08:02 spec
+    drwxrwxr-x 4 kumaran kumaran 4096 Mar 21 09:14 docs
+    drwxrwxr-x 2 kumaran kumaran 4096 Mar 21 09:14 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -675,7 +700,9 @@
 A permissive license whose main conditions require preservation of
 copyright and license notices. Contributors provide an express grant of
 patent rights. Licensed works, modifications, and larger works may be
 distributed under different terms and without source code.
 
 The full text of the license can be found
 [here](https://raw.githubusercontent.com/airtai/fastkafka/main/LICENSE).
+
+
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_application/app.py` & `fastkafka-0.6.0rc0/fastkafka/_application/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     KafkaServiceInfo,
     export_async_spec,
 )
 from .._components.benchmarking import _benchmark
 from .._components.logger import get_logger
 from .._components.meta import delegates, export, filter_using_signature, patch
 from .._components.producer_decorator import ProduceCallable, producer_decorator
+from .._components.task_streaming import StreamExecutor
 
 # %% ../../nbs/015_FastKafka.ipynb 3
 logger = get_logger(__name__)
 
 # %% ../../nbs/015_FastKafka.ipynb 9
 @delegates(AIOKafkaConsumer, but=["bootstrap_servers"])
 @delegates(AIOKafkaProducer, but=["bootstrap_servers"], keep=True)
@@ -84,15 +85,15 @@
     Args:
         kafka_brokers: Kafka brokers
 
     """
     if kafka_brokers is None:
         retval: KafkaBrokers = KafkaBrokers(
             brokers={
-                "localhost": KafkaBroker(
+                "localhost": KafkaBroker(  # type: ignore
                     url="https://localhost",
                     description="Local (dev) Kafka broker",
                     port="9092",
                 )
             }
         )
     else:
@@ -128,15 +129,15 @@
 
 # %% ../../nbs/015_FastKafka.ipynb 16
 def _get_contact_info(
     name: str = "Author",
     url: str = "https://www.google.com",
     email: str = "noreply@gmail.com",
 ) -> ContactInfo:
-    return ContactInfo(name=name, url=url, email=email)
+    return ContactInfo(name=name, url=url, email=email)  # type: ignore
 
 # %% ../../nbs/015_FastKafka.ipynb 18
 I = TypeVar("I", bound=BaseModel)
 O = TypeVar("O", BaseModel, Awaitable[BaseModel])
 
 F = TypeVar("F", bound=Callable)
 
@@ -163,15 +164,15 @@
                 the title will be set to empty string
             description: optional description for the documentation. If
                 None, the description will be set to empty string
             version: optional version for the documentation. If None,
                 the version will be set to empty string
             contact: optional contact for the documentation. If None, the
                 contact will be set to placeholder values:
-                name='Author' url=HttpUrl('https://www.google.com', ) email='noreply@gmail.com'
+                name='Author' url=HttpUrl(' https://www.google.com ', ) email='noreply@gmail.com'
             kafka_brokers: dictionary describing kafka brokers used for
                 generating documentation
             root_path: path to where documentation will be created
             lifespan: asynccontextmanager that is used for setting lifespan hooks.
                 __aenter__ is called before app start and __aexit__ after app stop.
                 The lifespan is called whe application is started as async context
                 manager, e.g.:`async with kafka_app...`
@@ -204,15 +205,18 @@
         # this is used as default parameters for creating AIOProducer and AIOConsumer objects
         self._kafka_config = _get_kafka_config(**kwargs)
 
         #
         self._consumers_store: Dict[
             str,
             Tuple[
-                ConsumeCallable, Callable[[bytes, ModelMetaclass], Any], Dict[str, Any]
+                ConsumeCallable,
+                Callable[[bytes, ModelMetaclass], Any],
+                Union[str, StreamExecutor, None],
+                Dict[str, Any],
             ],
         ] = {}
 
         self._producers_store: Dict[  # type: ignore
             str, Tuple[ProduceCallable, AIOKafkaProducer, Dict[str, Any]]
         ] = {}
 
@@ -374,14 +378,15 @@
 @patch
 @delegates(AIOKafkaConsumer)
 def consumes(
     self: FastKafka,
     topic: Optional[str] = None,
     decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = "json",
     *,
+    executor: Union[str, StreamExecutor, None] = None,
     prefix: str = "on_",
     **kwargs: Dict[str, Any],
 ) -> Callable[[ConsumeCallable], ConsumeCallable]:
     """Decorator registering the callback called when a message is received in a topic.
 
     This function decorator is also responsible for registering topics for AsyncAPI specificiation and documentation.
 
@@ -390,14 +395,22 @@
             decorated function when it receives a message from the topic,
             default: None. If the topic is not specified, topic name will be
             inferred from the decorated function name by stripping the defined prefix
         decoder: Decoder to use to decode messages consumed from the topic,
                 default: json - By default, it uses json decoder to decode
                 bytes to json string and then it creates instance of pydantic
                 BaseModel. It also accepts custom decoder function.
+        executor: Type of executor to choose for consuming tasks. Avaliable options
+                are "SequentialExecutor" and "DynamicTaskExecutor". The default option is
+                "SequentialExecutor" which will execute the consuming tasks sequentially.
+                If the consuming tasks have high latency it is recommended to use
+                "DynamicTaskExecutor" which will wrap the consuming functions into tasks
+                and run them in on asyncio loop in background. This comes with a cost of
+                increased overhead so use it only in cases when your consume functions have
+                high latency such as database queries or some other type of networking.
         prefix: Prefix stripped from the decorated function to define a topic name
             if the topic argument is not passed, default: "on_". If the decorated
             function name is not prefixed with the defined prefix and topic argument
             is not passed, then this method will throw ValueError
 
     Returns:
         A function returning the same function
@@ -407,25 +420,26 @@
 
     """
 
     def _decorator(
         on_topic: ConsumeCallable,
         topic: Optional[str] = topic,
         decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = decoder,
+        executor: Union[str, StreamExecutor, None] = executor,
         kwargs: Dict[str, Any] = kwargs,
     ) -> ConsumeCallable:
         topic_resolved: str = (
             _get_topic_name(topic_callable=on_topic, prefix=prefix)
             if topic is None
             else topic
         )
 
         decoder_fn = _get_decoder_fn(decoder) if isinstance(decoder, str) else decoder
-        self._consumers_store[topic_resolved] = (on_topic, decoder_fn, kwargs)
-
+        self._consumers_store[topic_resolved] = (on_topic, decoder_fn, executor, kwargs)
+        setattr(self, on_topic.__name__, on_topic)
         return on_topic
 
     return _decorator
 
 # %% ../../nbs/015_FastKafka.ipynb 29
 def _get_encoder_fn(encoder: str) -> Callable[[BaseModel], bytes]:
     """
@@ -479,29 +493,31 @@
         A function returning the same function
 
     Raises:
         ValueError: when needed
     """
 
     def _decorator(
-        on_topic: ProduceCallable,
+        to_topic: ProduceCallable,
         topic: Optional[str] = topic,
         kwargs: Dict[str, Any] = kwargs,
     ) -> ProduceCallable:
         topic_resolved: str = (
-            _get_topic_name(topic_callable=on_topic, prefix=prefix)
+            _get_topic_name(topic_callable=to_topic, prefix=prefix)
             if topic is None
             else topic
         )
 
-        self._producers_store[topic_resolved] = (on_topic, None, kwargs)
+        self._producers_store[topic_resolved] = (to_topic, None, kwargs)
         encoder_fn = _get_encoder_fn(encoder) if isinstance(encoder, str) else encoder
-        return producer_decorator(
-            self._producers_store, on_topic, topic_resolved, encoder_fn=encoder_fn
+        decorated = producer_decorator(
+            self._producers_store, to_topic, topic_resolved, encoder_fn=encoder_fn
         )
+        setattr(self, to_topic.__name__, decorated)
+        return decorated
 
     return _decorator
 
 # %% ../../nbs/015_FastKafka.ipynb 33
 @patch
 def get_topics(self: FastKafka) -> Iterable[str]:
     produce_topics = set(self._producers_store.keys())
@@ -558,20 +574,22 @@
         asyncio.create_task(
             aiokafka_consumer_loop(
                 topic=topic,
                 decoder_fn=decoder_fn,
                 callback=consumer,
                 msg_type=signature(consumer).parameters["msg"].annotation,
                 is_shutting_down_f=is_shutting_down_f,
+                executor=executor,
                 **{**default_config, **override_config},
             )
         )
         for topic, (
             consumer,
             decoder_fn,
+            executor,
             override_config,
         ) in self._consumers_store.items()
     ]
 
 
 @patch
 async def _shutdown_consumers(
@@ -736,15 +754,16 @@
     self._is_started = False
 
 # %% ../../nbs/015_FastKafka.ipynb 51
 @patch
 def create_docs(self: FastKafka) -> None:
     export_async_spec(
         consumers={
-            topic: callback for topic, (callback, _, _) in self._consumers_store.items()
+            topic: callback
+            for topic, (callback, _, _, _) in self._consumers_store.items()
         },
         producers={
             topic: callback for topic, (callback, _, _) in self._producers_store.items()
         },
         kafka_brokers=self._kafka_brokers,
         kafka_service_info=self._kafka_service_info,
         asyncapi_path=self._asyncapi_path,
@@ -786,15 +805,15 @@
                 if inspect.ismethod(f):
                     setattr(self, name, self._await_for(f))
 
 # %% ../../nbs/015_FastKafka.ipynb 56
 @patch
 def create_mocks(self: FastKafka) -> None:
     """Creates self.mocks as a named tuple mapping a new function obtained by calling the original functions and a mock"""
-    app_methods = [f for f, _, _ in self._consumers_store.values()] + [
+    app_methods = [f for f, _, _, _ in self._consumers_store.values()] + [
         f for f, _, _ in self._producers_store.values()
     ]
     self.AppMocks = namedtuple(  # type: ignore
         f"{self.__class__.__name__}Mocks", [f.__name__ for f in app_methods]
     )
 
     self.mocks = self.AppMocks(  # type: ignore
@@ -833,32 +852,33 @@
             return sync_inner
 
     self._consumers_store.update(
         {
             name: (
                 add_mock(f, getattr(self.mocks, f.__name__)),
                 decoder_fn,
+                executor,
                 kwargs,
             )
-            for name, (f, decoder_fn, kwargs) in self._consumers_store.items()
+            for name, (f, decoder_fn, executor, kwargs) in self._consumers_store.items()
         }
     )
 
     self._producers_store.update(
         {
             name: (
                 add_mock(f, getattr(self.mocks, f.__name__)),
                 producer,
                 kwargs,
             )
             for name, (f, producer, kwargs) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 62
+# %% ../../nbs/015_FastKafka.ipynb 61
 @patch
 def benchmark(
     self: FastKafka,
     interval: Union[int, timedelta] = 1,
     *,
     sliding_window_size: Optional[int] = None,
 ) -> Callable[[Callable[[I], Optional[O]]], Callable[[I], Optional[O]]]:
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_application/tester.py` & `fastkafka-0.6.0rc0/fastkafka/_application/tester.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 import asyncio
 import inspect
 from contextlib import asynccontextmanager
 from typing import *
 
 from pydantic import BaseModel
 
+from .. import KafkaEvent
 from .app import FastKafka
-from .._components.meta import delegates, patch
+from .._components.meta import delegates, export, patch
 from .._testing.apache_kafka_broker import ApacheKafkaBroker
 from .._testing.in_memory_broker import InMemoryBroker
 from .._testing.local_redpanda_broker import LocalRedpandaBroker
 
-# %% ../../nbs/016_Tester.ipynb 6
+# %% ../../nbs/016_Tester.ipynb 8
+@export("fastkafka.testing")
 class Tester(FastKafka):
     __test__ = False
 
     @delegates(ApacheKafkaBroker.__init__)
     def __init__(
         self,
         app: Union[FastKafka, List[FastKafka]],
@@ -138,21 +140,24 @@
     async def __aenter__(self) -> "Tester":
         self._ctx = self._create_ctx()
         return await self._ctx.__aenter__()
 
     async def __aexit__(self, *args: Any) -> None:
         await self._ctx.__aexit__(*args)
 
-
-Tester.__module__ = "fastkafka.testing"
-
-# %% ../../nbs/016_Tester.ipynb 11
+# %% ../../nbs/016_Tester.ipynb 13
 def mirror_producer(topic: str, producer_f: Callable[..., Any]) -> Callable[..., Any]:
     msg_type = inspect.signature(producer_f).return_annotation
 
+    if hasattr(msg_type, "__origin__") and msg_type.__origin__ == KafkaEvent:
+        msg_type = msg_type.__args__[0]
+
+    if hasattr(msg_type, "__origin__") and msg_type.__origin__ == list:
+        msg_type = msg_type.__args__[0]
+
     async def skeleton_func(msg: BaseModel) -> None:
         pass
 
     mirror_func = skeleton_func
     sig = inspect.signature(skeleton_func)
 
     # adjust name
@@ -169,15 +174,15 @@
         ]
     )
 
     mirror_func.__signature__ = sig  # type: ignore
 
     return mirror_func
 
-# %% ../../nbs/016_Tester.ipynb 13
+# %% ../../nbs/016_Tester.ipynb 16
 def mirror_consumer(topic: str, consumer_f: Callable[..., Any]) -> Callable[..., Any]:
     msg_type = inspect.signature(consumer_f).parameters["msg"]
 
     async def skeleton_func(msg: BaseModel) -> BaseModel:
         return msg
 
     mirror_func = skeleton_func
@@ -188,19 +193,19 @@
 
     # adjust arg and return val
     sig = sig.replace(parameters=[msg_type], return_annotation=msg_type.annotation)
 
     mirror_func.__signature__ = sig  # type: ignore
     return mirror_func
 
-# %% ../../nbs/016_Tester.ipynb 15
+# %% ../../nbs/016_Tester.ipynb 18
 @patch
 def create_mirrors(self: Tester) -> None:
     for app in self.apps:
-        for topic, (consumer_f, _, _) in app._consumers_store.items():
+        for topic, (consumer_f, _, _, _) in app._consumers_store.items():
             mirror_f = mirror_consumer(topic, consumer_f)
             mirror_f = self.produces()(mirror_f)  # type: ignore
             setattr(self, mirror_f.__name__, mirror_f)
         for topic, (producer_f, _, _) in app._producers_store.items():
             mirror_f = mirror_producer(topic, producer_f)
             mirror_f = self.consumes()(mirror_f)  # type: ignore
             setattr(self, mirror_f.__name__, mirror_f)
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_cli.py` & `fastkafka-0.6.0rc0/fastkafka/_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 # %% ../nbs/023_CLI.ipynb 1
 import asyncio
 import multiprocessing
 from typing import *
 
 import typer
 
+from ._components.logger import get_logger, supress_timestamps
+
 from . import _cli_docs, _cli_testing
-from ._components.logger import get_logger
 from ._server import run_fastkafka_server
 
 # %% ../nbs/023_CLI.ipynb 5
-logger = get_logger(__name__)
+supress_timestamps(False)
+logger = get_logger(__name__, level=20)
 
 # %% ../nbs/023_CLI.ipynb 8
 _app = typer.Typer(help="")
 
 # %% ../nbs/023_CLI.ipynb 9
 @_app.command(
     help="Runs Fast Kafka API application",
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_cli_docs.py` & `fastkafka-0.6.0rc0/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/_cli_testing.py` & `fastkafka-0.6.0rc0/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/_subprocess.py` & `fastkafka-0.6.0rc0/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.6.0rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,136 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/011_ConsumerLoop.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'sanitize_kafka_config', 'aiokafka_consumer_loop']
+__all__ = ['logger', 'AsyncConsume', 'AsyncConsumeMeta', 'SyncConsume', 'SyncConsumeMeta', 'ConsumeCallable', 'EventMetadata',
+           'sanitize_kafka_config', 'aiokafka_consumer_loop']
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 1
-from asyncio import iscoroutinefunction  # do not use the version from inspect
+import asyncio
+from asyncio import iscoroutinefunction, Task  # do not use the version from inspect
 from typing import *
+from functools import wraps, partial
+from dataclasses import dataclass
+from contextlib import asynccontextmanager
 
 import anyio
 import asyncer
 from aiokafka import AIOKafkaConsumer
 from aiokafka.structs import ConsumerRecord, TopicPartition
 from anyio.streams.memory import MemoryObjectReceiveStream
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
 from .logger import get_logger
-from .meta import delegates
+from .meta import delegates, export
+from .task_streaming import get_executor, StreamExecutor
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 5
 logger = get_logger(__name__)
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 9
-def _create_safe_callback(
-    callback: Callable[[BaseModel], Awaitable[None]]
-) -> Callable[[BaseModel], Awaitable[None]]:
+# %% ../../nbs/011_ConsumerLoop.ipynb 8
+@dataclass
+@export("fastkafka")
+class EventMetadata:
+    """A class for encapsulating Kafka record metadata.
+
+    Args:
+        topic: The topic this record is received from
+        partition: The partition from which this record is received
+        offset: The position of this record in the corresponding Kafka partition
+        timestamp: The timestamp of this record
+        timestamp_type: The timestamp type of this record
+        key: The key (or `None` if no key is specified)
+        value: The value
+        serialized_key_size: The size of the serialized, uncompressed key in bytes
+        serialized_value_size: The size of the serialized, uncompressed value in bytes
+        headers: The headers
     """
-    Wraps an async callback into a safe callback that catches any Exception and loggs them as warnings
 
-    Params:
-        callback: async callable that will be wrapped into a safe callback
+    topic: str
+    partition: int
+    offset: int
+    timestamp: int
+    timestamp_type: int
+    key: Optional[bytes]
+    value: Optional[bytes]
+    checksum: int
+    serialized_key_size: int
+    serialized_value_size: int
+    headers: Sequence[Tuple[str, bytes]]
+
+    @staticmethod
+    def create_event_metadata(record: ConsumerRecord) -> "EventMetadata":  # type: ignore
+        return EventMetadata(
+            topic=record.topic,
+            partition=record.partition,
+            offset=record.offset,
+            timestamp=record.timestamp,
+            timestamp_type=record.timestamp_type,
+            value=record.value,
+            checksum=record.checksum,
+            key=record.key,
+            serialized_key_size=record.serialized_key_size,
+            serialized_value_size=record.serialized_value_size,
+            headers=record.headers,
+        )
+
+# %% ../../nbs/011_ConsumerLoop.ipynb 11
+AsyncConsume = Callable[[BaseModel], Awaitable[None]]
+AsyncConsumeMeta = Callable[[BaseModel, EventMetadata], Awaitable[None]]
+SyncConsume = Callable[[BaseModel], None]
+SyncConsumeMeta = Callable[[BaseModel, EventMetadata], None]
+
+ConsumeCallable = Union[AsyncConsume, AsyncConsumeMeta, SyncConsume, SyncConsumeMeta]
+
+# %% ../../nbs/011_ConsumerLoop.ipynb 12
+def _callback_parameters_wrapper(
+    callback: Union[AsyncConsume, AsyncConsumeMeta]
+) -> AsyncConsumeMeta:
+    """Wraps an async callback and filters the arguments to pass based on if the function accepts EventMetadata as argument
+
+    Args:
+        callback: async callable that will be wrapped
 
     Returns:
-        Wrapped callback into a safe callback that handles exceptions
+        Wrapped callback with filtered params
     """
 
-    async def _safe_callback(
+    async def _params_wrap(
         msg: BaseModel,
-        callback: Callable[[BaseModel], Awaitable[None]] = callback,
+        meta: EventMetadata,
+        callback: Union[AsyncConsume, AsyncConsumeMeta] = callback,
     ) -> None:
-        try:
-            await callback(msg)
-        except Exception as e:
-            logger.warning(
-                f"_safe_callback(): exception caugth {e.__repr__()} while awaiting '{callback}({msg})'"
-            )
+        types = list(get_type_hints(callback).values())
+        args: List[Union[BaseModel, EventMetadata]] = [msg]
+        if EventMetadata in types:
+            args.insert(types.index(EventMetadata), meta)
+        await callback(*args)  # type: ignore
 
-    return _safe_callback
+    return _params_wrap
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 12
-def _prepare_callback(
-    callback: Callable[[BaseModel], Union[None, Awaitable[None]]]
-) -> Callable[[BaseModel], Awaitable[None]]:
+# %% ../../nbs/011_ConsumerLoop.ipynb 16
+def _prepare_callback(callback: ConsumeCallable) -> AsyncConsumeMeta:
     """
     Prepares a callback to be used in the consumer loop.
         1. If callback is sync, asyncify it
         2. Wrap the callback into a safe callback for exception handling
 
     Params:
         callback: async callable that will be prepared for use in consumer
 
     Returns:
         Prepared callback
     """
-    async_callback: Callable[[BaseModel], Awaitable[None]] = (
+    async_callback: Union[AsyncConsume, AsyncConsumeMeta] = (
         callback if iscoroutinefunction(callback) else asyncer.asyncify(callback)  # type: ignore
     )
-    return _create_safe_callback(async_callback)
+    return _callback_parameters_wrapper(async_callback)
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 14
+# %% ../../nbs/011_ConsumerLoop.ipynb 18
 async def _stream_msgs(  # type: ignore
     msgs: Dict[TopicPartition, bytes],
     send_stream: anyio.streams.memory.MemoryObjectSendStream[Any],
 ) -> None:
     """
     Decodes and streams the message and topic to the send_stream.
 
@@ -92,34 +150,26 @@
 
 def _decode_streamed_msgs(  # type: ignore
     msgs: List[ConsumerRecord], msg_type: BaseModel
 ) -> List[BaseModel]:
     decoded_msgs = [msg_type.parse_raw(msg.value.decode("utf-8")) for msg in msgs]
     return decoded_msgs
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 19
-async def _streamed_records(
-    receive_stream: MemoryObjectReceiveStream,
-) -> AsyncGenerator[Any, Any]:
-    async for records_per_topic in receive_stream:
-        for records in records_per_topic:
-            for record in records:
-                yield record
-
-
+# %% ../../nbs/011_ConsumerLoop.ipynb 23
 @delegates(AIOKafkaConsumer.getmany)
 async def _aiokafka_consumer_loop(  # type: ignore
     consumer: AIOKafkaConsumer,
     *,
     topic: str,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
-    callback: Callable[[BaseModel], Union[None, Awaitable[None]]],
+    callback: ConsumeCallable,
     max_buffer_size: int = 100_000,
     msg_type: Type[BaseModel],
     is_shutting_down_f: Callable[[], bool],
+    executor: Union[str, StreamExecutor, None] = None,
     **kwargs: Any,
 ) -> None:
     """
     Consumer loop for infinite pooling of the AIOKafka consumer for new messages. Calls consumer.getmany()
     and after the consumer return messages or times out, messages are decoded and streamed to defined callback.
 
     Params:
@@ -130,73 +180,49 @@
         max_buffer_size: Maximum number of unconsumed messages in the callback buffer
         msg_types: Dict of message types mapped to their respective topics
         is_shutting_down_f: Function for controlling the shutdown of consumer loop
     """
 
     prepared_callback = _prepare_callback(callback)
 
-    async def process_message_callback(
-        receive_stream: MemoryObjectReceiveStream[Any],
-        callback: Callable[[BaseModel], Awaitable[None]] = prepared_callback,
-        msg_type: Type[BaseModel] = msg_type,
-        topic: str = topic,
+    async def handle_msg(  # type: ignore
+        record: ConsumerRecord,
+        callback: AsyncConsumeMeta = prepared_callback,
         decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
+        msg_type: Type[BaseModel] = msg_type,
     ) -> None:
-        async with receive_stream:
-            try:
-                async for record in _streamed_records(receive_stream):
-                    try:
-                        msg = record.value
-                        decoded_msg = decoder_fn(msg, msg_type)
-                        await callback(decoded_msg)
-                    except Exception as e:
-                        logger.warning(
-                            f"process_message_callback(): Unexpected exception '{e.__repr__()}' caught and ignored for topic='{topic}' and message: {msg}"
-                        )
-            except Exception as e:
-                logger.warning(
-                    f"process_message_callback(): Unexpected exception '{e.__repr__()}' caught and ignored for topic='{topic}'"
-                )
+        await callback(
+            decoder_fn(record.value, msg_type),
+            EventMetadata.create_event_metadata(record),
+        )
 
-    send_stream, receive_stream = anyio.create_memory_object_stream(
-        max_buffer_size=max_buffer_size
-    )
+    async def poll_consumer(kwargs: Any = kwargs) -> List[ConsumerRecord]:  # type: ignore
+        msgs = await consumer.getmany(**kwargs)
+        return [msg for msg_group in msgs.values() for msg in msg_group]
 
-    async with anyio.create_task_group() as tg:
-        tg.start_soon(process_message_callback, receive_stream)
-        async with send_stream:
-            while not is_shutting_down_f():
-                msgs = await consumer.getmany(**kwargs)
-                try:
-                    await send_stream.send(msgs.values())
-                except Exception as e:
-                    logger.warning(
-                        f"_aiokafka_consumer_loop(): Unexpected exception '{e}' caught and ignored for messages: {msgs}"
-                    )
-            logger.info(
-                f"_aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain..."
-            )
+    await get_executor(executor).run(is_shutting_down_f, poll_consumer, handle_msg)
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 24
+# %% ../../nbs/011_ConsumerLoop.ipynb 28
 def sanitize_kafka_config(**kwargs: Any) -> Dict[str, Any]:
     """Sanitize Kafka config"""
     return {k: "*" * len(v) if "pass" in k.lower() else v for k, v in kwargs.items()}
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 26
+# %% ../../nbs/011_ConsumerLoop.ipynb 30
 @delegates(AIOKafkaConsumer)
 @delegates(_aiokafka_consumer_loop, keep=True)
 async def aiokafka_consumer_loop(
     topic: str,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     *,
     timeout_ms: int = 100,
     max_buffer_size: int = 100_000,
-    callback: Callable[[BaseModel], Union[None, Awaitable[None]]],
+    callback: ConsumeCallable,
     msg_type: Type[BaseModel],
     is_shutting_down_f: Callable[[], bool],
+    executor: Union[str, StreamExecutor, None] = None,
     **kwargs: Any,
 ) -> None:
     """Consumer loop for infinite pooling of the AIOKafka consumer for new messages. Creates and starts AIOKafkaConsumer
     and runs _aio_kafka_consumer loop fo infinite poling of the consumer for new messages.
 
     Args:
         topic: name of the topic to subscribe to
@@ -227,14 +253,15 @@
                 topic=topic,
                 decoder_fn=decoder_fn,
                 max_buffer_size=max_buffer_size,
                 timeout_ms=timeout_ms,
                 callback=callback,
                 msg_type=msg_type,
                 is_shutting_down_f=is_shutting_down_f,
+                executor=executor,
             )
         finally:
             await consumer.stop()
             logger.info(f"aiokafka_consumer_loop(): Consumer stopped.")
             logger.info(f"aiokafka_consumer_loop() finished.")
     except Exception as e:
         logger.error(
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/asyncapi.py` & `fastkafka-0.6.0rc0/fastkafka/_components/asyncapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/014_AsyncAPI.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'ConsumeCallable', 'sec_scheme_name_mapping', 'KafkaMessage', 'SecurityType', 'APIKeyLocation',
-           'SecuritySchema', 'KafkaBroker', 'ContactInfo', 'KafkaServiceInfo', 'KafkaBrokers', 'yaml_file_cmp',
-           'export_async_spec']
+__all__ = ['logger', 'sec_scheme_name_mapping', 'KafkaMessage', 'SecurityType', 'APIKeyLocation', 'SecuritySchema', 'KafkaBroker',
+           'ContactInfo', 'KafkaServiceInfo', 'KafkaBrokers', 'yaml_file_cmp', 'export_async_spec']
 
 # %% ../../nbs/014_AsyncAPI.ipynb 1
 import json
 import shutil
 import subprocess  # nosec: B404: Consider possible security implications associated with the subprocess module.
 import tempfile
 from datetime import timedelta
@@ -23,31 +22,29 @@
 import fastkafka._components.logger
 
 fastkafka._components.logger.should_supress_timestamps = True
 
 from .docs_dependencies import _check_npm_with_local
 from .logger import get_logger
 from .producer_decorator import KafkaEvent, ProduceCallable
+from .aiokafka_consumer_loop import ConsumeCallable
 
 # %% ../../nbs/014_AsyncAPI.ipynb 3
 logger = get_logger(__name__)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 5
-ConsumeCallable = Callable[[BaseModel], Union[Awaitable[None], None]]
-
-# %% ../../nbs/014_AsyncAPI.ipynb 6
 class KafkaMessage(BaseModel):
     class Config:
         """This class is used for specific JSON encoders, in our case to properly format timedelta in ISO format."""
 
         json_encoders = {
             timedelta: timedelta_isoformat,
         }
 
-# %% ../../nbs/014_AsyncAPI.ipynb 8
+# %% ../../nbs/014_AsyncAPI.ipynb 7
 class SecurityType(str, Enum):
     plain = "plain"
     userPassword = "userPassword"
     apiKey = "apiKey"
     X509 = "X509"
     symmetricEncryption = "symmetricEncryption"
     asymmetricEncryption = "asymmetricEncryption"
@@ -99,15 +96,15 @@
 
         return d
 
     def json(self, *args: Any, **kwargs: Any) -> str:
         """Serialize into JSON using dict()"""
         return json.dumps(self.dict(), *args, **kwargs)
 
-# %% ../../nbs/014_AsyncAPI.ipynb 10
+# %% ../../nbs/014_AsyncAPI.ipynb 9
 class KafkaBroker(BaseModel):
     """Kafka broker"""
 
     url: str = Field(..., example="localhost")
     description: str = Field("Kafka broker")
     port: str = Field("9092")
     protocol: str = Field("kafka")
@@ -123,34 +120,34 @@
 
         return d
 
     def json(self, *args: Any, **kwargs: Any) -> str:
         """Serialize into JSON using dict()"""
         return json.dumps(self.dict(), *args, **kwargs)
 
-# %% ../../nbs/014_AsyncAPI.ipynb 13
+# %% ../../nbs/014_AsyncAPI.ipynb 12
 class ContactInfo(BaseModel):
     name: str = Field(..., example="My company")
     url: HttpUrl = Field(..., example="https://www.github.com/mycompany")
     email: str = Field(..., example="noreply@mycompany.com")
 
 
 class KafkaServiceInfo(BaseModel):
     title: str = Field("Title")
     version: str = Field("0.0.1")
     description: str = Field("Description of the service")
     contact: ContactInfo = Field(
         ...,
     )
 
-# %% ../../nbs/014_AsyncAPI.ipynb 15
+# %% ../../nbs/014_AsyncAPI.ipynb 14
 class KafkaBrokers(BaseModel):
     brokers: Dict[str, KafkaBroker]
 
-# %% ../../nbs/014_AsyncAPI.ipynb 18
+# %% ../../nbs/014_AsyncAPI.ipynb 17
 # T = TypeVar("T")
 
 
 def _get_msg_cls_for_producer(f: ProduceCallable) -> Type[Any]:
     types = get_type_hints(f)
     return_type = types.pop("return", type(None))
     # @app.producer must define a return value
@@ -158,27 +155,35 @@
         raise ValueError(
             f"Producer function must have a defined return value, got {return_type} as return value"
         )
 
     if hasattr(return_type, "__origin__") and return_type.__origin__ == KafkaEvent:
         return_type = return_type.__args__[0]
 
+    if hasattr(return_type, "__origin__") and return_type.__origin__ == list:
+        return_type = return_type.__args__[0]
+
     if not hasattr(return_type, "json"):
         raise ValueError(f"Producer function return value must have json method")
     return return_type  # type: ignore
 
 # %% ../../nbs/014_AsyncAPI.ipynb 22
 def _get_msg_cls_for_consumer(f: ConsumeCallable) -> Type[Any]:
     types = get_type_hints(f)
     return_type = types.pop("return", type(None))
     types_list = list(types.values())
-    # @app.consumer takes only message argument
-    if len(types_list) != 1:
+    # @app.consumer first consumer argument must be a msg which is a subclass of BaseModel
+    try:
+        if issubclass(BaseModel, types_list[0]):
+            raise ValueError(
+                f"Consumer function first param must be a BaseModel subclass msg, got {types_list}"
+            )
+    except IndexError:
         raise ValueError(
-            f"Consumer function must have only one input param, got {types_list}"
+            f"Consumer function first param must be a BaseModel subclass msg, got {types_list}"
         )
     # @app.consumer does not return a value
     if return_type != type(None):
         raise ValueError(
             f"Consumer function cannot return any value, got {return_type}"
         )
     return types_list[0]  # type: ignore
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/benchmarking.py` & `fastkafka-0.6.0rc0/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.6.0rc0/fastkafka/_components/docs_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         raise RuntimeError(msg)
 
     logger.info("Installing NodeJS...")
     local_path.mkdir(exist_ok=True, parents=True)
     response = requests.get(
         node_url,
         stream=True,
+        timeout=60,
     )
     try:
         total = response.raw.length_remaining // 128
     except Exception:
         total = None
 
     with open(tgz_path, "wb") as f:
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/encoder/avro.py` & `fastkafka-0.6.0rc0/fastkafka/_components/encoder/avro.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/18_Avro_Encode_Decoder.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/018_Avro_Encode_Decoder.ipynb.
 
 # %% auto 0
 __all__ = ['logger', 'AvroBase', 'avro_encoder', 'avro_decoder', 'avsc_to_pydantic']
 
-# %% ../../../nbs/18_Avro_Encode_Decoder.ipynb 1
+# %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 1
 import io
 import json
 from typing import *
 
 import fastavro
 from pydantic import BaseModel, create_model
 from pydantic.main import ModelMetaclass
 
 from ..logger import get_logger
+from ..meta import export
 
-# %% ../../../nbs/18_Avro_Encode_Decoder.ipynb 4
+# %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 4
 logger = get_logger(__name__)
 
-# %% ../../../nbs/18_Avro_Encode_Decoder.ipynb 7
+# %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 7
+@export("fastkafka.encoder")
 class AvroBase(BaseModel):
     """This is base pydantic class that will add some methods"""
 
     @classmethod
     def avro_schema_for_pydantic(
         cls,
         pydantic_model: Union[BaseModel, ModelMetaclass],
@@ -198,34 +200,64 @@
         return {
             "type": "record",
             "namespace": namespace,
             "name": schema["title"],
             "fields": fields,
         }
 
-# %% ../../../nbs/18_Avro_Encode_Decoder.ipynb 11
+# %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 11
+@export("fastkafka.encoder")
 def avro_encoder(msg: BaseModel) -> bytes:
+    """
+    Encoder to encode pydantic instances to avro message
+
+    Args:
+        msg: An instance of pydantic basemodel
+
+    Returns:
+        A bytes message which is encoded from pydantic basemodel
+    """
     schema = fastavro.schema.parse_schema(AvroBase.avro_schema_for_pydantic(msg))
     bytes_writer = io.BytesIO()
     fastavro.schemaless_writer(bytes_writer, schema, msg.dict())
     raw_bytes = bytes_writer.getvalue()
     return raw_bytes
 
-# %% ../../../nbs/18_Avro_Encode_Decoder.ipynb 13
+# %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 13
+@export("fastkafka.encoder")
 def avro_decoder(raw_msg: bytes, cls: ModelMetaclass) -> Any:
+    """
+    Decoder to decode avro encoded messages to pydantic model instance
+
+    Args:
+        raw_msg: Avro encoded bytes message received from Kafka topic
+        cls: Pydantic class; This pydantic class will be used to construct instance of same class
+
+    Returns:
+        An instance of given pydantic class
+    """
     schema = fastavro.schema.parse_schema(AvroBase.avro_schema_for_pydantic(cls))
 
     bytes_reader = io.BytesIO(raw_msg)
     msg_dict = fastavro.schemaless_reader(bytes_reader, schema)
 
     return cls(**msg_dict)
 
-# %% ../../../nbs/18_Avro_Encode_Decoder.ipynb 16
+# %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 16
+@export("fastkafka.encoder")
 def avsc_to_pydantic(schema: Dict[str, Any]) -> ModelMetaclass:
-    """Generate python code of pydantic of given Avro Schema"""
+    """
+    Generate pydantic model from given Avro Schema
+
+    Args:
+        schema: Avro schema in dictionary format
+
+    Returns:
+        Pydantic model class built from given avro schema
+    """
     if "type" not in schema or schema["type"] != "record":
         raise AttributeError("Type not supported")
     if "name" not in schema:
         raise AttributeError("Name is required")
     if "fields" not in schema:
         raise AttributeError("fields are required")
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/helpers.py` & `fastkafka-0.6.0rc0/fastkafka/_components/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     return True
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 4
 import contextlib
 import importlib
 import os
 import sys
+from datetime import datetime, timedelta
 from functools import wraps
 from inspect import signature
 from pathlib import Path
 from typing import *
-from datetime import datetime, timedelta
 
 import docstring_parser
 import typer
 
 from .meta import delegates
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 6
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/logger.py` & `fastkafka-0.6.0rc0/fastkafka/_components/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 __all__ = ['should_supress_timestamps', 'logger_spaces_added', 'supress_timestamps', 'get_default_logger_configuration',
            'get_logger', 'set_level', 'cached_log']
 
 # %% ../../nbs/Logger.ipynb 2
 import logging
 import logging.config
 from typing import *
-from .meta import patch
+
 from .helpers import true_after
+from .meta import patch
 
 # %% ../../nbs/Logger.ipynb 4
 # Logger Levels
 # CRITICAL = 50
 # ERROR = 40
 # WARNING = 30
 # INFO = 20
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/meta.py` & `fastkafka-0.6.0rc0/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/_components/test_dependencies.py` & `fastkafka-0.6.0rc0/fastkafka/_components/test_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
     if not check_kafka():
         logger.info("Installing Kafka...")
         local_path.mkdir(exist_ok=True, parents=True)
         response = requests.get(
             kafka_url,
             stream=True,
+            timeout=60,
         )
         try:
             total = response.raw.length_remaining // 128
         except Exception:
             total = None
 
         with open(tgz_path, "wb") as f:
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_docusaurus_helper.py` & `fastkafka-0.6.0rc0/fastkafka/_docusaurus_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/096_Docusaurus_Helper.ipynb.
 
 # %% auto 0
-__all__ = ['SidebarT', 'fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'parse_contents', 'remove_section_contents',
-           'generate_sidebar']
+__all__ = ['fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'generate_sidebar']
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 2
 import itertools
 import re
 import types
 from inspect import Signature, getmembers, isclass, isfunction, signature
 from pathlib import Path
-from urllib.parse import urljoin
 from typing import *
+from urllib.parse import urljoin
 
 import yaml
-
 from docstring_parser import parse
 from docstring_parser.common import DocstringParam, DocstringRaises, DocstringReturns
 from nbdev.config import get_config
 from nbdev_mkdocs.mkdocs import (
     _add_all_submodules,
     _get_api_summary,
     _import_all_members,
@@ -278,70 +276,100 @@
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 36
 def _fix_special_symbols_in_html(contents: str) -> str:
     contents = contents.replace("”", '"')
     return contents
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 38
-def _remove_redundant_segment_from_link(url: str) -> str:
-    """Remove redundant segment from the end of a URL.
+def _add_file_extension_to_link(url: str) -> str:
+    """Add file extension to the last segment of a URL
 
     Args:
-        url: The URL to remove the a redundant segment.
+        url: A URL string.
 
     Returns:
-        The updated URL with the redundant segment removed, or the original URL if no redundant segment was found.
+        A string of the updated URL with a file extension added to the last segment of the URL.
     """
     segments = url.split("/#")[0].split("/")[-2:]
-    return (
-        url.replace(f"/{segments[1]}", "")
-        if segments[0] == segments[1].lower()
-        else url
-    )
+    return url.replace(f"/{segments[1]}", f"/{segments[1]}.md")
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 42
-def _fix_symbol_links(contents: str) -> str:
+def _fix_symbol_links(
+    contents: str, dir_prefix: str, doc_host: str, doc_baseurl: str
+) -> str:
     """Fix symbol links in Markdown content.
 
     Args:
         contents: The Markdown content to search for symbol links.
+        dir_prefix: Directory prefix to append in the relative URL.
+        doc_host: The host URL for the documentation site.
+        doc_baseurl: The base URL for the documentation site.
 
     Returns:
         str: The Markdown content with updated symbol links.
     """
-    cfg = get_config()
-    prefix = re.escape(urljoin(cfg["doc_host"] + "/", cfg["doc_baseurl"] + "/api"))
+    prefix = re.escape(urljoin(doc_host + "/", doc_baseurl))
     pattern = re.compile(rf"\[(.*?)\]\(({prefix}[^)]+)\)")
     matches = pattern.findall(contents)
     for match in matches:
         old_url = match[1]
-        new_url = _remove_redundant_segment_from_link(old_url).replace(
-            "/api/", "/docs/api/"
-        )
-        contents = contents.replace(old_url, new_url)
+        new_url = _add_file_extension_to_link(old_url).replace("/api/", "/docs/api/")
+        dir_prefix = "./" if dir_prefix == "" else dir_prefix
+        relative_url = dir_prefix + new_url.split("/docs/")[1]
+        contents = contents.replace(old_url, relative_url)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 48
+# %% ../nbs/096_Docusaurus_Helper.ipynb 49
+def _get_relative_url_prefix(docs_path: Path, sub_path: Path) -> str:
+    """Returns a relative url prefix from a sub path to a docs path.
+
+    Args:
+        docs_path (Path): The docs directory path.
+        sub_path (Path): The sub directory path.
+
+    Returns:
+        str: A string representing the relative path from the sub path to the docs path.
+
+    Raises:
+        ValueError: If the sub path is not a descendant of the docs path.
+    """
+    try:
+        relative_path = sub_path.relative_to(docs_path)
+    except ValueError:
+        raise ValueError(f"{sub_path} is not a descendant of {docs_path}")
+
+    return (
+        "../" * (len(relative_path.parts) - 1) if len(relative_path.parts) > 1 else ""
+    )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 51
 def fix_invalid_syntax_in_markdown(docs_path: str) -> None:
     """Fix invalid HTML syntax in markdown files and converts inline style attributes to JSX-compatible format.
 
     Args:
         docs_path: The path to the root directory to search for markdown files.
     """
+    cfg = get_config()
+    doc_host = cfg["doc_host"]
+    doc_baseurl = cfg["doc_baseurl"]
+
     markdown_files = _get_all_markdown_files_path(Path(docs_path))
     for file in markdown_files:
+        relative_url_prefix = _get_relative_url_prefix(Path(docs_path), file)
         contents = Path(file).read_text()
 
         contents = _convert_html_style_attribute_to_jsx(contents)
         contents = _fix_special_symbols_in_html(contents)
-        contents = _fix_symbol_links(contents)
+        contents = _fix_symbol_links(
+            contents, relative_url_prefix, doc_host, doc_baseurl
+        )
 
         file.write_text(contents)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 50
+# %% ../nbs/096_Docusaurus_Helper.ipynb 53
 def generate_markdown_docs(module_name: str, docs_path: str) -> None:
     """Generates Markdown documentation files for the symbols in the given module and save them to the given directory.
 
     Args:
         module_name: The name of the module to generate documentation for.
         docs_path: The path to the directory where the documentation files will be saved.
     """
@@ -354,72 +382,109 @@
         target_file_path = (
             "/".join(f"{symbol.__module__}.{symbol.__name__}".split(".")) + ".md"
         )
 
         with open((Path(docs_path) / "api" / target_file_path), "w") as f:
             f.write(content)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 52
-SidebarT = Union[str, List["SidebarT"], Dict[str, "SidebarT"]]
+# %% ../nbs/096_Docusaurus_Helper.ipynb 55
+def _parse_lines(lines: List[str]) -> Tuple[List[str], int]:
+    """Parse a list of lines and return a tuple containing a list of filenames and an index indicating how many lines to skip.
+
+    Args:
+        lines: A list of strings representing lines of input text.
+
+    Returns:
+        A tuple containing a list of strings representing the filenames extracted
+        from links in the lines and an integer representing the number of lines to skip.
+    """
+    index = next(
+        (i for i, line in enumerate(lines) if not line.strip().startswith("- [")),
+        len(lines),
+    )
+    return [line.split("(")[1][:-4] for line in lines[:index]], index
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 58
+def _parse_section(text: str, ignore_first_line: bool = False) -> List[Any]:
+    """Parse the given section contents and return a list of file names in the expected format.
+
+    Args:
+        text: A string representing the contents of a file.
+        ignore_first_line: Flag indicating whether to ignore the first line extracting the section contents.
+
+    Returns:
+        A list of filenames in the expected format
+    """
+    pattern = r"\[.*?\]\((.*?)\)|\[(.*?)\]\[(.*?)\]"
+    lines = text.split("\n")[1:] if ignore_first_line else text.split("\n")
+    ret_val = []
+    index = 0
+    while index < len(lines):
+        line = lines[index]
+        match = re.search(pattern, line.strip())
+        if match is not None:
+            ret_val.append(match.group(1).split(".md")[0])
+            index += 1
+        elif line.strip() != "":
+            value, skip_lines = _parse_lines(lines[index + 1 :])
+            ret_val.append({line.replace("-", "").strip(): value})
+            index += skip_lines + 1
+        else:
+            index += 1
+    return ret_val
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 61
+def _get_section_from_markdown(
+    markdown_text: str, section_header: str
+) -> Optional[str]:
+    """Get the contents of the section header from the given markdown text
 
+    Args:
+        markdown_text: A string containing the markdown text to extract the section from.
+        section_header: A string representing the header of the section to extract.
 
-def parse_contents(contents: List[SidebarT]) -> List[SidebarT]:
-    new: List[SidebarT] = []
-    for content in contents:
-        if isinstance(content, str):
-            new.append(content.split(".")[0])
-        if isinstance(content, dict):
-            new.append(remove_section_contents(content))  # type: ignore
-    return new
-
-
-def remove_section_contents(
-    section: Dict[str, "SidebarT"]
-) -> Dict[str, List[SidebarT]]:
-    new_section: Dict[str, List["SidebarT"]] = {}
-    new_section[section["section"]] = parse_contents(section["contents"])  # type: ignore
-    return new_section
+    Returns:
+        A string representing the contents of the section header if the section header
+        is present in the markdown text, else None
+    """
+    pattern = re.compile(rf"^- {section_header}\n((?:\s+- .*\n)+)", re.M)
+    match = pattern.search(markdown_text)
+    return match.group(1) if match else None
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 54
+# %% ../nbs/096_Docusaurus_Helper.ipynb 66
 def generate_sidebar(
-    nbs_sidebar: str = "/work/fastkafka/nbs/sidebar.yml",
+    summary_file: str = "./docusaurus/docs/SUMMARY.md",
+    summary: str = "",
     target: str = "./docusaurus/sidebars.js",
 ) -> None:
-    with open(nbs_sidebar, "r") as stream, open(target, "w") as target_stream:
-        try:
-            sidebar = yaml.safe_load(stream)
-            parsed_sidebar = parse_contents(sidebar["website"]["sidebar"]["contents"])
-            sidebar_str = str(parsed_sidebar)[1:-1] + ","
-            target_stream.write(
-                """module.exports = {
+    with open(summary_file, "r") as stream, open(target, "w") as target_stream:
+        summary_contents = stream.read()
+
+        guides_summary = _get_section_from_markdown(summary_contents, "Guides")
+        parsed_guides = _parse_section(guides_summary)  # type: ignore
+
+        api_summary = _get_section_from_markdown(summary_contents, "API")
+        parsed_api = _parse_section(api_summary, True)  # type: ignore
+
+        cli_summary = _get_section_from_markdown(summary_contents, "CLI")
+        parsed_cli = _parse_section(cli_summary)  # type: ignore
+
+        target_stream.write(
+            """module.exports = {
 tutorialSidebar: [
+    'index', {'Guides': 
     """
-                + sidebar_str
-                + """
-//         [require("./docs/reference/sidebar.json")],
-    {
-        "items": [
-            "api/fastkafka/FastKafka",
-            "api/fastkafka/KafkaEvent",
-            {
-              "items": [
-                "api/fastkafka/testing/ApacheKafkaBroker",
-                "api/fastkafka/testing/LocalRedpandaBroker",
-                "api/fastkafka/testing/Tester"
-              ],
-              "label": "testing",
-              "type": "category"
-            },
-        ],
-        "label": "API",
-        "type": "category"
-    },
-    {
-        "CLI": ['cli/fastkafka', 'cli/run_fastkafka_server_process'],
-    },
-
+            + str(parsed_guides)
+            + "},"
+            + "{'API': ["
+            + str(parsed_api)[1:-1]
+            + "]},"
+            + "{'CLI': "
+            + str(parsed_cli)
+            + "},"
+            + """
+    "LICENSE",
+    "CONTRIBUTING",
     "CHANGELOG",
 ],
 };"""
-            )
-        except yaml.YAMLError as exc:
-            print(exc)
+        )
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_helpers.py` & `fastkafka-0.6.0rc0/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/_modidx.py` & `fastkafka-0.6.0rc0/fastkafka/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,26 +89,28 @@
                                                                                                            'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester.using_local_redpanda': ( 'tester.html#tester.using_local_redpanda',
                                                                                                               'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.mirror_consumer': ( 'tester.html#mirror_consumer',
                                                                                                   'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.mirror_producer': ( 'tester.html#mirror_producer',
                                                                                                   'fastkafka/_application/tester.py')},
-            'fastkafka._components.aiokafka_consumer_loop': { 'fastkafka._components.aiokafka_consumer_loop._aiokafka_consumer_loop': ( 'consumerloop.html#_aiokafka_consumer_loop',
+            'fastkafka._components.aiokafka_consumer_loop': { 'fastkafka._components.aiokafka_consumer_loop.EventMetadata': ( 'consumerloop.html#eventmetadata',
+                                                                                                                              'fastkafka/_components/aiokafka_consumer_loop.py'),
+                                                              'fastkafka._components.aiokafka_consumer_loop.EventMetadata.create_event_metadata': ( 'consumerloop.html#eventmetadata.create_event_metadata',
+                                                                                                                                                    'fastkafka/_components/aiokafka_consumer_loop.py'),
+                                                              'fastkafka._components.aiokafka_consumer_loop._aiokafka_consumer_loop': ( 'consumerloop.html#_aiokafka_consumer_loop',
                                                                                                                                         'fastkafka/_components/aiokafka_consumer_loop.py'),
-                                                              'fastkafka._components.aiokafka_consumer_loop._create_safe_callback': ( 'consumerloop.html#_create_safe_callback',
-                                                                                                                                      'fastkafka/_components/aiokafka_consumer_loop.py'),
+                                                              'fastkafka._components.aiokafka_consumer_loop._callback_parameters_wrapper': ( 'consumerloop.html#_callback_parameters_wrapper',
+                                                                                                                                             'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._decode_streamed_msgs': ( 'consumerloop.html#_decode_streamed_msgs',
                                                                                                                                       'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._prepare_callback': ( 'consumerloop.html#_prepare_callback',
                                                                                                                                   'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._stream_msgs': ( 'consumerloop.html#_stream_msgs',
                                                                                                                              'fastkafka/_components/aiokafka_consumer_loop.py'),
-                                                              'fastkafka._components.aiokafka_consumer_loop._streamed_records': ( 'consumerloop.html#_streamed_records',
-                                                                                                                                  'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.aiokafka_consumer_loop': ( 'consumerloop.html#aiokafka_consumer_loop',
                                                                                                                                        'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.sanitize_kafka_config': ( 'consumerloop.html#sanitize_kafka_config',
                                                                                                                                       'fastkafka/_components/aiokafka_consumer_loop.py')},
             'fastkafka._components.asyncapi': { 'fastkafka._components.asyncapi.APIKeyLocation': ( 'asyncapi.html#apikeylocation',
                                                                                                    'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.ContactInfo': ( 'asyncapi.html#contactinfo',
@@ -251,16 +253,74 @@
                                                                                               'fastkafka/_components/meta.py')},
             'fastkafka._components.producer_decorator': { 'fastkafka._components.producer_decorator.KafkaEvent': ( 'producerdecorator.html#kafkaevent',
                                                                                                                    'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator._wrap_in_event': ( 'producerdecorator.html#_wrap_in_event',
                                                                                                                        'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.get_loop': ( 'producerdecorator.html#get_loop',
                                                                                                                  'fastkafka/_components/producer_decorator.py'),
+                                                          'fastkafka._components.producer_decorator.produce_batch': ( 'producerdecorator.html#produce_batch',
+                                                                                                                      'fastkafka/_components/producer_decorator.py'),
+                                                          'fastkafka._components.producer_decorator.produce_single': ( 'producerdecorator.html#produce_single',
+                                                                                                                       'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.producer_decorator': ( 'producerdecorator.html#producer_decorator',
-                                                                                                                           'fastkafka/_components/producer_decorator.py')},
+                                                                                                                           'fastkafka/_components/producer_decorator.py'),
+                                                          'fastkafka._components.producer_decorator.release_callback': ( 'producerdecorator.html#release_callback',
+                                                                                                                         'fastkafka/_components/producer_decorator.py'),
+                                                          'fastkafka._components.producer_decorator.send_batch': ( 'producerdecorator.html#send_batch',
+                                                                                                                   'fastkafka/_components/producer_decorator.py')},
+            'fastkafka._components.task_streaming': { 'fastkafka._components.task_streaming.DynamicTaskExecutor': ( 'taskstreaming.html#dynamictaskexecutor',
+                                                                                                                    'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.DynamicTaskExecutor.__init__': ( 'taskstreaming.html#dynamictaskexecutor.__init__',
+                                                                                                                             'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.DynamicTaskExecutor.run': ( 'taskstreaming.html#dynamictaskexecutor.run',
+                                                                                                                        'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.ExceptionMonitor': ( 'taskstreaming.html#exceptionmonitor',
+                                                                                                                 'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.ExceptionMonitor.__aenter__': ( 'taskstreaming.html#exceptionmonitor.__aenter__',
+                                                                                                                            'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.ExceptionMonitor.__aexit__': ( 'taskstreaming.html#exceptionmonitor.__aexit__',
+                                                                                                                           'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.ExceptionMonitor.__init__': ( 'taskstreaming.html#exceptionmonitor.__init__',
+                                                                                                                          'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.ExceptionMonitor._monitor_step': ( 'taskstreaming.html#exceptionmonitor._monitor_step',
+                                                                                                                               'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.ExceptionMonitor.on_error': ( 'taskstreaming.html#exceptionmonitor.on_error',
+                                                                                                                          'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.SequentialExecutor': ( 'taskstreaming.html#sequentialexecutor',
+                                                                                                                   'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.SequentialExecutor.__init__': ( 'taskstreaming.html#sequentialexecutor.__init__',
+                                                                                                                            'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.SequentialExecutor.run': ( 'taskstreaming.html#sequentialexecutor.run',
+                                                                                                                       'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.StreamExecutor': ( 'taskstreaming.html#streamexecutor',
+                                                                                                               'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.StreamExecutor.run': ( 'taskstreaming.html#streamexecutor.run',
+                                                                                                                   'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool': ( 'taskstreaming.html#taskpool',
+                                                                                                         'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.__aenter__': ( 'taskstreaming.html#taskpool.__aenter__',
+                                                                                                                    'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.__aexit__': ( 'taskstreaming.html#taskpool.__aexit__',
+                                                                                                                   'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.__init__': ( 'taskstreaming.html#taskpool.__init__',
+                                                                                                                  'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.__len__': ( 'taskstreaming.html#taskpool.__len__',
+                                                                                                                 'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.add': ( 'taskstreaming.html#taskpool.add',
+                                                                                                             'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.discard': ( 'taskstreaming.html#taskpool.discard',
+                                                                                                                 'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.TaskPool.log_error': ( 'taskstreaming.html#taskpool.log_error',
+                                                                                                                   'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming._process_items_coro': ( 'taskstreaming.html#_process_items_coro',
+                                                                                                                    'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming._process_items_task': ( 'taskstreaming.html#_process_items_task',
+                                                                                                                    'fastkafka/_components/task_streaming.py'),
+                                                      'fastkafka._components.task_streaming.get_executor': ( 'taskstreaming.html#get_executor',
+                                                                                                             'fastkafka/_components/task_streaming.py')},
             'fastkafka._components.test_dependencies': { 'fastkafka._components.test_dependencies._install_java': ( 'test_dependencies.html#_install_java',
                                                                                                                     'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies._install_kafka': ( 'test_dependencies.html#_install_kafka',
                                                                                                                      'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies._install_testing_deps': ( 'test_dependencies.html#_install_testing_deps',
                                                                                                                             'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies.check_java': ( 'test_dependencies.html#check_java',
@@ -369,16 +429,24 @@
                                                                                                                          'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.InMemoryProducer': ( 'inmemorybroker.html#inmemoryproducer',
                                                                                                                'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.InMemoryProducer.__call__': ( 'inmemorybroker.html#inmemoryproducer.__call__',
                                                                                                                         'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.InMemoryProducer.__init__': ( 'inmemorybroker.html#inmemoryproducer.__init__',
                                                                                                                         'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.InMemoryProducer._partition': ( 'inmemorybroker.html#inmemoryproducer._partition',
+                                                                                                                          'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.InMemoryProducer.create_batch': ( 'inmemorybroker.html#inmemoryproducer.create_batch',
+                                                                                                                            'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.InMemoryProducer.partitions_for': ( 'inmemorybroker.html#inmemoryproducer.partitions_for',
+                                                                                                                              'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.InMemoryProducer.send': ( 'inmemorybroker.html#inmemoryproducer.send',
                                                                                                                     'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.InMemoryProducer.send_batch': ( 'inmemorybroker.html#inmemoryproducer.send_batch',
+                                                                                                                          'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.InMemoryProducer.start': ( 'inmemorybroker.html#inmemoryproducer.start',
                                                                                                                      'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.InMemoryProducer.stop': ( 'inmemorybroker.html#inmemoryproducer.stop',
                                                                                                                     'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.KafkaPartition': ( 'inmemorybroker.html#kafkapartition',
                                                                                                              'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.KafkaPartition.__init__': ( 'inmemorybroker.html#kafkapartition.__init__',
@@ -401,14 +469,20 @@
                                                                                                               'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.KafkaTopic.write': ( 'inmemorybroker.html#kafkatopic.write',
                                                                                                                'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.KafkaTopic.write_with_key': ( 'inmemorybroker.html#kafkatopic.write_with_key',
                                                                                                                         'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.KafkaTopic.write_with_partition': ( 'inmemorybroker.html#kafkatopic.write_with_partition',
                                                                                                                               'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.MockBatch': ( 'inmemorybroker.html#mockbatch',
+                                                                                                        'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.MockBatch.__init__': ( 'inmemorybroker.html#mockbatch.__init__',
+                                                                                                                 'fastkafka/_testing/in_memory_broker.py'),
+                                                     'fastkafka._testing.in_memory_broker.MockBatch.append': ( 'inmemorybroker.html#mockbatch.append',
+                                                                                                               'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.split_list': ( 'inmemorybroker.html#split_list',
                                                                                                          'fastkafka/_testing/in_memory_broker.py')},
             'fastkafka._testing.local_redpanda_broker': { 'fastkafka._testing.local_redpanda_broker.LocalRedpandaBroker': ( 'localredpandabroker.html#localredpandabroker',
                                                                                                                             'fastkafka/_testing/local_redpanda_broker.py'),
                                                           'fastkafka._testing.local_redpanda_broker.LocalRedpandaBroker.__aenter__': ( 'localredpandabroker.html#localredpandabroker.__aenter__',
                                                                                                                                        'fastkafka/_testing/local_redpanda_broker.py'),
                                                           'fastkafka._testing.local_redpanda_broker.LocalRedpandaBroker.__aexit__': ( 'localredpandabroker.html#localredpandabroker.__aexit__',
@@ -445,8 +519,9 @@
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.mock_AIOKafkaProducer_send': ( 'test_utils.html#mock_aiokafkaproducer_send',
                                                                                                              'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.nb_safe_seed': ( 'test_utils.html#nb_safe_seed',
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.run_script_and_cancel': ( 'test_utils.html#run_script_and_cancel',
                                                                                                         'fastkafka/_testing/test_utils.py')},
+            'fastkafka.encoder': {'fastkafka.encoder.dummy': ('encoder_export.html#dummy', 'fastkafka/encoder.py')},
             'fastkafka.testing': {'fastkafka.testing.dummy': ('testing_export.html#dummy', 'fastkafka/testing.py')}}}
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_server.py` & `fastkafka-0.6.0rc0/fastkafka/_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 from contextlib import contextmanager
 from typing import *
 
 import asyncer
 import typer
 
 from ._components.helpers import _import_from_string
-from ._components.logger import get_logger
+from ._components.logger import get_logger, supress_timestamps
 
 # %% ../nbs/021_FastKafkaServer.ipynb 5
-logger = get_logger(__name__)
+supress_timestamps(False)
+logger = get_logger(__name__, level=20)
 
 # %% ../nbs/021_FastKafkaServer.ipynb 7
 class ServerProcess:
     def __init__(self, app: str, kafka_broker_name: str):
         self.app = app
         self.should_exit = False
         self.kafka_broker_name = kafka_broker_name
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.6.0rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import asyncer
 import nest_asyncio
 
 from .._components._subprocess import terminate_asyncio_process
 from .._components.helpers import in_notebook
 from .._components.logger import get_logger
-from .._components.meta import delegates, filter_using_signature, patch
+from .._components.meta import delegates, export, filter_using_signature, patch
 from .._components.test_dependencies import check_java, check_kafka
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 3
 if in_notebook():
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
@@ -152,14 +152,15 @@
 # The following configuration specifies the time, in milliseconds, that the GroupCoordinator will delay the initial consumer rebalance.
 group.initial.rebalance.delay.ms=0
 """
 
     return kafka_config
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 12
+@export("fastkafka.testing")
 class ApacheKafkaBroker:
     """ApacheKafkaBroker class, used for running unique kafka brokers in tests to prevent topic clashing."""
 
     @delegates(get_kafka_config_string)
     @delegates(get_zookeeper_config_string, keep=True)
     def __init__(
         self,
@@ -287,36 +288,37 @@
     async def __aenter__(self) -> str:
         #         ApacheKafkaBroker._check_deps()
         return await self._start()
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self._stop()
 
-
-ApacheKafkaBroker.__module__ = "fastkafka.testing"
-
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 14
 @patch(cls_method=True)  # type: ignore
 def _check_deps(cls: ApacheKafkaBroker) -> None:
     if not check_java():
         raise RuntimeError(
             "JDK installation not found! Please install JDK manually or run 'fastkafka testing install_deps'."
         )
     if not check_kafka():
         raise RuntimeError(
             "Kafka installation not found! Please install Kafka tools manually or run 'fastkafka testing install_deps'."
         )
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 16
 async def run_and_match(
-    *args: str, capture: str = "stdout", timeout: int = 5, pattern: str
+    *args: str,
+    capture: str = "stdout",
+    timeout: int = 5,
+    pattern: str,
+    num_to_match: int = 1,
 ) -> asyncio.subprocess.Process:
     # Create the subprocess; redirect the standard output
     # into a pipe.
-
+    matched = 0
     proc = await asyncio.create_subprocess_exec(
         *args,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
 
     # Read one line of output.
@@ -331,31 +333,36 @@
                 raise ValueError(
                     f"Unknown capture param value {capture}, supported values are 'stdout', 'stderr'"
                 )
             ddata = data.decode("utf-8")
 
             if len(re.findall(pattern, ddata)) > 0:
                 # print(f"Matched: {ddata}")
-                return proc
+                matched += 1
+                if matched == num_to_match:
+                    return proc
         except asyncio.exceptions.TimeoutError as e:
             pass
 
         if proc.returncode is not None:
             stdout, stderr = await proc.communicate()
             dstdout = stdout.decode("utf-8")
             dstderr = stderr.decode("utf-8")
-            raise RuntimeError(
-                f"stdout={dstdout}, stderr={dstderr}, returncode={proc.returncode}"
-            )
+            if proc.returncode == 0:
+                raise TimeoutError()
+            else:
+                raise RuntimeError(
+                    f"stdout={dstdout}, stderr={dstderr}, returncode={proc.returncode}"
+                )
 
     await terminate_asyncio_process(proc)
 
     raise TimeoutError()
 
-# %% ../../nbs/002_ApacheKafkaBroker.ipynb 18
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 19
 def get_free_port() -> str:
     s = socket.socket()
     s.bind(("127.0.0.1", 0))
     port = str(s.getsockname()[1])
     s.close()
     return port
 
@@ -499,15 +506,15 @@
 @patch
 async def _stop(self: ApacheKafkaBroker) -> None:
     await terminate_asyncio_process(self.kafka_task)  # type: ignore
     await terminate_asyncio_process(self.zookeeper_task)  # type: ignore
     self.temporary_directory.__exit__(None, None, None)  # type: ignore
     self._is_started = False
 
-# %% ../../nbs/002_ApacheKafkaBroker.ipynb 21
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 22
 @patch
 def start(self: ApacheKafkaBroker) -> str:
     """Starts a local kafka broker and zookeeper instance synchronously
     Returns:
        Kafka broker bootstrap server address in string format: add:port
     """
     logger.info(f"{self.__class__.__name__}.start(): entering...")
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.6.0rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/001_InMemoryBroker.ipynb.
 
 # %% auto 0
 __all__ = ['logger', 'KafkaRecord', 'KafkaPartition', 'KafkaTopic', 'split_list', 'GroupMetadata', 'InMemoryBroker',
-           'InMemoryConsumer', 'InMemoryProducer']
+           'InMemoryConsumer', 'InMemoryProducer', 'MockBatch']
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 1
 import asyncio
 import copy
 import hashlib
 import inspect
 import random
 import string
 import uuid
 from collections import namedtuple
 from contextlib import contextmanager
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import *
 
+import aiokafka
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord, RecordMetadata, TopicPartition
 
 import fastkafka._application.app
 import fastkafka._components.aiokafka_consumer_loop
 from .._components.logger import get_logger
 from fastkafka._components.meta import (
@@ -38,14 +39,20 @@
 @dataclass
 class KafkaRecord:
     topic: str = ""
     partition: int = 0
     key: Optional[bytes] = None
     value: bytes = b""
     offset: int = 0
+    timestamp = 0
+    timestamp_type = 0
+    checksum = 0
+    serialized_key_size = 0
+    serialized_value_size = 0
+    headers: Sequence[Tuple[str, bytes]] = field(default_factory=list)
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 7
 class KafkaPartition:
     def __init__(self, *, partition: int, topic: str):
         self.partition = partition
         self.topic = topic
         self.messages: List[KafkaRecord] = list()
@@ -419,14 +426,15 @@
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 46
 @patch
 @delegates(AIOKafkaConsumer.getmany)
 async def getmany(  # type: ignore
     self: InMemoryConsumer, **kwargs: Any
 ) -> Dict[TopicPartition, List[ConsumerRecord]]:
+    await asyncio.sleep(0)
     for topic in self._topics:
         return self.broker.read(
             bootstrap_server=self._bootstrap_servers,
             topic=topic,
             consumer_id=self._id,  # type: ignore
             group=self._group_id,  # type: ignore
             auto_offset_reset=self._auto_offset_reset,
@@ -452,22 +460,40 @@
 
     @delegates(AIOKafkaProducer.stop)
     async def stop(self, **kwargs: Any) -> None:
         raise NotImplementedError()
 
     @delegates(AIOKafkaProducer.send)
     async def send(  # type: ignore
-        self: AIOKafkaProducer,
+        self,
         topic: str,
         msg: bytes,
         key: Optional[bytes] = None,
         **kwargs: Any,
     ):
         raise NotImplementedError()
 
+    @delegates(AIOKafkaProducer.partitions_for)
+    async def partitions_for(self, topic: str) -> List[int]:
+        raise NotImplementedError()
+
+    @delegates(AIOKafkaProducer._partition)
+    def _partition(
+        self, topic: str, arg1: Any, arg2: Any, arg3: Any, key: bytes, arg4: Any
+    ) -> int:
+        raise NotImplementedError()
+
+    @delegates(AIOKafkaProducer.create_batch)
+    def create_batch(self) -> "MockBatch":
+        raise NotImplementedError()
+
+    @delegates(AIOKafkaProducer.send_batch)
+    async def send_batch(self, batch: "MockBatch", topic: str, partition: Any) -> None:
+        raise NotImplementedError()
+
 # %% ../../nbs/001_InMemoryBroker.ipynb 52
 @patch  # type: ignore
 @delegates(AIOKafkaProducer.start)
 async def start(self: InMemoryProducer, **kwargs: Any) -> None:
     logger.info("AIOKafkaProducer patched start() called()")
     if self.id is not None:
         raise RuntimeError(
@@ -506,15 +532,75 @@
     )
 
     async def _f(record: ConsumerRecord = record) -> RecordMetadata:  # type: ignore
         return record
 
     return asyncio.create_task(_f())
 
-# %% ../../nbs/001_InMemoryBroker.ipynb 61
+# %% ../../nbs/001_InMemoryBroker.ipynb 60
+@patch
+@delegates(AIOKafkaProducer.partitions_for)
+async def partitions_for(self: InMemoryProducer, topic: str) -> List[int]:
+    return [i for i in range(self.broker.num_partitions)]
+
+# %% ../../nbs/001_InMemoryBroker.ipynb 62
+@patch
+@delegates(AIOKafkaProducer._partition)
+def _partition(
+    self: InMemoryProducer,
+    topic: str,
+    arg1: Any,
+    arg2: Any,
+    arg3: Any,
+    key: bytes,
+    arg4: Any,
+) -> int:
+    return int(hashlib.sha256(key).hexdigest(), 16) % self.broker.num_partitions
+
+# %% ../../nbs/001_InMemoryBroker.ipynb 64
+class MockBatch:
+    def __init__(self) -> None:
+        self._batch: List[Tuple] = list()
+
+    def append(  # type: ignore
+        self, key: Optional[bytes], value: bytes, timestamp: int
+    ) -> RecordMetadata:
+        self._batch.append((key, value))
+        return RecordMetadata(
+            topic="",
+            partition=0,
+            topic_partition=None,
+            offset=0,
+            timestamp=timestamp,
+            timestamp_type=0,
+            log_start_offset=0,
+        )
+
+
+@patch
+@delegates(AIOKafkaProducer.create_batch)
+def create_batch(self: InMemoryProducer) -> "MockBatch":
+    return MockBatch()
+
+
+@patch
+@delegates(AIOKafkaProducer.send_batch)
+async def send_batch(
+    self: InMemoryProducer, batch: "MockBatch", topic: str, partition: Any
+) -> None:
+    for record in batch._batch:
+        self.broker.write(
+            bootstrap_server=self._bootstrap_servers,
+            topic=topic,
+            value=record[1],
+            key=record[0],
+            partition=partition,
+        )
+
+# %% ../../nbs/001_InMemoryBroker.ipynb 68
 @patch
 @contextmanager
 def lifecycle(self: InMemoryBroker) -> Iterator[InMemoryBroker]:
     logger.info(
         "InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!"
     )
     try:
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.6.0rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import asyncer
 import nest_asyncio
 
 from .._components._subprocess import terminate_asyncio_process
 from .._components.helpers import in_notebook
 from .._components.logger import get_logger, supress_timestamps
-from .._components.meta import delegates, patch
+from .._components.meta import delegates, export, patch
 from .apache_kafka_broker import get_free_port, run_and_match
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 3
 if in_notebook():
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
@@ -70,14 +70,15 @@
         mode,
         "--default-log-level",
         default_log_level,
     ]
     return redpanda_docker_cmd
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 8
+@export("fastkafka.testing")
 class LocalRedpandaBroker:
     """LocalRedpandaBroker class, used for running unique redpanda brokers in tests to prevent topic clashing."""
 
     @delegates(get_redpanda_docker_cmd, keep=True)
     def __init__(
         self,
         topics: Iterable[str] = [],
@@ -183,17 +184,14 @@
 
     async def __aenter__(self) -> str:
         return await self._start()
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self._stop()
 
-
-LocalRedpandaBroker.__module__ = "fastkafka.testing"
-
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 10
 async def check_docker() -> bool:
     try:
         docker_task = await run_and_match("docker", "-v", pattern="Docker version")
         return True
     except Exception as e:
         logger.debug(f"Error in check_docker() : {e}")
```

### Comparing `fastkafka-0.5.0rc0/fastkafka/_testing/test_utils.py` & `fastkafka-0.6.0rc0/fastkafka/_testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0rc0/fastkafka/testing.py` & `fastkafka-0.6.0rc0/fastkafka/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/000_Testing_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/000_Testing_export.ipynb 1
 from ._application.tester import Tester
+from ._components.meta import export
 from ._testing.apache_kafka_broker import ApacheKafkaBroker
 from ._testing.in_memory_broker import InMemoryBroker
 from ._testing.local_redpanda_broker import LocalRedpandaBroker
 from fastkafka._testing.test_utils import (
     display_docs,
     mock_AIOKafkaProducer_send,
     nb_safe_seed,
@@ -24,12 +25,10 @@
     "true_after",
     "mock_AIOKafkaProducer_send",
     "run_script_and_cancel",
     "display_docs",
 ]
 
 # %% ../nbs/000_Testing_export.ipynb 3
+@export("_dummy")
 def dummy() -> None:
     pass
-
-
-dummy.__module__ = "_dummy"
```

### Comparing `fastkafka-0.5.0rc0/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.6.0rc0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: fastkafka
-Version: 0.5.0rc0
-Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
-Home-page: https://github.com/airtai/fastkafka
-Author: airt
-Author-email: info@airt.ai
-License: Apache Software License 2.0
-Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
-Project-URL: CI, https://github.com/airtai/fastkafka/actions
-Project-URL: Documentation, https://fastkafka.airt.ai/
-Project-URL: Tutorial, https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb
-Keywords: nbdev jupyter notebook python kafka
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: avro
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
 FastKafka
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <b>Effortless Kafka integration for your web services</b>
 
@@ -285,15 +255,14 @@
   a new `IrisPrediction` message using this value and then returns it.
   The framework will call the `IrisPrediction.json().encode("utf-8")`
   function on the returned value and produce it to the specified topic.
 
 ``` python
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
 async def on_input_data(msg: IrisInputData):
-    global model
     species_class = ml_models["iris_predictor"].predict(
         [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
     )[0]
 
     to_predictions(species_class)
 
 
@@ -337,19 +306,15 @@
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker starting
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched start() called()
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
@@ -358,27 +323,24 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['predictions']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
+    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
-    [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
 We have created a Iris classification model and encapulated it into our
 fastkafka application. The app will consume the IrisInputData from the
@@ -401,14 +363,36 @@
 The service can be started using builtin faskafka run CLI command.
 Before we can do that, we will concatenate the code snippets from above
 and save them in a file `"application.py"`
 
 ``` python
 # content of the "application.py" file
 
+from contextlib import asynccontextmanager
+
+from sklearn.datasets import load_iris
+from sklearn.linear_model import LogisticRegression
+
+from fastkafka import FastKafka
+
+ml_models = {}
+
+
+@asynccontextmanager
+async def lifespan(app: FastKafka):
+    # Load the ML model
+    X, y = load_iris(return_X_y=True)
+    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
+        X, y
+    )
+    yield
+    # Clean up the ML models and release the resources
+    ml_models.clear()
+
+
 from pydantic import BaseModel, NonNegativeFloat, Field
 
 class IrisInputData(BaseModel):
     sepal_length: NonNegativeFloat = Field(
         ..., example=0.5, description="Sepal length in cm"
     )
     sepal_width: NonNegativeFloat = Field(
@@ -441,30 +425,30 @@
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
     title="Iris predictions",
     kafka_brokers=kafka_brokers,
+    lifespan=lifespan,
 )
 
-iris_species = ["setosa", "versicolor", "virginica"]
-
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
 async def on_input_data(msg: IrisInputData):
-    global model
-    species_class = model.predict([
-          [msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]
-        ])[0]
+    species_class = ml_models["iris_predictor"].predict(
+        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
+    )[0]
 
     to_predictions(species_class)
 
 
 @kafka_app.produces(topic="predictions")
 def to_predictions(species_class: int) -> IrisPrediction:
+    iris_species = ["setosa", "versicolor", "virginica"]
+
     prediction = IrisPrediction(species=iris_species[species_class])
     return prediction
 ```
 
 To run the service, you will need a running Kafka broker on localhost as
 specified in the `kafka_brokers` parameter above. We can start the Kafka
 broker locally using the
@@ -514,81 +498,63 @@
 fastkafka run --num-workers=2 --kafka-broker localhost application:kafka_app
 ```
 
 In the above command, we use `--num-workers` option to specify how many
 workers to launch and we use `--kafka-broker` option to specify which
 kafka broker configuration to use from earlier specified `kafka_brokers`
 
-    [558863]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [558863]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
-    [558865]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [558865]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Entering...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Starting send_stream
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.start(): Finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [558865]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [558865]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [558863]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [558863]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [558863]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [558863]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [558865]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [558865]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [558865]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.26.0.2', 9092)
-    [558863]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.26.0.2', 9092)
-    [558865]: [ERROR] aiokafka: Unable to update metadata from [0]
-    [558863]: [ERROR] aiokafka: Unable to update metadata from [0]
+    [801767]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [801765]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [801767]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [801765]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [801767]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [801767]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [801765]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [801765]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [801765]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [801765]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [801767]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [801767]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [801767]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
+    [801765]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
+    [801767]: [ERROR] aiokafka: Unable to update metadata from [0]
+    [801765]: [ERROR] aiokafka: Unable to update metadata from [0]
     ^C
     Starting process cleanup, this may take a few seconds...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 558863...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 558865...
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [558863]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
-    [558863]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [558865]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Entering...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Exiting send_stream
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: _aiokafka_producer_manager(): Finished.
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Stoping producer...
-    [558865]: [INFO] fastkafka._components.aiokafka_producer_manager: AIOKafkaProducerManager.stop(): Finished
-    [INFO] fastkafka._server: terminate_asyncio_process(): Process 558863 was already terminated.
-    [INFO] fastkafka._server: terminate_asyncio_process(): Process 558865 was already terminated.
+    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801765...
+    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801767...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
 
 You need to interupt running of the cell above by selecting
 `Runtime->Interupt execution` on the toolbar above.
 
 Finally, we can stop the local Kafka Broker:
 
 ``` python
 broker.stop()
 ```
 
     [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): entering...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 558265...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 558265 was already terminated.
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 557885...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 557885 was already terminated.
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 801303...
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 801303 was already terminated.
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 800930...
+    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 800930 was already terminated.
     [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): exited.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
@@ -604,15 +570,14 @@
 To generate the documentation programatically you just need to call the
 folloving command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: Old async specifications at '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml' does not exist.
     [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
     [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
     [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
@@ -621,16 +586,16 @@
 with:
 
 ``` sh
 ls -l asyncapi
 ```
 
     total 8
-    drwxrwxr-x 4 tvrtko tvrtko 4096 Apr  5 08:02 docs
-    drwxrwxr-x 2 tvrtko tvrtko 4096 Apr  5 08:02 spec
+    drwxrwxr-x 4 kumaran kumaran 4096 Mar 21 09:14 docs
+    drwxrwxr-x 2 kumaran kumaran 4096 Mar 21 09:14 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -705,9 +670,7 @@
 A permissive license whose main conditions require preservation of
 copyright and license notices. Contributors provide an express grant of
 patent rights. Licensed works, modifications, and larger works may be
 distributed under different terms and without source code.
 
 The full text of the license can be found
 [here](https://raw.githubusercontent.com/airtai/fastkafka/main/LICENSE).
-
-
```

### Comparing `fastkafka-0.5.0rc0/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.6.0rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 fastkafka/__init__.py
 fastkafka/_cli.py
 fastkafka/_cli_docs.py
 fastkafka/_cli_testing.py
 fastkafka/_docusaurus_helper.py
 fastkafka/_helpers.py
 fastkafka/_modidx.py
 fastkafka/_server.py
+fastkafka/encoder.py
 fastkafka/testing.py
 fastkafka.egg-info/PKG-INFO
 fastkafka.egg-info/SOURCES.txt
 fastkafka.egg-info/dependency_links.txt
 fastkafka.egg-info/entry_points.txt
 fastkafka.egg-info/not-zip-safe
 fastkafka.egg-info/requires.txt
@@ -28,14 +30,15 @@
 fastkafka/_components/asyncapi.py
 fastkafka/_components/benchmarking.py
 fastkafka/_components/docs_dependencies.py
 fastkafka/_components/helpers.py
 fastkafka/_components/logger.py
 fastkafka/_components/meta.py
 fastkafka/_components/producer_decorator.py
+fastkafka/_components/task_streaming.py
 fastkafka/_components/test_dependencies.py
 fastkafka/_components/encoder/__init__.py
 fastkafka/_components/encoder/avro.py
 fastkafka/_components/encoder/json.py
 fastkafka/_testing/__init__.py
 fastkafka/_testing/apache_kafka_broker.py
 fastkafka/_testing/in_memory_broker.py
```

### Comparing `fastkafka-0.5.0rc0/fastkafka.egg-info/requires.txt` & `fastkafka-0.6.0rc0/fastkafka.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 
 [avro]
 fastavro>=1.7.3
 
 [dev]
 PyYAML>=5.3.1
 aiohttp>=3.8.4
-bandit==1.7.4
-black==23.1.0
+bandit==1.7.5
+black==23.3.0
 email-validator==1.3.1
 fastavro>=1.7.3
 install-jdk==0.3.0
+ipython<8.13
 ipywidgets<=8.0.4,>=8.0
 isort==5.12.0
-mypy==1.0.1
+mypy==1.3.0
 nbconvert>=7.2.9
-nbdev-mkdocs==0.3.0
+nbdev-mkdocs==0.4.0
 nbformat>=5.7.3
 nbqa==1.6.3
 numpy>=1.21.0
 pandas>=1.2.0
-pre-commit==3.0.4
-pytest==7.2.1
+pre-commit==3.3.1
+pytest==7.3.1
 requests>=2.20
 scikit-learn==1.2.1
-semgrep==1.14.0
+semgrep==1.21.0
 
 [docs]
 PyYAML>=5.3.1
 aiohttp>=3.8.4
 
 [test]
 install-jdk==0.3.0
```

### Comparing `fastkafka-0.5.0rc0/settings.ini` & `fastkafka-0.6.0rc0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.5.0rc0
+version = 0.6.0rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 black_formatting = True
-docs_versioning = None
+docs_versioning = patch
 
 ### Docs ###
 branch = main
 custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
```

### Comparing `fastkafka-0.5.0rc0/setup.py` & `fastkafka-0.6.0rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,27 +49,28 @@
 
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 
 dev_requirements = [
     "nbconvert>=7.2.9",
     "nbformat>=5.7.3",
-    "nbdev-mkdocs==0.3.0",
-    "mypy==1.0.1",
-    "pre-commit==3.0.4",
+    "nbdev-mkdocs==0.4.0",
+    "mypy==1.3.0",
+    "pre-commit==3.3.1",
     "nbqa==1.6.3",
-    "black==23.1.0",
+    "black==23.3.0",
     "isort==5.12.0",
-    "bandit==1.7.4",
-    "semgrep==1.14.0",
-    "pytest==7.2.1",
+    "bandit==1.7.5",
+    "semgrep==1.21.0",
+    "pytest==7.3.1",
     "numpy>=1.21.0",
     "pandas>=1.2.0",
     "email-validator==1.3.1",
     "scikit-learn==1.2.1",
+    "ipython<8.13"
 ]
 
 project_urls = {
    'Bug Tracker': cfg['git_url'] + '/issues',
    'CI': cfg['git_url'] + '/actions',
    'Documentation': 'https://fastkafka.airt.ai/',
 #    'Source Code': cfg['git_url'],
```


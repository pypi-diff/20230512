# Comparing `tmp/eventiq-0.1.5.tar.gz` & `tmp/eventiq-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventiq-0.1.5.tar", max compression
+gzip compressed data, was "eventiq-0.1.6.tar", max compression
```

## Comparing `eventiq-0.1.5.tar` & `eventiq-0.1.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    11357 2023-05-09 21:04:19.342155 eventiq-0.1.5/LICENSE
--rw-r--r--   0        0        0     4649 2023-05-09 21:04:19.342155 eventiq-0.1.5/README.md
--rw-r--r--   0        0        0      772 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/__init__.py
--rw-r--r--   0        0        0       59 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/__main__.py
--rw-r--r--   0        0        0       22 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/_version.py
--rw-r--r--   0        0        0      171 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/__init__.py
--rw-r--r--   0        0        0     2636 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/generator.py
--rw-r--r--   0        0        0     1579 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/models.py
--rw-r--r--   0        0        0      426 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/registry.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/__init__.py
--rw-r--r--   0        0        0       59 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/kafka/__init__.py
--rw-r--r--   0        0        0     3673 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/kafka/broker.py
--rw-r--r--   0        0        0      482 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/kafka/settings.py
--rw-r--r--   0        0        0      163 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/__init__.py
--rw-r--r--   0        0        0     5447 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/broker.py
--rw-r--r--   0        0        0     2809 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/plugins.py
--rw-r--r--   0        0        0      617 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/settings.py
--rw-r--r--   0        0        0       61 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/pubsub/__init__.py
--rw-r--r--   0        0        0     2470 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/pubsub/broker.py
--rw-r--r--   0        0        0      179 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/pubsub/settings.py
--rw-r--r--   0        0        0       65 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/__init__.py
--rw-r--r--   0        0        0     5044 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/broker.py
--rw-r--r--   0        0        0      816 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/middlewares.py
--rw-r--r--   0        0        0      437 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/settings.py
--rw-r--r--   0        0        0      121 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/__init__.py
--rw-r--r--   0        0        0     1894 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/broker.py
--rw-r--r--   0        0        0     1767 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/plugins.py
--rw-r--r--   0        0        0      305 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/settings.py
--rw-r--r--   0        0        0     2004 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/stub.py
--rw-r--r--   0        0        0     9560 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/broker.py
--rw-r--r--   0        0        0     2466 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/cli.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/factory.py
--rw-r--r--   0        0        0     1824 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/models.py
--rw-r--r--   0        0        0      226 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/settings.py
--rw-r--r--   0        0        0     4206 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/consumer.py
--rw-r--r--   0        0        0      558 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/context.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/contrib/__init__.py
--rw-r--r--   0        0        0     1443 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/contrib/fastapi.py
--rw-r--r--   0        0        0      282 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/__init__.py
--rw-r--r--   0        0        0      670 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/json.py
--rw-r--r--   0        0        0      706 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/msgpack.py
--rw-r--r--   0        0        0      645 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/orjson.py
--rw-r--r--   0        0        0      494 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/pickle.py
--rw-r--r--   0        0        0      873 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/exceptions.py
--rw-r--r--   0        0        0     1148 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/logger.py
--rw-r--r--   0        0        0      784 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/message.py
--rw-r--r--   0        0        0     3333 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middleware.py
--rw-r--r--   0        0        0      354 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/__init__.py
--rw-r--r--   0        0        0      871 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/debug.py
--rw-r--r--   0        0        0      860 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/error.py
--rw-r--r--   0        0        0     1729 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/healthcheck.py
--rw-r--r--   0        0        0     4435 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/opentelemetry.py
--rw-r--r--   0        0        0     5115 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/prometheus.py
--rw-r--r--   0        0        0     3926 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/retries.py
--rw-r--r--   0        0        0     2352 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/models.py
--rw-r--r--   0        0        0      585 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/plugins.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/py.typed
--rw-r--r--   0        0        0      740 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/runner.py
--rw-r--r--   0        0        0     3649 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/service.py
--rw-r--r--   0        0        0      643 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/settings.py
--rw-r--r--   0        0        0     1253 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/types.py
--rw-r--r--   0        0        0      216 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/__init__.py
--rw-r--r--   0        0        0      192 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/datetime.py
--rw-r--r--   0        0        0      390 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/enum.py
--rw-r--r--   0        0        0     1862 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/functools.py
--rw-r--r--   0        0        0     1106 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/imports.py
--rw-r--r--   0        0        0     4258 2023-05-09 21:04:19.346155 eventiq-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 eventiq-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 11:16:55.023601 eventiq-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4649 2023-05-12 11:16:55.023601 eventiq-0.1.6/README.md
+-rw-r--r--   0        0        0      772 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/_version.py
+-rw-r--r--   0        0        0      171 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/asyncapi/__init__.py
+-rw-r--r--   0        0        0     2636 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/asyncapi/generator.py
+-rw-r--r--   0        0        0     1579 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/asyncapi/models.py
+-rw-r--r--   0        0        0      426 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/asyncapi/registry.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/kafka/__init__.py
+-rw-r--r--   0        0        0     3673 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/kafka/broker.py
+-rw-r--r--   0        0        0      482 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/kafka/settings.py
+-rw-r--r--   0        0        0      163 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/nats/__init__.py
+-rw-r--r--   0        0        0     5447 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/nats/broker.py
+-rw-r--r--   0        0        0     2809 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/nats/plugins.py
+-rw-r--r--   0        0        0      617 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/nats/settings.py
+-rw-r--r--   0        0        0       61 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/pubsub/__init__.py
+-rw-r--r--   0        0        0     2470 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/pubsub/broker.py
+-rw-r--r--   0        0        0      179 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/pubsub/settings.py
+-rw-r--r--   0        0        0       65 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     5044 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/rabbitmq/broker.py
+-rw-r--r--   0        0        0      816 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/rabbitmq/middlewares.py
+-rw-r--r--   0        0        0      437 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/rabbitmq/settings.py
+-rw-r--r--   0        0        0      121 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/redis/__init__.py
+-rw-r--r--   0        0        0     1894 2023-05-12 11:16:55.027601 eventiq-0.1.6/eventiq/backends/redis/broker.py
+-rw-r--r--   0        0        0     1767 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/backends/redis/plugins.py
+-rw-r--r--   0        0        0      305 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/backends/redis/settings.py
+-rw-r--r--   0        0        0     2004 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/backends/stub.py
+-rw-r--r--   0        0        0     9566 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/broker.py
+-rw-r--r--   0        0        0     2466 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/cli.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/config/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/config/factory.py
+-rw-r--r--   0        0        0     1824 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/config/models.py
+-rw-r--r--   0        0        0      226 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/config/settings.py
+-rw-r--r--   0        0        0     4206 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/consumer.py
+-rw-r--r--   0        0        0      558 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/context.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/contrib/__init__.py
+-rw-r--r--   0        0        0     1443 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/contrib/fastapi.py
+-rw-r--r--   0        0        0      282 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/encoders/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/encoders/json.py
+-rw-r--r--   0        0        0      706 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/encoders/msgpack.py
+-rw-r--r--   0        0        0      645 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/encoders/orjson.py
+-rw-r--r--   0        0        0      494 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/encoders/pickle.py
+-rw-r--r--   0        0        0      873 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/logger.py
+-rw-r--r--   0        0        0      784 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/message.py
+-rw-r--r--   0        0        0     3333 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middleware.py
+-rw-r--r--   0        0        0      354 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/debug.py
+-rw-r--r--   0        0        0      860 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/error.py
+-rw-r--r--   0        0        0     1729 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/healthcheck.py
+-rw-r--r--   0        0        0     4435 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/opentelemetry.py
+-rw-r--r--   0        0        0     5115 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/prometheus.py
+-rw-r--r--   0        0        0     3926 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/middlewares/retries.py
+-rw-r--r--   0        0        0     2352 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/models.py
+-rw-r--r--   0        0        0      585 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/py.typed
+-rw-r--r--   0        0        0      740 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/runner.py
+-rw-r--r--   0        0        0     3649 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/service.py
+-rw-r--r--   0        0        0      643 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/settings.py
+-rw-r--r--   0        0        0     1253 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/types.py
+-rw-r--r--   0        0        0      216 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/utils/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/utils/datetime.py
+-rw-r--r--   0        0        0      390 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/utils/enum.py
+-rw-r--r--   0        0        0     1862 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/utils/functools.py
+-rw-r--r--   0        0        0     1106 2023-05-12 11:16:55.031602 eventiq-0.1.6/eventiq/utils/imports.py
+-rw-r--r--   0        0        0     4258 2023-05-12 11:16:55.031602 eventiq-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 eventiq-0.1.6/PKG-INFO
```

### Comparing `eventiq-0.1.5/LICENSE` & `eventiq-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/README.md` & `eventiq-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.5
+Version: 0.1.6
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
```

### Comparing `eventiq-0.1.5/eventiq/__init__.py` & `eventiq-0.1.6/eventiq/__init__.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/asyncapi/generator.py` & `eventiq-0.1.6/eventiq/asyncapi/generator.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/asyncapi/models.py` & `eventiq-0.1.6/eventiq/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/kafka/broker.py` & `eventiq-0.1.6/eventiq/backends/kafka/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/nats/broker.py` & `eventiq-0.1.6/eventiq/backends/nats/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/nats/plugins.py` & `eventiq-0.1.6/eventiq/backends/nats/plugins.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/nats/settings.py` & `eventiq-0.1.6/eventiq/backends/nats/settings.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/pubsub/broker.py` & `eventiq-0.1.6/eventiq/backends/pubsub/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/rabbitmq/broker.py` & `eventiq-0.1.6/eventiq/backends/rabbitmq/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/rabbitmq/middlewares.py` & `eventiq-0.1.6/eventiq/backends/rabbitmq/middlewares.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/redis/broker.py` & `eventiq-0.1.6/eventiq/backends/redis/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/redis/plugins.py` & `eventiq-0.1.6/eventiq/backends/redis/plugins.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/backends/stub.py` & `eventiq-0.1.6/eventiq/backends/stub.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/broker.py` & `eventiq-0.1.6/eventiq/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,18 +224,18 @@
         await self._dispatch(f"before_{event}", *args, **kwargs)
 
     async def dispatch_after(self, event: str, *args, **kwargs) -> None:
         await self._dispatch(f"after_{event}", *args, **kwargs)
 
     @classmethod
     def from_settings(cls, settings: BrokerSettings, **kwargs: Any) -> Broker:
-        broker_cls: type[Broker] = cast(Type[Broker], settings.broker_class)
-        kw = settings.dict(exclude={"broker_cls"})
+        broker_class: type[Broker] = cast(Type[Broker], settings.broker_class)
+        kw = settings.dict(exclude={"broker_class"})
         kw.update(kwargs)
-        return broker_cls(**kw)
+        return broker_class(**kw)
 
     @classmethod
     def from_env(
         cls,
         **kwargs,
     ) -> Broker:
         return cls.from_settings(BrokerSettings(), **kwargs)
```

### Comparing `eventiq-0.1.5/eventiq/cli.py` & `eventiq-0.1.6/eventiq/cli.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/config/factory.py` & `eventiq-0.1.6/eventiq/config/factory.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/config/models.py` & `eventiq-0.1.6/eventiq/config/models.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/consumer.py` & `eventiq-0.1.6/eventiq/consumer.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/context.py` & `eventiq-0.1.6/eventiq/context.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/contrib/fastapi.py` & `eventiq-0.1.6/eventiq/contrib/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/encoders/json.py` & `eventiq-0.1.6/eventiq/encoders/json.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/encoders/msgpack.py` & `eventiq-0.1.6/eventiq/encoders/msgpack.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/encoders/orjson.py` & `eventiq-0.1.6/eventiq/encoders/orjson.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/exceptions.py` & `eventiq-0.1.6/eventiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/logger.py` & `eventiq-0.1.6/eventiq/logger.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/message.py` & `eventiq-0.1.6/eventiq/message.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middleware.py` & `eventiq-0.1.6/eventiq/middleware.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middlewares/debug.py` & `eventiq-0.1.6/eventiq/middlewares/debug.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middlewares/error.py` & `eventiq-0.1.6/eventiq/middlewares/error.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middlewares/healthcheck.py` & `eventiq-0.1.6/eventiq/middlewares/healthcheck.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middlewares/opentelemetry.py` & `eventiq-0.1.6/eventiq/middlewares/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middlewares/prometheus.py` & `eventiq-0.1.6/eventiq/middlewares/prometheus.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/middlewares/retries.py` & `eventiq-0.1.6/eventiq/middlewares/retries.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/models.py` & `eventiq-0.1.6/eventiq/models.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/plugins.py` & `eventiq-0.1.6/eventiq/plugins.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/runner.py` & `eventiq-0.1.6/eventiq/runner.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/service.py` & `eventiq-0.1.6/eventiq/service.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/settings.py` & `eventiq-0.1.6/eventiq/settings.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/types.py` & `eventiq-0.1.6/eventiq/types.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/utils/functools.py` & `eventiq-0.1.6/eventiq/utils/functools.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/eventiq/utils/imports.py` & `eventiq-0.1.6/eventiq/utils/imports.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.5/pyproject.toml` & `eventiq-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventiq"
-version = "0.1.5"
+version = "0.1.6"
 description = "Cloud native framework for building event driven applications in Python."
 authors = ["Radzim Kowalow <radzim.kowalow@performance-media.pl>"]
 readme = "README.md"
 license = "Apache License 2.0"
 documentation = "https://performancemedia.github.io/eventiq/"
 repository = "https://github.com/performancemedia/eventiq"
 classifiers = [
```

### Comparing `eventiq-0.1.5/PKG-INFO` & `eventiq-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventiq
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cloud native framework for building event driven applications in Python.
 Home-page: https://github.com/performancemedia/eventiq
 License: Apache-2.0
 Keywords: framework,asyncio,microservice,event-driven
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.8.1,<4.0
@@ -71,15 +71,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.5
+Version: 0.1.6
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
```


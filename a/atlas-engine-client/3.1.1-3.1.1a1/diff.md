# Comparing `tmp/atlas_engine_client-3.1.1.tar.gz` & `tmp/atlas_engine_client-3.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas_engine_client-3.1.1.tar", last modified: Fri May 12 10:19:17 2023, max compression
+gzip compressed data, was "atlas_engine_client-3.1.1a1.tar", last modified: Fri May 12 10:15:21 2023, max compression
```

## Comparing `atlas_engine_client-3.1.1.tar` & `atlas_engine_client-3.1.1a1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.966251 atlas_engine_client-3.1.1/atlas_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.966251 atlas_engine_client-3.1.1/atlas_engine_client/app_info/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/app_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/app_info/app_info_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.970251 atlas_engine_client-3.1.1/atlas_engine_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.970251 atlas_engine_client-3.1.1/atlas_engine_client/core/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.970251 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/application_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/data_object_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/empty_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/external_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/flow_node_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/manual_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/process_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/process_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/process_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/user_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/core/loop_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.970251 atlas_engine_client-3.1.1/atlas_engine_client/event/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/event/event_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.970251 atlas_engine_client-3.1.1/atlas_engine_client/external_task/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/external_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/external_task/client_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/external_task/external_task_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/external_task/external_task_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/external_task/functional_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/atlas_engine_client/flow_node_instance/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/flow_node_instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/flow_node_instance/flow_node_instance_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/atlas_engine_client/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/notification/notification_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/atlas_engine_client/process_definition/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/process_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/process_definition/process_definition_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/process_definition/start_callback_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/atlas_engine_client/process_instance/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/process_instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/process_instance/process_instance_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/atlas_engine_client/user_task/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/user_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/atlas_engine_client/user_task/user_task_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.966251 atlas_engine_client-3.1.1/atlas_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-12 10:19:17.000000 atlas_engine_client-3.1.1/atlas_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-12 10:19:17.000000 atlas_engine_client-3.1.1/atlas_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:19:17.000000 atlas_engine_client-3.1.1/atlas_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 10:19:17.000000 atlas_engine_client-3.1.1/atlas_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-12 10:19:17.000000 atlas_engine_client-3.1.1/atlas_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-12 10:19:17.000000 atlas_engine_client-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/core/test_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/core/test_loop_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/helper_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:17.974251 atlas_engine_client-3.1.1/tests/process_control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 10:19:09.000000 atlas_engine_client-3.1.1/tests/process_control/test_process_control_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.957779 atlas_engine_client-3.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-12 10:15:21.957779 atlas_engine_client-3.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.945778 atlas_engine_client-3.1.1a1/atlas_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.945778 atlas_engine_client-3.1.1a1/atlas_engine_client/app_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/app_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/app_info/app_info_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.945778 atlas_engine_client-3.1.1a1/atlas_engine_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.945778 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.949778 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/application_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/data_object_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/empty_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/external_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/flow_node_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/manual_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/process_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/process_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/process_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/user_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/core/loop_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.949778 atlas_engine_client-3.1.1a1/atlas_engine_client/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/event/event_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.953778 atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/external_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/external_task_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/functional_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.953778 atlas_engine_client-3.1.1a1/atlas_engine_client/flow_node_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/flow_node_instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/flow_node_instance/flow_node_instance_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.953778 atlas_engine_client-3.1.1a1/atlas_engine_client/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/notification/notification_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.953778 atlas_engine_client-3.1.1a1/atlas_engine_client/process_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/process_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/process_definition/process_definition_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/process_definition/start_callback_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.953778 atlas_engine_client-3.1.1a1/atlas_engine_client/process_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/process_instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/process_instance/process_instance_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.953778 atlas_engine_client-3.1.1a1/atlas_engine_client/user_task/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/user_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/atlas_engine_client/user_task/user_task_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.945778 atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-12 10:15:21.000000 atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-12 10:15:21.000000 atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:15:21.000000 atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 10:15:21.000000 atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-12 10:15:21.000000 atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:15:21.957779 atlas_engine_client-3.1.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-12 10:15:21.000000 atlas_engine_client-3.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.957779 atlas_engine_client-3.1.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.957779 atlas_engine_client-3.1.1a1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/core/test_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/core/test_loop_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/helper_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:21.957779 atlas_engine_client-3.1.1a1/tests/process_control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 10:15:17.000000 atlas_engine_client-3.1.1a1/tests/process_control/test_process_control_client.py
```

### Comparing `atlas_engine_client-3.1.1/PKG-INFO` & `atlas_engine_client-3.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas_engine_client
-Version: 3.1.1
+Version: 3.1.1a1
 Summary: A Client for the workflow engine of the ProcessCube platform.
 Home-page: https://github.com/atlas-engine/Client.py
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: ProcessCube@5Minds.de
 Keywords: workflow-engine atlas-engine client bpmn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atlas_engine_client-3.1.1/README.md` & `atlas_engine_client-3.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/__init__.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/app_info/app_info_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/app_info/app_info_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/client_factory.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/client_factory.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/__init__.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/base_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/base_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/application_info.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/application_info.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/data_object_instances.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/data_object_instances.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/empty_tasks.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/empty_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/events.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/events.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/external_tasks.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/external_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/flow_node_instances.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/flow_node_instances.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/manual_tasks.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/manual_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/process_definitions.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/process_definitions.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/process_instances.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/process_instances.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/process_models.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/process_models.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/api/helpers/user_tasks.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/api/helpers/user_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/base_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/base_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/core/loop_helper.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/core/loop_helper.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/event/event_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/event/event_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/external_task/client_wrapper.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/external_task/external_task_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/external_task_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/external_task/external_task_worker.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/external_task/external_task_worker.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/flow_node_instance/flow_node_instance_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/flow_node_instance/flow_node_instance_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/notification/notification_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/notification/notification_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/process_definition/process_definition_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/process_definition/process_definition_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/process_instance/process_instance_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/process_instance/process_instance_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client/user_task/user_task_client.py` & `atlas_engine_client-3.1.1a1/atlas_engine_client/user_task/user_task_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client.egg-info/PKG-INFO` & `atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-engine-client
-Version: 3.1.1
+Version: 3.1.1a1
 Summary: A Client for the workflow engine of the ProcessCube platform.
 Home-page: https://github.com/atlas-engine/Client.py
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: ProcessCube@5Minds.de
 Keywords: workflow-engine atlas-engine client bpmn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atlas_engine_client-3.1.1/atlas_engine_client.egg-info/SOURCES.txt` & `atlas_engine_client-3.1.1a1/atlas_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/setup.py` & `atlas_engine_client-3.1.1a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='atlas_engine_client',
-    version=setuptools.sic('3.1.1'),
+    version=setuptools.sic('3.1.1-alpha.1'),
     author="5Minds IT-Solutions GmbH & Co. KG",
     author_email="ProcessCube@5Minds.de",
     description="A Client for the workflow engine of the ProcessCube platform.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="workflow-engine atlas-engine client bpmn",
     url="https://github.com/atlas-engine/Client.py",
```

### Comparing `atlas_engine_client-3.1.1/tests/core/test_base_client.py` & `atlas_engine_client-3.1.1a1/tests/core/test_base_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/tests/helper_aiohttp.py` & `atlas_engine_client-3.1.1a1/tests/helper_aiohttp.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.1/tests/process_control/test_process_control_client.py` & `atlas_engine_client-3.1.1a1/tests/process_control/test_process_control_client.py`

 * *Files identical despite different names*


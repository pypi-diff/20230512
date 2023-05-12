# Comparing `tmp/statefun-tasks-0.9.92.tar.gz` & `tmp/statefun-tasks-0.9.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statefun-tasks-0.9.92.tar", last modified: Thu Apr 13 15:26:02 2023, max compression
+gzip compressed data, was "statefun-tasks-0.9.93.tar", last modified: Fri May 12 11:20:13 2023, max compression
```

## Comparing `statefun-tasks-0.9.92.tar` & `statefun-tasks-0.9.93.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.923625 statefun-tasks-0.9.92/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/LICENSE
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-13 15:26:02.919625 statefun-tasks-0.9.92/PKG-INFO
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      869 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/README.md
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-04-13 15:26:02.923625 statefun-tasks-0.9.92/setup.cfg
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-04-13 15:25:59.000000 statefun-tasks-0.9.92/setup.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.779627 statefun-tasks-0.9.92/statefun_tasks/
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      934 2023-04-13 15:25:59.000000 statefun-tasks-0.9.92/statefun_tasks/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/builtin.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/builtin_tasks.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.807626 statefun-tasks-0.9.92/statefun_tasks/client/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/client/__init__.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/client/tasks_client.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/client/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/context.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.819626 statefun-tasks-0.9.92/statefun_tasks/effects/
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/effects/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/effects/effect.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/effects/pause_pipeline_effect.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.831626 statefun-tasks-0.9.92/statefun_tasks/events/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/events/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/events/event_handlers.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.839626 statefun-tasks-0.9.92/statefun_tasks/extensions/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/extensions/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.847626 statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     5596 2023-04-13 15:25:59.000000 statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   115734 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/messages_pb2.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.851626 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.871626 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     6799 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.891626 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-03-03 19:15:45.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_emitter.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/task_submitter.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/protobuf.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/serialisation.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    16385 2023-04-10 12:06:04.000000 statefun-tasks-0.9.92/statefun_tasks/task_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.895626 statefun-tasks-0.9.92/statefun_tasks/task_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.919625 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/message_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_action_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     4382 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_request_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_response_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7655 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/tasks.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/type_helpers.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11331 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/utils.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.799626 statefun-tasks-0.9.92/statefun_tasks.egg-info/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/PKG-INFO
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     2111 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/requires.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/top_level.txt
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.612605 statefun-tasks-0.9.93/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/LICENSE
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-05-12 11:20:13.612605 statefun-tasks-0.9.93/PKG-INFO
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      869 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/README.md
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-05-12 11:20:13.612605 statefun-tasks-0.9.93/setup.cfg
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-05-12 11:20:04.000000 statefun-tasks-0.9.93/setup.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.468606 statefun-tasks-0.9.93/statefun_tasks/
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      934 2023-04-30 22:00:09.000000 statefun-tasks-0.9.93/statefun_tasks/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/builtin.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/builtin_tasks.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.504606 statefun-tasks-0.9.93/statefun_tasks/client/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/client/__init__.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/client/tasks_client.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/client/types.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/context.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.520605 statefun-tasks-0.9.93/statefun_tasks/effects/
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/effects/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/effects/effect.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/effects/pause_pipeline_effect.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.532605 statefun-tasks-0.9.93/statefun_tasks/events/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/events/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/events/event_handlers.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.536605 statefun-tasks-0.9.93/statefun_tasks/extensions/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/extensions/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.540605 statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     5596 2023-04-13 15:25:59.000000 statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   115734 2023-04-30 22:00:09.000000 statefun-tasks-0.9.93/statefun_tasks/messages_pb2.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_builder.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.544605 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.568605 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     6799 2023-04-30 23:05:05.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.588605 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-05-12 10:53:19.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/result_emitter.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/task_submitter.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/protobuf.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/serialisation.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    16690 2023-05-12 11:20:04.000000 statefun-tasks-0.9.93/statefun_tasks/task_builder.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.592605 statefun-tasks-0.9.93/statefun_tasks/task_impl/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.608605 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/message_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_action_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     4724 2023-05-12 11:20:04.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_request_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_response_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7655 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/tasks.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/type_helpers.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    11331 2023-04-30 23:05:05.000000 statefun-tasks-0.9.93/statefun_tasks/types.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/utils.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.492606 statefun-tasks-0.9.93/statefun_tasks.egg-info/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     2111 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/requires.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/top_level.txt
```

### Comparing `statefun-tasks-0.9.92/LICENSE` & `statefun-tasks-0.9.93/LICENSE`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/PKG-INFO` & `statefun-tasks-0.9.93/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.92
+Version: 0.9.93
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `statefun-tasks-0.9.92/README.md` & `statefun-tasks-0.9.93/README.md`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/setup.py` & `statefun-tasks-0.9.93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [
     'apache-flink-statefun>=3.2.0',
     'kafka-python'
 ]
 
 setuptools.setup(
     name="statefun-tasks",
-    version="0.9.92",
+    version="0.9.93",
     author="Frans King & Luke Ashworth",
     author_email="frans.king@sbbsystems.com",
     description="Tasks API for Stateful Functions on Flink",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://fransking.github.io/flink-statefun-tasks",
     packages=['statefun_tasks'] + [f'statefun_tasks.{package}' for package in setuptools.find_packages('statefun_tasks')],
```

### Comparing `statefun-tasks-0.9.92/statefun_tasks/__init__.py` & `statefun-tasks-0.9.93/statefun_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/builtin.py` & `statefun-tasks-0.9.93/statefun_tasks/builtin.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/builtin_tasks.py` & `statefun-tasks-0.9.93/statefun_tasks/builtin_tasks.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/client/tasks_client.py` & `statefun-tasks-0.9.93/statefun_tasks/client/tasks_client.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/client/types.py` & `statefun-tasks-0.9.93/statefun_tasks/client/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/context.py` & `statefun-tasks-0.9.93/statefun_tasks/context.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/events/event_handlers.py` & `statefun-tasks-0.9.93/statefun_tasks/events/event_handlers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py` & `statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/messages_pb2.py` & `statefun-tasks-0.9.93/statefun_tasks/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_builder.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_builder.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_aggregator.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/result_aggregator.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_emitter.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/result_emitter.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/task_submitter.py` & `statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/task_submitter.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/protobuf.py` & `statefun-tasks-0.9.93/statefun_tasks/protobuf.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/serialisation.py` & `statefun-tasks-0.9.93/statefun_tasks/serialisation.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/task_builder.py` & `statefun-tasks-0.9.93/statefun_tasks/task_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,24 @@
 
     :param default_namespace: namespace to expose functions under. Maps to Flink Statefun function namespace in module.yaml
     :param default_worker_name: worker name to expose.  Maps to Flink Statefun function type in module.yaml
     :param egress_type_name: egress type name.  Maps to Flink Statefun egress in module.yaml
     :param optional egress_message_max_size: maximum size of an egress message in bytes. If specified attempts to send messages over this size will raise a MessageSizeExceeded exception
     :param optional serialiser: serialiser to use (will use DefaultSerialiser if not set)
     :param optional state_expiration: duration after which state will be expired by Flink (expire_after_call)
+    :param optional keep_task_state: whether to keep state (request, result) associated with tasks as well as pipelines (defaults to false)
     """
-    def __init__(self, default_namespace: str = None, default_worker_name: str = None, egress_type_name: str = None, egress_message_max_size: int = None, serialiser = None, state_expiration: timedelta = None):
+    def __init__(self, 
+                 default_namespace: str = None, 
+                 default_worker_name: str = None, 
+                 egress_type_name: str = None, 
+                 egress_message_max_size: int = None, 
+                 serialiser = None, 
+                 state_expiration: timedelta = None,
+                 keep_task_state = False):
         self._default_namespace = default_namespace
         self._default_worker_name = default_worker_name
         self._egress_type_name = egress_type_name
         self._egress_message_max_size = egress_message_max_size
         self._serialiser = serialiser if serialiser is not None else DefaultSerialiser()
         self._bindings = {}
         self._events = EventHandlers()
@@ -55,15 +63,15 @@
             ValueSpec(name="pipeline_state", type=PIPELINE_STATE_TYPE, expire_after_call=state_expiration)
         ]
 
         self.register_builtin(run_pipeline, with_context=True, with_state=True)
         self.register_builtin(flatten_results)
 
         self._handlers = [
-            TaskRequestHandler(),
+            TaskRequestHandler(keep_task_state),
             TaskResponseHandler(),
             TaskActionHandler(),
             ChildPipelineHandler()
         ]
 
     @staticmethod
     def extend(function, retry_policy: RetryPolicy = None, **params):
```

### Comparing `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/child_pipeline_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/child_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/message_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_action_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_action_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_request_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_request_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from statefun_tasks.type_helpers import _create_task_exception
 from statefun_tasks.messages_pb2 import TaskRequest
 from statefun import Message
 from datetime import timedelta
 
 
 class TaskRequestHandler(MessageHandler):
-    def __init__(self):
+    def __init__(self, keep_task_state=True):
+        self._keep_task_state = keep_task_state
         pass
 
     def unpack(self, context: TaskContext, message: Message):
         if message.is_type(TASK_REQUEST_TYPE):
             task_input = message.as_type(TASK_REQUEST_TYPE)
             
             context.task_name = task_input.type
@@ -62,14 +63,22 @@
             await tasks.emit_result(context, task_request, task_exception)
 
         # else if we have a task result return it
         elif task_result is not None:
             context.storage.task_result = task_result
             await tasks.emit_result(context, task_request, task_result)
 
+        if not self._keep_task_state:
+            # clear state from intermediate tasks
+            if pipeline is None:
+                del context.storage.task_request
+
+            del context.storage.task_result
+            del context.storage.task_exception
+
     async def _attempt_retry(self, context, tasks, task_request, task_exception):
         task_state = context.task_state.by_uid[task_request.uid]
 
         if task_exception.maybe_retry and task_exception.retry_policy is not None:           
             if task_state.retry_count >= task_exception.retry_policy.max_retries:
                 return False
```

### Comparing `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_response_handler.py` & `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_response_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/tasks.py` & `statefun-tasks-0.9.93/statefun_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/type_helpers.py` & `statefun-tasks-0.9.93/statefun_tasks/type_helpers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/types.py` & `statefun-tasks-0.9.93/statefun_tasks/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks/utils.py` & `statefun-tasks-0.9.93/statefun_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.92/statefun_tasks.egg-info/PKG-INFO` & `statefun-tasks-0.9.93/statefun_tasks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.92
+Version: 0.9.93
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `statefun-tasks-0.9.92/statefun_tasks.egg-info/SOURCES.txt` & `statefun-tasks-0.9.93/statefun_tasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


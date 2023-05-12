# Comparing `tmp/mythic_container-0.2.8rc1.tar.gz` & `tmp/mythic_container-0.2.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.2.8rc1.tar", last modified: Wed May 10 16:59:45 2023, max compression
+gzip compressed data, was "mythic_container-0.2.8rc2.tar", last modified: Fri May 12 17:41:01 2023, max compression
```

## Comparing `mythic_container-0.2.8rc1.tar` & `mythic_container-0.2.8rc2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-10 16:59:45.643633 mythic_container-0.2.8rc1/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.8rc1/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-05-10 16:59:45.643299 mythic_container-0.2.8rc1/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.8rc1/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-10 16:59:45.593657 mythic_container-0.2.8rc1/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.8rc1/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.8rc1/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    79130 2023-05-10 16:51:54.000000 mythic_container-0.2.8rc1/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-10 16:59:45.639666 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7581 2023-05-09 13:37:04.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2101 2023-05-08 14:43:34.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.8rc1/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    22456 2023-05-05 22:49:39.000000 mythic_container-0.2.8rc1/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7251 2023-04-19 16:38:54.000000 mythic_container-0.2.8rc1/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-05-08 15:16:26.000000 mythic_container-0.2.8rc1/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2578 2023-05-10 16:59:33.000000 mythic_container-0.2.8rc1/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    37506 2023-05-10 16:58:58.000000 mythic_container-0.2.8rc1/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.8rc1/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.8rc1/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-10 16:59:45.642084 mythic_container-0.2.8rc1/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.8rc1/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.8rc1/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.8rc1/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.8rc1/mythic_container/logging.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.8rc1/mythic_container/logging_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    29520 2023-04-27 21:29:31.000000 mythic_container-0.2.8rc1/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    15080 2023-04-27 21:25:32.000000 mythic_container-0.2.8rc1/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.8rc1/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.8rc1/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-10 16:59:45.595298 mythic_container-0.2.8rc1/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-05-10 16:59:45.000000 mythic_container-0.2.8rc1/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-05-10 16:59:45.000000 mythic_container-0.2.8rc1/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-10 16:59:45.000000 mythic_container-0.2.8rc1/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-05-10 16:59:45.000000 mythic_container-0.2.8rc1/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-05-10 16:59:45.000000 mythic_container-0.2.8rc1/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-10 16:59:45.643792 mythic_container-0.2.8rc1/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1093 2023-05-10 16:59:28.000000 mythic_container-0.2.8rc1/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-12 17:41:01.961800 mythic_container-0.2.8rc2/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.8rc2/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-05-12 17:41:01.961572 mythic_container-0.2.8rc2/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.8rc2/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-12 17:41:01.924980 mythic_container-0.2.8rc2/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.8rc2/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.8rc2/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    79130 2023-05-10 16:51:54.000000 mythic_container-0.2.8rc2/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-12 17:41:01.958961 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7581 2023-05-09 13:37:04.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2101 2023-05-08 14:43:34.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.8rc2/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    22456 2023-05-05 22:49:39.000000 mythic_container-0.2.8rc2/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7773 2023-05-12 17:10:22.000000 mythic_container-0.2.8rc2/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-05-08 15:16:26.000000 mythic_container-0.2.8rc2/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2578 2023-05-12 17:39:51.000000 mythic_container-0.2.8rc2/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    37506 2023-05-10 16:58:58.000000 mythic_container-0.2.8rc2/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.8rc2/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.8rc2/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-12 17:41:01.960588 mythic_container-0.2.8rc2/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.8rc2/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.8rc2/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.8rc2/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.8rc2/mythic_container/logging.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.8rc2/mythic_container/logging_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    29520 2023-04-27 21:29:31.000000 mythic_container-0.2.8rc2/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    15080 2023-04-27 21:25:32.000000 mythic_container-0.2.8rc2/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.8rc2/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.8rc2/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-12 17:41:01.927126 mythic_container-0.2.8rc2/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-05-12 17:41:01.000000 mythic_container-0.2.8rc2/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-05-12 17:41:01.000000 mythic_container-0.2.8rc2/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-12 17:41:01.000000 mythic_container-0.2.8rc2/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-05-12 17:41:01.000000 mythic_container-0.2.8rc2/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-05-12 17:41:01.000000 mythic_container-0.2.8rc2/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-12 17:41:01.961892 mythic_container-0.2.8rc2/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1093 2023-05-12 17:39:32.000000 mythic_container-0.2.8rc2/setup.py
```

### Comparing `mythic_container-0.2.8rc1/LICENSE.md` & `mythic_container-0.2.8rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/PKG-INFO` & `mythic_container-0.2.8rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic_container
-Version: 0.2.8rc1
+Version: 0.2.8rc2
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.8rc1/README.md` & `mythic_container-0.2.8rc2/README.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/C2ProfileBase.py` & `mythic_container-0.2.8rc2/mythic_container/C2ProfileBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/LoggingBase.py` & `mythic_container-0.2.8rc2/mythic_container/LoggingBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicCommandBase.py` & `mythic_container-0.2.8rc2/mythic_container/MythicCommandBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.2.8rc2/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/MythicRPC.py` & `mythic_container-0.2.8rc2/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/PayloadBuilder.py` & `mythic_container-0.2.8rc2/mythic_container/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/TranslationBase.py` & `mythic_container-0.2.8rc2/mythic_container/TranslationBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,75 +97,81 @@
             await asyncio.gather(genKeys, customToMythic, mythicToCustom)
         except Exception as e:
             logger.exception(f"Translation gRPC services closed for {tr_name}: {e}")
 
 
 async def handleGenerateKeys(tr_name: str, client):
     try:
-        stream = client.GenerateEncryptionKeys()
-        await stream.write(TrGenerateEncryptionKeysMessageResponse(
-            Success=True,
-            TranslationContainerName=tr_name
-        ))
-        logger.debug(f"Connected to gRPC for generating encryption keys for {tr_name}")
-        async for request in stream.__aiter__():
-            try:
-                result = await translationServices[tr_name].generate_keys(request)
-                result.TranslationContainerName = tr_name
-                await stream.write(result)
-            except Exception as d:
-                logger.exception(f"Failed to process message:\n{d}")
-                await stream.write(TrGenerateEncryptionKeysMessageResponse(
-                    Success=False,
-                    TranslationContainerName=tr_name,
-                    Error=f"Failed to process message:\n{d}"
-                ))
+        while True:
+            stream = client.GenerateEncryptionKeys()
+            await stream.write(TrGenerateEncryptionKeysMessageResponse(
+                Success=True,
+                TranslationContainerName=tr_name
+            ))
+            logger.info(f"Connected to gRPC for generating encryption keys for {tr_name}")
+            async for request in stream:
+                try:
+                    result = await translationServices[tr_name].generate_keys(request)
+                    result.TranslationContainerName = tr_name
+                    await stream.write(result)
+                except Exception as d:
+                    logger.exception(f"Failed to process message:\n{d}")
+                    await stream.write(TrGenerateEncryptionKeysMessageResponse(
+                        Success=False,
+                        TranslationContainerName=tr_name,
+                        Error=f"Failed to process message:\n{d}"
+                    ))
+            logger.error(f"disconnected from gRPC for generating encryption keys for {tr_name}")
     except Exception as e:
         logger.exception(f"[-] exception in handleGenerateKeys for {tr_name}")
 
 
 async def handleCustomToMythic(tr_name: str, client):
     try:
-        stream = client.TranslateFromCustomToMythicFormat()
-        await stream.write(TrCustomMessageToMythicC2FormatMessageResponse(
-            Success=True,
-            TranslationContainerName=tr_name
-        ))
-        logger.debug(f"Connected to gRPC for handling CustomC2 to MythicC2 Translations for {tr_name}")
-        async for request in stream.__aiter__():
-            try:
-                result = await translationServices[tr_name].translate_from_c2_format(request)
-                result.TranslationContainerName = tr_name
-                await stream.write(result)
-            except Exception as d:
-                logger.exception(f"Failed to process message:\n{d}")
-                await stream.write(TrCustomMessageToMythicC2FormatMessageResponse(
-                    Success=False,
-                    TranslationContainerName=tr_name,
-                    Error=f"Failed to process message:\n{d}"
-                ))
+        while True:
+            stream = client.TranslateFromCustomToMythicFormat()
+            await stream.write(TrCustomMessageToMythicC2FormatMessageResponse(
+                Success=True,
+                TranslationContainerName=tr_name
+            ))
+            logger.info(f"Connected to gRPC for handling CustomC2 to MythicC2 Translations for {tr_name}")
+            async for request in stream:
+                try:
+                    result = await translationServices[tr_name].translate_from_c2_format(request)
+                    result.TranslationContainerName = tr_name
+                    await stream.write(result)
+                except Exception as d:
+                    logger.exception(f"Failed to process message:\n{d}")
+                    await stream.write(TrCustomMessageToMythicC2FormatMessageResponse(
+                        Success=False,
+                        TranslationContainerName=tr_name,
+                        Error=f"Failed to process message:\n{d}"
+                    ))
+            logger.error(f"disconnected from gRPC for doing custom->mythic c2 for {tr_name}")
     except Exception as e:
         logger.exception(f"[-] exception in handleCustomToMythic for {tr_name}")
 
 
 async def handleMythicToCustom(tr_name: str, client):
     try:
-        stream = client.TranslateFromMythicToCustomFormat()
-        await stream.write(TrMythicC2ToCustomMessageFormatMessageResponse(
-            Success=True,
-            TranslationContainerName=tr_name
-        ))
-        logger.debug(f"Connected to gRPC for handling MythicC2 to CustomC2 Translations for {tr_name}")
-        async for request in stream.__aiter__():
-            try:
-                result = await translationServices[tr_name].translate_to_c2_format(request)
-                result.TranslationContainerName = tr_name
-                await stream.write(result)
-            except Exception as d:
-                logger.exception(f"Failed to process message:\n{d}")
-                await stream.write(TrMythicC2ToCustomMessageFormatMessageResponse(
-                    Success=False,
-                    TranslationContainerName=tr_name,
-                    Error=f"Failed to process message:\n{d}"
-                ))
+        while True:
+            stream = client.TranslateFromMythicToCustomFormat()
+            await stream.write(TrMythicC2ToCustomMessageFormatMessageResponse(
+                Success=True,
+                TranslationContainerName=tr_name
+            ))
+            logger.info(f"Connected to gRPC for handling MythicC2 to CustomC2 Translations for {tr_name}")
+            async for request in stream:
+                try:
+                    result = await translationServices[tr_name].translate_to_c2_format(request)
+                    result.TranslationContainerName = tr_name
+                    await stream.write(result)
+                except Exception as d:
+                    logger.exception(f"Failed to process message:\n{d}")
+                    await stream.write(TrMythicC2ToCustomMessageFormatMessageResponse(
+                        Success=False,
+                        TranslationContainerName=tr_name,
+                        Error=f"Failed to process message:\n{d}"
+                    ))
+            logger.error(f"disconnected from gRPC for doing mythic->custom c2 for {tr_name}")
     except Exception as e:
         logger.exception(f"[-] exception in handleMythicToCustom for {tr_name}")
```

### Comparing `mythic_container-0.2.8rc1/mythic_container/WebhookBase.py` & `mythic_container-0.2.8rc2/mythic_container/WebhookBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/__init__.py` & `mythic_container-0.2.8rc2/mythic_container/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
-containerVersion = "v1.0.4"
+containerVersion = "v1.0.6"
 
-PyPi_version = "0.2.8-rc01"
+PyPi_version = "0.2.8-rc02"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
```

### Comparing `mythic_container-0.2.8rc1/mythic_container/agent_utils.py` & `mythic_container-0.2.8rc2/mythic_container/agent_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/c2_utils.py` & `mythic_container-0.2.8rc2/mythic_container/c2_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.2.8rc2/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.2.8rc2/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/logging.py` & `mythic_container-0.2.8rc2/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/logging_utils.py` & `mythic_container-0.2.8rc2/mythic_container/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/mythic_service.py` & `mythic_container-0.2.8rc2/mythic_container/mythic_service.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/rabbitmq.py` & `mythic_container-0.2.8rc2/mythic_container/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.2.8rc2/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container/webhook_utils.py` & `mythic_container-0.2.8rc2/mythic_container/webhook_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.2.8rc2/mythic_container.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic-container
-Version: 0.2.8rc1
+Version: 0.2.8rc2
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.8rc1/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.2.8rc2/mythic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc1/setup.py` & `mythic_container-0.2.8rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.2.8-rc01",
+    version="0.2.8-rc02",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```


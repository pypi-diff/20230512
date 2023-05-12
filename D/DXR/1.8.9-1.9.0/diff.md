# Comparing `tmp/DXR-1.8.9.tar.gz` & `tmp/DXR-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.8.9.tar", last modified: Tue May  9 06:06:15 2023, max compression
+gzip compressed data, was "DXR-1.9.0.tar", last modified: Fri May 12 06:22:06 2023, max compression
```

## Comparing `DXR-1.8.9.tar` & `DXR-1.9.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.646453 DXR-1.8.9/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.575241 DXR-1.8.9/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-09 06:06:15.000000 DXR-1.8.9/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1491 2023-05-09 06:06:15.000000 DXR-1.8.9/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-09 06:06:15.000000 DXR-1.8.9/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-09 06:06:15.000000 DXR-1.8.9/DXR.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-09 06:06:15.000000 DXR-1.8.9/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      132 2023-05-09 06:06:15.000000 DXR-1.8.9/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.576656 DXR-1.8.9/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7881 2023-05-08 11:48:13.000000 DXR-1.8.9/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.8.9/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.8.9/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.579523 DXR-1.8.9/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.8.9/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.586136 DXR-1.8.9/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.8.9/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.8.9/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2859 2023-05-09 02:03:01.000000 DXR-1.8.9/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2427 2023-04-28 02:39:04.000000 DXR-1.8.9/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.8.9/Dxr_file/dxr_requests.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.8.9/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.597723 DXR-1.8.9/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.8.9/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.8.9/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.8.9/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.8.9/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.8.9/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.8.9/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.8.9/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.8.9/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.602765 DXR-1.8.9/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.8.9/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-05-08 05:52:49.000000 DXR-1.8.9/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.8.9/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.8.9/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.8.9/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.604158 DXR-1.8.9/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.611718 DXR-1.8.9/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14345 2023-05-09 06:05:39.000000 DXR-1.8.9/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.8.9/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.614548 DXR-1.8.9/Dxr_redis/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:36:17.000000 DXR-1.8.9/Dxr_redis/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4615 2023-05-09 04:48:00.000000 DXR-1.8.9/Dxr_redis/redis_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.616263 DXR-1.8.9/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.8.9/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.620260 DXR-1.8.9/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.633608 DXR-1.8.9/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.635522 DXR-1.8.9/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.8.9/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.8.9/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.637224 DXR-1.8.9/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.8.9/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.9/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-09 06:06:15.645765 DXR-1.8.9/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.8.9/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 06:06:15.640877 DXR-1.8.9/dxr_cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-08 16:46:33.000000 DXR-1.8.9/dxr_cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.8.9/dxr_cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10414 2023-05-09 05:43:46.000000 DXR-1.8.9/dxr_cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-08 23:51:46.000000 DXR-1.8.9/dxr_cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.8.9/dxr_cli/utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-09 06:06:15.646672 DXR-1.8.9/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      688 2023-05-09 06:06:10.000000 DXR-1.8.9/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.726888 DXR-1.9.0/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.610026 DXR-1.9.0/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-12 06:22:06.000000 DXR-1.9.0/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1515 2023-05-12 06:22:06.000000 DXR-1.9.0/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-12 06:22:06.000000 DXR-1.9.0/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-12 06:22:06.000000 DXR-1.9.0/DXR.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-12 06:22:06.000000 DXR-1.9.0/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      132 2023-05-12 06:22:06.000000 DXR-1.9.0/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.614152 DXR-1.9.0/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7881 2023-05-08 11:48:13.000000 DXR-1.9.0/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.9.0/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.9.0/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.623826 DXR-1.9.0/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.9.0/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.633699 DXR-1.9.0/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.9.0/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.9.0/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2859 2023-05-09 02:03:01.000000 DXR-1.9.0/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3158 2023-05-12 06:09:12.000000 DXR-1.9.0/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.9.0/Dxr_file/dxr_requests.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.9.0/Dxr_file/dxr_ssh.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8416 2023-05-12 06:05:39.000000 DXR-1.9.0/Dxr_file/http_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.647806 DXR-1.9.0/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.9.0/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.9.0/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.9.0/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.9.0/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.9.0/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.9.0/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.9.0/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.9.0/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.659803 DXR-1.9.0/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.9.0/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-05-08 05:52:49.000000 DXR-1.9.0/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.9.0/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.9.0/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.9.0/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.663174 DXR-1.9.0/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.670582 DXR-1.9.0/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14345 2023-05-09 06:05:39.000000 DXR-1.9.0/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.9.0/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.681236 DXR-1.9.0/Dxr_redis/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:36:17.000000 DXR-1.9.0/Dxr_redis/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3946 2023-05-10 01:49:51.000000 DXR-1.9.0/Dxr_redis/redis_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.685455 DXR-1.9.0/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.9.0/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.691420 DXR-1.9.0/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.709699 DXR-1.9.0/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.711909 DXR-1.9.0/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.9.0/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.9.0/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.713981 DXR-1.9.0/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.9.0/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.9.0/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-12 06:22:06.725893 DXR-1.9.0/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.9.0/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-12 06:22:06.724389 DXR-1.9.0/dxr_cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-08 16:46:33.000000 DXR-1.9.0/dxr_cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.9.0/dxr_cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10414 2023-05-12 03:03:26.000000 DXR-1.9.0/dxr_cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-08 23:51:46.000000 DXR-1.9.0/dxr_cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.9.0/dxr_cli/utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-12 06:22:06.727139 DXR-1.9.0/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      688 2023-05-12 06:21:57.000000 DXR-1.9.0/setup.py
```

### Comparing `DXR-1.8.9/DXR.egg-info/SOURCES.txt` & `DXR-1.9.0/DXR.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Dxr_bytes/__init__.py
 Dxr_file/__init__.py
 Dxr_file/dxr_file.py
 Dxr_file/dxr_request.py
 Dxr_file/dxr_request_ros.py
 Dxr_file/dxr_requests.py
 Dxr_file/dxr_ssh.py
+Dxr_file/http_server.py
 Dxr_grpc/Datas_pb2.py
 Dxr_grpc/Datas_pb2_grpc.py
 Dxr_grpc/audios_pb2.py
 Dxr_grpc/audios_pb2_grpc.py
 Dxr_grpc/dxr_grpc_audio_client.py
 Dxr_grpc/dxr_grpc_audio_server.py
 Dxr_grpc/dxr_grpc_client.py
```

### Comparing `DXR-1.8.9/Dxr_Chat/ChatGPT.py` & `DXR-1.9.0/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_Chat/utils.py` & `DXR-1.9.0/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_bytes/Dxr_bytes.py` & `DXR-1.9.0/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_file/dxr_file.py` & `DXR-1.9.0/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_file/dxr_request.py` & `DXR-1.9.0/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_file/dxr_request_ros.py` & `DXR-1.9.0/Dxr_file/dxr_request_ros.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,22 +45,42 @@
                         callback(round(process * 100, 2), file_name)
                     count = 0
         # threading.Thread(target=callback, args=(100, file_name)).start()
         callback(100, file_name)
                     
     print('下载完成')
     return True
+
+def ssh_upload_file(local_path, remote_path, ip=None, user_name=None, password=None, port=22, callback=None):
+    # 使用requests上传文件,并调用callback函数,持续返回进度
+    url = f'http://{ip}:{port}/upload_single_file'
+    print(url)
+    # 获取文件的大小
+    file_size = os.path.getsize(local_path)
+    # 获取文件的名字
+    file_name = os.path.basename(local_path)
+    # 上传文件
+    with open(local_path, 'rb') as f:
+        response = requests.post(url, files={'file': (file_name, f)})
+        response.raise_for_status()
+    
+    print('上传完成')
+    return True
     
 def callback(process, filename):
     # 使用锁来确保线程安全
     with threading.Lock():
         print(process, filename)
     
     
 if __name__ == '__main__':
     remote_path = '/root/nav_ws/src/lidar_localization/Localization/data/latest/finalCloud.pcd'
     local_path = './'
     ip = '10.10.9.254'
     user_name = 'root'
     password = '0'
     port = 5000
-    res = ssh_download_file(remote_path, local_path, ip, user_name, password, port, callback)
+    # res = ssh_download_file(remote_path, local_path, ip, user_name, password, port, callback)
+    # print(res)
+    
+    res = ssh_upload_file("./test.pcd", remote_path, ip, user_name, password, port)
+    print(res)
```

### Comparing `DXR-1.8.9/Dxr_file/dxr_requests.py` & `DXR-1.9.0/Dxr_file/dxr_requests.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_file/dxr_ssh.py` & `DXR-1.9.0/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/Datas_pb2.py` & `DXR-1.9.0/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.9.0/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/audios_pb2.py` & `DXR-1.9.0/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.9.0/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.9.0/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.9.0/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.9.0/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.9.0/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_isapi/api.py` & `DXR-1.9.0/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_isapi/error.py` & `DXR-1.9.0/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_isapi/ir_client.py` & `DXR-1.9.0/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_log/log.py` & `DXR-1.9.0/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.9.0/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.9.0/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_mqtt/msg.py` & `DXR-1.9.0/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_redis/redis_client.py` & `DXR-1.9.0/Dxr_redis/redis_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,96 @@
-# redis连接池
-import redis, traceback, sys, time
-from loguru import logger
+import redis
+import sys
+import traceback
+import time
 import numpy as np
 import cv2
-import time
-
+from loguru import logger
 
 class RedisClient:
-    __instance = None
+    _instance = None
 
     def __new__(cls, *args, **kwargs):
-        # 单例模式
-        return cls.__instance or object.__new__(cls)
+        # Singleton pattern
+        if cls._instance is None:
+            cls._instance = object.__new__(cls)
+        return cls._instance
 
     def __init__(self, host, port, password=None):
         self.host = host
         self.port = port
         self.redis_conn = None
         try:
-            # 拿到一个Redis实例的连接池，避免每次建立、释放连接的开销，节省了每次连接用的时间
-            self.POLL = redis.ConnectionPool(host=self.host,
+            self.pool = redis.ConnectionPool(host=self.host,
                                              port=self.port,
                                              decode_responses=True,
                                              db=0,
                                              password=password,
                                              max_connections=100)
             logger.info(f'获取Redis连接池, Host={self.host}, Port={self.port}')
         except Exception as e:
-            logger.error(f'获取Redis连接池异常, 程序退出:{str(e)},traceback={traceback.format_exc()}')
+            logger.error("获取Redis连接池异常, 程序退出:{}Tracelog={}".format(str(e), traceback.format_exc()))
             sys.exit(0)
 
     def get_redis_client(self):
         try:
-            if self.redis_conn is not None:
-                # 从连接池中获取一个连接实例
-                self.redis_conn = redis.StrictRedis(connection_pool=self.POLL)
+            if self.redis_conn is None or not self.redis_conn.ping():
+                self.redis_conn = redis.StrictRedis(connection_pool=self.pool)
+
                 if self.redis_conn.ping():
                     logger.success(f'获取Redis连接成功, Host={self.host}, Port={self.port}')
-                # 清空所有的key
                 self.redis_conn.flushall()
-            return self.redis_conn
         except Exception as e:
-            logger.error(f'Redis连接*异常*:{str(e)},traceback={traceback.format_exc()}')
-            # 退出程序
-    
-            
+            logger.error("Redis连接*异常*:{}, Tracelog={}".format(str(e), traceback.format_exc()))
+
     def get_redis_data(self, key):
-        redis_conn = self.get_redis_client()
-        if redis_conn is None:
-            return None
-        res = redis_conn.get(key)
-        redis_out = {'Frame': None, 'bFlag': False, 'error': False, 'iTargetNum': 0, 'rect': [], 'sValue': ''}
-        if isinstance(res, str):
-            redis_data = eval(res)
-            # redis_data.pop('Frame')
-            i_type_list = [] # 算法类型
-            s_type_list = [] # 算法名称
-            if bool(redis_data):
-                if redis_data['Frame'] is not None:
-                    # 将字节数据转为 numpy 数组
-                    nparr = np.frombuffer(redis_data['Frame'], np.uint8)
-                    # 将 numpy 数组转为 cv2 图片格式
-                    redis_out['Frame'] = cv2.imdecode(nparr, cv2.IMREAD_COLOR)
-
-                result=redis_data['Result']
-                for algtyep in result:
-                    i_type_list.append(algtyep)
-                    # print(result[algtyep])
-                    s_type_list.append(result[algtyep].get('sType', ''))
-                    redis_out['bFlag'] = redis_out['bFlag'] or result[algtyep]['bFlag']
-                    redis_out['error'] = redis_out['error'] or result[algtyep]['error']
-                    if bool(result[algtyep]['lResults']):
-                        res_key = result[algtyep]['lResults'].get('res_key', 'rect')
-                        if res_key =='':
-                            res_key = 'rect'
-                        if res_key != '':
-                            redis_out['iTargetNum'] += len(result[algtyep]['lResults'][res_key])
-                        redis_out['rect'] = result[algtyep]['lResults'][res_key]
-                        redis_out['sValue'] = result[algtyep]['lResults'].get('sValue', '')
-                        Value = ''
-                        if isinstance(redis_out['sValue'], list) and len(redis_out['sValue'])>0:  # 如果 self.sValue 是一个列表
-                            Value = redis_out['sValue'][0]  # 将其转换为字符串并去掉第一层列表嵌套
-                            if isinstance(Value, list) and len(Value)>0:  # 如果字符串表示的值是一个列表
-                                Value = Value[0]  # 去掉第二层列表嵌套
-                        # 判断Value 为小数字符串或整数字符串
-                        if Value:
-                            redis_out['iTargetNum'] = Value
+        self.get_redis_client()
+        try:
+            res = self.redis_conn.get(key)
+            redis_out = {'Frame': None, 'bFlag': False, 'error': False, 'iTargetNum': 0, 'iType': '', 'sType': ''}
+            if res is not None:
+                redis_data = eval(res)
+                nparr = np.frombuffer(redis_data['Frame'], np.uint8)
+                redis_out['Frame'] = cv2.imdecode(nparr, cv2.IMREAD_COLOR)
+                result = redis_data.get('Result', {})
+                i_type_list = [str(alg_type) for alg_type in result.keys()]
+                s_type_list = [result[alg_type].get('sType', '') for alg_type in result.keys()]
                 redis_out['iType'] = ','.join(i_type_list)
                 redis_out['sType'] = ','.join(s_type_list)
-        return redis_out
 
+                for algtype in result:
+                    res_data = result[algtype]
+                    redis_out['bFlag'] = redis_out['bFlag'] or res_data['bFlag']
+                    redis_out['error'] = redis_out['error'] or res_data['error']
+                    res_results = res_data.get('lResults', {})
+                    rect = res_results.get('rect', [])
+                    redis_out['iTargetNum'] += len(rect)
+                    s_value = res_results.get('sValue', '')
+                    if s_value:
+                        redis_out['iTargetNum'] = s_value
+            return redis_out
+        except redis.exceptions.ConnectionError:
+            logger.error("Redis连接已断开，重新连接中...")
+            self.get_redis_client()
+            return self.get_redis_data(key)
+        except Exception as e:
+            logger.error("获取Redis数据异常:{}, Tracelog={}".format(str(e), traceback.format_exc()))
+            return None
 
+    def gen_redis_data(self, key):
+        while True:
+            result = self.get_redis_data(key)
+            if result is not None:
+                yield result
+            else:
+                time.sleep(0.1)
 
 if __name__ == '__main__':
-    # 密码
-    redis_client = RedisClient('10.10.9.46', 7777, '123456')
-    redis_out = redis_client.get_redis_data('cam_rtsp_left')
-    print(redis_out)
+    redis_client = RedisClient('10.10.8.43', 7777, '123456')
+    gen_data = redis_client.gen_redis_data('cam_rtsp_left')
+
+    for data in gen_data:
+        if data.get('Frame', None) is not None:
+            print(data['Frame'].shape)
+        else:
+            print('Frame data is None')
+            time.sleep(0.1)
```

### Comparing `DXR-1.8.9/Dxr_serial/Dxr_serial.py` & `DXR-1.9.0/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_utils/dxr_ftp.py` & `DXR-1.9.0/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_utils/dxr_utils.py` & `DXR-1.9.0/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/Datas_pb2.py` & `DXR-1.9.0/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.9.0/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/HCNetSDK.py` & `DXR-1.9.0/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/PlayCtrl.py` & `DXR-1.9.0/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/test_main.py` & `DXR-1.9.0/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/video.py` & `DXR-1.9.0/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/video_hk.py` & `DXR-1.9.0/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_video/video_server.py` & `DXR-1.9.0/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_voice/dxr_tts.py` & `DXR-1.9.0/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/Dxr_yaml/Dxr_yaml.py` & `DXR-1.9.0/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/README.md` & `DXR-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/dxr_cli/ChatGPT.py` & `DXR-1.9.0/dxr_cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/dxr_cli/cli.py` & `DXR-1.9.0/dxr_cli/cli.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/dxr_cli/code_execution.py` & `DXR-1.9.0/dxr_cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/dxr_cli/utils.py` & `DXR-1.9.0/dxr_cli/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.9/setup.py` & `DXR-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.8.9',
+    version='1.9.0',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat', 'Dxr_redis', 'dxr_cli'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```


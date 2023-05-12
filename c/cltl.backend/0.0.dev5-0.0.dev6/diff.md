# Comparing `tmp/cltl.backend-0.0.dev5.tar.gz` & `tmp/cltl.backend-0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltl.backend-0.0.dev5.tar", last modified: Thu Sep  1 11:58:59 2022, max compression
+gzip compressed data, was "cltl.backend-0.0.dev6.tar", last modified: Fri May 12 13:29:10 2023, max compression
```

## Comparing `cltl.backend-0.0.dev5.tar` & `cltl.backend-0.0.dev6.tar`

### file list

```diff
@@ -1,51 +1,63 @@
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.035060 cltl.backend-0.0.dev5/
--rw-r--r--   0 tkb        (501) staff       (20)     1069 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/LICENSE
--rw-r--r--   0 tkb        (501) staff       (20)     2275 2022-09-01 11:58:59.034756 cltl.backend-0.0.dev5/PKG-INFO
--rw-r--r--   0 tkb        (501) staff       (20)     1922 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/README.md
--rw-r--r--   0 tkb        (501) staff       (20)        9 2022-09-01 11:58:43.000000 cltl.backend-0.0.dev5/VERSION
--rw-r--r--   0 tkb        (501) staff       (20)       38 2022-09-01 11:58:59.035149 cltl.backend-0.0.dev5/setup.cfg
--rw-r--r--   0 tkb        (501) staff       (20)     1298 2022-09-01 11:52:29.000000 cltl.backend-0.0.dev5/setup.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.017341 cltl.backend-0.0.dev5/src/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.016476 cltl.backend-0.0.dev5/src/cltl/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.021888 cltl.backend-0.0.dev5/src/cltl/backend/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.026028 cltl.backend-0.0.dev5/src/cltl/backend/api/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     2367 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/backend.py
--rw-r--r--   0 tkb        (501) staff       (20)     9625 2022-07-06 09:25:04.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/camera.py
--rw-r--r--   0 tkb        (501) staff       (20)     1898 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/microphone.py
--rw-r--r--   0 tkb        (501) staff       (20)     1627 2022-09-01 10:05:04.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/serialization.py
--rw-r--r--   0 tkb        (501) staff       (20)     1538 2022-09-01 10:05:19.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/storage.py
--rw-r--r--   0 tkb        (501) staff       (20)      789 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/text_to_speech.py
--rw-r--r--   0 tkb        (501) staff       (20)     1195 2022-08-29 19:41:25.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/util.py
--rw-r--r--   0 tkb        (501) staff       (20)      418 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/container.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.028197 cltl.backend-0.0.dev5/src/cltl/backend/impl/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     7513 2022-08-29 19:43:19.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/cached_storage.py
--rw-r--r--   0 tkb        (501) staff       (20)     1689 2022-07-13 11:24:51.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/image_camera.py
--rw-r--r--   0 tkb        (501) staff       (20)     5894 2022-07-13 10:16:47.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_microphone.py
--rw-r--r--   0 tkb        (501) staff       (20)     2223 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_tts.py
--rw-r--r--   0 tkb        (501) staff       (20)     4932 2022-09-01 10:15:25.000000 cltl.backend-0.0.dev5/src/cltl/backend/server.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.030755 cltl.backend-0.0.dev5/src/cltl/backend/source/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     7937 2022-09-01 10:06:05.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/client_source.py
--rw-r--r--   0 tkb        (501) staff       (20)      328 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/console_source.py
--rw-r--r--   0 tkb        (501) staff       (20)     1987 2022-07-13 10:26:36.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/cv2_source.py
--rw-r--r--   0 tkb        (501) staff       (20)     2849 2022-07-13 09:22:46.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/pyaudio_source.py
--rw-r--r--   0 tkb        (501) staff       (20)        4 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/webrtc_audio.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.032540 cltl.backend-0.0.dev5/src/cltl/backend/spi/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)      830 2022-07-13 10:10:08.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/audio.py
--rw-r--r--   0 tkb        (501) staff       (20)      357 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/image.py
--rw-r--r--   0 tkb        (501) staff       (20)      764 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/text.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.020940 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/
--rw-r--r--   0 tkb        (501) staff       (20)     2275 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/PKG-INFO
--rw-r--r--   0 tkb        (501) staff       (20)     1257 2022-09-01 11:58:59.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/SOURCES.txt
--rw-r--r--   0 tkb        (501) staff       (20)        1 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/dependency_links.txt
--rw-r--r--   0 tkb        (501) staff       (20)       53 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/entry_points.txt
--rw-r--r--   0 tkb        (501) staff       (20)      173 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/requires.txt
--rw-r--r--   0 tkb        (501) staff       (20)       18 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/top_level.txt
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.017464 cltl.backend-0.0.dev5/src/cltl_service/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.034194 cltl.backend-0.0.dev5/src/cltl_service/backend/
--rw-r--r--   0 tkb        (501) staff       (20)    10243 2022-06-13 07:02:14.000000 cltl.backend-0.0.dev5/src/cltl_service/backend/backend.py
--rw-r--r--   0 tkb        (501) staff       (20)      595 2022-04-21 11:28:01.000000 cltl.backend-0.0.dev5/src/cltl_service/backend/schema.py
--rw-r--r--   0 tkb        (501) staff       (20)     3562 2022-09-01 10:08:25.000000 cltl.backend-0.0.dev5/src/cltl_service/backend/storage.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.200360 cltl.backend-0.0.dev6/
+-rw-r--r--   0 tkb        (501) staff       (20)     1069 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/LICENSE
+-rw-r--r--   0 tkb        (501) staff       (20)     2275 2023-05-12 13:29:10.199985 cltl.backend-0.0.dev6/PKG-INFO
+-rw-r--r--   0 tkb        (501) staff       (20)     1922 2022-11-09 08:53:42.000000 cltl.backend-0.0.dev6/README.md
+-rw-r--r--   0 tkb        (501) staff       (20)        9 2023-05-12 13:27:23.000000 cltl.backend-0.0.dev6/VERSION
+-rw-r--r--   0 tkb        (501) staff       (20)       38 2023-05-12 13:29:10.200455 cltl.backend-0.0.dev6/setup.cfg
+-rw-r--r--   0 tkb        (501) staff       (20)     1306 2023-05-12 13:26:33.000000 cltl.backend-0.0.dev6/setup.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.132939 cltl.backend-0.0.dev6/src/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.132049 cltl.backend-0.0.dev6/src/cltl/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.139254 cltl.backend-0.0.dev6/src/cltl/backend/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/__init__.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.143879 cltl.backend-0.0.dev6/src/cltl/backend/api/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)     2367 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/backend.py
+-rw-r--r--   0 tkb        (501) staff       (20)    10710 2023-04-03 08:06:06.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/camera.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1898 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/microphone.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1627 2022-09-01 10:05:04.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/serialization.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1538 2022-09-01 10:05:19.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/storage.py
+-rw-r--r--   0 tkb        (501) staff       (20)      789 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/text_to_speech.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1195 2022-08-29 19:41:25.000000 cltl.backend-0.0.dev6/src/cltl/backend/api/util.py
+-rw-r--r--   0 tkb        (501) staff       (20)      418 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/container.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.146155 cltl.backend-0.0.dev6/src/cltl/backend/impl/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/impl/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)     7659 2022-10-14 14:26:38.000000 cltl.backend-0.0.dev6/src/cltl/backend/impl/cached_storage.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1689 2022-07-13 11:24:51.000000 cltl.backend-0.0.dev6/src/cltl/backend/impl/image_camera.py
+-rw-r--r--   0 tkb        (501) staff       (20)     5894 2022-07-13 10:16:47.000000 cltl.backend-0.0.dev6/src/cltl/backend/impl/sync_microphone.py
+-rw-r--r--   0 tkb        (501) staff       (20)     2223 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/impl/sync_tts.py
+-rw-r--r--   0 tkb        (501) staff       (20)     4972 2023-05-12 13:21:36.000000 cltl.backend-0.0.dev6/src/cltl/backend/server.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.161018 cltl.backend-0.0.dev6/src/cltl/backend/source/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/source/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)     8063 2023-01-19 12:07:25.000000 cltl.backend-0.0.dev6/src/cltl/backend/source/client_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)      328 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/source/console_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1987 2022-07-13 10:26:36.000000 cltl.backend-0.0.dev6/src/cltl/backend/source/cv2_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)     2849 2022-07-13 09:22:46.000000 cltl.backend-0.0.dev6/src/cltl/backend/source/pyaudio_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)        4 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/source/webrtc_audio.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.164321 cltl.backend-0.0.dev6/src/cltl/backend/spi/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/spi/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)      830 2022-07-13 10:10:08.000000 cltl.backend-0.0.dev6/src/cltl/backend/spi/audio.py
+-rw-r--r--   0 tkb        (501) staff       (20)      357 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/spi/image.py
+-rw-r--r--   0 tkb        (501) staff       (20)      764 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl/backend/spi/text.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.138000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/
+-rw-r--r--   0 tkb        (501) staff       (20)     2275 2023-05-12 13:29:10.000000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/PKG-INFO
+-rw-r--r--   0 tkb        (501) staff       (20)     1566 2023-05-12 13:29:10.000000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/SOURCES.txt
+-rw-r--r--   0 tkb        (501) staff       (20)        1 2023-05-12 13:29:10.000000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/dependency_links.txt
+-rw-r--r--   0 tkb        (501) staff       (20)       53 2023-05-12 13:29:10.000000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/entry_points.txt
+-rw-r--r--   0 tkb        (501) staff       (20)      181 2023-05-12 13:29:10.000000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/requires.txt
+-rw-r--r--   0 tkb        (501) staff       (20)       18 2023-05-12 13:29:10.000000 cltl.backend-0.0.dev6/src/cltl.backend.egg-info/top_level.txt
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.133101 cltl.backend-0.0.dev6/src/cltl_service/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.190616 cltl.backend-0.0.dev6/src/cltl_service/backend/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/src/cltl_service/backend/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)    10462 2022-10-28 10:54:31.000000 cltl.backend-0.0.dev6/src/cltl_service/backend/backend.py
+-rw-r--r--   0 tkb        (501) staff       (20)      595 2022-04-21 11:28:01.000000 cltl.backend-0.0.dev6/src/cltl_service/backend/schema.py
+-rw-r--r--   0 tkb        (501) staff       (20)     3562 2022-09-01 10:08:25.000000 cltl.backend-0.0.dev6/src/cltl_service/backend/storage.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2023-05-12 13:29:10.199096 cltl.backend-0.0.dev6/tests/
+-rw-r--r--   0 tkb        (501) staff       (20)     3883 2022-04-21 11:39:47.000000 cltl.backend-0.0.dev6/tests/test_backend.py
+-rw-r--r--   0 tkb        (501) staff       (20)     9914 2022-04-21 11:36:51.000000 cltl.backend-0.0.dev6/tests/test_cached_storage.py
+-rw-r--r--   0 tkb        (501) staff       (20)     4544 2022-07-13 11:26:26.000000 cltl.backend-0.0.dev6/tests/test_image_camera.py
+-rw-r--r--   0 tkb        (501) staff       (20)     4811 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/tests/test_integration_mic_tts.py
+-rw-r--r--   0 tkb        (501) staff       (20)      740 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/tests/test_service_util.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1370 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/tests/test_storage.py
+-rw-r--r--   0 tkb        (501) staff       (20)     6172 2022-04-21 11:36:19.000000 cltl.backend-0.0.dev6/tests/test_storage_client.py
+-rw-r--r--   0 tkb        (501) staff       (20)     5769 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/tests/test_sync_microphone.py
+-rw-r--r--   0 tkb        (501) staff       (20)     3818 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev6/tests/test_sync_tts.py
```

### Comparing `cltl.backend-0.0.dev5/LICENSE` & `cltl.backend-0.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/PKG-INFO` & `cltl.backend-0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltl.backend
-Version: 0.0.dev5
+Version: 0.0.dev6
 Summary: Backend for Leolani
 Home-page: https://github.com/leolani/cltl-backend
 Author: CLTL
 Author-email: t.baier@vu.nl
 License: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cltl.backend-0.0.dev5/README.md` & `cltl.backend-0.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/setup.py` & `cltl.backend-0.0.dev6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,20 +28,20 @@
             "parameterized"
         ],
         "host": [
             "emissor",
             "cachetools",
             "pyaudio",
             "opencv-python",
-            "flask"
+            "flask<2.0"
         ],
         "service": [
             "cltl.combot",
             "emissor",
-            "flask",
+            "flask<2.0",
             "pyaudio",
             "requests",
             "sounddevice",
             "soundfile",
         ]
     },
     entry_points={
```

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/backend.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/backend.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/camera.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,25 @@
     def bounds(self):
         return Bounds(0, self.width, 0, self.height)
 
 
 @dataclass
 class Bounds:
     """
-    Rectangle Bounds Object.
+    Coordinate Bounds.
     """
     x0: float
     x1: float
     y0: float
     y1: float
 
+    @classmethod
+    def from_diagonal(cls, x0, y0, x1, y1):
+        return cls(x0, x1, y0, y1)
+
     @property
     def width(self) -> float:
         """
         Bounds Width
 
         Returns
         -------
@@ -203,23 +207,61 @@
         -------
         bounds: List[float]
         """
         return (self.x0, self.y0, self.x1, self.y1)
 
 
 @dataclass
+class View:
+    """3d view of the image"""
+    resolution: Tuple[int, int]
+    view: Bounds
+    depth: np.ndarray
+
+    @classmethod
+    def from_image(cls, image: Image):
+        return View(image.resolution.value, image.view, image.depth)
+
+    def angular_from_pixel(self, pixel_bounds: Bounds) -> Bounds:
+        pass
+
+    def pixel_from_angular(self, pixel_bounds: Bounds) -> Bounds:
+        pass
+
+    def position_from_pixel(self, pixel_bounds: Bounds) -> Bounds:
+        pass
+
+    def pixel_from_position(self, pixel_bounds: Bounds) -> Bounds:
+        pass
+
+    def angle(self, x: float, y: float) -> Tuple[float, float]:
+        pass
+
+    def pixel(self, azimuth: float, polar: float) -> Tuple[float, float]:
+        pass
+
+    @staticmethod
+    def to_cartesian(self, radius: float, azimuth: float, polar: float) -> Tuple[float, float, float]:
+        pass
+
+    @staticmethod
+    def to_spherical(self, x: float, y: float, z: float) -> Tuple[float, float, float]:
+        pass
+
+
+@dataclass
 class Image:
     """
     Abstract Image Container
 
     Parameters
     ----------
     image: np.ndarray
         RGB Image (height, width, 3) as Numpy Array
-    bounds: Bounds
+    view: Bounds
         Image Bounds (View Space) in Spherical Coordinates (Phi, Theta)
     depth: np.ndarray
         Image Depth (height, width) as Numpy Array
     """
     image: np.ndarray
     view: Tuple[float, float, float, float]
     depth: Optional[np.ndarray] = None
```

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/microphone.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/microphone.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/serialization.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/serialization.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/storage.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/storage.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/text_to_speech.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/api/util.py` & `cltl.backend-0.0.dev6/src/cltl/backend/api/util.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/impl/cached_storage.py` & `cltl.backend-0.0.dev6/src/cltl/backend/impl/cached_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
     def __init__(self, storage_path: str, min_buffer: int = 16):
         self._storage_path = Path(storage_path).resolve()
         self._cache = dict()
         self._cache_params = dict()
         self._min_buffer = min_buffer
 
+        os.makedirs(os.path.dirname(self._storage_path), exist_ok=True)
+
     def store(self, audio_id: str, audio: Union[np.array, Iterable[np.array]], sampling_rate: int):
         if isinstance(audio, np.ndarray):
             audio = [audio]
 
         self._cache[audio_id] = Queue()
 
         for frame in audio:
@@ -153,14 +155,16 @@
 
         return cls(backend_config.get("image_storage_path"), backend_config.get_int("image_cache"))
 
     def __init__(self, storage_path: str, max_buffer: int = 16):
         self._storage_path = Path(storage_path).resolve()
         self._cache = LRUCache(maxsize=max_buffer)
 
+        os.makedirs(os.path.dirname(self._storage_path), exist_ok=True)
+
     def store(self, image_id: str, image: Image):
         if image_id in self._cache:
             logger.warning("Image %s was already stored", image_id)
 
         self._cache[image_id] = image
         self._write(image_id, image)
```

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/impl/image_camera.py` & `cltl.backend-0.0.dev6/src/cltl/backend/impl/image_camera.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_microphone.py` & `cltl.backend-0.0.dev6/src/cltl/backend/impl/sync_microphone.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_tts.py` & `cltl.backend-0.0.dev6/src/cltl/backend/impl/sync_tts.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/server.py` & `cltl.backend-0.0.dev6/src/cltl/backend/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,8 +127,12 @@
                         default=8000, help="Web server port")
     args, _ = parser.parse_known_args()
 
     logger.info("Starting webserver with args: %s", args)
 
     server = BackendServer(args.rate, args.channels, args.frame_duration * args.rate // 1000,
                            CameraResolution[args.resolution.upper()], args.cam_index)
-    server.run(host="0.0.0.0", port=args.port)
+    server.run(host="0.0.0.0", port=args.port)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/source/client_source.py` & `cltl.backend-0.0.dev6/src/cltl/backend/source/client_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import re
+import time
 from types import SimpleNamespace
 from typing import Iterator
 from urllib.parse import urljoin
 
 import requests
 from cltl.combot.infra.config import ConfigurationManager
 from emissor.representation.scenario import Modality
@@ -209,18 +210,21 @@
 
         return CameraResolution[resolution_match.group(1)]
 
     def capture(self) -> Image:
         if not self._session:
             raise ValueError("session not started, call capture inside a context manager!")
 
+        start = time.time()
         with self._session.get(self._url, stream=True) as request:
             if request.status_code != 200:
                 code = request.status_code
                 text = request.text
                 raise ValueError(f"Requests to {self._url} failed ({code}): {text}")
 
             logger.debug("Connected to backend at %s", self._url)
 
             self._image = image_hook(request.json())
 
+        logger.debug("Captured image in %s from %s", time.time() - start, self._url)
+
         return self._image
```

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/source/cv2_source.py` & `cltl.backend-0.0.dev6/src/cltl/backend/source/cv2_source.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/source/pyaudio_source.py` & `cltl.backend-0.0.dev6/src/cltl/backend/source/pyaudio_source.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/spi/audio.py` & `cltl.backend-0.0.dev6/src/cltl/backend/spi/audio.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl/backend/spi/text.py` & `cltl.backend-0.0.dev6/src/cltl/backend/spi/text.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl.backend.egg-info/PKG-INFO` & `cltl.backend-0.0.dev6/src/cltl.backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltl.backend
-Version: 0.0.dev5
+Version: 0.0.dev6
 Summary: Backend for Leolani
 Home-page: https://github.com/leolani/cltl-backend
 Author: CLTL
 Author-email: t.baier@vu.nl
 License: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cltl.backend-0.0.dev5/src/cltl_service/backend/backend.py` & `cltl.backend-0.0.dev6/src/cltl_service/backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,20 @@
                     # ConnectionErrors may occur during start-up
                     logging.warning("Failed to capture to image: %s", e)
                     time.sleep(1)
                 except Exception as e:
                     logger.exception("Failed to capture to image: %s", e)
                     time.sleep(1)
 
-        self._image_thread = Thread(name="cltl.backend.image", target=run)
-        self._image_thread.start()
+        if self._image_topic:
+            self._image_thread = Thread(name="cltl.backend.image", target=run)
+            self._image_thread.start()
+        else:
+            logger.warning("No image topic configure")
+
 
     def _stop_image(self):
         if not self._image_thread:
             return
 
         self._image_thread.join()
         self._image_thread = None
@@ -184,16 +188,19 @@
                     # ConnectionErrors may occur during start-up
                     logging.warning("Failed to listen to mic: %s", e)
                     time.sleep(1)
                 except Exception as e:
                     logger.exception("Failed to listen to mic: %s", e)
                     time.sleep(1)
 
-        self._mic_thread = Thread(name="cltl.backend.mic", target=run)
-        self._mic_thread.start()
+        if self._mic_topic:
+            self._mic_thread = Thread(name="cltl.backend.mic", target=run)
+            self._mic_thread.start()
+        else:
+            logger.warning("No microphone topic configured")
 
     def _stop_mic(self):
         if not self._mic_thread:
             return
 
         self._mic_thread.join()
         self._mic_thread = None
```

### Comparing `cltl.backend-0.0.dev5/src/cltl_service/backend/schema.py` & `cltl.backend-0.0.dev6/src/cltl_service/backend/schema.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev5/src/cltl_service/backend/storage.py` & `cltl.backend-0.0.dev6/src/cltl_service/backend/storage.py`

 * *Files identical despite different names*


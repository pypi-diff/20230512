# Comparing `tmp/cltl.backend-0.0.dev3.tar.gz` & `tmp/cltl.backend-0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltl.backend-0.0.dev3.tar", last modified: Mon Dec 13 16:40:15 2021, max compression
+gzip compressed data, was "cltl.backend-0.0.dev5.tar", last modified: Thu Sep  1 11:58:59 2022, max compression
```

## Comparing `cltl.backend-0.0.dev3.tar` & `cltl.backend-0.0.dev5.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.122703 cltl.backend-0.0.dev3/
--rw-r--r--   0 tkb        (501) staff       (20)     1069 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/LICENSE
--rw-r--r--   0 tkb        (501) staff       (20)      420 2021-12-13 16:40:15.122408 cltl.backend-0.0.dev3/PKG-INFO
--rw-r--r--   0 tkb        (501) staff       (20)       47 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/README.md
--rw-r--r--   0 tkb        (501) staff       (20)        9 2021-12-13 16:39:48.000000 cltl.backend-0.0.dev3/VERSION
--rw-r--r--   0 tkb        (501) staff       (20)       38 2021-12-13 16:40:15.122799 cltl.backend-0.0.dev3/setup.cfg
--rw-r--r--   0 tkb        (501) staff       (20)     1183 2021-12-02 13:09:13.000000 cltl.backend-0.0.dev3/setup.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.106542 cltl.backend-0.0.dev3/src/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.105672 cltl.backend-0.0.dev3/src/cltl/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.110710 cltl.backend-0.0.dev3/src/cltl/backend/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.114488 cltl.backend-0.0.dev3/src/cltl/backend/api/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     1497 2021-10-22 13:47:52.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/backend.py
--rw-r--r--   0 tkb        (501) staff       (20)     8832 2021-11-04 21:30:57.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/camera.py
--rw-r--r--   0 tkb        (501) staff       (20)     1898 2021-10-24 22:43:20.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/microphone.py
--rw-r--r--   0 tkb        (501) staff       (20)     1540 2021-11-04 12:44:23.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/storage.py
--rw-r--r--   0 tkb        (501) staff       (20)      727 2021-10-22 16:04:20.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/text_to_speech.py
--rw-r--r--   0 tkb        (501) staff       (20)     1194 2021-10-27 11:20:49.000000 cltl.backend-0.0.dev3/src/cltl/backend/api/util.py
--rw-r--r--   0 tkb        (501) staff       (20)      418 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/src/cltl/backend/container.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.116198 cltl.backend-0.0.dev3/src/cltl/backend/impl/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/src/cltl/backend/impl/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     7253 2021-11-05 09:48:56.000000 cltl.backend-0.0.dev3/src/cltl/backend/impl/cached_storage.py
--rw-r--r--   0 tkb        (501) staff       (20)     5519 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl/backend/impl/sync_microphone.py
--rw-r--r--   0 tkb        (501) staff       (20)     1356 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl/backend/impl/sync_tts.py
--rw-r--r--   0 tkb        (501) staff       (20)     2980 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl/backend/server.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.118924 cltl.backend-0.0.dev3/src/cltl/backend/source/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/src/cltl/backend/source/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)     8199 2021-12-13 16:38:32.000000 cltl.backend-0.0.dev3/src/cltl/backend/source/client_source.py
--rw-r--r--   0 tkb        (501) staff       (20)      286 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl/backend/source/console_source.py
--rw-r--r--   0 tkb        (501) staff       (20)     1950 2021-11-04 11:03:26.000000 cltl.backend-0.0.dev3/src/cltl/backend/source/cv2_source.py
--rw-r--r--   0 tkb        (501) staff       (20)     2797 2021-10-22 16:12:29.000000 cltl.backend-0.0.dev3/src/cltl/backend/source/pyaudio_source.py
--rw-r--r--   0 tkb        (501) staff       (20)        4 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/src/cltl/backend/source/webrtc_audio.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.120484 cltl.backend-0.0.dev3/src/cltl/backend/spi/
--rw-r--r--   0 tkb        (501) staff       (20)        0 2021-09-23 06:24:21.000000 cltl.backend-0.0.dev3/src/cltl/backend/spi/__init__.py
--rw-r--r--   0 tkb        (501) staff       (20)      654 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl/backend/spi/audio.py
--rw-r--r--   0 tkb        (501) staff       (20)      357 2021-10-29 09:49:52.000000 cltl.backend-0.0.dev3/src/cltl/backend/spi/image.py
--rw-r--r--   0 tkb        (501) staff       (20)      653 2021-10-29 12:29:09.000000 cltl.backend-0.0.dev3/src/cltl/backend/spi/text.py
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.109886 cltl.backend-0.0.dev3/src/cltl.backend.egg-info/
--rw-r--r--   0 tkb        (501) staff       (20)      420 2021-12-13 16:40:15.000000 cltl.backend-0.0.dev3/src/cltl.backend.egg-info/PKG-INFO
--rw-r--r--   0 tkb        (501) staff       (20)     1138 2021-12-13 16:40:15.000000 cltl.backend-0.0.dev3/src/cltl.backend.egg-info/SOURCES.txt
--rw-r--r--   0 tkb        (501) staff       (20)        1 2021-12-13 16:40:15.000000 cltl.backend-0.0.dev3/src/cltl.backend.egg-info/dependency_links.txt
--rw-r--r--   0 tkb        (501) staff       (20)      165 2021-12-13 16:40:15.000000 cltl.backend-0.0.dev3/src/cltl.backend.egg-info/requires.txt
--rw-r--r--   0 tkb        (501) staff       (20)       18 2021-12-13 16:40:15.000000 cltl.backend-0.0.dev3/src/cltl.backend.egg-info/top_level.txt
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.106637 cltl.backend-0.0.dev3/src/cltl_service/
-drwxr-xr-x   0 tkb        (501) staff       (20)        0 2021-12-13 16:40:15.121900 cltl.backend-0.0.dev3/src/cltl_service/backend/
--rw-r--r--   0 tkb        (501) staff       (20)     3024 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl_service/backend/backend.py
--rw-r--r--   0 tkb        (501) staff       (20)     1198 2021-10-07 19:43:27.000000 cltl.backend-0.0.dev3/src/cltl_service/backend/schema.py
--rw-r--r--   0 tkb        (501) staff       (20)     3767 2021-12-10 09:35:08.000000 cltl.backend-0.0.dev3/src/cltl_service/backend/storage.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.035060 cltl.backend-0.0.dev5/
+-rw-r--r--   0 tkb        (501) staff       (20)     1069 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/LICENSE
+-rw-r--r--   0 tkb        (501) staff       (20)     2275 2022-09-01 11:58:59.034756 cltl.backend-0.0.dev5/PKG-INFO
+-rw-r--r--   0 tkb        (501) staff       (20)     1922 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/README.md
+-rw-r--r--   0 tkb        (501) staff       (20)        9 2022-09-01 11:58:43.000000 cltl.backend-0.0.dev5/VERSION
+-rw-r--r--   0 tkb        (501) staff       (20)       38 2022-09-01 11:58:59.035149 cltl.backend-0.0.dev5/setup.cfg
+-rw-r--r--   0 tkb        (501) staff       (20)     1298 2022-09-01 11:52:29.000000 cltl.backend-0.0.dev5/setup.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.017341 cltl.backend-0.0.dev5/src/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.016476 cltl.backend-0.0.dev5/src/cltl/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.021888 cltl.backend-0.0.dev5/src/cltl/backend/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.026028 cltl.backend-0.0.dev5/src/cltl/backend/api/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)     2367 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/backend.py
+-rw-r--r--   0 tkb        (501) staff       (20)     9625 2022-07-06 09:25:04.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/camera.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1898 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/microphone.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1627 2022-09-01 10:05:04.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/serialization.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1538 2022-09-01 10:05:19.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/storage.py
+-rw-r--r--   0 tkb        (501) staff       (20)      789 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/text_to_speech.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1195 2022-08-29 19:41:25.000000 cltl.backend-0.0.dev5/src/cltl/backend/api/util.py
+-rw-r--r--   0 tkb        (501) staff       (20)      418 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/container.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.028197 cltl.backend-0.0.dev5/src/cltl/backend/impl/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)     7513 2022-08-29 19:43:19.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/cached_storage.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1689 2022-07-13 11:24:51.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/image_camera.py
+-rw-r--r--   0 tkb        (501) staff       (20)     5894 2022-07-13 10:16:47.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_microphone.py
+-rw-r--r--   0 tkb        (501) staff       (20)     2223 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_tts.py
+-rw-r--r--   0 tkb        (501) staff       (20)     4932 2022-09-01 10:15:25.000000 cltl.backend-0.0.dev5/src/cltl/backend/server.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.030755 cltl.backend-0.0.dev5/src/cltl/backend/source/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)     7937 2022-09-01 10:06:05.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/client_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)      328 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/console_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)     1987 2022-07-13 10:26:36.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/cv2_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)     2849 2022-07-13 09:22:46.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/pyaudio_source.py
+-rw-r--r--   0 tkb        (501) staff       (20)        4 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/source/webrtc_audio.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.032540 cltl.backend-0.0.dev5/src/cltl/backend/spi/
+-rw-r--r--   0 tkb        (501) staff       (20)        0 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/__init__.py
+-rw-r--r--   0 tkb        (501) staff       (20)      830 2022-07-13 10:10:08.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/audio.py
+-rw-r--r--   0 tkb        (501) staff       (20)      357 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/image.py
+-rw-r--r--   0 tkb        (501) staff       (20)      764 2022-03-31 11:49:50.000000 cltl.backend-0.0.dev5/src/cltl/backend/spi/text.py
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.020940 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/
+-rw-r--r--   0 tkb        (501) staff       (20)     2275 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/PKG-INFO
+-rw-r--r--   0 tkb        (501) staff       (20)     1257 2022-09-01 11:58:59.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/SOURCES.txt
+-rw-r--r--   0 tkb        (501) staff       (20)        1 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/dependency_links.txt
+-rw-r--r--   0 tkb        (501) staff       (20)       53 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/entry_points.txt
+-rw-r--r--   0 tkb        (501) staff       (20)      173 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/requires.txt
+-rw-r--r--   0 tkb        (501) staff       (20)       18 2022-09-01 11:58:58.000000 cltl.backend-0.0.dev5/src/cltl.backend.egg-info/top_level.txt
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.017464 cltl.backend-0.0.dev5/src/cltl_service/
+drwxr-xr-x   0 tkb        (501) staff       (20)        0 2022-09-01 11:58:59.034194 cltl.backend-0.0.dev5/src/cltl_service/backend/
+-rw-r--r--   0 tkb        (501) staff       (20)    10243 2022-06-13 07:02:14.000000 cltl.backend-0.0.dev5/src/cltl_service/backend/backend.py
+-rw-r--r--   0 tkb        (501) staff       (20)      595 2022-04-21 11:28:01.000000 cltl.backend-0.0.dev5/src/cltl_service/backend/schema.py
+-rw-r--r--   0 tkb        (501) staff       (20)     3562 2022-09-01 10:08:25.000000 cltl.backend-0.0.dev5/src/cltl_service/backend/storage.py
```

### Comparing `cltl.backend-0.0.dev3/LICENSE` & `cltl.backend-0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev3/setup.py` & `cltl.backend-0.0.dev5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,23 +24,27 @@
     extras_require={
         "impl": [
             "mock",
             "requests",
             "parameterized"
         ],
         "host": [
+            "emissor",
             "cachetools",
             "pyaudio",
             "opencv-python",
             "flask"
         ],
         "service": [
             "cltl.combot",
             "emissor",
             "flask",
             "pyaudio",
             "requests",
             "sounddevice",
             "soundfile",
         ]
+    },
+    entry_points={
+        'console_scripts': ['leoserv = cltl.backend.server:main']
     }
 )
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/api/backend.py` & `cltl.backend-0.0.dev5/src/cltl/backend/api/backend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 import logging
 
+from cltl.backend.api.camera import Camera
 from cltl.backend.api.microphone import Microphone
 from cltl.backend.api.text_to_speech import TextToSpeech
 
 logger = logging.getLogger(__name__)
 
 
 class Backend:
     """
-    Abstract Backend on which all Backends are based
+    Central class providing all backend functionality.
 
     Exposes
     :class:`~cltl.backend.api.microphone.Microphone`
+    :class:`~cltl.backend.api.camera.Camera`
+    :class:`~cltl.backend.api.text_to_speech.TextToSpeech`
 
     Parameters
     ----------
     microphone: Microphone
         Backend :class:`~cltl.backend.api.microphone.Microphone`
+    camera: Camera
+        Backend :class:`~cltl.backend.api.camera.Camera`
+    tts: TextToSpeech
+        Backend :class:`~cltl.backend.api.tts.TextToSpeech`
     """
 
-    def __init__(self, microphone: Microphone):
+    def __init__(self, microphone: Microphone, camera: Camera, tts: TextToSpeech):
         self._microphone = microphone
+        self._camera = camera
+        self._tts = tts
 
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
     def start(self):
         if self._microphone:
             self._microphone.start()
+        if self._camera:
+            self._camera.start()
+        if self._tts:
+            self._tts.start()
 
     def stop(self):
-        self._stop_safe(self._microphone)
+        if self._microphone:
+            self._stop_safe(self._microphone)
+        if self._camera:
+            self._stop_safe(self._camera)
+        if self._tts:
+            self._stop_safe(self._tts)
 
     def _stop_safe(self, component):
         if component:
             try:
                 component.stop()
             except:
                 logger.exception("Failed to stop " + str(component))
@@ -51,16 +69,28 @@
         Returns
         -------
         Microphone
         """
         return self._microphone
 
     @property
+    def camera(self) -> Camera:
+        """
+        Reference to :class:`~cltl.backend.api.microphone.Camera`
+
+        Returns
+        -------
+        Camera
+        """
+        return self._camera
+
+
+    @property
     def text_to_speech(self) -> TextToSpeech:
         """
         Reference to :class:`~cltl.backend.api.text_to_speech.TextToSpeech`
 
         Returns
         -------
         TextToSpeech
         """
-        return self._text_to_speech
+        return self._tts
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/api/camera.py` & `cltl.backend-0.0.dev5/src/cltl/backend/api/camera.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,17 +30,21 @@
     def height(self):
         return self.value[0]
 
     @property
     def width(self):
         return self.value[1]
 
+    @property
+    def bounds(self):
+        return Bounds(0, self.width, 0, self.height)
+
 
 @dataclass
-class Bounds(object):
+class Bounds:
     """
     Rectangle Bounds Object.
     """
     x0: float
     x1: float
     y0: float
     y1: float
@@ -103,15 +107,15 @@
         """
 
         x0 = max(self.x0, bounds.x0)
         y0 = max(self.y0, bounds.y0)
         x1 = min(self.x1, bounds.x1)
         y1 = min(self.y1, bounds.y1)
 
-        return None if x0 >= x1 or y0 >= y1 else Bounds(x0, y0, x1, y1)
+        return None if x0 >= x1 or y0 >= y1 else Bounds(x0, x1, y0, y1)
 
     def overlap(self, other: Bounds) -> float:
         """
         Bounds Overlap Ratio
 
         Parameters
         ----------
@@ -185,17 +189,17 @@
         y_scale: float
 
         Returns
         -------
         bounds: Bounds
             Scaled Bounds object
         """
-        return Bounds(self.x0 * x_scale, self.y0 * y_scale, self.x1 * x_scale, self.y1 * y_scale)
+        return Bounds(self.x0 * x_scale, self.x1 * x_scale, self.y0 * y_scale, self.y1 * y_scale)
 
-    def to_tuple(self) -> Tuple[float, float, float, float]:
+    def to_diagonal(self) -> Tuple[float, float, float, float]:
         """
         Export Bounds as List
 
         Returns
         -------
         bounds: List[float]
         """
@@ -213,18 +217,22 @@
         RGB Image (height, width, 3) as Numpy Array
     bounds: Bounds
         Image Bounds (View Space) in Spherical Coordinates (Phi, Theta)
     depth: np.ndarray
         Image Depth (height, width) as Numpy Array
     """
     image: np.ndarray
-    bounds: Bounds
+    view: Tuple[float, float, float, float]
     depth: Optional[np.ndarray] = None
 
     @property
+    def bounds(self) -> Bounds:
+        return self.resolution.bounds
+
+    @property
     def resolution(self) -> CameraResolution:
         try:
             return CameraResolution(self.image.shape[:2])
         except ValueError:
             return CameraResolution.NATIVE
 
     def get_section(self, bounds: Bounds) -> np.ndarray:
@@ -282,16 +290,16 @@
         ----------
         coordinates: Tuple[float, float]
 
         Returns
         -------
         direction: Tuple[float, float]
         """
-        return (self.bounds.x0 + coordinates[0] * self.bounds.width,
-                self.bounds.y0 + coordinates[1] * self.bounds.height)
+        return (self.view.x0 + coordinates[0] * self.view.width,
+                self.view.y0 + coordinates[1] * self.view.height)
 
     def frustum(self, depth_min: float, depth_max: float) -> np.ndarray:
         """
         Calculate `Frustum <https://en.wikipedia.org/wiki/Viewing_frustum>`_ of the camera at image time (visualisation)
 
         Parameters
         ----------
@@ -303,24 +311,24 @@
         Returns
         -------
         frustum: np.ndarray
             Numpy array of shape (2,4,4) containing near view and far view planes in the first dimension.
         """
         return np.array([
             # Near Viewing Plane
-            [spherical2cartesian(self.bounds.x0, self.bounds.y0, depth_min),
-            spherical2cartesian(self.bounds.x0, self.bounds.y1, depth_min),
-            spherical2cartesian(self.bounds.x1, self.bounds.y1, depth_min),
-            spherical2cartesian(self.bounds.x1, self.bounds.y0, depth_min)],
+            [spherical2cartesian(self.view.x0, self.view.y0, depth_min),
+            spherical2cartesian(self.view.x0, self.view.y1, depth_min),
+            spherical2cartesian(self.view.x1, self.view.y1, depth_min),
+            spherical2cartesian(self.view.x1, self.view.y0, depth_min)],
 
             # Far Viewing Plane
-            [spherical2cartesian(self.bounds.x0, self.bounds.y0, depth_max),
-            spherical2cartesian(self.bounds.x0, self.bounds.y1, depth_max),
-            spherical2cartesian(self.bounds.x1, self.bounds.y1, depth_max),
-            spherical2cartesian(self.bounds.x1, self.bounds.y0, depth_max)]
+            [spherical2cartesian(self.view.x0, self.view.y0, depth_max),
+            spherical2cartesian(self.view.x0, self.view.y1, depth_max),
+            spherical2cartesian(self.view.x1, self.view.y1, depth_max),
+            spherical2cartesian(self.view.x1, self.view.y0, depth_max)]
         ])
 
 
 class Camera(abc.ABC):
     def __enter__(self):
         self.start()
         return self
@@ -331,25 +339,45 @@
     def start(self):
         pass
 
     def stop(self):
         pass
 
     @property
-    def rate(self) -> int:
+    def rate(self) -> float:
+        """Rate of the camera recording.
+
+        Returns
+        -------
+        float
+            Images per seconds recorded by the Camera.
+
+            If a negative rate is returned, only capturing images is supported,
+            if a zero is returned, the camera will record at the maximum available rate.
+        """
         raise NotImplementedError()
 
     @property
     def resolution(self) -> CameraResolution:
         raise NotImplementedError()
 
     @contextmanager
+    def capture(self) -> Image:
+        """
+        Retrieve an Image from the camera.
+        """
+        raise NotImplementedError()
+
+    @contextmanager
     def record(self) -> Iterable[Image]:
         """
         Retrieve stream of Images from the camera.
+
+        Images are recorded with the rate returned by `rate`. The rate may be
+        influenced by the speed at which the returned iterable is consumed.
         """
         raise NotImplementedError()
 
     def stop_recording(self):
         """
         Stop adding new images to the image stream.
         """
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/api/microphone.py` & `cltl.backend-0.0.dev5/src/cltl/backend/api/microphone.py`

 * *Files identical despite different names*

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/api/storage.py` & `cltl.backend-0.0.dev5/src/cltl/backend/api/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import abc
-from typing import Iterable, List, Union
+from typing import Iterable, Union
 
 import numpy as np
 
 from cltl.backend.api.camera import Image
 from cltl.backend.api.microphone import AudioParameters
 
 STORAGE_SCHEME = "cltl-storage"
 
 
 # TODO rename id to identifier
 class AudioStorage(abc.ABC):
-    def store(self, id: str, audio: Union[np.ndarray, List[np.ndarray]], sampling_rate: int):
+    def store(self, id: str, audio: Union[np.ndarray, Iterable[np.ndarray]], sampling_rate: int):
         raise NotImplementedError()
 
     def get(self, id: str, offset: int = 0, length: int = -1) -> (Iterable[np.ndarray], AudioParameters):
         """
         Return audio data for the given id, starting from the given offset.
 
         Parameters
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/api/text_to_speech.py` & `cltl.backend-0.0.dev5/src/cltl/backend/api/text_to_speech.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import abc
 import logging
+from typing import Any
+
 
 logger = logging.getLogger(__name__)
 
 
 class TextToSpeech(abc.ABC):
-    def __enter__(self):
+    def __enter__(self) -> Any:
         self.start()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.stop()
 
-    def start(self):
+    def start(self) -> Any:
         raise NotImplementedError()
 
-    def stop(self):
+    def stop(self) -> None:
         raise NotImplementedError()
 
-    def say(self, text: str):
+    def say(self, text: str) -> None:
         raise NotImplementedError()
 
     @property
     def is_talking(self) -> bool:
         raise NotImplementedError()
 
     @property
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/api/util.py` & `cltl.backend-0.0.dev5/src/cltl/backend/api/util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
     x,y,z: float, float, float
 
     """
     x = depth * np.sin(theta) * np.cos(phi)
     y = depth * np.cos(theta)
     z = depth * np.sin(theta) * np.sin(phi)
 
-    return x, y, z
+    return x, y, z
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/impl/cached_storage.py` & `cltl.backend-0.0.dev5/src/cltl/backend/impl/cached_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import logging
 import os.path
 import pickle
-import time
 from pathlib import Path
 from queue import Queue, Empty
 from types import SimpleNamespace
 from typing import Iterable, Union
 
 import cv2
 import numpy as np
 import soundfile as sf
 from cachetools import LRUCache
 from cltl.combot.infra.config import ConfigurationManager
+from cltl.combot.infra.time_util import timestamp_now
 
 from cltl.backend.api.camera import Image, Bounds
 from cltl.backend.api.storage import AudioStorage, AudioParameters, ImageStorage
 
 logger = logging.getLogger(__name__)
 
 
@@ -67,18 +67,20 @@
             data = np.concatenate(audio)
 
         if not data.dtype == np.int16:
             raise ValueError(f"Wrong sample depth: {data.dtype}")
 
         sf.write(str(self._storage_path / f"{id_}.wav"), data, sampling_rate)
 
-        metadata = {"timestamp": time.time(), "parameters": self._cache_params[id_]}
+        metadata = {"timestamp": timestamp_now(), "parameters": self._cache_params[id_]}
         with open(self._storage_path / f"{id_}_meta.json", 'w') as f:
             json.dump(metadata, f, default=vars)
 
+        logger.debug("Stored audio files %s", self._storage_path / f"{id_}")
+
     def get(self, id_: str, offset: int = 0, length: int = -1) -> (Iterable[np.array], AudioParameters):
         try:
             parameters = self._cache_params[id_]
         except KeyError:
             parameters = AudioParameters(**vars(self._read_meta_from_file(id_).parameters))
 
         def audio_generator():
@@ -159,18 +161,19 @@
         if image_id in self._cache:
             logger.warning("Image %s was already stored", image_id)
 
         self._cache[image_id] = image
         self._write(image_id, image)
 
     def _write(self, image_id: str, image: Image):
-        cv2.imwrite(str(self._storage_path / f"{image_id}.png"), image.image)
+        cv2.imwrite(str(self._storage_path / f"{image_id}.png"),
+                    cv2.cvtColor(image.image, cv2.COLOR_RGB2BGR))
 
         with open(self._storage_path / f"{image_id}_meta.json", 'w') as f:
-            json.dump({'bounds': image.bounds}, f, default=vars)
+            json.dump({'bounds': image.bounds.to_diagonal(), 'view': image.view}, f, default=vars)
 
         if image.depth is not None:
             with open(self._storage_path / f"{image_id}_depth.pkl", 'wb') as f:
                 pickle.dump(image.depth, f)
 
     def get(self, image_id: str) -> Image:
         try:
@@ -182,17 +185,18 @@
             return image
 
     def _read(self, image_id: str):
         if not os.path.isfile(self._storage_path / f"{image_id}.png"):
             raise KeyError(f"No image with id {image_id} found in the storage")
 
         image = cv2.imread(str(self._storage_path / f"{image_id}.png"))
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
 
         with open(self._storage_path / f"{image_id}_meta.json", 'r') as f:
-            bounds = Bounds(**json.load(f)['bounds'])
+            view = Bounds(**json.load(f)['view'])
 
         depth = None
         if os.path.isfile(self._storage_path / f"{image_id}_depth.pkl"):
             with open(self._storage_path / f"{image_id}_depth.pkl", 'rb') as f:
                 depth = pickle.load(f)
 
-        return Image(image, bounds, depth)
+        return Image(image, view, depth)
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/impl/sync_microphone.py` & `cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_microphone.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import contextlib
 import logging
-from typing import Iterator
+from typing import Iterator, Iterable
 
 import numpy as np
 from cltl.combot.infra.resource.api import ResourceManager
 from cltl.combot.infra.resource.threaded import ThreadedResourceManager
 from cltl.combot.infra.util import ThreadsafeBoolean
 
 from cltl.backend.api.microphone import Microphone, AUDIO_RESOURCE_NAME, MIC_RESOURCE_NAME, AudioParameters
@@ -43,14 +43,15 @@
         """
         Initiate resources for synchronization.
         """
         self._resource_manager.provide_resource(AUDIO_RESOURCE_NAME)
         self._resource_manager.provide_resource(MIC_RESOURCE_NAME)
         self._audio_lock = self._resource_manager.get_read_lock(AUDIO_RESOURCE_NAME)
         self._mic_lock = self._resource_manager.get_write_lock(MIC_RESOURCE_NAME)
+        self._mic_lock.acquire()
 
     def stop(self):
         """
         Tear down resources for synchronization.
         """
         if self._audio_lock.locked:
             self._audio_lock.release()
@@ -70,15 +71,15 @@
             self._try_mute()
 
     @property
     def muted(self) -> bool:
         return self._mic_lock.locked
 
     @contextlib.contextmanager
-    def listen(self) -> Iterator[np.array]:
+    def listen(self) -> [Iterable[np.ndarray], AudioParameters]:
         """
         Provide audio input from the microphone.
 
         To avoid interference with audio output we use the following strategy:
 
         * Mute the microphone whenever speakers are active
         * Delay speakers until listening stops
@@ -96,16 +97,18 @@
               (speaker is active, mic is waiting to listen again)
             * when the AUDIO Reader-lock is acquired, it releases the MIC Writer-lock
               (speaker ends, listening starts again)
         """
         while self.muted:
             self._try_unmute()
 
-        with self._source as audio:
-            yield self._get_audio(audio), self.parameters
+        with self._source as source:
+            yield self._get_audio(source.audio), self.parameters
+
+        self._try_mute()
 
     def _get_audio(self, audio) -> Iterator[np.array]:
         frame = False
         audio_frames = iter(audio)
         while frame is not None:
             if self._audio_lock.interrupted or self._interrupt.value:
                 self._try_mute()
@@ -121,34 +124,43 @@
         try:
             return next(audio)
         except StopIteration:
             logger.warning("AudioSource stopped iteration without sentinel value")
             return None
 
     def _try_unmute(self):
-        logger.debug("Try to unmute microphone")
+        logger.debug("Try to unmute microphone (lock interrupted: %s, interrupted: %s)", self._audio_lock.interrupted, self._interrupt.value)
         if self._audio_lock.acquire(blocking=True, timeout=self._timeout_interval):
             self._audio_lock.interrupt_writers(False)
             if self._mic_lock.locked:
                 self._mic_lock.release()
+
+            self._interrupt.value = False
+
             logger.info("Microphone unmuted")
+
             return True
 
         self._audio_lock.interrupt_writers()
+
         return False
 
     def _try_mute(self):
-        logger.debug("Try to mute microphone")
+        logger.debug("Try to mute microphone (lock interrupted: %s, interrupted: %s)", self._audio_lock.interrupted, self._interrupt.value)
         if self._mic_lock.acquire(blocking=True, timeout=self._timeout_interval):
             self._mic_lock.interrupt_readers(False)
             if self._audio_lock.locked:
                 self._audio_lock.release()
+            self._interrupt.value = False
+
             logger.info("Microphone muted")
+
             return True
 
         self._mic_lock.interrupt_readers()
+
         return False
 
 
 class SimpleMicrophone(SynchronizedMicrophone):
     def __init__(self, source: AudioSource):
         super().__init__(source, ThreadedResourceManager())
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/impl/sync_tts.py` & `cltl.backend-0.0.dev5/src/cltl/backend/impl/sync_tts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,50 @@
 import logging
 
 from cltl.combot.infra.resource.api import ResourceManager
+from cltl.combot.infra.util import ThreadsafeBoolean
 
 from cltl.backend.api.microphone import AUDIO_RESOURCE_NAME
 from cltl.backend.api.text_to_speech import TextToSpeech
 from cltl.backend.spi.audio import AudioSource
+from cltl.backend.spi.text import TextOutput
 
 logger = logging.getLogger(__name__)
 
 
+class TextOutputTTS(TextToSpeech):
+    def __init__(self, text_output: TextOutput, language: str = None):
+        self._text_output = text_output
+        self._language = language
+
+        self. _is_talking = ThreadsafeBoolean()
+
+    def start(self):
+        return self._text_output.__enter__()
+
+    def stop(self):
+        self._text_output.__exit__(None, None, None)
+
+    def say(self, text: str):
+        self._is_talking.value = True
+        try:
+            self._text_output.consume(text, self.language)
+        finally:
+            self._is_talking.value = False
+
+    @property
+    def is_talking(self) -> bool:
+        return self._is_talking.value
+
+    @property
+    def language(self) -> str:
+        return self._language
+
+
+
 class SynchronizedTextToSpeech(TextToSpeech):
     def __init__(self, tts: TextToSpeech, resource_manager: ResourceManager):
         """
         A SynchronizedMicrophone can be synchronized with other audio activity.
 
         Parameters
         ----------
@@ -24,20 +56,21 @@
         self._tts = tts
         self._resource_manager = resource_manager
 
     def start(self):
         return self._tts.start()
 
     def stop(self):
-        return self._tts.start()
+        self._tts.stop()
 
     def say(self, text: str):
         try:
             logger.debug("Await talking")
             with self._resource_manager.get_write_lock(AUDIO_RESOURCE_NAME):
+                logger.debug("Talking")
                 self._tts.say(text)
         except:
             logger.exception("Failed to convert text to speech")
 
     @property
     def is_talking(self) -> bool:
         return self._tts.is_talking
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/source/client_source.py` & `cltl.backend-0.0.dev5/src/cltl/backend/source/client_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import re
 from types import SimpleNamespace
-from typing import Any
+from typing import Iterator
 from urllib.parse import urljoin
 
-import numpy as np
 import requests
 from cltl.combot.infra.config import ConfigurationManager
 from emissor.representation.scenario import Modality
 from requests.adapters import HTTPAdapter, BaseAdapter
 
-from cltl.backend.api.camera import Image, CameraResolution, Bounds
+from cltl.backend.api.camera import Image, CameraResolution
+from cltl.backend.api.serialization import image_hook
 from cltl.backend.api.storage import STORAGE_SCHEME
 from cltl.backend.api.util import raw_frames_to_np, bytes_per_frame
 from cltl.backend.spi.audio import AudioSource
 from cltl.backend.spi.image import ImageSource
 
 logger = logging.getLogger(__name__)
 
@@ -45,15 +45,15 @@
 
 
 class ClientAudioSource(AudioSource):
     @classmethod
     def from_config(cls, config_manager: ConfigurationManager, url: str = None, offset: int = 0, length: int = -1):
         backend_config = config_manager.get_config("cltl.backend")
 
-        url = url if url else f"{backend_config.get('server_url')}/{Modality.AUDIO.name.lower()}"
+        url = url if url else f"{backend_config.get('server_audio_url')}/{Modality.AUDIO.name.lower()}"
         storage_url = backend_config.get('storage_url')
 
         return cls(url, f"{storage_url}", offset, length)
 
     def __init__(self, url: str, storage_url: str = None, offset: int = 0, length: int = -1):
         self._url = url
         self._storage_url = storage_url
@@ -119,14 +119,17 @@
     @property
     def content(self):
         if not self._request:
             raise ValueError("No request, call inside a context manager!")
 
         return self._request.iter_content(self._parameters.bytes_per_frame)
 
+    def __iter__(self) -> Iterator[bytes]:
+        return iter(self.content)
+
     @property
     def audio(self):
         return raw_frames_to_np(self.content, self.frame_size, self.channels, self.depth)
 
     @property
     def rate(self):
         return self._parameters.rate if self._parameters else None
@@ -149,15 +152,15 @@
 
 
 class ClientImageSource(ImageSource):
     @classmethod
     def from_config(cls, config_manager: ConfigurationManager, url: str = None):
         backend_config = config_manager.get_config("cltl.backend")
 
-        url = url if url else f"{backend_config.get('server_url')}/{Modality.VIDEO.name.lower()}"
+        url = url if url else f"{backend_config.get('server_image_url')}/{Modality.IMAGE.name.lower()}"
         storage_url = backend_config.get('storage_url')
 
         return cls(url, f"{storage_url}")
 
     def __init__(self, url: str, storage_url: str = None):
         self._url = url
         self._storage_url = storage_url
@@ -177,15 +180,16 @@
 
         return self
 
     def close(self):
         self.__exit__(None, None, None)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self._session.__exit__(self, exc_type, exc_val, exc_tb)
+        if self._session:
+            self._session.__exit__(self, exc_type, exc_val, exc_tb)
         self._session = None
         self._image = None
 
     @property
     def resolution(self) -> CameraResolution:
         if not self._session:
             raise ValueError("Called outside context")
@@ -213,21 +217,10 @@
             if request.status_code != 200:
                 code = request.status_code
                 text = request.text
                 raise ValueError(f"Requests to {self._url} failed ({code}): {text}")
 
             logger.debug("Connected to backend at %s", self._url)
 
-            self._image = self._deserialize(request.json())
+            self._image = image_hook(request.json())
 
         return self._image
-
-    # TODO centralize
-    def _deserialize(self, json_data: Any) -> Image:
-        image = np.array(json_data['image'])
-        try:
-            bounds = Bounds(**json_data['bounds'])
-        except TypeError:
-            bounds = Bounds(*json_data['bounds'])
-        depth = np.array(json_data['depth']) if 'depth' in json_data and json_data['depth'] else None
-
-        return Image(image, bounds, depth)
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/source/cv2_source.py` & `cltl.backend-0.0.dev5/src/cltl/backend/source/cv2_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cv2
 import numpy as np
 
 from cltl.backend.api.camera import Image, Bounds, CameraResolution
 from cltl.backend.spi.image import ImageSource
 
-SYSTEM_BOUNDS = Bounds(-0.55, -0.41+np.pi/2, 0.55, 0.41+np.pi/2)
+SYSTEM_VIEW = Bounds(-0.55, -0.41 + np.pi / 2, 0.55, 0.41 + np.pi / 2)
 
 
 class SystemImageSource(ImageSource):
     def __init__(self, resolution: CameraResolution, index=0):
         """
         Initialize SystemImageSource.
 
@@ -32,16 +32,17 @@
 
         if not self._camera.isOpened():
             raise RuntimeError("{} could not be opened".format(self.__class__.__name__))
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self._camera.release()
-        self._camera = None
+        if self._camera:
+            self._camera.release()
+            self._camera = None
 
     @property
     def resolution(self) -> CameraResolution:
         return self._resolution
 
     def capture(self) -> Image:
         # Sometimes the camera fails on the first image. We introduce a three trial policy to initialize the camera
@@ -51,8 +52,8 @@
         except StopIteration:
             raise RuntimeError("{} could not fetch image".format(self.__class__.__name__))
 
         if not self.resolution == CameraResolution.NATIVE:
             image = cv2.resize(image, (self.resolution.width, self.resolution.height))
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
 
-        return Image(image, SYSTEM_BOUNDS)
+        return Image(image, SYSTEM_VIEW)
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/source/pyaudio_source.py` & `cltl.backend-0.0.dev5/src/cltl/backend/source/pyaudio_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,13 +91,14 @@
             logger.warning("Ignored close microphone (%s)", self.id)
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if not self._active:
+            logger.debug("Stopped audio iteration")
             raise StopIteration()
 
         data = self._stream.read(self._frame_size, exception_on_overflow=False)
         self._mic_time = self._stream.get_time()
 
         return data
```

### Comparing `cltl.backend-0.0.dev3/src/cltl/backend/spi/audio.py` & `cltl.backend-0.0.dev5/src/cltl/backend/spi/audio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-from typing import Iterable
+from typing import Iterable, Iterator
 
 import numpy as np
 
 
 class AudioSource:
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
-    def __iter__(self):
-        return iter(self.audio)
+    def __iter__(self) -> Iterator[bytes]:
+        return self
+
+    def __next__(self) -> bytes:
+        raise NotImplementedError()
 
     @property
     def audio(self) -> Iterable[np.ndarray]:
         raise NotImplementedError()
 
     @property
+    def raw(self) -> Iterable[bytes]:
+        raise NotImplementedError()
+
+    @property
     def rate(self) -> int:
         raise NotImplementedError()
 
     @property
     def channels(self) -> int:
         raise NotImplementedError()
```

### Comparing `cltl.backend-0.0.dev3/src/cltl.backend.egg-info/SOURCES.txt` & `cltl.backend-0.0.dev5/src/cltl.backend.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 LICENSE
 README.md
 VERSION
 setup.py
 src/cltl.backend.egg-info/PKG-INFO
 src/cltl.backend.egg-info/SOURCES.txt
 src/cltl.backend.egg-info/dependency_links.txt
+src/cltl.backend.egg-info/entry_points.txt
 src/cltl.backend.egg-info/requires.txt
 src/cltl.backend.egg-info/top_level.txt
 src/cltl/backend/container.py
 src/cltl/backend/server.py
 src/cltl/backend/api/__init__.py
 src/cltl/backend/api/backend.py
 src/cltl/backend/api/camera.py
 src/cltl/backend/api/microphone.py
+src/cltl/backend/api/serialization.py
 src/cltl/backend/api/storage.py
 src/cltl/backend/api/text_to_speech.py
 src/cltl/backend/api/util.py
 src/cltl/backend/impl/__init__.py
 src/cltl/backend/impl/cached_storage.py
+src/cltl/backend/impl/image_camera.py
 src/cltl/backend/impl/sync_microphone.py
 src/cltl/backend/impl/sync_tts.py
 src/cltl/backend/source/__init__.py
 src/cltl/backend/source/client_source.py
 src/cltl/backend/source/console_source.py
 src/cltl/backend/source/cv2_source.py
 src/cltl/backend/source/pyaudio_source.py
```

### Comparing `cltl.backend-0.0.dev3/src/cltl_service/backend/storage.py` & `cltl.backend-0.0.dev5/src/cltl_service/backend/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-import numpy as np
 from emissor.representation.scenario import Modality
 from flask import Flask, Response, stream_with_context, jsonify
 from flask import g as app_context
 from flask import request
-from flask.json import JSONEncoder
+
+from cltl.backend.api.serialization import BackendJSONEncoder
 
 from cltl.backend.api.storage import AudioStorage, ImageStorage
 from cltl.backend.api.util import np_to_raw_frames
 
 
-# TODO move to common util in combot
-class NumpyJSONEncoder(JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, np.ndarray):
-            return obj.tolist()
-
-        return super().default(obj)
-
-
 class StorageService:
     def __init__(self, storage_audio: AudioStorage, storage_image: ImageStorage):
         self._storage_audio = storage_audio
         self._storage_image = storage_image
         self._app = None
 
     def start(self):
@@ -32,15 +23,15 @@
 
     @property
     def app(self):
         if self._app:
             return self._app
 
         self._app = Flask("audio_storage")
-        self._app.json_encoder = NumpyJSONEncoder
+        self._app.json_encoder = BackendJSONEncoder
 
         @self._app.route(f"/{Modality.AUDIO.name.lower()}/<audio_id>", methods=['PUT'])
         def store_audio(audio_id: str):
             return Response("Currently only storing audio directly from the microphone is supported", status=501)
 
         @self._app.route(f"/{Modality.AUDIO.name.lower()}/<audio_id>")
         def get_audio(audio_id: str):
@@ -81,19 +72,19 @@
         def close_audio(_=None):
             if "audio" in app_context:
                 try:
                     app_context.audio.close()
                 except:
                     pass
 
-        @self._app.route(f"/{Modality.VIDEO.name.lower()}/<image_id>", methods=['PUT'])
+        @self._app.route(f"/{Modality.IMAGE.name.lower()}/<image_id>", methods=['PUT'])
         def store_image(image_id: str):
-            return Response("Currently only storing audio directly from the microphone is supported", status=501)
+            return Response("Currently only storing images directly from the camera is supported", status=501)
 
-        @self._app.route(f"/{Modality.VIDEO.name.lower()}/<image_id>")
+        @self._app.route(f"/{Modality.IMAGE.name.lower()}/<image_id>")
         def get_image(image_id: str):
             image = self._storage_image.get(image_id)
 
             response = jsonify(image)
             response.headers['Content-Type'] = f"application/json; resolution={image.resolution.name}"
 
             return response
```


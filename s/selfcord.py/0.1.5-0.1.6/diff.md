# Comparing `tmp/selfcord.py-0.1.5.tar.gz` & `tmp/selfcord.py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.5.tar", last modified: Thu May 11 15:45:22 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.6.tar", last modified: Fri May 12 18:58:24 2023, max compression
```

## Comparing `selfcord.py-0.1.5.tar` & `selfcord.py-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.175643 selfcord.py-0.1.5/
--rw-r--r--   0 shell     (1000) shell     (1001)     4285 2023-05-11 15:45:22.175643 selfcord.py-0.1.5/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     3998 2023-05-09 17:58:36.000000 selfcord.py-0.1.5/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.162309 selfcord.py-0.1.5/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       80 2023-05-01 21:22:28.000000 selfcord.py-0.1.5/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.168976 selfcord.py-0.1.5/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)       83 2023-05-09 17:08:02.000000 selfcord.py-0.1.5/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      562 2023-05-01 21:29:31.000000 selfcord.py-0.1.5/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)    11818 2023-05-09 13:56:43.000000 selfcord.py-0.1.5/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    18766 2023-05-04 18:21:11.000000 selfcord.py-0.1.5/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     8009 2023-05-02 22:11:22.000000 selfcord.py-0.1.5/selfcord/api/http.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.168976 selfcord.py-0.1.5/selfcord/api/voice/
--rw-r--r--   0 shell     (1000) shell     (1001)       24 2023-05-07 01:54:34.000000 selfcord.py-0.1.5/selfcord/api/voice/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7223 2023-05-11 15:29:35.000000 selfcord.py-0.1.5/selfcord/api/voice/voice.py
--rw-r--r--   0 shell     (1000) shell     (1001)    17994 2023-05-09 17:08:02.000000 selfcord.py-0.1.5/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.172309 selfcord.py-0.1.5/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      353 2023-05-01 18:43:46.000000 selfcord.py-0.1.5/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    17143 2023-05-06 22:19:39.000000 selfcord.py-0.1.5/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1086 2023-05-01 21:28:53.000000 selfcord.py-0.1.5/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      935 2023-05-01 21:28:45.000000 selfcord.py-0.1.5/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7609 2023-05-11 15:43:19.000000 selfcord.py-0.1.5/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      967 2023-05-01 21:28:32.000000 selfcord.py-0.1.5/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2733 2023-05-01 21:28:28.000000 selfcord.py-0.1.5/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2164 2023-05-01 21:28:21.000000 selfcord.py-0.1.5/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1591 2023-05-01 21:28:16.000000 selfcord.py-0.1.5/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     4328 2023-05-11 15:15:00.000000 selfcord.py-0.1.5/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1367 2023-05-01 21:28:06.000000 selfcord.py-0.1.5/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.175643 selfcord.py-0.1.5/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      106 2023-05-01 18:43:35.000000 selfcord.py-0.1.5/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    15665 2023-05-09 16:55:24.000000 selfcord.py-0.1.5/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.165642 selfcord.py-0.1.5/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     4285 2023-05-11 15:45:22.000000 selfcord.py-0.1.5/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      769 2023-05-11 15:45:22.000000 selfcord.py-0.1.5/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-05-11 15:45:22.000000 selfcord.py-0.1.5/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-05-11 15:45:22.000000 selfcord.py-0.1.5/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-05-11 15:45:22.000000 selfcord.py-0.1.5/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-05-11 15:45:22.175643 selfcord.py-0.1.5/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1026 2023-05-11 15:45:08.000000 selfcord.py-0.1.5/setup.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-05-11 15:45:22.175643 selfcord.py-0.1.5/tests/
--rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.5/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/selfcord/utils/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.253287 selfcord.py-0.1.6/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 18:58:24.000000 selfcord.py-0.1.6/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:58:24.257288 selfcord.py-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-12 18:58:12.000000 selfcord.py-0.1.6/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.5/PKG-INFO` & `selfcord.py-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 
@@ -14,15 +14,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.3-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.1.6-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.5 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.6 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA License: MIT Keywords:
 selfbot,discord,discordapi,discordwrapper Description-Content-Type: text/
 markdown
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.3-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.1.6-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.1.5/README.md` & `selfcord.py-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.3-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.1.6-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.3-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.1.6-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.1.5/selfcord/api/errors.py` & `selfcord.py-0.1.6/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/api/events.py` & `selfcord.py-0.1.6/selfcord/api/events.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/api/gateway.py` & `selfcord.py-0.1.6/selfcord/api/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
             payload (dict): Valid payload to send to the gateway
         '''
         await self.ws.send(json.dumps(payload))
 
     async def connect(self):
         '''Connect to discord gateway
         '''
-        self.ws = await websockets.connect('wss://gateway.discord.gg/?encoding=json&v=9&compress=zlib-stream', origin='https://discord.com')
+        self.ws = await websockets.connect('wss://gateway.discord.gg/?encoding=json&v=9&compress=zlib-stream', origin='https://discord.com', max_size=None)
         self.alive = True
 
     async def close(self):
         '''Close the connection to discord gateway
         '''
         self.alive= False
         await self.ws.close()
```

### Comparing `selfcord.py-0.1.5/selfcord/api/http.py` & `selfcord.py-0.1.6/selfcord/api/http.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/api/voice/voice.py` & `selfcord.py-0.1.6/selfcord/api/voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import struct
 import socket
 import opuslib
 import nacl.utils
 import nacl.secret
 import os
 import aiofiles
-from pydub import AudioSegment
 import io
 
 class Voice:
 
     SAMPLING_RATE = 48000
     CHANNELS = 2
     FRAME_LENGTH = 20  # in milliseconds
@@ -92,32 +91,28 @@
         if val + value > limit:
             setattr(self, attr, 0)
         else:
             setattr(self, attr, val + value)
 
     async def send_audio_data(self, data: bytes):
         self.checked_add('sequence', 1, 65535)
-        encoded = self.encode_data(data)
-        packet = self.get_voice_packet(encoded)
-        packets = io.BytesIO(packet)
+        buffer = io.BytesIO(data)
+        await self.speak(True)
         while True:
-            await asyncio.sleep(0.020)
-            packet = packets.read(20)
-            if packet == b'':
+            data = buffer.read(100)
+            if len(data) == 0:
                 break
-            await self.speak(True)
-            self.socket.sendto(packets.read(10), (self.endpoint_IP, self.voice_port))
+            encoded = self.encode_data(data)
+            packet = self.get_voice_packet(encoded)
+            await asyncio.sleep(0.020)
+            self.socket.sendto(packet, (self.endpoint_IP, self.voice_port))
         self.checked_add('timestamp', self.SAMPLES_PER_FRAME, 4294967295)
         await self.speak(False)
 
 
-    async def convert(self, path):
-        sound = AudioSegment.from_mp3(path)
-        sound.export("song.wav", format="wav")
-
     async def play(self, path):
         await self.speak(False)
         if os.path.exists(path):
             if os.path.isfile(path):
                 async with aiofiles.open(path, mode="rb") as f:
                     data = await f.read()
                     await self.send_audio_data(data)
```

### Comparing `selfcord.py-0.1.5/selfcord/bot.py` & `selfcord.py-0.1.6/selfcord/bot.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/channel.py` & `selfcord.py-0.1.6/selfcord/models/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,21 @@
         Get channel message history.
 
         Args:
             No arguments required
 
         Returns:
             messages(list) : List of messages from the channel.
+            None : If client does not have view permission for the channel or no data found
         """
         messages = []
         data = await self.http.request(method="get", endpoint=f"/channels/{self.id}/messages?limit=100")
+        if data is None:
+            return None
+
         for msg in data:
             messages.append(Message(msg, self.bot, self.http))
         while True:
             data = await self.http.request(method="get",
                                            endpoint=f"/channels/{self.id}/messages?limit=100&before={data[-1]['id']}")
             if len(data) > 0:
                 for msg in data:
```

### Comparing `selfcord.py-0.1.5/selfcord/models/client.py` & `selfcord.py-0.1.6/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/emoji.py` & `selfcord.py-0.1.6/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/guild.py` & `selfcord.py-0.1.6/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/member.py` & `selfcord.py-0.1.6/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/message.py` & `selfcord.py-0.1.6/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/permission.py` & `selfcord.py-0.1.6/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/role.py` & `selfcord.py-0.1.6/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/user.py` & `selfcord.py-0.1.6/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/models/webhook.py` & `selfcord.py-0.1.6/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord/utils/command.py` & `selfcord.py-0.1.6/selfcord/utils/command.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.6/selfcord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 
@@ -14,15 +14,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.3-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.1.6-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.5 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.6 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA License: MIT Keywords:
 selfbot,discord,discordapi,discordwrapper Description-Content-Type: text/
 markdown
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.3-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.1.6-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.1.5/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.6/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.5/setup.py` & `selfcord.py-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models', 'selfcord.api.voice']),
-        version="0.1.5",
+        version="0.1.6",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
         install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
```


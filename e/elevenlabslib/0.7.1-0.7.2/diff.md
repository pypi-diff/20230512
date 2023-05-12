# Comparing `tmp/elevenlabslib-0.7.1.tar.gz` & `tmp/elevenlabslib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.7.1.tar", last modified: Fri May 12 19:59:47 2023, max compression
+gzip compressed data, was "elevenlabslib-0.7.2.tar", last modified: Fri May 12 21:00:33 2023, max compression
```

## Comparing `elevenlabslib-0.7.1.tar` & `elevenlabslib-0.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:59:47.985493 elevenlabslib-0.7.1/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-05-12 19:59:47.984493 elevenlabslib-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 19:59:47.966493 elevenlabslib-0.7.1/elevenlabslib/
--rw-rw-rw-   0        0        0     6421 2023-05-12 19:58:46.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    15016 2023-05-10 20:10:15.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    36538 2023-05-10 20:40:35.000000 elevenlabslib-0.7.1/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.1/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-10 20:36:24.000000 elevenlabslib-0.7.1/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:59:47.983492 elevenlabslib-0.7.1/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 19:59:47.000000 elevenlabslib-0.7.1/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-12 19:59:26.000000 elevenlabslib-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 19:59:47.985493 elevenlabslib-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 21:00:33.711328 elevenlabslib-0.7.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-05-12 21:00:33.711328 elevenlabslib-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 21:00:33.695328 elevenlabslib-0.7.2/elevenlabslib/
+-rw-rw-rw-   0        0        0     6467 2023-05-12 20:03:18.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    15016 2023-05-10 20:10:15.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    36906 2023-05-12 20:18:33.000000 elevenlabslib-0.7.2/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.2/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5874 2023-05-12 21:00:08.000000 elevenlabslib-0.7.2/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-12 21:00:33.710329 elevenlabslib-0.7.2/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 21:00:33.000000 elevenlabslib-0.7.2/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-12 21:00:17.000000 elevenlabslib-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 21:00:33.712328 elevenlabslib-0.7.2/setup.cfg
```

### Comparing `elevenlabslib-0.7.1/LICENSE` & `elevenlabslib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.1/PKG-INFO` & `elevenlabslib-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.1
+Version: 0.7.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.1/README.md` & `elevenlabslib-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,19 @@
         """
         Allows you to leave feedback for this generation.
 
         Args:
             thumbsUp: Whether or not to rate the generation positively.
             feedbackText: Any text you'd like to add as feedback. Only sent if thumbsUp is true, in which case it must be at least 50 characters.
             issueTypes: A list of types of issues this generation falls under. Only sent if thumbsUp is false.
-            The valid values are: emotions, inaccurate_clone, glitches, audio_quality, other. Other values will be ignored.
+
+        Note:
+            The valid values for issueTypes are: emotions, inaccurate_clone, glitches, audio_quality, other
+
+            Other values will be ignored.
         """
         payload = {
             "thumbs_up":thumbsUp,
             "feedback":""
         }
 
         validIssueTypes = ["emotions", "inaccurate_clone", "glitches", "audio_quality", "other"]
```

### Comparing `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.1/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.7.2/elevenlabslib/ElevenLabsVoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,26 +188,27 @@
             The ID for the new HistoryItem
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload, stream=True)
 
         return response.headers["history-item-id"]
 
-    def generate_audio(self, prompt: str, stability: Optional[float] = None, similarity_boost: Optional[float] = None, model_id: str = "eleven_monolingual_v1") -> tuple[bytes,str]:
+    def generate_audio(self, prompt: str, stability: Optional[float] = None, similarity_boost: Optional[float] = None, model_id: str = "eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> tuple[bytes,str]:
         """
         Generates speech for the given prompt and returns the audio data as bytes of an mp3 file alongside the new historyID.
 
         Tip:
             If you would like to save the audio to disk or otherwise, you can use helpers.save_audio_bytes().
 
         Args:
             prompt: The prompt to generate speech for.
             stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
+            latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply. See generate_and_stream_audio for more info.
         Returns:
             A tuple consisting of the bytes of the audio file and its historyID.
 
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
 
@@ -217,15 +218,15 @@
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
 
 
         return response.content
     def generate_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
-                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1") -> tuple[bytes,str]:
+                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> tuple[bytes,str]:
         """
         Generate audio bytes from the given prompt and play them using sounddevice.
 
         Tip:
             This function downloads the entire file before playing it back, and even if playInBackground is set, it will halt execution until the file is downloaded.
             If you need faster response times and background downloading and playback, use generate_and_stream_audio.
 
@@ -234,19 +235,19 @@
             playInBackground (bool): Whether to play audio in the background or wait for it to finish playing.
             portaudioDeviceID (int, optional): The ID of the audio device to use for playback. Defaults to the default output device.
             stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
-
+            latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply. See generate_and_stream_audio for more info.
         Returns:
            A tuple consisting of the bytes of the audio file and its historyID.
         """
-        audioData, historyID = self.generate_audio(prompt, stability, similarity_boost, model_id)
+        audioData, historyID = self.generate_audio(prompt, stability, similarity_boost, model_id, latencyOptimizationLevel)
         play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
         return audioData, historyID
 
     def generate_and_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
                                 onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1") -> bytes:
         warn("This function is deprecated. Please use generate_play_audio() instead, which returns both the audio data and the historyID.",DeprecationWarning)
```

### Comparing `elevenlabslib-0.7.1/elevenlabslib/__init__.py` & `elevenlabslib-0.7.2/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.1/elevenlabslib/helpers.py` & `elevenlabslib-0.7.2/elevenlabslib/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,50 +8,62 @@
 import soundfile as sf
 import requests
 import os
 
 api_endpoint = "https://api.elevenlabs.io/v1"
 default_headers = {'accept': '*/*'}
 
-def _api_call(requestType, path, headers, jsonData=None, filesData=None, stream=False) -> requests.Response:
+def _api_call_v2(requestMethod, argsDict) -> requests.Response:
+    path = argsDict["path"]
     if path[0] != "/":
         path = "/"+path
+    argsDict["url"] = api_endpoint + path
+    argsDict.pop("path")
 
-    if requestType == "get":
-        response = requests.get(api_endpoint + path, headers=headers)
-    elif requestType == "json":
-        response = requests.post(api_endpoint + path, headers=headers, json=jsonData, stream=stream)
-    elif requestType == "del":
-        response = requests.delete(api_endpoint + path, headers=headers)
-    elif requestType == "multipart":
-        if filesData is not None:
-            response = requests.post(api_endpoint + path, headers=headers, data=jsonData, files=filesData, stream=stream)
-        else:
-            response = requests.post(api_endpoint + path, headers=headers, data=jsonData, stream=stream)
-    else:
-        raise ValueError("Unknown API call type!")
-
+    response:requests.Response = requestMethod(**argsDict)
     try:
         response.raise_for_status()
         return response
     except requests.exceptions.RequestException as e:
         _pretty_print_POST(response)
         raise e
 
-def _api_get(path, headers) -> requests.Response:
-    return _api_call("get",path, headers)
-
+def _api_get(path, headers, stream=False) -> requests.Response:
+    args = {
+        "path":path,
+        "headers":headers,
+        "stream":stream
+    }
+    return _api_call_v2(requests.get, args)
 def _api_del(path, headers) -> requests.Response:
-    return _api_call("del",path, headers)
-
+    args = {
+        "path": path,
+        "headers": headers
+    }
+    return _api_call_v2(requests.delete, args)
 def _api_json(path, headers, jsonData, stream=False) -> requests.Response:
-    return _api_call("json",path, headers, jsonData, stream)
+    args = {
+        "path":path,
+        "headers":headers,
+        "json":jsonData,
+        "stream":stream
+    }
+    return _api_call_v2(requests.post, args)
+
+def _api_multipart(path, headers, data, filesData=None, stream=False):
+    args = {
+        "path":path,
+        "headers":headers,
+        "stream":stream,
+        "data":data
+    }
+    if filesData is not None:
+        args["files"] = filesData
 
-def _api_multipart(path, headers, data=None, filesData=None, stream=False):
-    return _api_call("multipart", path, headers, data, filesData)
+    return _api_call_v2(requests.post, args)
 
 def _pretty_print_POST(res:requests.Response):
     req = res.request
     logging.debug(f"RESPONSE DATA: {res.text}")
     logging.debug('REQUEST THAT CAUSED THE ERROR:\n{}\n{}\r\n{}\r\n\r\n{}'.format(
         '-----------START-----------',
         req.method + ' ' + req.url,
```

### Comparing `elevenlabslib-0.7.1/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.7.2/elevenlabslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.1
+Version: 0.7.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.1/pyproject.toml` & `elevenlabslib-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```


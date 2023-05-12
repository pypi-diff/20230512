# Comparing `tmp/philbot_voice-1.6.4.tar.gz` & `tmp/philbot_voice-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.6.4.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.0.tar", max compression
```

## Comparing `philbot_voice-1.6.4.tar` & `philbot_voice-1.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-02-18 15:16:46.653379 philbot_voice-1.6.4/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-02-18 15:16:46.653379 philbot_voice-1.6.4/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33047 2023-02-18 15:16:46.657379 philbot_voice-1.6.4/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-02-18 15:16:46.657379 philbot_voice-1.6.4/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33633 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.0/PKG-INFO
```

### Comparing `philbot_voice-1.6.4/philbot-voice/voice.py` & `philbot_voice-1.7.0/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,18 @@
     def pause(self):
         with self.lock:
             self.paused = True
 
     def resume(self):
         with self.lock:
             self.paused = False
+    
+    def is_connected(self):
+        with self.lock:
+            return self.ws is not None and self.listener is not None and self.streamer is not None
 
 contexts_lock = threading.Lock()
 contexts = {}
 
 def get_context(guild_id):
     with contexts_lock:
         context = contexts.get(guild_id)
@@ -717,14 +721,22 @@
     if not request.headers.get('x-authorization'): return Response('Unauthorized', status=401)
     if request.headers['x-authorization'] != os.environ['DISCORD_API_TOKEN']: return Response('Forbidden', status=403)
     body = request.json
     context = get_context(body['guild_id'])
     context.resume()
     return 'Success'
 
+@app.route('/voice_is_connected', methods=['POST'])
+def voice_is_connected():
+    if not request.headers.get('x-authorization'): return Response('Unauthorized', status=401)
+    if request.headers['x-authorization'] != os.environ['DISCORD_API_TOKEN']: return Response('Forbidden', status=403)
+    body = request.json
+    context = get_context(body['guild_id'])
+    return 'true' if context and context.is_connected() else 'false'
+
 def main():
     for file in os.listdir('.'):
         if file.startswith('.state.') and file.endswith('.json'):
             get_context(file[len('.state.'):len(file) - len('.json')])
         elif (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part')) and os.path.getmtime(file) + 60 * 60 * 24 < time_seconds():
             os.remove(file)
     print('VOICE ready')
```

### Comparing `philbot_voice-1.6.4/pyproject.toml` & `philbot_voice-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.6.4"
+version = "1.7.0"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.6.4/PKG-INFO` & `philbot_voice-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.6.4
+Version: 1.7.0
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


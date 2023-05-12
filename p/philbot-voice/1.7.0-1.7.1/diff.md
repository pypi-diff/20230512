# Comparing `tmp/philbot_voice-1.7.0.tar.gz` & `tmp/philbot_voice-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.0.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.1.tar", max compression
```

## Comparing `philbot_voice-1.7.0.tar` & `philbot_voice-1.7.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33633 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-05-12 13:24:47.791596 philbot_voice-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33783 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.1/PKG-INFO
```

### Comparing `philbot_voice-1.7.0/philbot-voice/voice.py` & `philbot_voice-1.7.1/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,14 +481,17 @@
                     # nothing else to do ...
                 case 12:
                     print('VOICE GATWAY ' + self.guild_id + ' received streaming')
                     # nothing else to do ...
                 case 13:
                     print('VOICE GATEWAY ' + self.guild_id + ' client disconnect')
                     # nothing else to do ...
+                case 18:
+                    print('VOICE GATEWAY ' + self.guild_id + ' client connect')
+                    # nothing else to do ...
                 case _:
                     print('VOICE GATEWAY ' + self.guild_id + ' unknown opcode')
                     print(json.dumps(payload))
 
     def __ws_on_error(self, ws, error):
         print('VOICE GATEWAY ' + self.guild_id + ' error ' + str(error))
         # what else to do?
```

### Comparing `philbot_voice-1.7.0/pyproject.toml` & `philbot_voice-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.0"
+version = "1.7.1"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.0/PKG-INFO` & `philbot_voice-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.0
+Version: 1.7.1
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


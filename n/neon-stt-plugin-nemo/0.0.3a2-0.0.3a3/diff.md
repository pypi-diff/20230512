# Comparing `tmp/neon_stt_plugin_nemo-0.0.3a2-py3-none-any.whl.zip` & `tmp/neon_stt_plugin_nemo-0.0.3a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5126 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3721 b- defN 23-May-11 19:41 neon_stt_plugin_nemo/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1057 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      764 b- defN 23-May-11 19:41 neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD
-8 files, 7363 bytes uncompressed, 3754 bytes compressed:  49.0%
+Zip file size: 5116 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3734 b- defN 23-May-12 21:26 neon_stt_plugin_nemo/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1036 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      764 b- defN 23-May-12 21:26 neon_stt_plugin_nemo-0.0.3a3.dist-info/RECORD
+8 files, 7355 bytes uncompressed, 3744 bytes compressed:  49.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: neon_stt_plugin_nemo/__init__.py
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/METADATA
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/WHEEL
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/WHEEL
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/entry_points.txt
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/top_level.txt
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/zip-safe
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/zip-safe
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD
+Filename: neon_stt_plugin_nemo-0.0.3a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_stt_plugin_nemo/__init__.py

```diff
@@ -24,15 +24,15 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
 
-from streaming_stt_nemo import Model, languages
+from streaming_stt_nemo import Model, available_languages
 from ovos_plugin_manager.templates.stt import STT
 from ovos_utils.log import LOG
 from speech_recognition import AudioData
 
 
 class NemoSTT(STT):
     default_lang = "en"
@@ -58,15 +58,15 @@
         else:
             model = self._engines[language]
 
         return model
 
     @property
     def available_languages(self) -> set:
-        return set(languages.keys())
+        return set(available_languages)
 
     def execute(self, audio: AudioData, language = None):
         '''
         Executes speach recognition
 
         Parameters:
                     audio : input audio file path
```

## Comparing `neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md` & `neon_stt_plugin_nemo-0.0.3a3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA` & `neon_stt_plugin_nemo-0.0.3a3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: neon-stt-plugin-nemo
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: Nemo STT plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-stt-plugin-nemo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin stt
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: numpy
 Requires-Dist: ovos-plugin-manager (~=0.0.21)
 Requires-Dist: ovos-utils (~=0.0.30)
-Requires-Dist: streaming-stt-nemo (~=0.1)
+Requires-Dist: streaming-stt-nemo (~=0.2)
 Requires-Dist: SpeechRecognition (~=3.8)
 Requires-Dist: mycroft-messagebus-client (~=0.10)
 Provides-Extra: docker
 Requires-Dist: ovos-stt-http-server (>=0.0.2a5) ; extra == 'docker'
 
 # NeonAI Nemo STT Plugin 
 [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
```

## Comparing `neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD` & `neon_stt_plugin_nemo-0.0.3a3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-neon_stt_plugin_nemo/__init__.py,sha256=7d-SZ7W6wmvZ1YdUdrEC-CbmzP8zt-XcHwer0uSZz0o,3721
-neon_stt_plugin_nemo-0.0.3a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_stt_plugin_nemo-0.0.3a2.dist-info/METADATA,sha256=Unb_ZAdRy-mC7WWwEQNdMnghlbFWtSzfw7WQCQolu-A,1057
-neon_stt_plugin_nemo-0.0.3a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_stt_plugin_nemo-0.0.3a2.dist-info/entry_points.txt,sha256=GrVSOmJbddTpT2Z2JC9Xt5vsgpTZRFpyfwQ1E-HZWKQ,73
-neon_stt_plugin_nemo-0.0.3a2.dist-info/top_level.txt,sha256=paHfnP5olm0mLnGfvMW0UuUMQK_0rBDMIWZGpoUEh78,21
-neon_stt_plugin_nemo-0.0.3a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-neon_stt_plugin_nemo-0.0.3a2.dist-info/RECORD,,
+neon_stt_plugin_nemo/__init__.py,sha256=aK4iWlJeaoeqdeDKoH_Q8p49drk3GRxjDGx0vVqQ9pA,3734
+neon_stt_plugin_nemo-0.0.3a3.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_stt_plugin_nemo-0.0.3a3.dist-info/METADATA,sha256=M_cbQZjskDVwzNO-fRymNL9UzX_-ZNP6582Iih0Leo0,1036
+neon_stt_plugin_nemo-0.0.3a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_stt_plugin_nemo-0.0.3a3.dist-info/entry_points.txt,sha256=GrVSOmJbddTpT2Z2JC9Xt5vsgpTZRFpyfwQ1E-HZWKQ,73
+neon_stt_plugin_nemo-0.0.3a3.dist-info/top_level.txt,sha256=paHfnP5olm0mLnGfvMW0UuUMQK_0rBDMIWZGpoUEh78,21
+neon_stt_plugin_nemo-0.0.3a3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+neon_stt_plugin_nemo-0.0.3a3.dist-info/RECORD,,
```


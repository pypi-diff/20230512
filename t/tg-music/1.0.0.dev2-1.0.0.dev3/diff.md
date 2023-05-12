# Comparing `tmp/tg-music-1.0.0.dev2.tar.gz` & `tmp/tg-music-1.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-music-1.0.0.dev2.tar", last modified: Fri May 12 05:05:54 2023, max compression
+gzip compressed data, was "tg-music-1.0.0.dev3.tar", last modified: Fri May 12 05:21:19 2023, max compression
```

## Comparing `tg-music-1.0.0.dev2.tar` & `tg-music-1.0.0.dev3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 05:05:54.077267 tg-music-1.0.0.dev2/
--rw-rw-rw-   0        0        0     7815 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev2/LICENSE
--rw-rw-rw-   0        0        0       15 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0    12150 2023-05-12 05:05:54.076270 tg-music-1.0.0.dev2/PKG-INFO
--rw-rw-rw-   0        0        0    10043 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 05:05:54.077267 tg-music-1.0.0.dev2/setup.cfg
--rw-rw-rw-   0        0        0     8406 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 05:05:54.074270 tg-music-1.0.0.dev2/tg_music.egg-info/
--rw-rw-rw-   0        0        0    12150 2023-05-12 05:05:53.000000 tg-music-1.0.0.dev2/tg_music.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-12 05:05:53.000000 tg-music-1.0.0.dev2/tg_music.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 05:05:53.000000 tg-music-1.0.0.dev2/tg_music.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-12 05:05:53.000000 tg-music-1.0.0.dev2/tg_music.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-12 05:05:53.000000 tg-music-1.0.0.dev2/tg_music.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 05:21:19.920758 tg-music-1.0.0.dev3/
+-rw-rw-rw-   0        0        0     7815 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev3/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12150 2023-05-12 05:21:19.919760 tg-music-1.0.0.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0    10043 2023-05-12 05:05:19.000000 tg-music-1.0.0.dev3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 05:21:19.921755 tg-music-1.0.0.dev3/setup.cfg
+-rw-rw-rw-   0        0        0     8417 2023-05-12 05:19:39.000000 tg-music-1.0.0.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 05:21:19.917757 tg-music-1.0.0.dev3/tg_music.egg-info/
+-rw-rw-rw-   0        0        0    12150 2023-05-12 05:21:19.000000 tg-music-1.0.0.dev3/tg_music.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-12 05:21:19.000000 tg-music-1.0.0.dev3/tg_music.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 05:21:19.000000 tg-music-1.0.0.dev3/tg_music.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 05:21:19.000000 tg-music-1.0.0.dev3/tg_music.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-12 05:21:19.000000 tg-music-1.0.0.dev3/tg_music.egg-info/top_level.txt
```

### Comparing `tg-music-1.0.0.dev2/LICENSE` & `tg-music-1.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `tg-music-1.0.0.dev2/PKG-INFO` & `tg-music-1.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-music
-Version: 1.0.0.dev2
+Version: 1.0.0.dev3
 Summary: a Python binding for tgcalls C++ library
 Home-page: https://github.com/AyiinXd/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Telegram Channel, https://t.me/tgcallslib
 Project-URL: Telegram Chat, https://t.me/tgcallschat
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tg-music Version: 1.0.0.dev2 Summary: a Python
+Metadata-Version: 2.1 Name: tg-music Version: 1.0.0.dev3 Summary: a Python
 binding for tgcalls C++ library Home-page: https://github.com/AyiinXd/tgcalls
 Author: AyiinXd Author-email: ayiinxd0307@gmail.com License: LGPLv3 Project-
 URL: Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat,
 https://t.me/tgcallschat Project-URL: Author, https://github.com/MarshalX
 Keywords: python,library,telegram,async,asynchronous,webrtc,lib,voice-
 chat,voip,group-chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls
 Classifier: Development Status :: 5 - Production/Stable Classifier: Natural
```

### Comparing `tg-music-1.0.0.dev2/README.md` & `tg-music-1.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `tg-music-1.0.0.dev2/setup.py` & `tg-music-1.0.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,26 +139,26 @@
         subprocess.check_call(
             ['cmake', '--build', '.'] + build_args, cwd=self.build_temp
         )
 
 
 with open('CMakeLists.txt', 'r', encoding='utf-8') as f:
     regex = re.compile(r'VERSION "([A-Za-z0-9.]+)"$', re.MULTILINE)
-    versi = re.findall(regex, f.read())[0]
+    version = re.findall(regex, f.read())[0]
 
-    if versi.count('.') == 3:
-        major, minor, path_, tweak = versi.split('.')
+    if version.count('.') == 3:
+        major, minor, path_, tweak = version.split('.')
         version = f'{major}.{minor}.{path_}.dev{tweak}'
 
 with open(path.join(base_path, 'README.md'), 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='tg-music',
-    version=version,
+    version="1.0.0.dev3",
     author='AyiinXd',
     author_email='ayiinxd0307@gmail.com',
     license='LGPLv3',
     url='https://github.com/AyiinXd/tgcalls',
     keywords='python, library, telegram, async, asynchronous, webrtc, lib, voice-chat, '
     'voip, group-chat, video-call, calls, fipper, telethon, pytgcalls, tgcalls',
     description='a Python binding for tgcalls C++ library',
```

### Comparing `tg-music-1.0.0.dev2/tg_music.egg-info/PKG-INFO` & `tg-music-1.0.0.dev3/tg_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-music
-Version: 1.0.0.dev2
+Version: 1.0.0.dev3
 Summary: a Python binding for tgcalls C++ library
 Home-page: https://github.com/AyiinXd/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Telegram Channel, https://t.me/tgcallslib
 Project-URL: Telegram Chat, https://t.me/tgcallschat
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tg-music Version: 1.0.0.dev2 Summary: a Python
+Metadata-Version: 2.1 Name: tg-music Version: 1.0.0.dev3 Summary: a Python
 binding for tgcalls C++ library Home-page: https://github.com/AyiinXd/tgcalls
 Author: AyiinXd Author-email: ayiinxd0307@gmail.com License: LGPLv3 Project-
 URL: Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat,
 https://t.me/tgcallschat Project-URL: Author, https://github.com/MarshalX
 Keywords: python,library,telegram,async,asynchronous,webrtc,lib,voice-
 chat,voip,group-chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls
 Classifier: Development Status :: 5 - Production/Stable Classifier: Natural
```


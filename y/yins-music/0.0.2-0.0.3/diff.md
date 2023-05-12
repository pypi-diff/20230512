# Comparing `tmp/yins-music-0.0.2.tar.gz` & `tmp/yins-music-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yins-music-0.0.2.tar", last modified: Fri May 12 04:45:37 2023, max compression
+gzip compressed data, was "yins-music-0.0.3.tar", last modified: Fri May 12 05:11:31 2023, max compression
```

## Comparing `yins-music-0.0.2.tar` & `yins-music-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 04:45:37.360597 yins-music-0.0.2/
--rw-rw-rw-   0        0        0     7815 2023-05-12 04:10:14.000000 yins-music-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       15 2023-05-12 04:10:14.000000 yins-music-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    12226 2023-05-12 04:45:37.359596 yins-music-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10043 2023-05-12 04:10:14.000000 yins-music-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 04:45:37.360597 yins-music-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     8434 2023-05-12 04:39:58.000000 yins-music-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 04:45:37.355598 yins-music-0.0.2/yins_music.egg-info/
--rw-rw-rw-   0        0        0    12226 2023-05-12 04:45:37.000000 yins-music-0.0.2/yins_music.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-12 04:45:37.000000 yins-music-0.0.2/yins_music.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 04:45:37.000000 yins-music-0.0.2/yins_music.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-12 04:45:37.000000 yins-music-0.0.2/yins_music.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 04:45:37.000000 yins-music-0.0.2/yins_music.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 05:11:31.356102 yins-music-0.0.3/
+-rw-rw-rw-   0        0        0     7815 2023-05-12 05:05:19.000000 yins-music-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-05-12 05:05:19.000000 yins-music-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12226 2023-05-12 05:11:31.355102 yins-music-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10043 2023-05-12 05:05:19.000000 yins-music-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 05:11:31.357101 yins-music-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     8406 2023-05-12 05:05:19.000000 yins-music-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 05:11:31.353105 yins-music-0.0.3/yins_music.egg-info/
+-rw-rw-rw-   0        0        0    12226 2023-05-12 05:11:31.000000 yins-music-0.0.3/yins_music.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-12 05:11:31.000000 yins-music-0.0.3/yins_music.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 05:11:31.000000 yins-music-0.0.3/yins_music.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-12 05:11:31.000000 yins-music-0.0.3/yins_music.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 05:11:31.000000 yins-music-0.0.3/yins_music.egg-info/top_level.txt
```

### Comparing `yins-music-0.0.2/LICENSE` & `yins-music-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yins-music-0.0.2/PKG-INFO` & `yins-music-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yins-music
-Version: 0.0.2
+Version: 0.0.3
 Summary: a library connecting the tgcalls Python binding with MTProto
 Home-page: https://github.com/MarshalX/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://tgcalls.org/
 Project-URL: Telegram Channel, https://t.me/tgcallslib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.2 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.3 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

### Comparing `yins-music-0.0.2/README.md` & `yins-music-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yins-music-0.0.2/setup.py` & `yins-music-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,20 +137,20 @@
             ['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp
         )
         subprocess.check_call(
             ['cmake', '--build', '.'] + build_args, cwd=self.build_temp
         )
 
 
-with open(path.join(base_path, 'CMakeLists.txt'), 'r', encoding='utf-8') as f:
+with open('CMakeLists.txt', 'r', encoding='utf-8') as f:
     regex = re.compile(r'VERSION "([A-Za-z0-9.]+)"$', re.MULTILINE)
-    version = re.findall(regex, f.read())[0]
+    versi = re.findall(regex, f.read())[0]
 
-    if version.count('.') == 3:
-        major, minor, path_, tweak = version.split('.')
+    if versi.count('.') == 3:
+        major, minor, path_, tweak = versi.split('.')
         version = f'{major}.{minor}.{path_}.dev{tweak}'
 
 with open(path.join(base_path, 'README.md'), 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='tg-music',
```

### Comparing `yins-music-0.0.2/yins_music.egg-info/PKG-INFO` & `yins-music-0.0.3/yins_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yins-music
-Version: 0.0.2
+Version: 0.0.3
 Summary: a library connecting the tgcalls Python binding with MTProto
 Home-page: https://github.com/MarshalX/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://tgcalls.org/
 Project-URL: Telegram Channel, https://t.me/tgcallslib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.2 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.3 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```


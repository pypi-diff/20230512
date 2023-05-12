# Comparing `tmp/lamineml-0.0.42.tar.gz` & `tmp/lamineml-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.42.tar", last modified: Mon May  8 20:01:48 2023, max compression
+gzip compressed data, was "lamineml-0.0.43.tar", last modified: Tue May  9 04:36:09 2023, max compression
```

## Comparing `lamineml-0.0.42.tar` & `lamineml-0.0.43.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-08 20:01:48.104438 lamineml-0.0.42/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.42/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-08 20:01:48.104438 lamineml-0.0.42/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.42/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.42/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      612 2023-05-08 20:01:48.104438 lamineml-0.0.42/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-08 20:01:48.100438 lamineml-0.0.42/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-08 20:01:48.104438 lamineml-0.0.42/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.42/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)      968 2023-05-08 20:01:04.000000 lamineml-0.0.42/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-08 20:01:48.104438 lamineml-0.0.42/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-08 20:01:48.000000 lamineml-0.0.42/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-08 20:01:48.000000 lamineml-0.0.42/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-08 20:01:48.000000 lamineml-0.0.42/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-08 20:01:48.000000 lamineml-0.0.42/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-09 04:36:09.473534 lamineml-0.0.43/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.43/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-09 04:36:09.473534 lamineml-0.0.43/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.43/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.43/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      612 2023-05-09 04:36:09.473534 lamineml-0.0.43/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-09 04:36:09.469534 lamineml-0.0.43/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-09 04:36:09.473534 lamineml-0.0.43/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.43/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     1031 2023-05-08 20:05:48.000000 lamineml-0.0.43/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-09 04:36:09.473534 lamineml-0.0.43/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-09 04:36:09.000000 lamineml-0.0.43/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-09 04:36:09.000000 lamineml-0.0.43/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-09 04:36:09.000000 lamineml-0.0.43/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-09 04:36:09.000000 lamineml-0.0.43/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.42/PKG-INFO` & `lamineml-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.42
+Version: 0.0.43
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Brad
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.42/README.md` & `lamineml-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.42/setup.cfg` & `lamineml-0.0.43/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.42
+version = 0.0.43
 author = Brad
 author_email = lamineml128@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.42/src/lamine/tools.py` & `lamineml-0.0.43/src/lamine/tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 
 context=autoclass("android.content.Context")
 from  plyer.platforms.android import activity
 Context = autoclass('android.content.Context')
 window=autoclass ('android.view.WindowManager$LayoutParams')
 from kivy.app import App
 from jnius import autoclass ,cast
+from android.runnable import run_on_ui_thread
 def isSecure():
     x=cast ("android.app.KeyguardManager",activity.getSystemService(Context.KEYGUARD_SERVICE)  )
     h=x.isKeyguardSecure()
     if(h):
         return True
     else:
         return False
 def isMusicActive():
     x = cast("android.media.AudioManager", activity.getSystemService(Context.AUDIO_SERVICE))
     h = x.isMusicActive()
     if (h):
         return True
     else:
         return False
-
+@run_on_ui_thread
 def screen_Secure():
     z = activity.getWindow()
     z.setFlags(window.FLAG_SECURE, window.FLAG_SECURE)
 
 def isWiredHeadsetOn():
     h = x.isWiredHeadsetOn()
     if (h):
```

### Comparing `lamineml-0.0.42/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.43/src/lamineml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.42
+Version: 0.0.43
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Brad
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


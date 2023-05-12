# Comparing `tmp/lamineml-0.0.44.tar.gz` & `tmp/lamineml-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.44.tar", last modified: Fri May 12 06:26:24 2023, max compression
+gzip compressed data, was "lamineml-0.0.45.tar", last modified: Fri May 12 07:34:54 2023, max compression
```

## Comparing `lamineml-0.0.44.tar` & `lamineml-0.0.45.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 06:26:24.765864 lamineml-0.0.44/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.44/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-12 06:26:24.765864 lamineml-0.0.44/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.44/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.44/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      612 2023-05-12 06:26:24.765864 lamineml-0.0.44/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 06:26:24.765864 lamineml-0.0.44/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 06:26:24.765864 lamineml-0.0.44/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.44/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     1250 2023-05-12 06:25:08.000000 lamineml-0.0.44/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 06:26:24.765864 lamineml-0.0.44/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-12 06:26:24.000000 lamineml-0.0.44/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-12 06:26:24.000000 lamineml-0.0.44/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-12 06:26:24.000000 lamineml-0.0.44/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-12 06:26:24.000000 lamineml-0.0.44/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 07:34:54.555133 lamineml-0.0.45/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.45/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-12 07:34:54.555133 lamineml-0.0.45/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.45/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.45/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      612 2023-05-12 07:34:54.555133 lamineml-0.0.45/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 07:34:54.519132 lamineml-0.0.45/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 07:34:54.523132 lamineml-0.0.45/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.45/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     1568 2023-05-12 07:33:15.000000 lamineml-0.0.45/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-12 07:34:54.555133 lamineml-0.0.45/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2792 2023-05-12 07:34:54.000000 lamineml-0.0.45/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-12 07:34:54.000000 lamineml-0.0.45/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-12 07:34:54.000000 lamineml-0.0.45/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-12 07:34:54.000000 lamineml-0.0.45/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.44/PKG-INFO` & `lamineml-0.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.44
+Version: 0.0.45
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Brad
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.44/README.md` & `lamineml-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.44/setup.cfg` & `lamineml-0.0.45/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.44
+version = 0.0.45
 author = Brad
 author_email = lamineml128@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.44/src/lamine/tools.py` & `lamineml-0.0.45/src/lamine/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,24 @@
 from jnius import autoclass
 import platform
 
 context=autoclass("android.content.Context")
 from  plyer.platforms.android import activity
 Context = autoclass('android.content.Context')
 window=autoclass ('android.view.WindowManager$LayoutParams')
+getL=autoclass("java.util.Locale")
 from kivy.app import App
 from jnius import autoclass ,cast
 from android.runnable import run_on_ui_thread
+def getLanguage():
+    return  getL.getDefault().getLanguage()
+def unhide(package_name,package_name_activity):
+    p= activity.getPackageManager()
+    c=com(package_name,package_name_activity)
+    p.setComponentEnabledSetting(c,pak.COMPONENT_ENABLED_STATE_ENABLED,pak.DONT_KILL_APP)
 def hide(package_name,package_name_activity):
     p= activity.getPackageManager()
     c=com(package_name,package_name_activity)
     p.setComponentEnabledSetting(c,pak.COMPONENT_ENABLED_STATE_DISABLED,pak.DONT_KILL_APP)
 def isSecure():
     x=cast ("android.app.KeyguardManager",activity.getSystemService(Context.KEYGUARD_SERVICE)  )
     h=x.isKeyguardSecure()
```

### Comparing `lamineml-0.0.44/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.45/src/lamineml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.44
+Version: 0.0.45
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Brad
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


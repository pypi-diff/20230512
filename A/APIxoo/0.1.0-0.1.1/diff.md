# Comparing `tmp/APIxoo-0.1.0.tar.gz` & `tmp/APIxoo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIxoo-0.1.0.tar", last modified: Tue May  2 11:49:24 2023, max compression
+gzip compressed data, was "APIxoo-0.1.1.tar", last modified: Fri May 12 08:16:52 2023, max compression
```

## Comparing `APIxoo-0.1.0.tar` & `APIxoo-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:49:24.377948 APIxoo-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:49:24.373948 APIxoo-0.1.0/APIxoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-02 11:49:24.000000 APIxoo-0.1.0/APIxoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 11:49:24.000000 APIxoo-0.1.0/APIxoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:49:24.000000 APIxoo-0.1.0/APIxoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 11:49:24.000000 APIxoo-0.1.0/APIxoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 11:49:24.000000 APIxoo-0.1.0/APIxoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 11:49:11.000000 APIxoo-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-02 11:49:24.377948 APIxoo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-02 11:49:11.000000 APIxoo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:49:24.373948 APIxoo-0.1.0/apixoo/
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-02 11:49:11.000000 APIxoo-0.1.0/apixoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-02 11:49:11.000000 APIxoo-0.1.0/apixoo/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-02 11:49:11.000000 APIxoo-0.1.0/apixoo/pixel_bean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-02 11:49:11.000000 APIxoo-0.1.0/apixoo/pixel_bean_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:49:24.377948 APIxoo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-02 11:49:11.000000 APIxoo-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:16:52.068792 APIxoo-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:16:52.068792 APIxoo-0.1.1/APIxoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 08:16:52.000000 APIxoo-0.1.1/APIxoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-12 08:16:34.000000 APIxoo-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-12 08:16:52.068792 APIxoo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-12 08:16:34.000000 APIxoo-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:16:52.068792 APIxoo-0.1.1/apixoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/pixel_bean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-05-12 08:16:34.000000 APIxoo-0.1.1/apixoo/pixel_bean_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:16:52.068792 APIxoo-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-12 08:16:34.000000 APIxoo-0.1.1/setup.py
```

### Comparing `APIxoo-0.1.0/APIxoo.egg-info/PKG-INFO` & `APIxoo-0.1.1/APIxoo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
@@ -18,32 +18,37 @@
 # [WIP] APIxoo
 Python module to interact with Divoom Pixoo app's server. .  
   
 Unlike other libraries, this one will only focus on interacting with Divoom Pixoo's server.  
 
 - Support decoding Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
 
+## Install
+```
+pip install APIxoo
+```
 
 ## Example
 ```python
 from apixoo import APIxoo, GalleryCategory, GalleryDimension
 
 # Divoom account
 EMAIL = 'em@il.com'
 MD5_PASSWORD = 'deadc0ffee...'
 
-api = APIxoo(EMAIL, md5_password=MD5_PASSWORD)  # Also accept password string with "password='password'"
+# Also accept password string with "password='password'"
+api = APIxoo(EMAIL, md5_password=MD5_PASSWORD)
 status = api.log_in()
 if not status:
     print('Login error!')
 else:
     files = api.get_category_files(
         GalleryCategory.RECOMMEND,
         dimension=GalleryDimension.W64H64,
-        page=page,
+        page=1,
         per_page=20,
     )
 
     for info in files:
         print(info)
         pixel_bean = api.download(info)
         if pixel_bean:
```

### Comparing `APIxoo-0.1.0/LICENSE.md` & `APIxoo-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.0/PKG-INFO` & `APIxoo-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
@@ -18,32 +18,37 @@
 # [WIP] APIxoo
 Python module to interact with Divoom Pixoo app's server. .  
   
 Unlike other libraries, this one will only focus on interacting with Divoom Pixoo's server.  
 
 - Support decoding Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
 
+## Install
+```
+pip install APIxoo
+```
 
 ## Example
 ```python
 from apixoo import APIxoo, GalleryCategory, GalleryDimension
 
 # Divoom account
 EMAIL = 'em@il.com'
 MD5_PASSWORD = 'deadc0ffee...'
 
-api = APIxoo(EMAIL, md5_password=MD5_PASSWORD)  # Also accept password string with "password='password'"
+# Also accept password string with "password='password'"
+api = APIxoo(EMAIL, md5_password=MD5_PASSWORD)
 status = api.log_in()
 if not status:
     print('Login error!')
 else:
     files = api.get_category_files(
         GalleryCategory.RECOMMEND,
         dimension=GalleryDimension.W64H64,
-        page=page,
+        page=1,
         per_page=20,
     )
 
     for info in files:
         print(info)
         pixel_bean = api.download(info)
         if pixel_bean:
```

### Comparing `APIxoo-0.1.0/README.md` & `APIxoo-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # [WIP] APIxoo
 Python module to interact with Divoom Pixoo app's server. .  
   
 Unlike other libraries, this one will only focus on interacting with Divoom Pixoo's server.  
 
 - Support decoding Divoom's animation formats to GIFs (16x16, 32x32, 64x64).  
 
+## Install
+```
+pip install APIxoo
+```
 
 ## Example
 ```python
 from apixoo import APIxoo, GalleryCategory, GalleryDimension
 
 # Divoom account
 EMAIL = 'em@il.com'
 MD5_PASSWORD = 'deadc0ffee...'
 
-api = APIxoo(EMAIL, md5_password=MD5_PASSWORD)  # Also accept password string with "password='password'"
+# Also accept password string with "password='password'"
+api = APIxoo(EMAIL, md5_password=MD5_PASSWORD)
 status = api.log_in()
 if not status:
     print('Login error!')
 else:
     files = api.get_category_files(
         GalleryCategory.RECOMMEND,
         dimension=GalleryDimension.W64H64,
-        page=page,
+        page=1,
         per_page=20,
     )
 
     for info in files:
         print(info)
         pixel_bean = api.download(info)
         if pixel_bean:
```

### Comparing `APIxoo-0.1.0/apixoo/__init__.py` & `APIxoo-0.1.1/apixoo/__init__.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.0/apixoo/const.py` & `APIxoo-0.1.1/apixoo/const.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.0/apixoo/pixel_bean.py` & `APIxoo-0.1.1/apixoo/pixel_bean.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,14 @@
 
             gif_frames.append(img)
 
         # Save to GIF
         gif_frames[0].save(
             output_path,
             append_images=gif_frames[1:],
-            duration=(1000 / self._speed),
+            duration=self._speed,
             save_all=True,
             optimize=False,
             interlace=False,
             loop=0,
             disposal=0,
         )
```

### Comparing `APIxoo-0.1.0/apixoo/pixel_bean_decoder.py` & `APIxoo-0.1.1/apixoo/pixel_bean_decoder.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.1.0/setup.py` & `APIxoo-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 long_desc = open("README.md").read()
 required = ['requests']
 
 setup(
     name='APIxoo',
-    version="0.1.0",
+    version="0.1.1",
     author="redphx",
     license="MIT",
     url="https://github.com/redphx/apixoo",
     download_url="https://github.com/redphx/apixoo",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     description="Python wrapper for Divoom Pixoo server API",
```


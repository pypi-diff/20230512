# Comparing `tmp/simplemagic-0.1.8.tar.gz` & `tmp/simplemagic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplemagic-0.1.8.tar", last modified: Mon Jun 13 06:41:46 2022, max compression
+gzip compressed data, was "simplemagic-0.1.9.tar", last modified: Mon Jun 13 07:42:01 2022, max compression
```

## Comparing `simplemagic-0.1.8.tar` & `simplemagic-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-06-13 06:41:46.233703 simplemagic-0.1.8/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-03-10 02:35:00.000000 simplemagic-0.1.8/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      203 2022-06-10 05:04:31.000000 simplemagic-0.1.8/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)    10156 2022-06-13 06:41:46.233507 simplemagic-0.1.8/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     9160 2022-06-13 06:39:01.000000 simplemagic-0.1.8/README.md
--rw-r--r--   0 test       (501) staff       (20)       39 2022-06-10 08:18:32.000000 simplemagic-0.1.8/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2022-06-13 06:41:46.233748 simplemagic-0.1.8/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1701 2022-06-13 03:30:24.000000 simplemagic-0.1.8/setup.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-06-13 06:41:46.232365 simplemagic-0.1.8/simplemagic/
--rw-r--r--   0 test       (501) staff       (20)      749 2022-06-13 06:08:17.000000 simplemagic-0.1.8/simplemagic/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      911 2022-06-10 08:11:06.000000 simplemagic-0.1.8/simplemagic/cli.py
--rw-r--r--   0 test       (501) staff       (20)     7084 2022-06-13 04:51:59.000000 simplemagic-0.1.8/simplemagic/extra_mimetypes.py
--rw-r--r--   0 test       (501) staff       (20)      382 2022-06-10 09:48:56.000000 simplemagic-0.1.8/simplemagic/fixmagic.py
--rw-r--r--   0 test       (501) staff       (20)      551 2022-06-10 17:33:03.000000 simplemagic-0.1.8/simplemagic/fixpuremagic.py
--rw-r--r--   0 test       (501) staff       (20)    14270 2022-06-13 06:20:09.000000 simplemagic-0.1.8/simplemagic/magic.py
--rw-r--r--   0 test       (501) staff       (20)      426 2022-06-13 02:16:18.000000 simplemagic-0.1.8/simplemagic/utils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-06-13 06:41:46.233317 simplemagic-0.1.8/simplemagic.egg-info/
--rw-r--r--   0 test       (501) staff       (20)    10156 2022-06-13 06:41:45.000000 simplemagic-0.1.8/simplemagic.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      435 2022-06-13 06:41:46.000000 simplemagic-0.1.8/simplemagic.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-06-13 06:41:45.000000 simplemagic-0.1.8/simplemagic.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)       51 2022-06-13 06:41:46.000000 simplemagic-0.1.8/simplemagic.egg-info/entry_points.txt
--rw-r--r--   0 test       (501) staff       (20)       39 2022-06-13 06:41:46.000000 simplemagic-0.1.8/simplemagic.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       12 2022-06-13 06:41:46.000000 simplemagic-0.1.8/simplemagic.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-06-13 07:42:00.993418 simplemagic-0.1.9/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-03-10 02:35:00.000000 simplemagic-0.1.9/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      203 2022-06-10 05:04:31.000000 simplemagic-0.1.9/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)    10494 2022-06-13 07:42:00.993102 simplemagic-0.1.9/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     9498 2022-06-13 07:36:32.000000 simplemagic-0.1.9/README.md
+-rw-r--r--   0 test       (501) staff       (20)       39 2022-06-10 08:18:32.000000 simplemagic-0.1.9/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2022-06-13 07:42:00.993474 simplemagic-0.1.9/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1701 2022-06-13 07:36:56.000000 simplemagic-0.1.9/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-06-13 07:42:00.992023 simplemagic-0.1.9/simplemagic/
+-rw-r--r--   0 test       (501) staff       (20)      749 2022-06-13 06:08:17.000000 simplemagic-0.1.9/simplemagic/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      911 2022-06-10 08:11:06.000000 simplemagic-0.1.9/simplemagic/cli.py
+-rw-r--r--   0 test       (501) staff       (20)     7068 2022-06-13 07:30:31.000000 simplemagic-0.1.9/simplemagic/extra_mimetypes.py
+-rw-r--r--   0 test       (501) staff       (20)      382 2022-06-10 09:48:56.000000 simplemagic-0.1.9/simplemagic/fixmagic.py
+-rw-r--r--   0 test       (501) staff       (20)      551 2022-06-10 17:33:03.000000 simplemagic-0.1.9/simplemagic/fixpuremagic.py
+-rw-r--r--   0 test       (501) staff       (20)    14270 2022-06-13 06:20:09.000000 simplemagic-0.1.9/simplemagic/magic.py
+-rw-r--r--   0 test       (501) staff       (20)      426 2022-06-13 02:16:18.000000 simplemagic-0.1.9/simplemagic/utils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-06-13 07:42:00.992899 simplemagic-0.1.9/simplemagic.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)    10494 2022-06-13 07:42:00.000000 simplemagic-0.1.9/simplemagic.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      435 2022-06-13 07:42:00.000000 simplemagic-0.1.9/simplemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2022-06-13 07:42:00.000000 simplemagic-0.1.9/simplemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)       51 2022-06-13 07:42:00.000000 simplemagic-0.1.9/simplemagic.egg-info/entry_points.txt
+-rw-r--r--   0 test       (501) staff       (20)       39 2022-06-13 07:42:00.000000 simplemagic-0.1.9/simplemagic.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       12 2022-06-13 07:42:00.000000 simplemagic-0.1.9/simplemagic.egg-info/top_level.txt
```

### Comparing `simplemagic-0.1.8/LICENSE` & `simplemagic-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simplemagic-0.1.8/PKG-INFO` & `simplemagic-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: simplemagic
-Version: 0.1.8
-Summary: Simple file magic. We try to get file's mimetype using 'file-magic', 'command file' and 'puremagic'. On linux we need system package 'file-libs' which mostly already installed. On MacOS we need system package 'libimage' which can be installed by 'brew install libmagic'. On windows we need file command which can be install by 'pacman -S file' within msys2. If system package missing, we try to get the file's mimetype using 'puremagic' which is write in pure python without any extra depends.
-Author: zencore
-Author-email: dobetter@zencore.cn
-License: MIT
-Keywords: libmagic,file-magic,file
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # simplemagic
 
 Simple file magic. We try to get file's mimetype using 'file-magic', 'command file' and 'puremagic'. On linux we need system package 'file-libs' which mostly already installed. On MacOS we need system package 'libimage' which can be installed by 'brew install libmagic'. On windows we need file command which can be install by 'pacman -S file' within msys2. If system package missing, we try to get the file's mimetype using 'puremagic' which is write in pure python without any extra depends.
 
 ## Install
 
 ```
@@ -295,7 +279,13 @@
 - Add magic_content_length parameter in function is_file_content_matches_with_file_extension to control the stream content read length locally.
 - Fix export api name problem.
 
 ### v0.1.8
 
 - Add lax_extensions parameter in function is_file_content_matches_with_file_extension to support lax extension compares, especially for user missing .jpg, .png extension for images.
 - Add LAX_IMAGE_EXTENSIONS = [".png", ".jpg", ".jpe", ".jpeg", ".gif", ".bmp", ".tif", ".tiff", ".webp", ".ico"].
+
+### v0.1.9
+
+- Remove .svg from text/plain, for both libmagic and puremagic are not treat .svg file as text/plain. libmagic treat it as image/svg+xml, and puremagic treat it as application/xml. If put .svg in candidate extensions of text/plain, in image lex compares model, will allow user upload plain text script in image file field.
+
+
```

### Comparing `simplemagic-0.1.8/README.md` & `simplemagic-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: simplemagic
+Version: 0.1.9
+Summary: Simple file magic. We try to get file's mimetype using 'file-magic', 'command file' and 'puremagic'. On linux we need system package 'file-libs' which mostly already installed. On MacOS we need system package 'libimage' which can be installed by 'brew install libmagic'. On windows we need file command which can be install by 'pacman -S file' within msys2. If system package missing, we try to get the file's mimetype using 'puremagic' which is write in pure python without any extra depends.
+Author: zencore
+Author-email: dobetter@zencore.cn
+License: MIT
+Keywords: libmagic,file-magic,file
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # simplemagic
 
 Simple file magic. We try to get file's mimetype using 'file-magic', 'command file' and 'puremagic'. On linux we need system package 'file-libs' which mostly already installed. On MacOS we need system package 'libimage' which can be installed by 'brew install libmagic'. On windows we need file command which can be install by 'pacman -S file' within msys2. If system package missing, we try to get the file's mimetype using 'puremagic' which is write in pure python without any extra depends.
 
 ## Install
 
 ```
@@ -279,7 +295,13 @@
 - Add magic_content_length parameter in function is_file_content_matches_with_file_extension to control the stream content read length locally.
 - Fix export api name problem.
 
 ### v0.1.8
 
 - Add lax_extensions parameter in function is_file_content_matches_with_file_extension to support lax extension compares, especially for user missing .jpg, .png extension for images.
 - Add LAX_IMAGE_EXTENSIONS = [".png", ".jpg", ".jpe", ".jpeg", ".gif", ".bmp", ".tif", ".tiff", ".webp", ".ico"].
+
+### v0.1.9
+
+- Remove .svg from text/plain, for both libmagic and puremagic are not treat .svg file as text/plain. libmagic treat it as image/svg+xml, and puremagic treat it as application/xml. If put .svg in candidate extensions of text/plain, in image lex compares model, will allow user upload plain text script in image file field.
+
+
```

### Comparing `simplemagic-0.1.8/setup.py` & `simplemagic-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, 'requirements.txt'), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="simplemagic",
-    version="0.1.8",
+    version="0.1.9",
     description="Simple file magic. We try to get file's mimetype using 'file-magic', 'command file' and 'puremagic'. On linux we need system package 'file-libs' which mostly already installed. On MacOS we need system package 'libimage' which can be installed by 'brew install libmagic'. On windows we need file command which can be install by 'pacman -S file' within msys2. If system package missing, we try to get the file's mimetype using 'puremagic' which is write in pure python without any extra depends.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
```

### Comparing `simplemagic-0.1.8/simplemagic/__init__.py` & `simplemagic-0.1.9/simplemagic/__init__.py`

 * *Files identical despite different names*

### Comparing `simplemagic-0.1.8/simplemagic/cli.py` & `simplemagic-0.1.9/simplemagic/cli.py`

 * *Files identical despite different names*

### Comparing `simplemagic-0.1.8/simplemagic/extra_mimetypes.py` & `simplemagic-0.1.9/simplemagic/extra_mimetypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,14 @@
         ".in",
         ".bashrc",
         ".bash_profile",
         ".bash_history",
         ".csv",
         ".reg",
         ".inf",
-        ".svg",
         ".less",
         ".scss",
         ".ftl",
         ".xsd",
         ".htaccess",
     ],
     # 'application/vnd.binary' equivalent to 'application/octet-stream'
```

### Comparing `simplemagic-0.1.8/simplemagic/fixpuremagic.py` & `simplemagic-0.1.9/simplemagic/fixpuremagic.py`

 * *Files identical despite different names*

### Comparing `simplemagic-0.1.8/simplemagic/magic.py` & `simplemagic-0.1.9/simplemagic/magic.py`

 * *Files identical despite different names*

### Comparing `simplemagic-0.1.8/simplemagic.egg-info/PKG-INFO` & `simplemagic-0.1.9/simplemagic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplemagic
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple file magic. We try to get file's mimetype using 'file-magic', 'command file' and 'puremagic'. On linux we need system package 'file-libs' which mostly already installed. On MacOS we need system package 'libimage' which can be installed by 'brew install libmagic'. On windows we need file command which can be install by 'pacman -S file' within msys2. If system package missing, we try to get the file's mimetype using 'puremagic' which is write in pure python without any extra depends.
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: libmagic,file-magic,file
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -295,7 +295,13 @@
 - Add magic_content_length parameter in function is_file_content_matches_with_file_extension to control the stream content read length locally.
 - Fix export api name problem.
 
 ### v0.1.8
 
 - Add lax_extensions parameter in function is_file_content_matches_with_file_extension to support lax extension compares, especially for user missing .jpg, .png extension for images.
 - Add LAX_IMAGE_EXTENSIONS = [".png", ".jpg", ".jpe", ".jpeg", ".gif", ".bmp", ".tif", ".tiff", ".webp", ".ico"].
+
+### v0.1.9
+
+- Remove .svg from text/plain, for both libmagic and puremagic are not treat .svg file as text/plain. libmagic treat it as image/svg+xml, and puremagic treat it as application/xml. If put .svg in candidate extensions of text/plain, in image lex compares model, will allow user upload plain text script in image file field.
+
+
```


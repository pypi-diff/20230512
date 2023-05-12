# Comparing `tmp/cartson-2.3.5b9.dev0-py3-none-any.whl.zip` & `tmp/cartson-3.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 39503 bytes, number of entries: 17
+Zip file size: 39210 bytes, number of entries: 17
 -rw-r--r--  2.0 unx     1079 b- defN 23-May-10 21:33 carson/LICENSE
--rw-r--r--  2.0 unx    10278 b- defN 23-May-12 21:11 carson/__init__.py
+-rw-r--r--  2.0 unx     9896 b- defN 23-May-12 19:41 carson/__init__.py
 -rw-r--r--  2.0 unx     5022 b- defN 23-May-10 21:33 carson/__main__.py
 -rw-r--r--  2.0 unx     6804 b- defN 23-May-10 21:33 carson/auth.py
 -rw-r--r--  2.0 unx     4296 b- defN 23-May-10 21:33 carson/config.py
 -rw-r--r--  2.0 unx    30044 b- defN 23-May-10 21:33 carson/core.py
 -rw-r--r--  2.0 unx    13502 b- defN 23-May-10 21:33 carson/endpoints.py
 -rw-r--r--  2.0 unx     5028 b- defN 23-May-10 21:33 carson/logging.py
 -rw-r--r--  2.0 unx    18665 b- defN 23-May-10 21:33 carson/stream.py
 -rw-r--r--  2.0 unx     1215 b- defN 23-May-10 21:33 carson/utils.py
 -rw-r--r--  2.0 unx      488 b- defN 23-May-10 21:33 carson/plat/Windows.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 21:33 carson/plat/__init__.py
--rw-r--r--  2.0 unx     8190 b- defN 23-May-12 20:50 carson/version/__init__.py
--rw-r--r--  2.0 unx    13763 b- defN 23-May-12 21:13 cartson-2.3.5b9.dev0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 21:13 cartson-2.3.5b9.dev0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-12 21:13 cartson-2.3.5b9.dev0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1299 b- defN 23-May-12 21:13 cartson-2.3.5b9.dev0.dist-info/RECORD
-17 files, 119772 bytes uncompressed, 37413 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx     8190 b- defN 23-May-12 20:03 carson/version/__init__.py
+-rw-r--r--  2.0 unx    13633 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1270 b- defN 23-May-12 20:38 cartson-3.3.3.dist-info/RECORD
+17 files, 119231 bytes uncompressed, 37176 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: carson/plat/__init__.py
 Comment: 
 
 Filename: carson/version/__init__.py
 Comment: 
 
-Filename: cartson-2.3.5b9.dev0.dist-info/METADATA
+Filename: cartson-3.3.3.dist-info/METADATA
 Comment: 
 
-Filename: cartson-2.3.5b9.dev0.dist-info/WHEEL
+Filename: cartson-3.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: cartson-2.3.5b9.dev0.dist-info/top_level.txt
+Filename: cartson-3.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cartson-2.3.5b9.dev0.dist-info/RECORD
+Filename: cartson-3.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carson/__init__.py

```diff
@@ -13,20 +13,17 @@
 __license__ = 'MIT'
 __url__ = 'https://github.com/mloyd/carson'
 __author__ = 'Michael Loyd'
 __author_email__ = 'michael@loyd.org'
 __copyright__ = "Copyright 2021 %s" % __author__
 
 try:
-    _dist = distribution(__package__)         # Could raise PackageNotFoundError
-    _summary = _dist.metadata['Summary']      # Could return None if not build with a summary
-    _version = _summary.split(' ', 1)[0]      # 'Version=1.2.3+b8-1a146aa  Description=An asynci...'
-    __version__ = _version.split('=', 1)[-1]  # 'Version=1.2.3+b8-1a146aa
-except (PackageNotFoundError, AttributeError):
-    # AttributeError is if metadata was build without a description (a.k.a. Summary is missing)
+    _dist = distribution(__package__)
+    __version__ = _dist.metadata['Version']
+except PackageNotFoundError:
     __version__ += '-unsupported'
 
 try:
     # To deal with an annoying event loop implementation differences.  That's right, Windows, I'm
     # looking right at you buddy.
     import platform, importlib
     importlib.import_module(f'.plat.{platform.system()}', package=__package__)
```

## Comparing `cartson-2.3.5b9.dev0.dist-info/METADATA` & `cartson-3.3.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 Metadata-Version: 2.1
 Name: cartson
-Version: 2.3.5b9.dev0
-Summary: Version=2.3.5+b9-a3fbac7-unsupported  Description=An asyncio package to interact with the Tesla JSON web service.
+Version: 3.3.3
 Author-email: Michael Loyd <michael@loyd.org>
 License: MIT
 Project-URL: url, https://github.com/mloyd/carson
 Keywords: tesla,asyncio,json
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```


# Comparing `tmp/dknovautils-0.1.4.tar.gz` & `tmp/dknovautils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.1.4.tar", last modified: Wed May 10 07:22:01 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.1.5.tar", last modified: Fri May 12 06:46:19 2023, max compression
```

## Comparing `dknovautils-0.1.4.tar` & `dknovautils-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-10 07:22:01.000000 dknovautils-0.1.4/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2448 2023-05-10 03:57:08.000000 dknovautils-0.1.4/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8644 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.4/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1153 2023-05-07 16:31:40.000000 dknovautils-0.1.4/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      501 2023-05-07 13:41:47.000000 dknovautils-0.1.4/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.4/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.4/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.4/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-10 07:22:01.000000 dknovautils-0.1.4/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.4/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-10 07:22:01.000000 dknovautils-0.1.4/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.4/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-10 07:22:01.000000 dknovautils-0.1.4/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1159 2023-05-10 07:22:01.000000 dknovautils-0.1.4/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-12 06:46:19.000000 dknovautils-0.1.5/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2523 2023-05-12 05:07:32.000000 dknovautils-0.1.5/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8651 2023-05-12 06:46:18.000000 dknovautils-0.1.5/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.5/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1153 2023-05-07 16:31:40.000000 dknovautils-0.1.5/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-12 06:46:18.000000 dknovautils-0.1.5/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      501 2023-05-07 13:41:47.000000 dknovautils-0.1.5/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.5/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.5/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.5/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        6 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-12 06:46:19.000000 dknovautils-0.1.5/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.5/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-12 06:46:19.000000 dknovautils-0.1.5/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.5/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-12 06:46:19.000000 dknovautils-0.1.5/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1159 2023-05-12 06:46:18.000000 dknovautils-0.1.5/setup.py
```

### Comparing `dknovautils-0.1.4/dknovautils/commons.py` & `dknovautils-0.1.5/dknovautils/commons.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,19 @@
     pass
 
 
 def dtprint(s: str):
     iprint(s)
 
 
-def iprint(obj):
-    iprint_debug(obj)
+def iprint(obj, level=LLevel.Debug):
+    _iprint(obj, level=level)
+
+# def iprint(obj):
+#     iprint_debug(obj)
 
 
 def iprint_trace(obj):
     _iprint(obj, level=LLevel.Trace)
 
 
 def iprint_debug(obj):
```

### Comparing `dknovautils-0.1.4/dknovautils/dkat.py` & `dknovautils-0.1.5/dknovautils/dkat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 
 import dknovautils
 from dknovautils.commons import *
 
-import beepy
 
-
-DkAppVer = '0.1.4'
+DkAppVer = '0.1.5'
 
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
@@ -82,15 +80,15 @@
     
     dtstr = datetime.now().strftime("%Y%m%dT%H%M%S")
 
         
     '''
 
     @classmethod
-    def log_basicConfig(cls, filename='tmp_test.log', loggerName='dkn', level=logging.DEBUG, initInnerLoggerFun=True):
+    def log_basicConfig(cls, filename=None, loggerName='dkn', level=logging.DEBUG, initInnerLoggerFun=True):
         '''
         这个 dkn logger的设置好像不太好。
         暂时不用这个
 
         '''
 
         # AT.unsupported()
@@ -146,24 +144,26 @@
             return
         else:
             AT.__beep_last_time = now
             AT.beep(tone)
 
     @staticmethod
     def beep(tone='ping'):
-        beepy.beep(sound=tone)
+        if False:
+            import beepy
+            beepy.beep(sound=tone)
 
     @staticmethod
     def beep2():
         #!wget -q -T 1 http://localhost:333/hello
         print('\7')
 
     @staticmethod
     def vassert_(b: bool, s: str = None):
-        AT.assert_(b, s)        
+        AT.assert_(b, s)
 
     @classmethod
     def never(cls, s=None):
         AT.assert_(False,  s if s is not None else 'should never come here')
 
     @staticmethod
     def checksys():
@@ -315,15 +315,15 @@
     # def f_matploglib_logger():
     #     logger = logging.getLogger('matplotlib.font_manager')
     #     logger.setLevel(level=logging.INFO)
 
     @staticmethod
     def log_conf_matploglib_logger(level=logging.INFO):
         logger = logging.getLogger('matplotlib.font_manager')
-        logger.setLevel(level=level)        
+        logger.setLevel(level=level)
 
     VERSION = DkAppVer
 
 
 class DkAstException(Exception):
     pass
```

### Comparing `dknovautils-0.1.4/dknovautils/dkipy.py` & `dknovautils-0.1.5/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.4/dknovautils/dk_imports.py` & `dknovautils-0.1.5/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.4/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.5/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.4/PKG-INFO` & `dknovautils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.4/setup.py` & `dknovautils-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.1.4'
+DkAppVer = '0.1.5'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```


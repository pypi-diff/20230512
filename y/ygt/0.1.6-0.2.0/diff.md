# Comparing `tmp/ygt-0.1.6.tar.gz` & `tmp/ygt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.1.6.tar", last modified: Fri Apr 28 22:29:48 2023, max compression
+gzip compressed data, was "ygt-0.2.0.tar", last modified: Thu May 11 21:53:40 2023, max compression
```

## Comparing `ygt-0.1.6.tar` & `ygt-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.421758 ygt-0.1.6/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.6/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.6/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     3734 2023-04-28 22:29:48.421633 ygt-0.1.6/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     3338 2023-04-28 20:30:43.000000 ygt-0.1.6/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-28 22:27:57.000000 ygt-0.1.6/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-28 22:29:48.421793 ygt-0.1.6/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.6/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.406686 ygt-0.1.6/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.413190 ygt-0.1.6/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.6/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.6/src/ygt/autohint_trash.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.6/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5234 2023-04-25 12:51:05.000000 ygt-0.1.6/src/ygt/fontViewDialog.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.414149 ygt-0.1.6/src/ygt/fonts/
--rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.6/src/ygt/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 peterbaker   (504) staff       (20)    12952 2023-04-26 00:07:28.000000 ygt-0.1.6/src/ygt/freetypeFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.421360 ygt-0.1.6/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.6/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.6/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.6/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.6/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.6/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.6/src/ygt/icons/stem_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.6/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.6/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.6/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    56264 2023-04-21 04:37:29.000000 ygt-0.1.6/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    65557 2023-04-28 10:05:58.000000 ygt-0.1.6/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.6/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   121428 2023-04-28 11:52:09.000000 ygt-0.1.6/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   141294 2023-04-28 12:16:44.000000 ygt-0.1.6/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.6/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    22566 2023-04-28 18:49:42.000000 ygt-0.1.6/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    10040 2023-04-21 04:31:07.000000 ygt-0.1.6/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5674 2023-04-22 03:26:07.000000 ygt-0.1.6/src/ygt/ygStems.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.6/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.414038 ygt-0.1.6/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     3734 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.6/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.559806 ygt-0.2.0/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.2.0/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.2.0/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4156 2023-05-11 21:53:40.559655 ygt-0.2.0/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3760 2023-05-10 10:57:33.000000 ygt-0.2.0/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-05-07 10:38:16.000000 ygt-0.2.0/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-05-11 21:53:40.559841 ygt-0.2.0/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.2.0/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.543127 ygt-0.2.0/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.543974 ygt-0.2.0/src/hooks/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)      103 2023-05-04 12:22:22.000000 ygt-0.2.0/src/hooks/hook-freetype.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)      143 2023-05-07 08:59:05.000000 ygt-0.2.0/src/hooks/hook-xgridfit.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.551104 ygt-0.2.0/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.2.0/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.2.0/src/ygt/autohint_trash.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3721 2023-05-04 10:24:55.000000 ygt-0.2.0/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6108 2023-05-06 09:50:32.000000 ygt-0.2.0/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.551979 ygt-0.2.0/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.2.0/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    14419 2023-05-04 19:50:13.000000 ygt-0.2.0/src/ygt/freetypeFont.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)      492 2023-05-02 11:52:02.000000 ygt-0.2.0/src/ygt/harfbuzzFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.559333 ygt-0.2.0/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.2.0/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.2.0/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.2.0/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.2.0/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.2.0/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.2.0/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.2.0/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.2.0/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.2.0/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6030 2023-05-03 03:10:09.000000 ygt-0.2.0/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    61400 2023-05-11 11:19:08.000000 ygt-0.2.0/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    69578 2023-05-11 12:12:33.000000 ygt-0.2.0/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.2.0/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   118711 2023-05-07 08:05:34.000000 ygt-0.2.0/src/ygt/ygHintEditor.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   141199 2023-05-07 11:23:51.000000 ygt-0.2.0/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     9038 2023-05-11 15:28:45.000000 ygt-0.2.0/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24210 2023-05-05 23:01:15.000000 ygt-0.2.0/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10146 2023-05-11 03:15:43.000000 ygt-0.2.0/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5652 2023-05-02 21:03:38.000000 ygt-0.2.0/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.2.0/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:53:40.551875 ygt-0.2.0/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4156 2023-05-11 21:53:40.000000 ygt-0.2.0/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1335 2023-05-11 21:53:40.000000 ygt-0.2.0/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-05-11 21:53:40.000000 ygt-0.2.0/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-05-11 21:53:40.000000 ygt-0.2.0/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-05-11 21:53:40.000000 ygt-0.2.0/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       27 2023-05-11 21:53:40.000000 ygt-0.2.0/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       54 2023-05-06 10:50:11.000000 ygt-0.2.0/src/ygt.py
```

### Comparing `ygt-0.1.6/LICENSE` & `ygt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/PKG-INFO` & `ygt-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.6
+Version: 0.2.0
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,25 +26,39 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
+### Verasion 0.2.0
+
+Enabled merge (Ygt can add its hints to existing hints).
+
+Added files supporting creation of executables.
+
+Changed shortcuts: Ctrl-P = Hint Preview; Ctrl-L: Set Resolution.
+
+Fixed a bug that left some untouched points with "touched" flags.
+
+Can override light or dark theme for the Preview panels.
+
+Various bug fixes, efficiencies, and other improvements in the code.
+
 ### Version 0.1.6 (2023-4-28)
 
 Select more than one untouched point when adding shift, align, or interpolate hints to create a hint with a set as target. This formerly had to be done with a separate “Make Set” command.
 
 “Make Set” command has been removed as unnecessary.
 
 To add a point to a shift, align, or interpolate hint, select the hint and at least one untouched point, and press the **plus** key.
 
 To delete a point or points from a shift, align, or interpolate hint, select one ore more points belonging to the hint and press the **hyphen** or **minus** key.
 
-Corrected background color of preview panels when dark theme is active.
+Corrected background color of preview panels when dark theme is active. New color scheme for dark theme.
 
 ### Version 0.1.5 (2023-4-25)
 
 Various UI refinements: initial scaling of glyphs, spacebar to temporarily switch to panning mode, and more.
 
 User now confronts only one kind of stem hint: Ygt guesses (more or less accurately) the distance type.
```

### Comparing `ygt-0.1.6/README.md` & `ygt-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,39 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
+### Verasion 0.2.0
+
+Enabled merge (Ygt can add its hints to existing hints).
+
+Added files supporting creation of executables.
+
+Changed shortcuts: Ctrl-P = Hint Preview; Ctrl-L: Set Resolution.
+
+Fixed a bug that left some untouched points with "touched" flags.
+
+Can override light or dark theme for the Preview panels.
+
+Various bug fixes, efficiencies, and other improvements in the code.
+
 ### Version 0.1.6 (2023-4-28)
 
 Select more than one untouched point when adding shift, align, or interpolate hints to create a hint with a set as target. This formerly had to be done with a separate “Make Set” command.
 
 “Make Set” command has been removed as unnecessary.
 
 To add a point to a shift, align, or interpolate hint, select the hint and at least one untouched point, and press the **plus** key.
 
 To delete a point or points from a shift, align, or interpolate hint, select one ore more points belonging to the hint and press the **hyphen** or **minus** key.
 
-Corrected background color of preview panels when dark theme is active.
+Corrected background color of preview panels when dark theme is active. New color scheme for dark theme.
 
 ### Version 0.1.5 (2023-4-25)
 
 Various UI refinements: initial scaling of glyphs, spacebar to temporarily switch to panning mode, and more.
 
 User now confronts only one kind of stem hint: Ygt guesses (more or less accurately) the distance type.
```

### Comparing `ygt-0.1.6/pyproject.toml` & `ygt-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ygt"
-version = "0.1.6"
+version = "0.2.0"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "A graphical hint editor for TrueType fonts"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
```

### Comparing `ygt-0.1.6/src/ygt/autohint_trash.py` & `ygt-0.2.0/src/ygt/autohint_trash.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/cvGuesser.py` & `ygt-0.2.0/src/ygt/cvGuesser.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def refresh(self) -> None:
         self.delete_all_vars()
         d = self.get_all_variant_cvs()
         self.add_variants_to_cvt(d)
 
     def delete_all_vars(self) -> None:
-        k = self.cvt.keys()
+        k = self.cvt.keys
         for kk in k:
             cv = self.cvt.get_cv(kk)
             try:
                 # if there's no "origin" in the cv, we can't replace the vars.
                 if "origin" in cv:
                     del cv["var"]
             except Exception:
@@ -36,24 +36,24 @@
     def make_instance(self, vals: dict) -> None:
         self.current_instance = instancer.instantiateVariableFont(self.ft_font, vals)
 
     def get_all_variant_cvs(self) -> dict:
         # We end up with a dict:
         # {master_id: {cv_name: val, ...}, ...}
         result = {}
-        k = self.masters.keys()
+        k = self.masters.keys
         for kk in k:
             c = self.get_cvs_for_master(kk)
             if len(c) > 0:
                 result[kk] = c
         return result
 
     def add_variants_to_cvt(self, d: dict) -> None:
         # d is a dict in the format produced by get_all_variant_cvs.
-        ck = self.cvt.keys()
+        ck = self.cvt.keys
         dk = d.keys()
         for ckk in ck:  # iterate through CVs.
             for dkk in dk:  # iterate through masters
                 if ckk in d[dkk]:  # if the master has an entry for the current CV,
                     cv = self.cvt.get_cv(ckk)  # create a "var" entry in the CV.
                     if not "var" in cv:
                         cv["var"] = {}
@@ -64,15 +64,15 @@
         # "origin" field. Get the list of y values (function below) and
         # use those to figure out the value of the cv for this glyph.
         # Compare the new position with that of the default cv.
         # If different, store. If the same, discard.
         result = {}
         coords = self.masters.get_master_coords(master_id)
         self.make_instance(coords)
-        k = self.cvt.keys()
+        k = self.cvt.keys
         for kk in k:
             cv = self.cvt.get_cv(kk)
             if type(cv) is dict and "origin" in cv:
                 if cv["type"] == "pos":
                     glyph_name = cv["origin"]["glyph"]
                     ptnum = cv["origin"]["ptnum"]
                     y_pos = self.y_list(glyph_name)[ptnum[0]]
```

### Comparing `ygt-0.1.6/src/ygt/fontViewDialog.py` & `ygt-0.2.0/src/ygt/fontViewDialog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .freetypeFont import freetypeFont, RENDER_GRAYSCALE
 from fontTools import subset
 from .ygModel import ygFont
 from math import ceil
 from PyQt6.QtCore import Qt, QRect, pyqtSignal
-from PyQt6.QtWidgets import QWidget, QDialog, QGridLayout, QVBoxLayout, QScrollArea
-from PyQt6.QtGui import QPainter, QBrush, QPen, QColor, QPalette
+from PyQt6.QtWidgets import QWidget, QDialog, QGridLayout, QVBoxLayout, QScrollArea, QLabel
+from PyQt6.QtGui import QPainter, QBrush, QPen, QColor, QPalette, QPixmap
 import numpy
 from tempfile import SpooledTemporaryFile
 import copy
 
 
 # A window (not a dialog, despite the filename, retained to avoid complicating
 # the history in the repository) that displays all the non-composite glyphs
@@ -19,15 +19,14 @@
 class fontViewWindow(QWidget):
     """This window presents a grid showing all the glyphs in glyph_list--
     that is, those glyphs that are not made of composites. This display
     indicates which characters are hinted (their cells have blue backgrounds).
     It also works as a navigation aid: just click on any character.
 
     """
-
     sig_switch_to_glyph = pyqtSignal(object)
 
     def __init__(
             self, filename: str, yg_font: ygFont, glyph_list: list, top_window
         ) -> None:
         super().__init__()
         self.valid = True
@@ -51,14 +50,15 @@
             tf.seek(0)
             self.face = freetypeFont(tf, size=24, render_mode=RENDER_GRAYSCALE)
             tf.close()
         if not self.face.valid:
             self.valid = False
             return
         self.glyph_list = glyph_list
+        self.glyph_index = {}
 
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
         bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
         self.dark_theme = text_hsv_value > bg_hsv_value
 
         self._layout = QVBoxLayout()
         self.setLayout(self._layout)
@@ -67,79 +67,105 @@
         scroll_area.setWidget(fvp)
         self._layout.addWidget(scroll_area)
 
         self.sig_switch_to_glyph.connect(
             self.top_window.glyph_pane.switch_from_font_viewer
         )
 
+    def update_cell(self, g):
+        gc = self.glyph_index[g]
+        # print("via update_cell " + str(id(gc)))
+        gc.make_pixmap()
+        gc.update()
+
     def clicked_glyph(self, g: str) -> None:
         self.sig_switch_to_glyph.emit(g)
 
 
 class fontViewPanel(QWidget):
     def __init__(self, dialog: fontViewWindow) -> None:
         super().__init__()
+        self.dialog = dialog
         gl = dialog.glyph_list
         numchars = len(gl)
         cols = 10
         rows = ceil(numchars / 10)
         self.setMinimumSize(cols * 36, rows * 36)
         self._layout = QGridLayout()
         self._layout.setHorizontalSpacing(0)
         self._layout.setVerticalSpacing(0)
         self.setContentsMargins(0, 0, 0, 0)
         self.setLayout(self._layout)
         row = 0
         col = 0
         self._layout.setRowMinimumHeight(row, 36)
         for g in gl:
-            self._layout.addWidget(fontViewCell(dialog, g), row, col)
+            fvc = fontViewCell(dialog, g)
+            self._layout.addWidget(fvc, row, col)
+            self.dialog.glyph_index[g[1]] = fvc
             col += 1
             if col == 10:
                 row += 1
                 self._layout.setRowMinimumHeight(row, 36)
                 col = 0
         if dialog.dark_theme:
             self.setStyleSheet("background-color: black;")
         else:
             self.setStyleSheet("background-color: white;")
 
 
-class fontViewCell(QWidget):
+class fontViewCell(QLabel):
     def __init__(self, dialog: fontViewWindow, glyph: list) -> None:
         super().__init__()
         self.dialog = dialog
         self.glyph = glyph[1]
         self.setFixedSize(36, 36)
+        self.has_hints = False
+        self.pixmap = None
+        self.make_pixmap()
+
+    def make_pixmap(self) -> None:
+        """ Make a pixmap for this cell and draw the glyph on it.
+            This makes for rapid painting and fast scrolling. If there's
+            a change, simply repaint the pixmap and call update() on the
+            cell.
+        """
+        # Test to see if we really need to paint the pixmap.
+        has_hints_now = self.dialog.yg_font.has_hints(self.glyph)
+        if self.pixmap != None and self.has_hints == has_hints_now:
+            return
+        else:
+            self.has_hints = has_hints_now
 
-    def paintEvent(self, event) -> None:
-        painter = QPainter(self)
-
-        dark_theme = self.dialog.dark_theme
+        if self.pixmap == None:
+            self.pixmap = QPixmap(36,36)
 
-        brush = QBrush()
-        if self.dialog.yg_font.has_hints(self.glyph):
-            if dark_theme:
-                brush.setColor(QColor(0, 0, 186, 128))
+        if self.dialog.dark_theme:
+            if self.has_hints:
+                self.pixmap.fill(QColor(0, 0, 186, 128))
             else:
-                brush.setColor(QColor(186, 255, 255, 128))
+                self.pixmap.fill(QColor("black"))
         else:
-            if dark_theme:
-                brush.setColor(QColor("black"))
+            if self.has_hints:
+                self.pixmap.fill(QColor(186, 255, 255, 128))
             else:
-                brush.setColor(QColor("white"))
-        brush.setStyle(Qt.BrushStyle.SolidPattern)
-        rect = QRect(0, 0, self.width(), self.height())
-        painter.fillRect(rect, brush)
+                self.pixmap.fill(QColor("white"))
+
+        painter = QPainter(self.pixmap)
 
         ind = self.dialog.face.name_to_index(self.glyph)
         self.dialog.face.set_char(ind)
         baseline = (
             round((36 - self.dialog.face.face_height) / 2) + self.dialog.face.ascender
         )
         xpos = round((36 - self.dialog.face.advance) / 2)
-        self.dialog.face.draw_char(painter, xpos, baseline, dark_theme = dark_theme)
+        self.dialog.face.draw_char(
+            painter, xpos, baseline, dark_theme = self.dialog.dark_theme
+        )
 
         painter.end()
 
+        self.setPixmap(self.pixmap)
+
     def mousePressEvent(self, event) -> None:
+        # print("Thie is " + str(id(self)))
         self.dialog.clicked_glyph(self.glyph)
```

### Comparing `ygt-0.1.6/src/ygt/fonts/SourceCodePro-Regular.ttf` & `ygt-0.2.0/src/ygt/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/freetypeFont.py` & `ygt-0.2.0/src/ygt/freetypeFont.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# from functools import lru_cache
 from typing import Optional
 import freetype as ft # type: ignore
 import numpy
 import copy
 from tempfile import SpooledTemporaryFile
 from PyQt6.QtGui import QColor, QPen
 from PyQt6.QtCore import QRect, QLine
+import uharfbuzz as uhb
 
 
 RENDER_GRAYSCALE = 1
 RENDER_LCD_1 = 2
 RENDER_LCD_2 = 3
 
 
@@ -55,18 +57,43 @@
         instance: str = None
     ) -> None:
         self.valid = True
         try:
             if type(font) is SpooledTemporaryFile:
                 font.seek(0)
                 self.face = ft.Face(font)
+                # Experimental code, for harfbuzz.
+                # Here's what we're going to have to do.
+                #    1. Load the whole font into Harfbuzz (shall we do this just once for
+                #       the session?)
+                #    2. Display features, let user choose.
+                #    3. Let hb.shape get us a new string
+                #    4. Get glyph names.
+                #    5. Send list of names to Xgridfit, get back list of indices.
+                #    6. Draw the glyphs.
+                #font.seek(0)
+                #font_data = font.read()
+                #hb_face = uhb.Face(font_data)
+                #hb_font = uhb.Font(hb_face)
+                #buf = uhb.Buffer()
+                #buf.add_str("first flat office")
+                #buf.guess_segment_properties()
+                #features = {"kern": True, "liga": True}
+                #uhb.shape(hb_font, buf, features)
+                #print(uhb._harfbuzz.ot_layout_language_get_feature_tags(hb_face, "GSUB"))
+                # End of harfbuzz experiment.
                 font.close()
+                #import uharfbuzz as hb
+                #test = hb.Blob(self.face)
+                #print(test)
             else:
                 self.face = ft.Face(font)
-        except Exception:
+        except Exception as e:
+            print(e.args)
+            print(e)
             self.valid = False
             return
         self.char_size = size * 64
         self.size = 30
         self.ascender = 0
         self.descender = 0
         self.face_height = 0
@@ -153,18 +180,14 @@
         """
         self.glyph_index = glyph_index
         flags = 4  # i.e. grayscale
         if self.render_mode in [RENDER_LCD_1, RENDER_LCD_2]:
             flags = ft.FT_LOAD_RENDER | ft.FT_LOAD_TARGET_LCD
         if not self.hinting_on:
             flags = flags | ft.FT_LOAD_NO_HINTING | ft.FT_LOAD_NO_AUTOHINT
-        # For some UFOs, font view is hanging here (with load_glyph). It doesn't
-        # hang except with
-        # UFOs, and it generates the preview well from the same in-memory TTFont.
-        # So what are we doing differently when generating the font view?
         self.face.load_glyph(self.glyph_index, flags=flags)
         self.glyph_slot = self.face.glyph
         self.advance = round(self.glyph_slot.advance.x / 64)
         self.bitmap_top = self.glyph_slot.bitmap_top
         self.bitmap_left = self.glyph_slot.bitmap_left
         self.top_offset = self.ascender - self.bitmap_top
 
@@ -187,14 +210,21 @@
         for i in range(rows):
             data.extend(self.glyph_slot.bitmap.buffer[i * pitch : i * pitch + width])
         if render_mode == RENDER_GRAYSCALE:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, width)
         else:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, int(width / 3), 3)
 
+    #@lru_cache(maxsize = 2048)
+    #def _get_lcd_color(self, rgb, dark_theme):
+    #    if dark_theme:
+    #        return QColor(rgb[0], rgb[1], rgb[2])
+    #    return QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
+
+
     def _draw_char_lcd(
             self,
             painter,
             x,
             y,
             spacing_mark = False,
             dark_theme = False,
@@ -231,14 +261,17 @@
         qp.setWidth(1)
         for row in Z:
             xpos = starting_xpos
             for col in row:
                 rgb = []
                 for elem in col:
                     rgb.append(elem)
+                # The cached function doesn't help at all (timer produces about the same result).
+                # Look for other possibilities for optimization.
+                #qc = self._get_lcd_color(tuple(rgb), dark_theme)
                 if dark_theme:
                     qc = QColor(rgb[0], rgb[1], rgb[2])
                 else:
                     qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
                 if qc != white_color:
                     qp.setColor(qc)
                     painter.setPen(qp)
```

### Comparing `ygt-0.1.6/src/ygt/icons/align.png` & `ygt-0.2.0/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/anchor.png` & `ygt-0.2.0/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/black_distance.png` & `ygt-0.2.0/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/cursor-icon-off.png` & `ygt-0.2.0/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/cursor-icon-on.png` & `ygt-0.2.0/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/cv.png` & `ygt-0.2.0/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/cv_guess.png` & `ygt-0.2.0/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/gray_distance.png` & `ygt-0.2.0/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/hand-icon-off.png` & `ygt-0.2.0/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/hand-icon-on.png` & `ygt-0.2.0/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/horizontal-off.png` & `ygt-0.2.0/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/horizontal-on.png` & `ygt-0.2.0/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/interpolate.png` & `ygt-0.2.0/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/make_set.png` & `ygt-0.2.0/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/program.png` & `ygt-0.2.0/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/shift.png` & `ygt-0.2.0/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/stem_distance.png` & `ygt-0.2.0/src/ygt/icons/stem_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/vertical-off.png` & `ygt-0.2.0/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/vertical-on.png` & `ygt-0.2.0/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/icons/white_distance.png` & `ygt-0.2.0/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/macfuncDialog.py` & `ygt-0.2.0/src/ygt/macfuncDialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if self.yg_callable == None:
             try:
                 self.yg_callable = self.yg_font.macros[self.yg_hint.name]
             except Exception as e:
                 # print("in function dialog:")
                 # print("Error: " + str(e))
                 pass
-        self.hint_type = _hint.yg_hint.hint_type()
+        self.hint_type = _hint.yg_hint.hint_type
         self._layout = QVBoxLayout()
         QBtn = (
             QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
         )
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
@@ -98,42 +98,42 @@
                     pass
         for w in self.widgets:
             self._layout.addLayout(w)
         self._layout.addWidget(self.buttonBox)
         self.setLayout(self._layout)
 
     def accept(self) -> None:
-        self.result_dict = {"nm": self.yg_hint.macfunc_name()}
+        self.result_dict = {"nm": self.yg_hint.macfunc_name}
         for w in self.widgets:
             if w.itemAt(1).widget().text() != "None": # type: ignore
                 self.result_dict[w.itemAt(0).widget().text()] = ( # type: ignore
                     w.itemAt(1).widget().text() # type: ignore
                 )
         # So param_list is the answer from this dialog. Don't plug it into the
         # hint here, but rather in a QUndoCommand.
-        # self.yg_hint._source[self.yg_hint.hint_type()] = param_list
+        # self.yg_hint._source[self.yg_hint.hint_type] = param_list
         super().accept()
 
 
 class ygCVTWidget(QComboBox):
     def __init__(self, hint: Any, _type: str, default: str) -> None:
         super().__init__()
         self.addItem("None")
         # self.setInsertPolicy(QComboBox.InsertPolicy.InsertAlphabetically)
-        # cv_list = hint.yg_glyph.yg_font.cvt.get_list(_type, hint.yg_glyph.current_axis())
+        # cv_list = hint.yg_glyph.yg_font.cvt.get_list(_type, hint.yg_glyph.axis)
         cv_list = hint.yg_glyph.yg_font.cvt.get_list(
             hint.yg_glyph,
             type=_type,
-            axis=hint.yg_glyph.current_axis(),
+            axis=hint.yg_glyph.axis,
             cat=hint.yg_glyph.get_category(),
             suffix=hint.yg_glyph.get_suffixes(),
         )
         cv_list.sort()
         for c in cv_list:
             self.addItem(c)
             if c == default:
                 self.setCurrentText(default)
-        if hint.cv():
-            self.setCurrentText(hint.cv())
+        if hint.cv:
+            self.setCurrentText(hint.cv)
 
     def text(self) -> str:
         return self.currentText()
```

### Comparing `ygt-0.1.6/src/ygt/makeCVDialog.py` & `ygt-0.2.0/src/ygt/makeCVDialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Union, Any, Tuple, Optional
 from PyQt6.QtWidgets import (
     QDialog,
     QVBoxLayout,
     QHBoxLayout,
+    QGridLayout,
     QDialogButtonBox,
     QComboBox,
     QLineEdit,
     QLabel,
     QWidget,
     QTabWidget,
     QListWidget,
@@ -115,15 +116,15 @@
 
         # Set up CV list.
 
         self.cv_list_layout = QVBoxLayout()
         self.button_layout = QHBoxLayout()
 
         self.cv_list = QListWidget()
-        self.cv_list.addItems(self._cvt.keys())
+        self.cv_list.addItems(self._cvt.keys)
         self.current_list_item = self.cv_list.item(0)
         self.cv_list.setCurrentItem(self.current_list_item)
         self._current_cv_name = self.current_list_item.text()
         self.cv_list.itemActivated.connect(self.new_item)
 
         # And the edit pane.
 
@@ -162,29 +163,29 @@
     def change_name_in_list(self, n) -> None:
         self.current_list_item.setText(n)
 
     def del_cv(self) -> None:
         self._cvt.del_cv(self._current_cv_name)
         self.cv_list.clear()
         try:
-            self._current_cv_name = list(self._cvt.keys())[0]
+            self._current_cv_name = list(self._cvt.keys)[0]
         except IndexError:
             return
         self.refresh()
 
     def refresh(self) -> None:
         """This is the place to figure out whether the source
         or masters have been changed: if not, we don't have to
         go through all this.
         """
         if not len(self._cvt):
             self.add_cv()
         self._current_cv = self._cvt.get_cv(self._current_cv_name)
         self.cv_list.clear()
-        self.cv_list.addItems(self._cvt.keys())
+        self.cv_list.addItems(self._cvt.keys)
         matches = self.cv_list.findItems(
             self._current_cv_name, Qt.MatchFlag.MatchExactly
         )
         if len(matches) > 0:
             self.cv_list.setCurrentItem(matches[0])
         else:
             try:
@@ -333,15 +334,15 @@
         self.masters = self.yg_font.masters
 
         self.layout_obj = QHBoxLayout()
         self.master_list_layout = QVBoxLayout()
         self.button_layout = QHBoxLayout()
 
         self.master_list = QListWidget()
-        self.master_list.addItems(self.masters.names())
+        self.master_list.addItems(self.masters.names)
         self.current_list_item = self.master_list.item(0)
         self.master_list.setCurrentItem(self.current_list_item)
         self.master_list.itemActivated.connect(self.new_item)
 
         self._current_master = self.masters.master_by_name(
             self.current_list_item.text()
         )
@@ -384,38 +385,38 @@
             self.edit_pane = masterWidget(
                 self.masters, self.current_master_id(), self.yg_font
             )
             self.layout_obj.addWidget(self.edit_pane)
 
     def add_master(self) -> None:
         master_dict = {}
-        axis_tags = self.yg_font.axis_tags()
+        axis_tags = self.yg_font.axis_tags
         for a in axis_tags:
             master_dict[a] = 0.0
         master_id = random_id("master")
         master_vals = {"name": master_id, "vals": master_dict}
         self.yg_font.masters.add_master(master_id, master_vals)
         self.refresh()
 
     def del_master(self) -> None:
         self.yg_font.masters.del_by_name(self.current_master_name())
         self.master_list.clear()
         try:
             self._current_master = self.masters.master_by_name(
-                self.yg_font.masters.names()[0]
+                self.yg_font.masters.names[0]
             )
         except IndexError:
             return
         self.refresh()
 
     def refresh(self) -> None:
         if not len(self.yg_font.masters):
             return
         self.master_list.clear()
-        self.master_list.addItems(self.yg_font.masters.names())
+        self.master_list.addItems(self.yg_font.masters.names)
         matches = self.master_list.findItems(
             self.current_master_name(), Qt.MatchFlag.MatchExactly
         )
         if len(matches) > 0:
             self.master_list.setCurrentItem(matches[0])
         else:
             try:
@@ -449,15 +450,15 @@
         self.master_layout = QVBoxLayout()
         self.name_layout = QHBoxLayout()
         self.name_layout.addWidget(QLabel("Name"))
         self.master_name_widget = masterNameWidget(self.masters, self.m_id)
         self.name_layout.addWidget(self.master_name_widget)
         self.master_layout.addLayout(self.name_layout)
         self.names = []
-        axis_tags = yg_font.axis_tags()
+        axis_tags = yg_font.axis_tags
         for axis_name in axis_tags:
             axis_val_layout = QHBoxLayout()
             axis_val_layout.addWidget(QLabel(axis_name))
             n = masterValWidget(self.masters, self.m_id, axis_name)
             self.names.append(n)
             axis_val_layout.addWidget(n)
             self.master_layout.addLayout(axis_val_layout)
@@ -647,15 +648,15 @@
         # Set up variants tab
 
         self.variants_tab_layout = None
         if self.variants_tab:
             self.variants_tab_layout = QVBoxLayout()
             self.var_widgets = []
             self.var_layouts = []
-            master_keys = self.masters.keys() # type: ignore
+            master_keys = self.masters.keys # type: ignore
             for k in master_keys:
                 self.var_layouts.append(QHBoxLayout())
                 self.var_layouts[-1].addWidget(QLabel(self.masters.get_master_name(k))) # type: ignore
                 self.var_widgets.append(cvVarWidget(k, self.cv_source))
                 self.var_layouts[-1].addWidget(self.var_widgets[-1])
 
         for w in self.gen_widgets:
@@ -852,37 +853,86 @@
     yg_font (ygFont): the font now being edited.
     """
 
     def __init__(self, yg_font: ygFont) -> None:
         super().__init__()
         self.yg_font = yg_font
         self.defaults = yg_font.defaults
-        self.layout_obj = QVBoxLayout()
+        self.layout_obj = QGridLayout()
+        self.layout_obj.setHorizontalSpacing(20)
+        self.layout_obj.setVerticalSpacing(0)
         self.ignore_signal = False
 
         self.tt_defaults = QCheckBox("Use TrueType defaults")
+        s =  "<span>If</span> this is checked, all instructions in the CVT program that set "
+        s += "defaults will be ignored."
+        self.tt_defaults.setToolTip(s)
         self.tt_defaults.stateChanged.connect(self.toggle_tt_defaults)
 
         self.init_graphics = QCheckBox("Initialize graphics")
+        s =  "<span>If</span> this is checked, code to initialize graphics variables will "
+        s += "be inserted at the beginning of each glyph program. This should "
+        s += "normally be left unchecked, as these variables are seldom "
+        s += "consulted in modern TrueType hinting."
+        self.init_graphics.setToolTip(s)
         self.init_graphics.stateChanged.connect(self.toggle_init_graphics)
 
         self.assume_always_y = QCheckBox("Assume axis always y")
+        s =  "<span>Instructs</span> the compiler to assume that you are only hinting on "
+        s += "y axis. When this is checked, Ygt will perform several optimizations."
+        self.assume_always_y.setToolTip(s)
         self.assume_always_y.stateChanged.connect(self.toggle_assume_always_y)
 
         self.counterclockwise = QCheckBox("Outer contours counter-clockwise")
+        s =  "<span>When</span> outer contours are counter-clockwise, Ygt will guess distance types "
+        s += "wrongly. Check this box and it will guess correctly. You should also "
+        s += "select View→Point coordinates since contours will probably be reversed "
+        s += "when you generate the font, throwing off the point indices."
+        self.counterclockwise.setToolTip(s)
         self.counterclockwise.stateChanged.connect(self.toggle_counterclockwise)
 
         self.cleartype = QCheckBox("Cleartype")
+        s =  "<span>If</span> this box is checked, MS Windows will render your font"
+        s += "in native ClearType mode."
+        self.cleartype.setToolTip(s)
         self.cleartype.stateChanged.connect(self.toggle_cleartype)
 
-        self.layout_obj.addWidget(self.tt_defaults)
-        self.layout_obj.addWidget(self.init_graphics)
-        self.layout_obj.addWidget(self.assume_always_y)
-        self.layout_obj.addWidget(self.counterclockwise)
-        self.layout_obj.addWidget(self.cleartype)
+        self.mergemode = QCheckBox("Merge mode")
+        s =  "<span>Check</span> this box if you are hinting a font containing hints that you "
+        s += "want to retain. Glyphs that you’ve hinted will use your hints. Your functions "
+        s += "and control values will be appended to the ones already in the font."
+        self.mergemode.setToolTip(s)
+        self.mergemode.stateChanged.connect(self.toggle_mergemode)
+
+        self.replaceprep = QCheckBox("Replace CVT program")
+        s =  "<span>Only</span> available when merge mode is active. If you check this box, "
+        s += "the CVT program generated by Ygt will replace the one in the font. Otherwise, "
+        s += "the Ygt CVT program will be appended to the existing one."
+        self.replaceprep.setToolTip(s)
+        self.replaceprep.stateChanged.connect(self.toggle_replaceprep)
+
+        self.functionbase = functionBaseWidget(self.defaults)
+        s =  "In merge mode, <span>set</span> 'function-base' to a non-zero value if Ygt guesses wrongly "
+        s += "about the highest-numbered function in the font to which you are adding hints."
+        self.functionbase.setToolTip(s)
+
+        self.layout_obj.addWidget(self.tt_defaults, 1, 1)
+        self.layout_obj.addWidget(self.init_graphics, 2, 1)
+        self.layout_obj.addWidget(self.cleartype, 3, 1)
+        self.layout_obj.addWidget(self.assume_always_y, 4, 1)
+        self.layout_obj.addWidget(self.counterclockwise, 1, 2)
+        self.layout_obj.addWidget(self.mergemode, 2, 2)
+        self.layout_obj.addWidget(self.replaceprep, 3, 2)
+        self.functionbase.setFixedWidth(int(self.functionbase.width() /4))
+        function_base_layout = QHBoxLayout()
+        # function_base_layout.setAlignment(Qt.AlignmentFlag.AlignLeft)
+        function_base_layout.addWidget(QLabel("function base"))
+        function_base_layout.addWidget(self.functionbase, alignment = Qt.AlignmentFlag.AlignLeft)
+        self.layout_obj.addLayout(function_base_layout, 4, 2)
+
         self.setLayout(self.layout_obj)
 
         self.refresh()
 
     def toggle_counterclockwise(self) -> None:
         if self.ignore_signal:
             return
@@ -919,14 +969,34 @@
         if self.ignore_signal:
             return
         if self.cleartype.isChecked():
             self.defaults.set_default({"cleartype": True})
         else:
             self.defaults.del_default("cleartype")
 
+    def toggle_mergemode(self) -> None:
+        if self.ignore_signal:
+            return
+        if self.mergemode.isChecked():
+            self.defaults.set_default({"merge-mode": True})
+            self.replaceprep.setEnabled(True)
+            self.functionbase.setEnabled(True)
+        else:
+            self.defaults.del_default("merge-mode")
+            self.replaceprep.setEnabled(False)
+            self.functionbase.setEnabled(False)
+
+    def toggle_replaceprep(self) -> None:
+        if self.ignore_signal:
+            return
+        if bool(self.defaults.get_default("merge-mode")) and self.replaceprep.isChecked():
+            self.defaults.set_default({"replace-prep": True})
+        else:
+            self.defaults.del_default("replace-prep")
+
     def fixup(self) -> None:
         pass
 
     def refresh(self, ign: bool = True) -> None:
         self.ignore_signal = ign
 
         t = self.defaults.get_default("use-truetype-defaults")
@@ -939,14 +1009,20 @@
 
         t = self.defaults.get_default("assume-always-y")
         self.assume_always_y.setChecked(bool(t))
 
         t = self.defaults.get_default("cleartype")
         self.cleartype.setChecked(bool(t))
 
+        t = self.defaults.get_default("merge-mode")
+        self.mergemode.setChecked(bool(t))
+
+        t = self.defaults.get_default("replace-prep")
+        self.replaceprep.setChecked(bool(t))
+
         self.ignore_signal = False
 
 
 class makeCVDialog(QDialog, cvSource):
     """A dialog for creating a cv. This doesn't edit the cvt source
     directly, but instead works on a fragment of cv code to be
     added when the accept() function is called.
@@ -1409,14 +1485,52 @@
         k = "None"
         if v and self.var_id in v:
             k = v[self.var_id]
         self.setText(str(k))
         self.set_clean()
 
 
+class functionBaseWidget(QLineEdit):
+    def __init__(self, defaults):
+        super().__init__()
+        self.defaults = defaults
+        init_val = self.defaults.get_default("function-base")
+        if init_val == None:
+            init_val = 0
+        self.setText(str(init_val))
+        self.setValidator(QIntValidator(0, 255))
+        self.editingFinished.connect(self.text_changed)
+        self.last_val = self.text()
+
+    def _text(self) -> str:
+        return self.text().strip()
+
+    def fixup(self) -> None:
+        t = self._text()
+        if t != self.last_val:
+            try:
+                i = int(t)
+            except ValueError:
+                i = 0
+            self.defaults.set_default({"function-base": i})
+
+    def text_changed(self) -> None:
+        t = self._text()
+        if t != self.last_val:
+            self.fixup()
+            self.last_val = t
+
+    def refresh(self) -> None:
+        fb = self.defaults.get_default("function-base")
+        if fb == None:
+            self.setText("0")
+        else:
+            self.setText(str(fb))
+
+
 class cvValueWidget(QLineEdit):
     """Widget for editing the value of a CV.
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ygt-0.1.6/src/ygt/window.py` & `ygt-0.2.0/src/ygt/window.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+# ApplicationSpecificRole
 # import inspect
 from typing import Any, TypeVar, Union, Optional
 import sys
 import os
 import copy
 import yaml
 from .ygModel import ygFont, ygGlyph, unicode_cat_names
 from .fontViewDialog import fontViewWindow
 from .ygPreview import ygPreview, ygStringPreview, ygPreviewContainer
 from .ygYAMLEditor import ygYAMLEditor, editorDialog
 from .ygHintEditor import ygGlyphScene, ygGlyphView
 from .ygPreferences import ygPreferences, open_config
 from .ygSchema import (
     is_cvt_valid,
-    is_cvar_valid,
     is_prep_valid,
     are_macros_valid,
     are_functions_valid,
     are_defaults_valid,
     are_names_valid,
     are_properties_valid,
 )
 from .ygError import ygErrorMessages
 from .makeCVDialog import fontInfoWindow
-from xgridfit import compile_list, compile_all # type: ignore
+from xgridfit import compile_list # type: ignore
+from xgridfit import run as xgf_run # type: ignore
 from fontTools import ufoLib # type: ignore
 from PyQt6.QtCore import Qt, QSize, QThread, pyqtSlot, pyqtSignal, QObject, QEvent
 from PyQt6.QtWidgets import (
     QWidget,
     QApplication,
     QMainWindow,
     QSplitter,
@@ -54,14 +55,15 @@
     QFontDatabase,
 )
 from fontTools import ttLib, ufoLib # type: ignore
 
 # FileNameVar = TypeVar("FileNameVar", str, tuple[str, Any])
 FileNameVar = Union[str, tuple[str, Any]]
 # FileNameVar = Any
+ygt_version = "0.2.0"
 
 
 class ygPreviewFontMaker(QThread):
     """To be run from a QThread. This is because it can take the better
     part of a second to generate a preview, even on a pretty fast
     machine, and we want to be able to run this on a signal without
     making the GUI balky.
@@ -100,44 +102,77 @@
 
 class ygFontGenerator(QThread):
     """For generating whole fonts."""
 
     sig_font_gen_done = pyqtSignal(object)
     sig_font_gen_error = pyqtSignal()
 
-    def __init__(self, font: ttLib.TTFont, source: dict, output_font: str) -> None:
+    def __init__(
+            self,
+            font: ttLib.TTFont,
+            source: dict,
+            output_font: str,
+            mergemode: bool = False,
+            replaceprep: bool = False,
+            functionbase: int = 0,
+            initgraphics: bool = False,
+            assume_y: bool = False,
+            cleartype: bool = True, # Not yet hooked up
+            use_truetype_defaults: bool = False, # Not yet hooked up
+        ) -> None:
         super().__init__()
         self.ft_font = font
         self.source = source
         self.output_font = output_font
         self.error = False
+        self.mergemode = mergemode
+        self.replaceprep = replaceprep
+        self.functionbase = functionbase
+        self.initgraphics = initgraphics
+        self.assume_y = "no"
+        if assume_y:
+            self.assume_y = "yes"
+        self.cleartype = "no"
+        if cleartype:
+            self.cleartype = "yes"
+        self.use_truetype_defaults = use_truetype_defaults
 
     def run(self) -> None:
         try:
             font = copy.deepcopy(self.ft_font)
-            failed_glyph_list = compile_all(font, self.source, self.output_font)
+            # failed_glyph_list = compile_all(font, self.source, self.output_font)
+            err, failed_glyph_list = xgf_run(
+                font = font,
+                yaml = self.source,
+                outputfont = self.output_font,
+                quiet = 3,
+                mergemode = self.mergemode,
+                replaceprep = self.replaceprep,
+                functionbase = self.functionbase,
+                initgraphics = self.initgraphics,
+                assume_y = self.assume_y,
+            )
             self.sig_font_gen_done.emit(failed_glyph_list)
         except KeyError as e:
             self.sig_font_gen_error.emit()
 
 
 class MainWindow(QMainWindow):
     def __init__(
             self,
             app: QApplication,
             win_list: Optional[list] = None,
             prefs: Optional[ygPreferences] = None,
             parent = None
         ):
         super(MainWindow, self).__init__(parent=parent)
+        # undo_group will hold undo stacks for each edited glyph and
+        # font-level data.
         self.undo_group = QUndoGroup()
         self.undo_group.cleanChanged.connect(self.clean_changed)
-        # The undo registry should keep a record of undo stacks for each
-        # glyph that has been edited, and for the prep, cvar, fpgm, macros,
-        # and defaults.
         self.error_manager = ygErrorMessages(self)
         if not win_list:
             self.win_list = [self]
         else:
             self.win_list = win_list
         self.filename = ""
         # self.filename_extension = ""
@@ -152,16 +187,21 @@
         self.statusbar = self.statusBar()
         self.statusbar_label = QLabel()
         self.statusbar_label.setStyleSheet(
             "QLabel {font-family: Source Code Pro, monospace; margin-left: 10px; }"
         )
         self.statusbar.addWidget(self.statusbar_label)
 
-        self.prog_path = os.path.split(__file__)[0]
-        self.icon_path = self.prog_path + "/icons/"
+        if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
+            self.icon_path = os.path.split(sys._MEIPASS)[0]
+            self.icon_path = os.path.join(sys._MEIPASS, "icons")
+        else:
+            self.icon_path = os.path.split(__file__)[0]
+            self.icon_path = os.path.join(self.icon_path, "icons/")
+
         self.setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
         self.setWindowTitle("YGT")
         self.toolbar = self.addToolBar("Tools")
         self.toolbar.setIconSize(QSize(32, 32))
         self.progress_bar: Optional[QProgressBar] = None
         self.progress_bar_action: Optional[QAction] = None
         self.spacer = QWidget()
@@ -193,19 +233,22 @@
         else:
             self.get_preferences(prefs)
 
         self.recents_display: list = []
         self.recents_actions: list = []
         self.instance_actions: list = []
         self.window_list: list = []
-        # self.thread = None
         self.preview_maker: Optional[ygPreviewFontMaker] = None
         self.font_generator: Optional[ygFontGenerator] = None
         self.auto_preview_update = True
 
+        #
+        # Build menus and toolbar
+        #
+
         self.menu = self.menuBar()
 
         #
         # File menu
         #
 
         self.file_menu = self.menu.addMenu("&File")
@@ -236,14 +279,19 @@
 
         self.file_menu.addSeparator()
 
         self.font_info_action = self.file_menu.addAction("Font Info")
         self.font_info_action.setShortcut(QKeySequence("Ctrl+i"))
         self.font_info_action.setEnabled(False)
 
+        self.file_menu.addSeparator()
+
+        self.about_action = self.file_menu.addAction("About YGT")
+        self.about_action.setMenuRole(QAction.MenuRole.ApplicationSpecificRole)
+
         self.file_menu.aboutToShow.connect(self.file_menu_about_to_show)
 
         #
         # Edit Menu
         #
 
         self.edit_menu = self.menu.addMenu("&Edit")
@@ -309,31 +357,45 @@
 
         self.pv_smaller_ten_action = self.preview_menu.addAction("Shrink by Ten")
         self.pv_smaller_ten_action.setShortcut(
             QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_Down) # type: ignore
         )
         self.pv_smaller_ten_action.setEnabled(False)
 
-        self.pv_show_hints_action = self.preview_menu.addAction("Show hinting")
-        self.pv_show_hints_action.setShortcut(QKeySequence("Ctrl+t"))
+        self.pv_show_hints_action = self.preview_menu.addAction("Hint preview")
+        self.pv_show_hints_action.setShortcut(QKeySequence("Ctrl+p"))
         self.pv_show_hints_action.setCheckable(True)
         self.pv_show_hints_action.setChecked(True)
         self.pv_show_hints_action.setEnabled(False)
 
         self.pv_show_grid_action = self.preview_menu.addAction("Show grid")
         self.pv_show_grid_action.setCheckable(True)
         self.pv_show_grid_action.setChecked(True)
         self.pv_show_grid_action.setEnabled(False)
 
         self.instance_menu: Optional[QMenu] = None
 
         self.preview_menu.addSeparator()
 
-        self.pv_set_size_action = self.preview_menu.addAction("Pixels per Em...")
-        self.pv_set_size_action.setShortcut(QKeySequence("Ctrl+p"))
+        self.pv_theme_menu = self.preview_menu.addMenu("Theme")
+        self.pv_theme_auto_action = self.pv_theme_menu.addAction("Auto")
+        self.pv_theme_light_action = self.pv_theme_menu.addAction("Light")
+        self.pv_theme_dark_action = self.pv_theme_menu.addAction("Dark")
+        self.theme_action_group = QActionGroup(self.pv_theme_menu)
+        self.theme_action_group.addAction(self.pv_theme_auto_action)
+        self.theme_action_group.addAction(self.pv_theme_light_action)
+        self.theme_action_group.addAction(self.pv_theme_dark_action)
+        self.pv_theme_auto_action.setCheckable(True)
+        self.pv_theme_light_action.setCheckable(True)
+        self.pv_theme_dark_action.setCheckable(True)
+        self.pv_theme_auto_action.setChecked(True)
+        self.pv_theme_menu.setEnabled(False)
+
+        self.pv_set_size_action = self.preview_menu.addAction("Set resolution...")
+        self.pv_set_size_action.setShortcut(QKeySequence("Ctrl+l"))
         self.pv_set_size_action.setEnabled(False)
 
         self.pv_render_mode_menu = self.preview_menu.addMenu("Render mode")
         self.pv_mode_1_action = self.pv_render_mode_menu.addAction("Grayscale")
         self.pv_mode_2_action = self.pv_render_mode_menu.addAction("Subpixel (1)")
         self.pv_mode_3_action = self.pv_render_mode_menu.addAction("Subpixel (2)")
         self.render_action_group = QActionGroup(self.pv_render_mode_menu)
@@ -431,135 +493,130 @@
 
         axis_action_group = QActionGroup(self.toolbar)
         axis_action_group.setExclusive(True)
 
         self.vertical_action = self.toolbar.addAction("Vertical hinting")
         vertical_icon = QIcon()
         vertical_icon.addPixmap(
-            QPixmap(self.icon_path + "vertical-on.png"), state=QIcon.State.On
+            QPixmap(os.path.join(self.icon_path, "vertical-on.png")), state=QIcon.State.On
         )
         vertical_icon.addPixmap(
-            QPixmap(self.icon_path + "vertical-off.png"), state=QIcon.State.Off
+            QPixmap(os.path.join(self.icon_path, "vertical-off.png")), state=QIcon.State.Off
         )
         self.vertical_action.setIcon(vertical_icon)
         self.vertical_action.setCheckable(True)
 
         self.horizontal_action = self.toolbar.addAction("Horizontal hinting")
         horizontal_icon = QIcon()
         horizontal_icon.addPixmap(
-            QPixmap(self.icon_path + "horizontal-on.png"), state=QIcon.State.On
+            QPixmap(os.path.join(self.icon_path, "horizontal-on.png")), state=QIcon.State.On
         )
         horizontal_icon.addPixmap(
-            QPixmap(self.icon_path + "horizontal-off.png"), state=QIcon.State.Off
+            QPixmap(os.path.join(self.icon_path, "horizontal-off.png")), state=QIcon.State.Off
         )
         self.horizontal_action.setIcon(horizontal_icon)
         self.horizontal_action.setCheckable(True)
 
         axis_action_group.addAction(self.vertical_action)
         axis_action_group.addAction(self.horizontal_action)
         self.vertical_action.setChecked(True)
         self.vertical_action.setEnabled(False)
         self.horizontal_action.setEnabled(False)
 
         cursor_action_group = QActionGroup(self.toolbar)
         cursor_action_group.setExclusive(True)
 
-        self.cursor_action = self.toolbar.addAction("Cursor (Edit hints)")
+        self.cursor_action = self.toolbar.addAction("Editing cursor")
         cursor_icon = QIcon()
         cursor_icon.addPixmap(
-            QPixmap(self.icon_path + "cursor-icon-on.png"), state=QIcon.State.On
+            QPixmap(os.path.join(self.icon_path, "cursor-icon-on.png")), state=QIcon.State.On
         )
         cursor_icon.addPixmap(
-            QPixmap(self.icon_path + "cursor-icon-off.png"), state=QIcon.State.Off
+            QPixmap(os.path.join(self.icon_path, "cursor-icon-off.png")), state=QIcon.State.Off
         )
         self.cursor_action.setIcon(cursor_icon)
         self.cursor_action.setCheckable(True)
 
         self.toolbar.insertSeparator(self.cursor_action)
 
-        self.hand_action = self.toolbar.addAction("Hand (Pan the canvas)")
+        self.hand_action = self.toolbar.addAction("Panning Cursor (spacebar)")
         hand_icon = QIcon()
         hand_icon.addPixmap(
-            QPixmap(self.icon_path + "hand-icon-on.png"), state=QIcon.State.On
+            QPixmap(os.path.join(self.icon_path, "hand-icon-on.png")), state=QIcon.State.On
         )
         hand_icon.addPixmap(
-            QPixmap(self.icon_path + "hand-icon-off.png"), state=QIcon.State.Off
+            QPixmap(os.path.join(self.icon_path, "hand-icon-off.png")), state=QIcon.State.Off
         )
         self.hand_action.setIcon(hand_icon)
         self.hand_action.setCheckable(True)
 
         cursor_action_group.addAction(self.cursor_action)
         cursor_action_group.addAction(self.hand_action)
         self.cursor_action.setChecked(True)
         self.cursor_action.setEnabled(False)
         self.hand_action.setEnabled(False)
 
         self.stem_action = self.toolbar.addAction("Stem (T)")
-        self.stem_action.setIcon(QIcon(QPixmap(self.icon_path + "stem_distance.png")))
+        self.stem_action.setIcon(QIcon(QPixmap(os.path.join(self.icon_path, "stem_distance.png"))))
         self.stem_action.setShortcuts(
             [
                 QKeySequence(Qt.Key.Key_T),
                 QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_T), # type: ignore
                 QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_T), # type: ignore
                 QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_T), # type: ignore
             ]
         )
         self.stem_action.setEnabled(False)
 
         self.toolbar.insertSeparator(self.stem_action)
 
         self.shift_action = self.toolbar.addAction("Shift (H)")
-        self.shift_action.setIcon(QIcon(QPixmap(self.icon_path + "shift.png")))
+        self.shift_action.setIcon(QIcon(QPixmap(os.path.join(self.icon_path, "shift.png"))))
         self.shift_action.setShortcuts(
             [QKeySequence(Qt.Key.Key_H), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_H)] # type: ignore
         )
         self.shift_action.setEnabled(False)
 
         self.align_action = self.toolbar.addAction("Align (L)")
-        self.align_action.setIcon(QIcon(QPixmap(self.icon_path + "align.png")))
+        self.align_action.setIcon(QIcon(QPixmap(os.path.join(self.icon_path, "align.png"))))
         self.align_action.setShortcuts(
             [QKeySequence(Qt.Key.Key_L), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_L)] # type: ignore
         )
         self.align_action.setEnabled(False)
 
         self.interpolate_action = self.toolbar.addAction("Interpolate (I)")
         self.interpolate_action.setIcon(
-            QIcon(QPixmap(self.icon_path + "interpolate.png"))
+            QIcon(QPixmap(os.path.join(self.icon_path, "interpolate.png")))
         )
         self.interpolate_action.setShortcuts(
             [QKeySequence(Qt.Key.Key_I), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_I)] # type: ignore
         )
         self.interpolate_action.setEnabled(False)
 
         self.anchor_action = self.toolbar.addAction("Anchor (A)")
-        self.anchor_action.setIcon(QIcon(QPixmap(self.icon_path + "anchor.png")))
+        self.anchor_action.setIcon(QIcon(QPixmap(os.path.join(self.icon_path, "anchor.png"))))
         self.anchor_action.setShortcuts(
             [
                 QKeySequence(Qt.Key.Key_A),
                 QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_A), # type: ignore
                 QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_A), # type: ignore
                 QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_A), # type: ignore
             ]
         )
         self.anchor_action.setEnabled(False)
 
-        #self.make_set_action = self.toolbar.addAction("Make Set (K)")
-        #self.make_set_action.setIcon(QIcon(QPixmap(self.icon_path + "make_set.png")))
-        #self.make_set_action.setShortcut(QKeySequence(Qt.Key.Key_K))
-        #self.make_set_action.setEnabled(False)
-
         self.make_cv_guess_action = self.toolbar.addAction("Guess Control Value (?)")
         self.make_cv_guess_action.setIcon(
-            QIcon(QPixmap(self.icon_path + "cv_guess.png"))
+            QIcon(QPixmap(os.path.join(self.icon_path, "cv_guess.png")))
         )
         self.make_cv_guess_action.setShortcut(QKeySequence(Qt.Key.Key_Question))
         self.make_cv_guess_action.setEnabled(False)
 
         self.make_cv_action = self.toolbar.addAction("Make Control Value (C)")
-        self.make_cv_action.setIcon(QIcon(QPixmap(self.icon_path + "cv.png")))
+        self.make_cv_action.setIcon(QIcon(QPixmap(os.path.join(self.icon_path, "cv.png"))))
         self.make_cv_action.setShortcut(QKeySequence(Qt.Key.Key_C))
         self.make_cv_action.setEnabled(False)
 
         self.central_widget = self.qs
         self.setCentralWidget(self.central_widget)
 
         self.setup_file_connections()
@@ -612,23 +669,24 @@
             self.horizontal_action.setChecked(True)
 
     @pyqtSlot(object)
     def preview_ready(self, args: dict) -> None:
         try:
             glyph_index = args["gindex"][self.preview_glyph_name]
             self.yg_preview.fetch_glyph(args["font"], glyph_index)
+            self.yg_preview.make_pixmap()
             self.yg_preview.update()
         except Exception:
             pass
 
     @pyqtSlot()
     def toggle_auto_preview(self) -> None:
         self.auto_preview_update = not self.auto_preview_update
         try:
-            self.glyph_pane.viewer.yg_glyph.set_auto_preview_connection()
+            self.glyph_pane.yg_glyph_scene.yg_glyph.set_auto_preview_connection()
         except Exception as e:
             # print(e)
             pass
 
     @pyqtSlot()
     def preview_current_glyph(self) -> None:
         self._preview_current_glyph()
@@ -639,15 +697,15 @@
                 return
         except RuntimeError as e:
             # We get this RuntimeError when self.thread has been garbage collected.
             # It means that it's safe to run the rest of this function.
             pass
         source = self.yg_font.source
         font = self.yg_font.preview_font
-        self.preview_glyph_name = self.glyph_pane.viewer.yg_glyph.gname
+        self.preview_glyph_name = self.glyph_pane.yg_glyph_scene.yg_glyph.gname
         preview_text = self.yg_string_preview.panel._text
         self.preview_glyph_name_list = []
         if preview_text != None and len(preview_text) > 0:
             l = self.yg_font.string_to_name_list(preview_text)
             # l is the list with reduncancies removed.
             self.preview_glyph_name_list.extend(l)
         if not self.preview_glyph_name in self.preview_glyph_name_list:
@@ -691,15 +749,15 @@
     # Font view window
     #
 
     @pyqtSlot()
     def show_font_view(self) -> None:
         """Display the modeless dialog in fontViewWindow.py."""
         if not self.font_viewer:
-            font_name = self.yg_font.font_files.in_font()
+            font_name = self.yg_font.font_files.in_font
             glyph_list = self.yg_font.glyph_list
             self.font_viewer = fontViewWindow(font_name, self.yg_font, glyph_list, self)
         if self.font_viewer.valid:
             self.font_viewer.show()
             self.font_viewer.raise_()
             self.font_viewer.activateWindow()
         else:
@@ -710,41 +768,34 @@
     #
     # Indices vs. coordinates outline display
     #
 
     @pyqtSlot()
     def index_labels(self) -> None:
         self.points_as_coords = False
-        self.glyph_pane.viewer.set_point_display("index")
+        self.glyph_pane.yg_glyph_scene.set_point_display("index")
 
     @pyqtSlot()
     def coord_labels(self) -> None:
         self.points_as_coords = True
-        self.glyph_pane.viewer.set_point_display("coord")
+        self.glyph_pane.yg_glyph_scene.set_point_display("coord")
 
     #
     # Prep for menu display
     #
 
     @pyqtSlot()
     def view_menu_about_to_show(self) -> None:
         if self.points_as_coords:
             self.index_label_action.setEnabled(True)
             self.coord_label_action.setEnabled(False)
         else:
             self.index_label_action.setEnabled(False)
             self.coord_label_action.setEnabled(True)
 
-    # @pyqtSlot()
-    # def window_menu_about_to_show(self) -> None:
-    #    if len(self.win_list) > 0:
-    #        wins = []
-    #        for w in self.win_list:
-    #            wins.append(w.filename)
-
     @pyqtSlot()
     def file_menu_about_to_show(self) -> None:
         self.recents_display = []
         self.disconnect_recents_connections()
         self.recent_menu.clear()
         self.recents_actions.clear()
         self.recents_display.clear()
@@ -772,14 +823,15 @@
             self.recent_menu.setEnabled(False)
 
     @pyqtSlot()
     def preview_menu_about_to_show(self) -> None:
         if self.yg_preview != None:
             if self.yg_preview.face != None:
                 self.pv_render_mode_menu.setEnabled(True)
+            self.pv_theme_menu.setEnabled(True)
             self.pv_show_hints_action.setChecked(self.yg_preview.hinting_on)
             self.pv_show_grid_action.setChecked(self.yg_preview.show_grid)
         self.toggle_auto_preview_action.setChecked(self.auto_preview_update)
 
     @pyqtSlot()
     def edit_menu_about_to_show(self) -> None:
         if self.undo_group.canUndo():
@@ -816,14 +868,15 @@
         self.save_as_action.triggered.connect(self.save_as)
         self.quit_action.triggered.connect(
             self.quit, type=Qt.ConnectionType.QueuedConnection
         )
         self.open_action.triggered.connect(self.open_file)
         self.save_font_action.triggered.connect(self.export_font)
         self.font_info_action.triggered.connect(self.edit_font_info)
+        self.about_action.triggered.connect(self.show_about_dialog)
 
     def setup_recents_connections(self) -> None:
         for a in self.recents_actions:
             a.triggered.connect(self.open_recent)
 
     def disconnect_recents_connections(self) -> None:
         for a in self.recents_actions:
@@ -862,14 +915,17 @@
         self.pv_bigger_ten_action.triggered.connect(self.yg_preview.bigger_ten)
         self.pv_smaller_one_action.triggered.connect(self.yg_preview.smaller_one)
         self.pv_smaller_ten_action.triggered.connect(self.yg_preview.smaller_ten)
         self.pv_set_size_action.triggered.connect(self.show_ppem_dialog)
         self.pv_mode_1_action.triggered.connect(self.yg_preview.render1)
         self.pv_mode_2_action.triggered.connect(self.yg_preview.render2)
         self.pv_mode_3_action.triggered.connect(self.yg_preview.render3)
+        self.pv_theme_auto_action.triggered.connect(self.yg_preview.set_theme_auto)
+        self.pv_theme_light_action.triggered.connect(self.yg_preview.set_theme_light)
+        self.pv_theme_dark_action.triggered.connect(self.yg_preview.set_theme_dark)
         self.pv_show_hints_action.triggered.connect(self.yg_preview.toggle_show_hints)
         self.pv_show_grid_action.triggered.connect(self.yg_preview.toggle_grid)
 
     def setup_preview_instance_connections(self) -> None:
         if self.yg_font.is_variable_font and self.instance_actions != None:
             self.prev_instance_action.triggered.connect(self.yg_preview.next_instance)
             self.next_instance_action.triggered.connect(self.yg_preview.prev_instance)
@@ -901,53 +957,54 @@
         self.hand_action.toggled.connect(self.set_mouse_panning)
         self.cursor_action.toggled.connect(self.set_mouse_editing)
 
     def setup_glyph_pane_connections(self) -> None:
         self.setup_nav_connections()
         self.setup_zoom_connections()
         self.source_editor.setup_editor_signals(
-            self.glyph_pane.viewer.yg_glyph.save_editor_source
+            self.glyph_pane.yg_glyph_scene.yg_glyph.save_editor_source
         )
         self.source_editor.setup_status_indicator(self.set_status_validity_msg)
         self.setup_cursor_connections()
 
     def connect_editor_signals(self) -> None:
         self.source_editor.setup_editor_signals(
-            self.glyph_pane.viewer.yg_glyph.save_editor_source
+            self.glyph_pane.yg_glyph_scene.yg_glyph.save_editor_source
         )
 
     def disconnect_editor_signals(self) -> None:
         self.source_editor.disconnect_editor_signals(
-            self.glyph_pane.viewer.yg_glyph.save_editor_source
+            self.glyph_pane.yg_glyph_scene.yg_glyph.save_editor_source
         )
 
+    #
+    # GUI setup
+    #
+
     def set_up_instance_list(self) -> None:
         if self.yg_font.is_variable_font and hasattr(self.yg_font, "instances"):
             self.preview_menu.addSeparator()
             self.prev_instance_action = self.preview_menu.addAction("Previous instance")
             self.prev_instance_action.setShortcut(QKeySequence(Qt.Key.Key_Less))
             self.next_instance_action = self.preview_menu.addAction("Next instance")
             self.next_instance_action.setShortcut(QKeySequence(Qt.Key.Key_Greater))
             self.instance_menu = self.preview_menu.addMenu("&Instances")
             self.instance_actions = []
             instance_names = []
             for k in self.yg_font.instances.keys():
                 self.instance_actions.append(self.instance_menu.addAction(k))
                 instance_names.append(k)
             self.yg_preview.add_instances(self.yg_font.instances)
-            self.yg_preview.instance = self.yg_font.default_instance()
+            self.yg_preview.instance = self.yg_font.default_instance
             self.prev_instance_action.setEnabled(False)
             self.next_instance_action.setEnabled(False)
             self.instance_menu.setEnabled(False)
 
-    #
-    # GUI setup
-    #
-
     def set_size_and_position(self):
+        """Set size and position of the main window."""
         if self.preferences.geometry_valid():
             self.setGeometry(
                 self.preferences["top_window_pos_x"],
                 self.preferences["top_window_pos_y"],
                 self.preferences["top_window_width"],
                 self.preferences["top_window_height"],
             )
@@ -998,14 +1055,15 @@
         self.undo_group.addStack(s)
 
     def set_all_clean(self):
         s = self.undo_group.stacks()
         for ss in s:
             ss.setClean()
 
+    # Could be a property
     def is_file_clean(self):
         s = self.undo_group.stacks()
         for ss in s:
             if not ss.isClean():
                 return False
         return True
 
@@ -1015,33 +1073,33 @@
 
     @pyqtSlot()
     def save_yaml_file(self) -> None:
         self._save_yaml_file()
 
     def _save_yaml_file(self) -> None:
         if self.yg_font and (not self.is_file_clean()):
-            glyph = self.glyph_pane.viewer.yg_glyph
+            glyph = self.glyph_pane.yg_glyph_scene.yg_glyph
             glyph_backup = copy.deepcopy(glyph.gsource)
             glyph.cleanup_glyph()
-            self.yg_font.cleanup_font(glyph.glyph_name())
+            self.yg_font.cleanup_font(glyph.gname)
             self.yg_font.source_file.save_source()
             glyph.gsource.clear()
             for k in glyph_backup.keys():
                 glyph.gsource[k] = glyph_backup[k]
             self.set_all_clean()
             self.set_window_title()
 
     def save_as(self) -> None:
         self.yg_font.source_file.filename = QFileDialog(parent=self).getSaveFileName()[
             0
         ]
         if not self.yg_font.source_file.filename:
             return
         self.preferences.add_recent(self.yg_font.source_file.filename)
-        glyph = self.glyph_pane.viewer.yg_glyph
+        glyph = self.glyph_pane.yg_glyph_scene.yg_glyph
         glyph_backup = copy.deepcopy(glyph.gsource)
         glyph.cleanup_glyph()
         self.yg_font.source_file.save_source(top_window=self)
         glyph.gsource.clear()
         for k in glyph_backup.keys():
             glyph.gsource[k] = glyph_backup[k]
         self.set_all_clean()
@@ -1052,31 +1110,48 @@
             if self.font_generator != None and self.font_generator.isRunning():
                 return
         except RuntimeError as e:
             # We get this RuntimeError when self.thread has been garbage collected.
             # It means that it's safe to run the rest of this function.
             pass
         source = self.yg_font.source
-        new_file_name = self.yg_font.font_files.out_font()
-        in_file_name = self.yg_font.font_files.in_font()
+        new_file_name = self.yg_font.font_files.out_font
+        in_file_name = self.yg_font.font_files.in_font
         if new_file_name == None or in_file_name == None:
             return
         source = self.yg_font.source
         font = self.yg_font.preview_font
         msg_box = QMessageBox(self)
         msg_box.setText("Ready to export " + new_file_name + "?")
         msg_box.setStandardButtons(
             QMessageBox.StandardButton.Cancel | QMessageBox.StandardButton.Save
         )
         msg_box.setIcon(QMessageBox.Icon.Question)
         msg_box.setDefaultButton(QMessageBox.StandardButton.Save)
         ret = msg_box.exec()
         if ret == QMessageBox.StandardButton.Cancel:
             return
-        self.font_generator = ygFontGenerator(font, source, new_file_name)
+        mergemode = bool(self.yg_font.defaults.get_default("merge-mode"))
+        replaceprep = bool(self.yg_font.defaults.get_default("replace-prep"))
+        initgraphics = bool(self.yg_font.defaults.get_default("init-graphics")) # ***
+        assume_y = bool(self.yg_font.defaults.get_default("assume-always-y"))
+        try:
+            functionbase = int(self.yg_font.defaults.get_default("function-base"))
+        except TypeError:
+            functionbase = 0
+        self.font_generator = ygFontGenerator(
+            font,
+            source,
+            new_file_name,
+            mergemode = mergemode,
+            replaceprep = replaceprep,
+            functionbase = functionbase,
+            initgraphics = initgraphics,
+            assume_y = assume_y
+        )
         self.font_generator.finished.connect(self.font_generator.deleteLater)
         self.font_generator.sig_font_gen_done.connect(self.font_gen_finished)
         self.font_generator.sig_font_gen_error.connect(self.font_gen_error)
         self.font_generator.start()
         self.progress_bar = QProgressBar()
         self.progress_bar.setMaximum(0)
         self.progress_bar_action = self.toolbar.insertWidget(
@@ -1258,15 +1333,14 @@
         self.code_menu.setEnabled(True)
         self.view_menu.setEnabled(True)
 
         if filename:
             self.preferences.add_recent(filename)
             split_fn = os.path.splitext(filename)
             fn_base = split_fn[0]
-            # self.filename_extension = extension = split_fn[1]
             extension = split_fn[1]
             yaml_source = {}
             # If file is .ttf, create a skeleton yaml_source and a ygt_filename.
             # If file is .ufo, read yaml source if possible, or if not create skeleton.
             if extension == ".ttf":
                 ygt_filename = fn_base + ".yaml"
                 self.preferences.add_recent(ygt_filename)
@@ -1297,26 +1371,26 @@
                 self.yg_font = ygFont(self, yaml_source, ygt_filename=ygt_filename)
             else:
                 self.yg_font = ygFont(self, filename)
             self.yg_font.setup_error_signal(self.error_manager.new_message)
 
             if (
                 "current_glyph" in self.preferences
-                and self.yg_font.full_name() in self.preferences["current_glyph"]
+                and self.yg_font.full_name in self.preferences["current_glyph"]
             ):
-                initGlyph = self.preferences["current_glyph"][self.yg_font.full_name()]
+                initGlyph = self.preferences["current_glyph"][self.yg_font.full_name]
             else:
                 initGlyph = "A"
             modelGlyph = ygGlyph(self.preferences, self.yg_font, initGlyph)
             modelGlyph.set_yaml_editor(self.source_editor)
-            viewer = ygGlyphScene(self.preferences, modelGlyph)
-            view = ygGlyphView(self.preferences, viewer, self.yg_font)
-            viewer.owner = view
+            yg_glyph_scene = ygGlyphScene(self.preferences, modelGlyph)
+            view = ygGlyphView(self.preferences, yg_glyph_scene, self.yg_font)
+            yg_glyph_scene.owner = view
             self.add_glyph_pane(view)
-            view.centerOn(view.viewer.center_x, view.sceneRect().center().y())
+            view.centerOn(view.yg_glyph_scene.center_x, view.sceneRect().center().y())
             self.set_window_title()
             self.set_up_instance_list()
             self.setup_editor_connections()
             self.setup_preview_instance_connections()
             self.setup_point_label_connections()
             # Should we send a signal for preview update from here?
             self._preview_current_glyph()
@@ -1325,14 +1399,15 @@
     #
     # GUI management
     #
 
     def setup_stem_buttons(self, axis):
         pass
 
+    @pyqtSlot(object)
     def selection_changed(self, selection_profile: list):
         total_selected = selection_profile[0] + selection_profile[1]
         # fix up make cv button
         if total_selected >= 1 and total_selected <= 2:
             self.make_cv_action.setEnabled(True)
         else:
             self.make_cv_action.setEnabled(False)
@@ -1345,20 +1420,14 @@
             self.anchor_action.setEnabled(True)
             self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             # self.make_set_action.setEnabled(False)
         elif selection_profile[0] == 1 and selection_profile[1] >= 1:
-            # Enable make set button
-            #if 1 in selection_profile[2] or 2 in selection_profile[2]:
-            #    self.make_set_action.setEnabled(True)
-            #else:
-            #    self.make_set_action.setEnabled(False)
-            # stem_action only if 1 pt touched and 1 pt untouched.
             if selection_profile[1] == 1:
                 self.stem_action.setEnabled(True)
             else:
                 self.stem_action.setEnabled(False)
             # shift_action and align_action if 1 pt touched and 1 or more untouched.
             if selection_profile[1] >= 1:
                 self.shift_action.setEnabled(True)
@@ -1391,41 +1460,54 @@
 
     def set_window_title(self) -> None:
         """And also the status bar"""
         base = "YGT"
         if self.yg_font:
             base += (
                 " -- "
-                + str(self.yg_font.family_name())
-                + "-"
-                + str(self.yg_font.style_name())
+                + self.yg_font.full_name
             )
             if not self.is_file_clean():
                 base += "*"
         self.setWindowTitle(base)
         if self.glyph_pane:
             self.set_statusbar_text(None)
 
     def set_statusbar_text(self, valid: Union[bool, None]) -> None:
-        status_text = self.glyph_pane.viewer.yg_glyph.gname
+        status_text = self.glyph_pane.yg_glyph_scene.yg_glyph.gname
         status_text += (
-            " - " + unicode_cat_names[self.glyph_pane.viewer.yg_glyph.get_category()]
+            " - " + unicode_cat_names[self.glyph_pane.yg_glyph_scene.yg_glyph.get_category()]
         )
         status_text += " (" + self.current_axis + ")"
         if valid != None:
             status_text += " ("
             if valid:
                 status_text += "Valid)"
             else:
                 status_text += "Invalid)"
         self.statusbar_label.setText(status_text)
 
     def set_status_validity_msg(self, t: str) -> None:
         self.set_statusbar_text(bool(t))
 
+    @pyqtSlot()
+    def show_about_dialog(self) -> None:
+        msg = QMessageBox(self)
+        msg.setWindowTitle("About YGT")
+        msg.setText("YGT " + ygt_version)
+        detailed_text = "TrueType Hint Editor.\n"
+        detailed_text += "Copyright © 2023 by Peter S. Baker.\n"
+        detailed_text += "Apache License, version 2.0. \n\n"
+        detailed_text += "For further information, visit https://github.com/psb1558/ygt."
+        msg.setDetailedText(detailed_text)
+        # Will need to mess with size hints and policies to do this.
+        # msg.resize(round(msg.width() * 2), round(msg.height() * 2))
+        msg.setStandardButtons(QMessageBox.StandardButton.NoButton)
+        msg.exec()
+
     def show_error_message(self, msg_list: list) -> None:
         msg = QMessageBox(self)
         if msg_list[0] == "Warning":
             msg.setIcon(QMessageBox.Icon.Warning)
         elif msg_list[0] == "Error":
             msg.setIcon(QMessageBox.Icon.Critical)
         msg.setWindowTitle(msg_list[1])
@@ -1435,22 +1517,22 @@
     #
     # Editors in dialogs
     #
 
     @pyqtSlot()
     def indices_to_coords(self) -> None:
         try:
-            self.glyph_pane.viewer.yg_glyph.indices_to_coords()
+            self.glyph_pane.yg_glyph_scene.yg_glyph.indices_to_coords()
         except Exception as e:
             print(e)
 
     @pyqtSlot()
     def coords_to_indices(self) -> None:
         try:
-            self.glyph_pane.viewer.yg_glyph.coords_to_indices()
+            self.glyph_pane.yg_glyph_scene.yg_glyph.coords_to_indices()
         except Exception as e:
             print(e)
 
     @pyqtSlot()
     def edit_cvt(self) -> None:
         self.cvt_editor = editorDialog(
             self.preferences, self.yg_font.cvt, "cvt", is_cvt_valid
@@ -1471,24 +1553,14 @@
     def edit_prep(self) -> None:
         self.prep_editor = editorDialog(
             self.preferences, self.yg_font.prep, "prep", is_prep_valid
         )
         self.prep_editor.show()
         self.prep_editor.activateWindow()
 
-    # @pyqtSlot()
-    # def edit_cvar(self) -> None:
-    #    self.cvar_editor = editorDialog(self.preferences,
-    #                                             self.yg_font.cvar,
-    #                                             "cvar",
-    #                                             is_cvar_valid,
-    #                                             top_structure="list")
-    #    self.cvar_editor.show()
-    #    self.cvar_editor.activateWindow()
-
     @pyqtSlot()
     def edit_functions(self) -> None:
         self.function_editor = editorDialog(
             self.preferences,
             self.yg_font.functions_func,
             "functions",
             are_functions_valid,
@@ -1512,26 +1584,26 @@
         self.default_editor.show()
         self.default_editor.activateWindow()
 
     @pyqtSlot()
     def edit_names(self) -> None:
         self.names_editor = editorDialog(
             self.preferences,
-            self.glyph_pane.viewer.yg_glyph.names,
+            self.glyph_pane.yg_glyph_scene.yg_glyph.names,
             "names",
             are_names_valid,
         )
         self.names_editor.show()
         self.names_editor.activateWindow()
 
     @pyqtSlot()
     def edit_properties(self) -> None:
         self.properties_editor = editorDialog(
             self.preferences,
-            self.glyph_pane.viewer.yg_glyph.props,
+            self.glyph_pane.yg_glyph_scene.yg_glyph.props,
             "properties",
             are_properties_valid,
         )
         self.properties_editor.show()
         self.properties_editor.activateWindow()
 
     #
@@ -1603,14 +1675,15 @@
             result = self.save_query()
             if result == 1:
                 event.ignore()
             else:
                 self.del_from_win_list(self)
                 event.accept()
 
+    # Could be property
     def all_clean(self) -> bool:
         for w in self.win_list:
             if not w.is_file_clean():
                 return False
         return True
 
     def quit(self) -> None:
@@ -1645,19 +1718,20 @@
 
     def resizeEvent(self, event):
         self.preferences.set_top_window_size(
             event.size().width(), event.size().height()
         )
 
     def moveEvent(self, event):
-        self.preferences.set_top_window_pos(event.pos().x(), event.pos().y())
+        if hasattr(self, "preferences"):
+            self.preferences.set_top_window_pos(event.pos().x(), event.pos().y())
 
     def event(self, event) -> bool:
         if event.type() == event.Type.WindowActivate and self.glyph_pane:
-                self.glyph_pane.viewer.yg_glyph.undo_stack.setActive(True)
+                self.glyph_pane.yg_glyph_scene.yg_glyph.undo_stack.setActive(True)
         return super().event(event)
 
     def get_preferences(self, prefs: Optional[ygPreferences]) -> None:
         self.preferences = prefs
         self.points_as_coords = self.preferences.points_as_coords()
         self.zoom_factor = self.preferences.zoom_factor()
         self.show_off_curve_points = self.preferences.show_off_curve_points()
@@ -1665,16 +1739,17 @@
 
     def set_preferences(self) -> None:
         self.preferences.set_points_as_coords(self.points_as_coords)
         self.preferences.set_zoom_factor(self.zoom_factor)
         self.preferences.set_show_off_curve_points(self.show_off_curve_points)
         self.preferences.set_show_point_numbers(self.show_point_numbers)
 
+    # Could be property
     def current_glyph(self):
-        return self.glyph_pane.viewer.yg_glyph
+        return self.glyph_pane.yg_glyph_scene.yg_glyph
 
 
 class mainWinEventFilter(QObject):
     def __init__(self, top_win):
         super().__init__()
         self.top_window = top_win
 
@@ -1682,21 +1757,41 @@
         if event.type() == QEvent.Type.ActivationChange:
             if self.top_window.isActiveWindow():
                 self.top_window.preferences["top_window"] = self.top_window
         return super().eventFilter(source, event)
 
 
 def main():
-    # from PyQt6.QtGui import QPalette
-    # print(dir(Qt))
-    # print(inspect.getargspec(freetype.Face.get_glyph_name))
+    #import uharfbuzz as hb
+    #from inspect import getfullargspec, signature
+    # print(dir(QMessageBox))
+    #print(dir(hb._harfbuzz.Font))
+    #print(dir(hb._harfbuzz.Buffer))
 
     app = QApplication([])
-    font_id = QFontDatabase.addApplicationFont(os.path.dirname(__file__) + "/fonts/SourceCodePro-Regular.ttf")
+
+    if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
+        # font_path = os.path.split(sys._MEIPASS)[0]
+        print(sys._MEIPASS)
+        font_path = os.path.join(
+            sys._MEIPASS,
+            "fonts",
+            "SourceCodePro-Regular.ttf"
+        )
+        print(font_path)
+        # font_path += "/Resources/fonts/SourceCodePro-Regular.ttf"
+    else:
+        font_path = os.path.join(
+            os.path.dirname(__file__),
+            "fonts/SourceCodePro-Regular.ttf"
+        )
+        #font_path = os.path.dirname(__file__) + "/fonts/SourceCodePro-Regular.ttf"
+    
+    font_id = QFontDatabase.addApplicationFont(font_path)
     if font_id == -1:
-        print("Can't find the font Source Code Pro.")
+        print("Can't find font Source Code Pro.")
     top_window = MainWindow(app)
     top_window.get_preferences(open_config(top_window))
     app.setWindowIcon(QIcon(top_window.icon_path + "program.png"))
     top_window.set_size_and_position()
     top_window.show()
     sys.exit(app.exec())
```

### Comparing `ygt-0.1.6/src/ygt/ygError.py` & `ygt-0.2.0/src/ygt/ygError.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt/ygHintEditor.py` & `ygt-0.2.0/src/ygt/ygHintEditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     QDialog,
     QInputDialog,
     QLineEdit,
     QGraphicsProxyWidget,
     QStyleOptionGraphicsItem,
 )
 from fontTools.pens.basePen import BasePen  # type: ignore
-# from fontTools.pens.boundsPen import BoundsPen
 from .ygPreferences import ygPreferences
 
 
 HINT_ARROW_WIDTH = 3
 HINT_ANCHOR_WIDTH = 3
 HINT_LINK_WIDTH = 1
 HINT_ARROWHEAD_WIDTH = 2
@@ -96,17 +95,14 @@
 HINT_FUNC_SELECT_DARK = QColor(38, 191, 74, 192)
 
 HINT_INTERPOLATE_COLOR = QColor(255, 127, 0, 128)
 HINT_INTERPOLATE_DARK = QColor(212, 187, 106, 192)
 HINT_INTERPOLATE_SELECT_COLOR = QColor(215, 87, 0, 128)
 HINT_INTERPOLATE_SELECT_DARK = QColor(255, 195, 0, 192)
 
-#SET_COLOR = QColor(128, 128, 128, 128)
-#SET_SELECT_COLOR = QColor(128, 128, 128, 225)
-
 POINT_ONCURVE_OUTLINE = QColor("red")
 POINT_OFFCURVE_FILL = QColor("white")
 POINT_ONCURVE_FILL = QColor("white")
 POINT_OFFCURVE_OUTLINE = QColor(127, 127, 255, 255)
 POINT_OFFCURVE_SELECTED = QColor(127, 127, 255, 255)
 POINT_ONCURVE_SELECTED = QColor(127, 127, 255, 255)
 PREVIEW_BASE_COLOR = QColor(64, 33, 31, 255)
@@ -129,30 +125,28 @@
     "stem": HINT_STEM_COLOR,
     "whitedist": HINT_STEM_COLOR,
     "blackdist": HINT_STEM_COLOR,
     "graydist": HINT_STEM_COLOR,
     "move": HINT_STEM_COLOR,
     "macro": HINT_FUNC_COLOR,
     "function": HINT_FUNC_COLOR,
-    # "set": SET_COLOR,
 }
 
 _HINT_DARK = {
     "anchor": HINT_ANCHOR_DARK,
     "align": HINT_ALIGN_DARK,
     "shift": HINT_SHIFT_DARK,
     "interpolate": HINT_INTERPOLATE_DARK,
     "stem": HINT_STEM_DARK,
     "whitedist": HINT_STEM_DARK,
     "blackdist": HINT_STEM_DARK,
     "graydist": HINT_STEM_DARK,
     "move": HINT_STEM_DARK,
     "macro": HINT_FUNC_DARK,
     "function": HINT_FUNC_DARK,
-    # "set": SET_COLOR,
 }
 
 SELECTED_HINT_COLOR = {}
 
 _SELECTED_HINT_COLOR = {
     "anchor": HINT_ANCHOR_SELECT_COLOR,
     "align": HINT_ALIGN_SELECT_COLOR,
@@ -161,35 +155,33 @@
     "stem": HINT_STEM_SELECT_COLOR,
     "whitedist": HINT_STEM_SELECT_COLOR,
     "blackdist": HINT_STEM_SELECT_COLOR,
     "graydist": HINT_STEM_SELECT_COLOR,
     "move": HINT_STEM_SELECT_COLOR,
     "macro": HINT_FUNC_SELECT_COLOR,
     "function": HINT_FUNC_SELECT_COLOR,
-    # "set": SET_SELECT_COLOR,
 }
 
 _SELECTED_HINT_DARK = {
     "anchor": HINT_ANCHOR_SELECT_DARK,
     "align": HINT_ALIGN_SELECT_DARK,
     "shift": HINT_SHIFT_SELECT_DARK,
     "interpolate": HINT_INTERPOLATE_SELECT_DARK,
     "stem": HINT_STEM_SELECT_DARK,
     "whitedist": HINT_STEM_SELECT_DARK,
     "blackdist": HINT_STEM_SELECT_DARK,
     "graydist": HINT_STEM_SELECT_DARK,
     "move": HINT_STEM_SELECT_DARK,
     "macro": HINT_FUNC_SELECT_DARK,
     "function": HINT_FUNC_SELECT_DARK,
-    # "set": SET_SELECT_COLOR,
 }
 
 # Classes in this file:
 
-# QtPen (BasePen): copied from fontTools so we could drop a reference to Qt5.
+# QtPen(BasePen): copied from fontTools so we could drop a reference to Qt5.
 # ygSelectable: inherited by objects that can be selected.
 # ygHintView(QGraphicsItem, ygSelectable): Interface with a hint (ygModel.ygHint)
 # ygGraphicalHintComponent: Superclass for a visible piece of a hint.
 # ygArrowHead(QGraphicsPolygonItem, ygGraphicalHintComponent):
 #                    Arrowhead component of a visible hint.
 # ygBorderLine(QGraphicsLineItem, ygGraphicalHintComponent):
 #                    Borderline around certain hints.
@@ -198,16 +190,16 @@
 # ygHintButton(QGraphicsEllipseItem, ygGraphicalHintComponent):
 #                    A button to display in the middle of a hint stem. Makes it
 #                    easier to select with mouse.
 # ygPointMarker(QGraphicsEllipseItem, ygGraphicalHintComponent):
 #                    Thickens and adds color to a point.
 # ygPointable: superclass for objects that an arrow can point at.
 # ygPointCollectionView(QGraphicsItem, ygGraphicalHintComponent, ygPointable):
-#                    Visible representation of a collection of points.
-# ygSetView(QGraphicsItem, ygGraphicalHintComponent):
+#                    A collection of points appears in a box.
+# ygSetView(ygPointCollectionView):
 #                    Visible representation of a set (of points).
 # ygSelection(QObject): Keeps track of selected objects.
 # ygPointView(QGraphicsEllipseItem, ygSelectable, ygPointable):
 #                    Visual representation of a point.
 # SelectionRect(QGraphicsRectItem): For making marquee selections.
 # ygGlyphScene(QGraphicsScene): Visual representation of a glyph (with points,
 #                    ygHintView objects, etc.)
@@ -269,15 +261,15 @@
 
     def _prepare_graphics(self) -> None:
         pass
 
     def update(self) -> None:
         pass
 
-    def _is_yg_selected(self) -> bool:
+    def selected(self) -> bool:
         pass
 
     def yg_select(self) -> None:
         pass
 
     def yg_unselect(self) -> None:
         pass
@@ -296,51 +288,51 @@
 
         args[1] (ygModel.ygHint): a hint from the ygModel
 
         args[2]: either a component of the graphical hint or a list of them.
 
         """
         super().__init__()
-        self._is_selected = False
-        self.yg_glyph_view = args[0]
+        self._selected = False
+        self.yg_glyph_scene = args[0]
         self.yg_hint = args[1]
         self.label: Optional[QLabel] = None
         self.label_proxy = None
         self.description = self._set_description()
         if len(args) >= 3:
             # graphical_hint may arrive as an irregularly nested list.
             # flatten it into a simple list
             self.graphical_hint = list(self._traverse(args[2]))
             for g in self.graphical_hint:
                 g.setParentItem(self)
 
     def _set_description(self) -> str:
-        result = self.yg_hint.hint_type()
+        result = self.yg_hint.hint_type
         if hasattr(self.yg_hint, "cvt"):
-            result += " (" + str(self.yg_hint.cv()) + ")"
+            result += " (" + str(self.yg_hint.cv) + ")"
         # Tooltip not yet. By default, the tooltip appears when the mouse is
         # anywhere in a widget's bounding rect. For hints that is not helpful.
         # *** There is a way to change this behavior: figure it out later.
         # self.setToolTip(result)
         return result
 
     def _set_name(self, name: str) -> None:
         self.yg_hint.name = name
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: gray;}")
         self.label.setText(name)
-        self.label_proxy = self.yg_glyph_view.addWidget(self.label)
+        self.label_proxy = self.yg_glyph_scene.addWidget(self.label)
         rect = self.boundingRect()
         self.label.move(
             round(rect.topLeft().x()), round(rect.topLeft().y() - self.label.height())
         )
 
     def _remove_labels(self) -> None:
         if self.label_proxy:
-            self.yg_glyph_view.removeItem(self.label_proxy)
+            self.yg_glyph_scene.removeItem(self.label_proxy)
         for g in self.graphical_hint:
             if hasattr(g, "_remove_labels"):
                 g._remove_labels()
 
     # Adapted from https://stackoverflow.com/questions/6340351/iterating-through-list-of-list-in-python
     # Presumed public domain.
     def _traverse(self, o) -> Any:
@@ -383,28 +375,28 @@
         """In ygHintView. Returns a ygPointMarker."""
         if len(self.graphical_hint) >= 1:
             for g in self.graphical_hint:
                 if type(g) is ygPointMarker and g.contains(pt):
                     return g
         return None
 
-    def get_scene(self) -> "ygGlyphScene":
-        return self.yg_glyph_view
+    #def get_scene(self) -> "ygGlyphScene":
+    #    return self.yg_glyph_scene
 
     def _target_list(self) -> list:
         """Returns a list of target points for this hint."""
-        mpt = self.yg_glyph_view.resolve_point_identifier(self.yg_hint.target())
+        mpt = self.yg_glyph_scene.resolve_point_identifier(self.yg_hint.target)
         mypoints = []
         if type(mpt) is ygSet:
-            for p in mpt.point_list():
+            for p in mpt.point_list:
                 mypoints.append(p)
         elif type(mpt) is ygParams:
             mypoints.extend(self._get_macfunc_targets(mpt))
         elif type(mpt) is not list:
-            mypoints.append(self.yg_glyph_view.resolve_point_identifier(mpt))
+            mypoints.append(self.yg_glyph_scene.resolve_point_identifier(mpt))
         return mypoints
 
     def _update_touches(self) -> None:
         self._remove_touches()
         self._touch_all_points()
 
     def _get_macfunc_targets(self, p: ygParams) -> list:
@@ -413,22 +405,21 @@
         as "target."
 
         """
         macfunc_name = self.yg_hint.name
         plist = []
         if macfunc_name != None:
             try:
-                if self.yg_hint.hint_type() == "macro":
-                    macfunc = self.yg_glyph_view.yg_glyph.yg_font.macros[macfunc_name]
-                elif self.yg_hint.hint_type() == "function":
-                    macfunc = self.yg_glyph_view.yg_glyph.yg_font.functions[
+                if self.yg_hint.hint_type == "macro":
+                    macfunc = self.yg_glyph_scene.yg_glyph.yg_font.macros[macfunc_name]
+                elif self.yg_hint.hint_type == "function":
+                    macfunc = self.yg_glyph_scene.yg_glyph.yg_font.functions[
                         macfunc_name
                     ]
                 else:
-                    # raise Exception(str(macfunc_name) + " not function or macro!")
                     return plist
                 k = p.point_dict.keys()
                 for kk in k:
                     if (
                         kk in macfunc
                         and "subtype" in macfunc[kk]
                         and macfunc[kk]["subtype"] == "target"
@@ -440,33 +431,36 @@
 
     def _touch_untouch(self, point_list: list, touch: bool) -> None:
         """Touch or untouch the points in point_list. When touch=False,
         remove self from the owners list, and mark the point as untouched
         only if there are no other owners.
 
         """
-        ptindex = self.yg_glyph_view.yg_point_view_index
+        ptindex = self.yg_glyph_scene.yg_point_view_index
         for p in point_list:
             if type(p) is ygSet:
-                self._touch_untouch(p.point_list(), touch)
+                self._touch_untouch(p.point_list, touch)
             elif type(p) is ygParams:
                 self._touch_untouch(self._get_macfunc_targets(p), touch)
             else:
+                pp = ptindex[p.id]
                 if touch:
                     try:
                         ptindex[p.id].touched = True
                         ptindex[p.id].owners.append(self)
                     except Exception:
                         pass
                 else:
                     try:
                         ptindex[p.id].owners.remove(self)
                         if len(ptindex[p.id].owners) == 0:
                             ptindex[p.id].touched = False
-                    except Exception:
+                    except Exception as e:
+                        #print(str(e.args))
+                        #print(str(e))
                         pass
 
     def _touch_all_points(self) -> None:
         """Mark each point affected by this hint as 'touched,' and record
         this hint as an owner in its 'owners" list. To orient new hints
         correctly, we need to be accurate about which points are touched.
 
@@ -480,44 +474,44 @@
 
         """
         self._touch_untouch(self._target_list(), False)
 
     def _process_click_on_hint(self, obj, with_shift: bool, is_left: bool) -> None:
         if is_left:
             if with_shift:
-                self.yg_glyph_view.yg_selection._toggle_object(self)
+                self.yg_glyph_scene.yg_selection._toggle_object(self)
             else:
-                self.yg_glyph_view.yg_selection._add_object(self, False)
+                self.yg_glyph_scene.yg_selection._add_object(self, False)
 
     def _prepare_graphics(self) -> None:
         # In ygHintView
         if len(self.graphical_hint) >= 1:
             for c in self.graphical_hint:
                 if isinstance(c, ygGraphicalHintComponent):
                     c._prepare_graphics(
-                        is_selected=self._is_selected,
-                        hint_type=self.yg_hint.hint_type(),
+                        is_selected=self._selected,
+                        hint_type=self.yg_hint.hint_type,
                     )
 
-    def _is_yg_selected(self) -> bool:
-        return self._is_selected
+    def selected(self) -> bool:
+        return self._selected
 
     def update(self, rect: QRectF = None) -> None:  # type: ignore
         if len(self.graphical_hint) >= 1:
             for c in self.graphical_hint:
                 c.update()
         super().update(rect=self.boundingRect())
 
     def yg_select(self) -> None:
-        self._is_selected = True
+        self._selected = True
         self._prepare_graphics()
         self.update()
 
     def yg_unselect(self) -> None:
-        self._is_selected = False
+        self._selected = False
         self._prepare_graphics()
         self.update()
 
 
 class ygGraphicalHintComponent:
     def _prepare_graphics(self, **kwargs) -> None:
         ...
@@ -571,17 +565,15 @@
         hint_type = kwargs["hint_type"]
         if is_selected:
             pen_color = SELECTED_HINT_COLOR[hint_type]
         else:
             pen_color = HINT_COLOR[hint_type]
         pen = QPen(pen_color)
         pen.setWidth(HINT_ARROWHEAD_WIDTH)
-        # brush = QBrush(pen_color)
         self.setPen(pen)
-        # self.setBrush(brush)
 
     def setPos(self, qpf):
         # These little offsets were made by experimentation.  But see if they
         # can be abstracted somehow.
         if self.direction == "down":
             nqp = QPointF(qpf.x() - 8, qpf.y() - 6)
         elif self.direction == "up":
@@ -590,15 +582,14 @@
             nqp = QPointF(qpf.x() - 4, qpf.y() - 8)
         else:
             nqp = QPointF(qpf.x() - 6, qpf.y() - 8)
         super().setPos(nqp)
 
     def mousePressEvent(self, event):
         # In ygArrowHead
-        # This doesn't seem to be working. Why not?
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         is_left = event.button() == Qt.MouseButton.LeftButton
         self.parentItem()._process_click_on_hint(self, with_shift, is_left)
 
 
@@ -697,19 +688,17 @@
             box_ratio = xdistance / ydistance
         except ZeroDivisionError:
             box_ratio = 0
         # Generate a keyword to describe the shape of the box.
         if xdistance == 0 and ydistance == 0:
             self._shape = "invisible"
             self.arrow_axis = None
-        # elif box_ratio < 0.05:
         elif xdistance < 10:
             self._shape = "y only"
             self.arrow_axis = "y"
-        # elif box_ratio >= 1.0 and box_ratio <= 1.5:
         elif ydistance < 10:
             self._shape = "x only"
             self.arrow_axis = "x"
         elif box_ratio < 0.3333:
             self._shape = "tall"
             self.arrow_axis = "y"
         elif box_ratio > 3:
@@ -854,27 +843,27 @@
         is_left = event.button() == Qt.MouseButton.LeftButton
         self.parentItem()._process_click_on_hint(self, with_shift, is_left)  # type: ignore
 
 
 class ygHintButton(QGraphicsEllipseItem, ygGraphicalHintComponent):
     """A button to display mid-stem, to make an easy target for a mouse."""
 
-    def __init__(self, viewer: "ygGlyphScene", location: QPoint, hint: ygHint) -> None:
-        """viewer: a ygGlyphScene object
+    def __init__(self, yg_glyph_scene: "ygGlyphScene", location: QPoint, hint: ygHint) -> None:
+        """yg_glyph_scene: a ygGlyphScene object
         location: QPoint
         hint: ygModel.ygHint
         """
-        self.viewer = viewer
+        self.yg_glyph_scene = yg_glyph_scene
         self.diameter = HINT_BUTTON_DIA + 2
         loc_offset = self.diameter - (self.diameter / 2)
         self.location = QPointF(location.x() - loc_offset, location.y() - loc_offset)
         self.yg_hint = hint
         super().__init__(QRectF(self.location, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
-        self._prepare_graphics(is_selected=False, hint_type=self.yg_hint.hint_type())
+        self._prepare_graphics(is_selected=False, hint_type=self.yg_hint.hint_type)
 
     def _prepare_graphics(self, **kwargs) -> None:
         # for ygHintButton
         is_selected = kwargs["is_selected"]
         hint_type = kwargs["hint_type"]
         pen = QPen()
         brush = QBrush()
@@ -898,15 +887,15 @@
 
 
 class ygPointMarker(QGraphicsEllipseItem, ygGraphicalHintComponent):
     """pt has got to be a ygPointView."""
 
     def __init__(
         self,
-        viewer: "ygGlyphScene",
+        yg_glyph_scene: "ygGlyphScene",
         pt: "ygPointView",
         hint_type: str,
         name: str = None,
         id=None,
         parent=None,
     ):
         self.pt = pt
@@ -922,32 +911,29 @@
             self.diameter = POINT_OFFCURVE_DIA + 2
         super().__init__(QRectF(self.glocation, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
         self._prepare_graphics(is_selected=False, hint_type=hint_type)
         self.label_proxy = None
         if self.name != None:
             self._prepare_label()
-            self.label_proxy = viewer.addWidget(self.label)
-        self.viewer = viewer
+            self.label_proxy = yg_glyph_scene.addWidget(self.label)
+        self.yg_glyph_scene = yg_glyph_scene
 
     def _prepare_label(self) -> None:
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: gray;}")
         self.label.setText(str(self.name))
         self.label.move(round(self._x + self.diameter), round(self._y + self.diameter))
 
-    def _get_model_point(self) -> ygPoint:
-        return self.pt.yg_point
-
-    def _get_view_point(self):
-        return self.pt
+    #def _get_view_point(self):
+    #    return self.pt
 
     def _remove_labels(self):
         if self.label_proxy:
-            self.viewer.removeItem(self.label_proxy)
+            self.yg_glyph_scene.removeItem(self.label_proxy)
 
     def _prepare_graphics(self, **kwargs):
         # For ygPointMarker
         is_selected = kwargs["is_selected"]
         hint_type = kwargs["hint_type"]
         pen = QPen()
         pen.setWidth(HINT_ANCHOR_WIDTH)
@@ -957,16 +943,16 @@
                 self.label.show()
         else:
             pen.setColor(HINT_COLOR[hint_type])
             if self.label:
                 self.label.hide()
         self.setPen(pen)
 
-    def get_scene(self):
-        return self.viewer
+    #def get_scene(self) -> "ygGlyphScene":
+    #    return self.yg_glyph_scene
 
     def mousePressEvent(self, event):
         # In ygPointMarker
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         is_left = event.button() == Qt.MouseButton.LeftButton
@@ -987,41 +973,41 @@
 
 
 class ygPointCollectionView(QGraphicsItem, ygGraphicalHintComponent, ygPointable):
     """A graphical representation of a collection of points. Select by clicking
     one of the points, or by clicking the border.
 
     Parameters:
-    viewer (ygGlyphScene): The scene for this editing pane
+    yg_glyph_scene (ygGlyphScene): The scene for this editing pane
 
     yg_params (ygModel.ygParams): The collection of params for a function
     or macro
 
     hint_type (str): The type of this hint (it must be "function" or
     "macro")
 
     """
 
-    def __init__(self, viewer: "ygGlyphScene", *args) -> None:
+    def __init__(self, yg_glyph_scene: "ygGlyphScene", *args) -> None:
         super().__init__()
-        self.yg_viewer = viewer
+        self.yg_glyph_scene = yg_glyph_scene
         self.point_dict = {}
         if type(args[0]) is ygParams:
             self.yg_params = args[0]
             kk = self.yg_params.point_dict.keys()
             for k in kk:
-                self.point_dict[k] = viewer.resolve_point_identifier(
+                self.point_dict[k] = yg_glyph_scene.resolve_point_identifier(
                     self.yg_params.point_dict[k]
                 )
             self.hint_type = self.yg_params.hint_type
         else:
             point_list = args[0]
             self.hint_type = args[1]
             for p in point_list:
-                pp = viewer.resolve_point_identifier(p)
+                pp = yg_glyph_scene.resolve_point_identifier(p)
                 if type(pp) is ygPoint:
                     self.point_dict[pp.preferred_label()] = pp
                 elif type(pp) is ygSet:
                     self.point_dict[pp.main_point().preferred_label()] = pp.main_point()
         self.point_markers = self._make_point_markers()
         lines, self.rect = self._boundingLines()
         self.borders = []
@@ -1052,19 +1038,19 @@
     def visible_objects(self):
         return self.point_markers + self.borders
 
     def _make_point_markers(self):
         kk = self.point_dict.keys()
         marker_list = []
         for k in kk:
-            p = self.yg_viewer.resolve_point_identifier(self.point_dict[k])
+            p = self.yg_glyph_scene.resolve_point_identifier(self.point_dict[k])
             if type(p) is ygSet:
                 p = p.main_point()
-            ptv = self.yg_viewer.yg_point_view_index[p.id]
-            h = ygPointMarker(self.yg_viewer, ptv, self.hint_type, name=k)
+            ptv = self.yg_glyph_scene.yg_point_view_index[p.id]
+            h = ygPointMarker(self.yg_glyph_scene, ptv, self.hint_type, name=k)
             marker_list.append(h)
         return marker_list
 
     def paint(self, painter, option, widget):
         """Got to be here, but it doesn't have to do anything."""
         pass
 
@@ -1154,134 +1140,131 @@
         is_left = event.button() == Qt.MouseButton.LeftButton
         self.parentItem()._process_click_on_hint(self, with_shift, is_left)  # type: ignore
 
 
 class ygSetView(ygPointCollectionView):
     """A graphical representation of a list of points."""
 
-    def __init__(self, viewer: "ygGlyphScene", yg_set: ygSet, hint_type: str) -> None:
-        super().__init__(viewer, yg_set.point_list(), hint_type)
-        self.viewer = viewer
+    def __init__(self, yg_glyph_scene: "ygGlyphScene", yg_set: ygSet, hint_type: str) -> None:
+        super().__init__(yg_glyph_scene, yg_set.point_list, hint_type)
+        self.yg_glyph_scene = yg_glyph_scene
         self.hint_type = hint_type
 
 
 class ygSelection(QObject):
     """A list of selected objects (points, hints, or both).
 
     The class has functions for manipulating the list.
     """
 
     sig_selection_changed = pyqtSignal(object)
 
-    def __init__(self, viewer: "ygGlyphScene") -> None:
+    def __init__(self, yg_glyph_scene: "ygGlyphScene") -> None:
         super().__init__()
         self.selected_objects: list = []
-        self.viewer = viewer
+        self.yg_glyph_scene = yg_glyph_scene
 
     def setup_selection_signal(self, f: Optional[Callable]) -> None:
         self.sig_selection_changed.connect(f)
 
-    def get_scene(self) -> "ygGlyphScene":
-        return self.viewer
+    #def get_scene(self) -> "ygGlyphScene":
+    #    return self.yg_glyph_scene
 
     def send_signal(self) -> None:
-        self.sig_selection_changed.emit(self.viewer.selection_profile())
+        self.sig_selection_changed.emit(self.yg_glyph_scene.selection_profile())
 
     def _cancel_selection(self, emit_signal: bool = True) -> None:
         for p in self.selected_objects:
-            if p._is_yg_selected:
+            if p.selected:
                 p.yg_unselect()
                 p._prepare_graphics()
                 p.update()
         self.selected_objects = []
-        self.viewer.update()
+        self.yg_glyph_scene.update()
         if emit_signal:
-            self.sig_selection_changed.emit(self.viewer.selection_profile())
+            self.send_signal()
+            #self.sig_selection_changed.emit(self.yg_glyph_scene.selection_profile())
 
     def _add_object(self, obj: ygSelectable, add_to_selection: bool) -> None:
         if not add_to_selection:
             self._cancel_selection(emit_signal=False)
         # Not sure what to do about next line. Study Protocol further?
         # isVisible is inherited from QGraphicsItem, and here we look
         # both at that and at things inherited from ygSelectable.
         if obj.isVisible():  # type: ignore
             obj.yg_select()
             self.selected_objects.append(obj)
             obj._prepare_graphics()
             obj.update()
-        self.sig_selection_changed.emit(self.viewer.selection_profile())
-
-    # This is never called.
-    # def _cancel_object(self, obj):
-    #     obj.yg_unselect()
-    #     self.selected_objects.remove(obj)
-    #     obj._prepare_graphics()
-    #     obj.update()
-    #     self.sig_selection_changed.emit(self.viewer.selection_profile())
+        self.send_signal()
+        # self.sig_selection_changed.emit(self.yg_glyph_scene.selection_profile())
 
     def _toggle_object(self, obj: ygSelectable) -> None:
         # Problem as in _add_object above.
         if not obj.isVisible():  # type: ignore
             return
-        if obj._is_yg_selected():
+        if obj.selected():
             obj.yg_unselect()
             self.selected_objects.remove(obj)
         else:
             obj.yg_select()
             self.selected_objects.append(obj)
         obj._prepare_graphics()
         obj.update()
-        self.sig_selection_changed.emit(self.viewer.selection_profile())
+        self.send_signal()
+        # self.sig_selection_changed.emit(self.yg_glyph_scene.selection_profile())
 
     def _add_rect(self, rect: QRectF, add_to_selection: bool) -> None:
         """This method of selecting doesn't work on hints."""
         if not add_to_selection:
             self._cancel_selection()
-        for ptv in self.viewer.yg_point_view_list:
+        for ptv in self.yg_glyph_scene.yg_point_view_list:
             if ptv.isVisible() and rect.contains(ptv.glocation):
                 ptv.yg_select()
                 self.selected_objects.append(ptv)
                 ptv._prepare_graphics()
                 ptv.update()
-        self.sig_selection_changed.emit(self.viewer.selection_profile())
+        self.send_signal()
+        #self.sig_selection_changed.emit(self.yg_glyph_scene.selection_profile())
 
     def _toggle_rect(self, rect: QRectF) -> None:
         """This method of selecting doesn't work on hints."""
-        for ptv in self.viewer.yg_point_view_list:
+        for ptv in self.yg_glyph_scene.yg_point_view_list:
             if ptv.isVisible() and rect.contains(ptv.glocation):
-                if ptv._is_yg_selected():
+                if ptv.selected():
                     ptv.yg_unselect()
                 else:
                     ptv.yg_select()
-                if ptv._is_yg_selected():
+                if ptv.selected():
                     self.selected_objects.append(ptv)
                 else:
                     self.selected_objects.remove(ptv)
                 ptv._prepare_graphics()
                 ptv.update()
-        self.sig_selection_changed.emit(self.viewer.selection_profile())
+        self.send_signal()
+        # self.sig_selection_changed.emit(self.yg_glyph_scene.selection_profile())
 
 
 class ygPointView(QGraphicsEllipseItem, ygSelectable, ygPointable):
     """A visible point"""
 
-    def __init__(self, viewer: "ygGlyphScene", yg_point: ygPoint):
-        self._is_selected = False
+    def __init__(self, yg_glyph_scene: "ygGlyphScene", yg_point: ygPoint):
+        self._selected = False
         self.yg_point = yg_point
         if yg_point.on_curve:
             self.diameter = POINT_ONCURVE_DIA
         else:
             self.diameter = POINT_OFFCURVE_DIA
         # glocation is a QPointF. Initialize at 0,0: must be set later.
         self.glocation = QPointF(0, 0)
         super().__init__(QRectF(self.glocation, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
         self.border_width = 1
         self.index = -1
-        self.viewer = viewer
+        self.yg_glyph_scene = yg_glyph_scene
         self.point_number_label: Optional[QLabel] = None
         self.point_number_label_proxy: Optional[QGraphicsProxyWidget] = None
         self.touched = False
         # These are the ygHintView objects that touch this point. When a hint
         # is removed from ygGlyphScene, remove the reference from this list.
         # If a hint being removed makes this list empty, remove the "touched"
         # flag from this ygPointView.
@@ -1291,15 +1274,15 @@
         return self.glocation
 
     def center_point(self) -> QPointF:
         return self.glocation
 
     def _prepare_graphics(self) -> None:
         # For ygPointView
-        if self._is_yg_selected():
+        if self.selected():
             if self.yg_point.on_curve:
                 brushColor = POINT_ONCURVE_SELECTED
             else:
                 brushColor = POINT_OFFCURVE_SELECTED
         else:
             brushColor = POINT_ONCURVE_FILL
         if self.yg_point.on_curve:
@@ -1308,16 +1291,16 @@
             penColor = POINT_OFFCURVE_OUTLINE
         pen = QPen(penColor)
         pen.setWidth(self.border_width)
         brush = QBrush(brushColor)
         self.setBrush(brush)
         self.setPen(pen)
 
-    def get_scene(self) -> "ygGlyphScene":
-        return self.viewer
+    #def get_scene(self) -> "ygGlyphScene":
+    #    return self.yg_glyph_scene
 
     def has_label(self) -> bool:
         return self.point_number_label != None
 
     def add_label(self) -> None:
         """Adds a label for this point. The label is supplied by the model
         point, which will supply an index, a pair of coordinates, or a
@@ -1328,56 +1311,56 @@
         self.point_number_label = QLabel()
         self.point_number_label.setStyleSheet(
             "QLabel {background-color: transparent; color: red; font-size: 90%}"
         )
         self.point_number_label.setText(
             str(self.yg_point.preferred_label(normalized=True))
         )
-        self.point_number_label_proxy = self.viewer.addWidget(self.point_number_label)
+        self.point_number_label_proxy = self.yg_glyph_scene.addWidget(self.point_number_label)
         label_x = self.glocation.x() + self.diameter
         label_y = self.glocation.y() - self.point_number_label.height()
         self.point_number_label.move(round(label_x), round(label_y))
 
     def del_label(self) -> None:
         if self.point_number_label:
-            self.viewer.removeItem(self.point_number_label_proxy)
+            self.yg_glyph_scene.removeItem(self.point_number_label_proxy)
             self.point_number_label = None
             self.point_number_label_proxy = None
 
     def update(self):
         pass
 
-    def _is_yg_selected(self) -> bool:
-        return self._is_selected
+    def selected(self) -> bool:
+        return self._selected
 
     def yg_select(self) -> None:
-        self._is_selected = True
+        self._selected = True
         self._prepare_graphics()
         self.update()
 
     def yg_unselect(self) -> None:
-        self._is_selected = False
+        self._selected = False
         self._prepare_graphics()
         self.update()
 
     def contains(self, p: QPointF) -> bool:
         return self.mapToScene(self.boundingRect()).boundingRect().contains(p)
 
     def mousePressEvent(self, event) -> None:
         # In ygPointView
         # Select when clicked, eiher adding to or replacing current selection.
         modifier = QApplication.keyboardModifiers()
         if (
             modifier & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier:
             if event.button() == Qt.MouseButton.LeftButton:
-                self.viewer.yg_selection._toggle_object(self)
+                self.yg_glyph_scene.yg_selection._toggle_object(self)
         else:
             if event.button() == Qt.MouseButton.LeftButton:
-                self.viewer.yg_selection._add_object(self, False)
+                self.yg_glyph_scene.yg_selection._add_object(self, False)
 
 
 class SelectionRect(QGraphicsRectItem):
     """The rubber band that appears while dragging to select points."""
 
     def __init__(self, qr: QRectF) -> None:
         super(SelectionRect, self).__init__(qr)
@@ -1388,15 +1371,14 @@
     """The workspace.
 
     Holds all the visible items belonging to hints.
 
     """
 
     sig_new_hint = pyqtSignal(object)
-    # sig_viewer_ready = pyqtSignal()
     sig_reverse_hint = pyqtSignal(object)
     sig_change_hint_color = pyqtSignal(object)
     sig_off_curve_visibility = pyqtSignal()
     sig_make_macfunc = pyqtSignal(object)
     sig_assign_macfunc_point = pyqtSignal(object)
     sig_edit_macfunc_params = pyqtSignal(object)
     sig_change_cv = pyqtSignal(object)
@@ -1457,19 +1439,19 @@
         self.setSceneRect(QRectF(0, 0, self.canvas_size[0], self.canvas_size[1]))
         self.xTranslate = self.canvas_size[2]
         self.yTranslate = self.canvas_size[3]
 
 
         # Try to get rid of ref to this scene in the model's ygGlyph class.
         # For now, we've got to ignore the type so as to avoid circular imports.
-        self.yg_glyph.glyph_viewer = self  # type: ignore
+        self.yg_glyph.yg_glyph_scene = self  # type: ignore
 
         # Make graphical points
 
-        for p in self.yg_glyph.points():
+        for p in self.yg_glyph.points:
             yg_point_view = ygPointView(self, p)
             self.yg_point_view_index[p.id] = yg_point_view
             self.yg_point_view_list.append(yg_point_view)
 
         # Set up dimensions; scale the glyph.
 
         self.adv = 0
@@ -1507,25 +1489,23 @@
         self.sig_change_cv.connect(self.change_cv)
         self.sig_reverse_hint.connect(self.reverse_hint)
         self.sig_swap_macfunc_points.connect(self.swap_macfunc_points)
         self.sig_change_hint_color.connect(self.change_hint_color)
         self.sig_edit_macfunc_params.connect(self.edit_macfunc_params)
         self.sig_off_curve_visibility.connect(self.toggle_off_curve_visibility)
         self.sig_make_macfunc.connect(self.make_macfunc)
-        # self.sig_macfunc_target.connect(self.macfunc_target)
-        # self.sig_macfunc_ref.connect(self.macfunc_ref)
         self.sig_toggle_point_numbers.connect(self.toggle_point_numbers)
         self.sig_set_category.connect(self.set_category)
         self.sig_round_hint.connect(self.toggle_hint_rounding)
         self.sig_min_dist.connect(self.toggle_min_dist)
         self.sig_name_points.connect(self.name_points)
 
         # Get and display the hints.
 
-        self.install_hints(self.yg_glyph.hints())
+        self.install_hints(self.yg_glyph.hints)
 
     #
     # Sizing and zooming
     #
 
     def size_report(self) -> None:
         """For diagnostics."""
@@ -1547,26 +1527,26 @@
         # We are ignoring the zoom_factor setting in the preferences now, in favor
         # of setting an optimal zoom factor in the __init__ of ygGlyphScene. Survey
         # uses of the preferences object to make sure this is so.
         self.preferences.top_window().zoom_factor = self.zoom_factor
         self.scale_glyph()
         self.center_x = self.xTranslate + round(self.adv / 2)
         self.update()
-        self.install_hints(self.yg_glyph.hints())
+        self.install_hints(self.yg_glyph.hints)
         # This will have the effect of moving point labels to the new positions
         # of the points. Affect only those already visible.
         for p in self.yg_point_view_list:
             if p.has_label():
                 p.add_label()
 
     def reset_scale(self) -> None:
         c = self.original_coordinates
         ft_font = self.yg_glyph.yg_font.ft_font
         ft_font["glyf"]._setCoordinates(
-            self.yg_glyph.glyph_name(), c, ft_font["hmtx"].metrics
+            self.yg_glyph.gname, c, ft_font["hmtx"].metrics
         )
 
     def scale_glyph(self) -> None:
         # Start out clean, with coordinates as in original font. That way,
         # zoom_factor always operates on the original, as opposed to the last
         # value.
         ft_font = self.yg_glyph.yg_font.ft_font
@@ -1580,34 +1560,34 @@
                 ft_font["glyf"]._getCoordinatesAndControls(
                     self.yg_glyph.gname, ft_font["hmtx"].metrics
                 )[0]
             )
         c = copy.deepcopy(self.original_coordinates)
         c.scale((self.zoom_factor, self.zoom_factor))
         ft_font["glyf"]._setCoordinates(
-            self.yg_glyph.glyph_name(), c, ft_font["hmtx"].metrics
+            self.yg_glyph.gname, c, ft_font["hmtx"].metrics
         )
         self.yg_glyph.ft_glyph.recalcBounds(self.yg_glyph.yg_font.ft_font["glyf"])
         self.adv, self.lsb = self.yg_glyph.yg_font.ft_font["hmtx"].metrics[
-            self.yg_glyph.glyph_name()
+            self.yg_glyph.gname
         ]
         self.canvas_size = self._calc_canvas_size()
         self.setSceneRect(QRectF(0, 0, self.canvas_size[0], self.canvas_size[1]))
         self.xTranslate = self.canvas_size[2]
         self.yTranslate = self.canvas_size[3]
         for c_index, cc in enumerate(c):
             try:
                 p = self.yg_point_view_list[c_index]
                 p.glocation = self._font2Qt(cc[0], cc[1], p.yg_point.on_curve)
                 p.setPos(p.glocation)
             except IndexError as e:
                 # fontTools coordinate list has phantom points at the end, which we ignore.
                 pass
 
-        glyph_set = {self.yg_glyph.glyph_name(): self.yg_glyph.ft_glyph}
+        glyph_set = {self.yg_glyph.gname: self.yg_glyph.ft_glyph}
         self.path = QPainterPath()
         self.qt_pen = QtPen(glyph_set, path=self.path)
         self.yg_glyph.ft_glyph.draw(self.qt_pen, self.yg_glyph.yg_font.ft_font["glyf"])
 
     def _calc_canvas_size(self) -> Tuple[int, int, int, int]:
         """This calculates a canvas that will do for the entire font. The result
         can be awkward (see the absurd situation in Junicode, which has an
@@ -1693,15 +1673,15 @@
         painter.translate(QPointF(self.xTranslate, self.yTranslate * -1))
 
         pen = painter.pen()
 
         if self.preferences["show_metrics"]:
             pen.setWidth(1)
             if self.dark_theme:
-                pen.setColor(QColor(200, 200, 200, 50))
+                pen.setColor(QColor(220, 220, 220, 75))
                 HINT_COLOR = _HINT_DARK
                 SELECTED_HINT_COLOR = _SELECTED_HINT_DARK
             else:
                 pen.setColor(QColor(50, 50, 50, 50))
                 HINT_COLOR = _HINT_COLOR
                 SELECTED_HINT_COLOR = _SELECTED_HINT_COLOR
             painter.setPen(pen)
@@ -1728,15 +1708,15 @@
         _selected_objects = self.selected_objects(False)
         selected_hint = None
         for s in _selected_objects:
             if type(s) is ygHintView or type(s) is ygHint:
                 selected_hint = self._model_hint(s)
                 break
         if selected_hint != None:
-            htn = self.get_hint_type_num(selected_hint.hint_type())
+            htn = self.get_hint_type_num(selected_hint.hint_type)
             cv_type = "pos"
             if htn == 3:
                 cv_type = "dist"
             cv_list = self.yg_glyph.yg_font.cvt.get_list(
                 self.yg_glyph,
                 type=cv_type,
                 axis=self.current_axis(),
@@ -1752,15 +1732,15 @@
                 pass
 
     def guess_cv_for_hint(self, hint: ygHint) -> None:
         """Like guess_cv(), but this is called as part of the process of constructing
         a hint, and therefore should not trigger a signal.
         """
         if hint != None:
-            htn = self.get_hint_type_num(hint.hint_type())
+            htn = self.get_hint_type_num(hint.hint_type)
             cv_type = "pos"
             if htn == 3:
                 cv_type = "dist"
             cv_list = self.yg_glyph.yg_font.cvt.get_list(
                 self.yg_glyph,
                 type=cv_type,
                 axis=self.current_axis(),
@@ -1776,15 +1756,15 @@
                 pass
 
     @pyqtSlot(object)
     def edit_macfunc_params(self, hint: ygHintView) -> None:
         ed_dialog = macfuncDialog(hint)
         r = ed_dialog.exec()
         if r == QDialog.DialogCode.Accepted:
-            hint.yg_hint.set_macfunc_other_args(ed_dialog.result_dict)
+            hint.yg_hint.macfunc_other_args = ed_dialog.result_dict
 
     @pyqtSlot()
     def toggle_off_curve_visibility(self) -> None:
         self.off_curve_points_showing = not self.off_curve_points_showing
         self.preferences.top_window().show_off_curve_points = (
             self.off_curve_points_showing
         )
@@ -1795,45 +1775,14 @@
                     if self.point_numbers_showing:
                         p.add_label()
                 else:
                     p.hide()
                     if self.point_numbers_showing:
                         p.del_label()
 
-    #def make_set(self) -> None:
-    #    """In the hint model, the target can be either a ygPoint or a ygSet.
-    #    This function takes the current selection, several ygPoint, and turns
-    #    them into a ygSet, which it substitutes for the ygPoint. Note that
-    #    exactly one selected point must be touched, and at least one
-    #    selected point must be untouched.
-    #    """
-    #    selected_points = self.selected_objects(True)
-    #    touched_points = []
-    #    untouched_points = []
-    #    for s in selected_points:
-    #        if s.touched:
-    #            touched_points.append(s)
-    #        else:
-    #            untouched_points.append(s)
-    #    if len(untouched_points) < 1 or len(touched_points) != 1:
-    #        return
-    #    touched_point = touched_points[0]
-    #    hint = touched_point.owners[0]
-    #    hint_model = hint.yg_hint
-    #    if not hint_model.hint_type() in ["shift", "align", "interpolate"]:
-    #        return
-    #    new_list = []
-    #    for p in selected_points:
-    #        new_list.append(self._model_point(p))
-    #    # params: ygModel.ygHint, list of ygModel.ygPoint, touched ygModel.ygPoint, callback func.
-    #    self.yg_glyph.make_set(
-    #        hint_model, new_list, touched_point.yg_point, hint._update_touches
-    #    )
-    #    self.yg_glyph.hint_changed(hint_model)
-
     def make_control_value(self) -> None:
         """ With one or two points selected, launch a dialog for making a pos or dist CV.
         """
         sel = self.selected_objects(True)
         if len(sel) == 0:
             return
         if len(sel) >= 1:
@@ -1863,14 +1812,19 @@
                 (
                     lambda: "coord"
                     if self.preferences.top_window().points_as_coords
                     else "index"
                 )()
             )
 
+    def untouch_all(self):
+        for p in self.yg_point_view_list:
+            p.touched = False
+            p.owners.clear()
+
     @pyqtSlot(object)
     def change_hint_color(self, _params: dict) -> None:
         _params["hint"].yg_hint.change_hint_color(_params["color"])
 
     @pyqtSlot(object)
     def toggle_hint_rounding(self, hint: ygHintView) -> None:
         self._model_hint(hint).toggle_rounding()
@@ -1958,18 +1912,20 @@
         hint_list: All the hints for either the y or the x axis
         for this glyph, in a list.
 
         """
         # Remove the old hints (destroying the ygHintView wrappers) and empty
         # out the list storing them.
         for h in self.yg_hint_view_list:
-            h._remove_touches()
             if h in self.items():
                 h._remove_labels()
                 self.removeItem(h)
+        # This may seem crazy, but it seems most reliable and stable if we
+        # delete all touch data and build it again.
+        self.untouch_all()
         self.yg_hint_view_list.clear()
         # The hints we get from the model are ygModel.ygHint objects, using
         # any legal Xgridfit identifier for the points. Wrap each one in a
         # ygHintView object.
         for h in hint_list:
             vh = self._make_visible_hint(h)
             self.yg_hint_view_list.append(vh)
@@ -2024,15 +1980,15 @@
             or len(profile[3]) != 0
         ):
             return
         selected_points = self.selected_objects(True)
         if len(selected_points) > 0:
             try:
                 owner_hint = None
-                hint_list = self.yg_glyph.hints()
+                hint_list = self.yg_glyph.hints
                 model_points = []
                 for p in selected_points:
                     model_points.append(self._model_point(p))
                 for h in hint_list:
                     if h.contains_points(model_points):
                         owner_hint = h
                         break
@@ -2043,21 +1999,21 @@
             except Exception as e:
                 pass
 
     #
     # Utilities
     #
 
-    def get_scene(self) -> "ygGlyphScene":
-        """Returns the current scene (always this object!)
-
-        Returns:
-        ygGlyphScene: this scene
-        """
-        return self
+    #def get_scene(self) -> "ygGlyphScene":
+    #    """Returns the current scene (always this object!)
+    #
+    #    Returns:
+    #    ygGlyphScene: this scene
+    #    """
+    #    return self
 
     def _mouse_over_point(self, qp: QPoint) -> ygPointView:
         """In ygGlyphScene. Determines whether the mouse is positioned over a point.
 
         Parameters:
         qp (QPos): The current position of the mouse
 
@@ -2123,26 +2079,26 @@
         s = self.selected_objects(True)
         touched_point_count = untouched_point_count = 0
         owner_types = []
         for ss in s:
             if ss.touched:
                 touched_point_count += 1
                 for h in ss.owners:
-                    htn = hint_type_nums[h.yg_hint.hint_type()]
+                    htn = hint_type_nums[h.yg_hint.hint_type]
                     if not htn in owner_types:
                         owner_types.append(htn)
             else:
                 untouched_point_count += 1
         selected_hint_types = []
         s = self.selected_objects(False)
         hint_count = 0
         for ss in s:
             if type(ss) is ygHintView:
                 hint_count += 1
-                htn = hint_type_nums[ss.yg_hint.hint_type()]
+                htn = hint_type_nums[ss.yg_hint.hint_type]
                 if not htn in selected_hint_types:
                     selected_hint_types.append(htn)
         return (
             touched_point_count,
             untouched_point_count,
             owner_types,
             selected_hint_types,
@@ -2206,15 +2162,15 @@
 
     def _model_point(self, p: Union[ygPointView, ygPoint]) -> ygPoint:
         if type(p) is ygPointView:
             return p.yg_point
         return p  # type: ignore
 
     def current_axis(self) -> str:
-        return self.yg_glyph.current_axis()
+        return self.yg_glyph.axis
 
     def _distance(
         self, pt_a: Union[ygPointView, ygPoint], pt_b: Union[ygPointView, ygPoint]
     ) -> int:
         """Returns the distance between two points (in font units) along
         the current axis.
         """
@@ -2236,44 +2192,44 @@
         hint (ygHint): The hint from the model
 
         Returns:
         ygHintView: The graphical hint, if one has been made (None if not)
 
         """
         # Make sure we've got the hint type
-        hint_type = hint.hint_type()
+        hint_type = hint.hint_type
         hint_type_num = self.get_hint_type_num(hint_type)
 
         # Build the visible hints
         if hint_type_num == 0:
             # 0 = draw a circle around a point.
-            target = self.resolve_point_identifier(hint.target())
+            target = self.resolve_point_identifier(hint.target)
             if type(target) is ygSet:
                 target = target.main_point()
             gtarget = self.yg_point_view_index[target.id]
             hpm = ygPointMarker(self, gtarget, "anchor")
             yg_hint_view = ygHintView(self, hint, hpm)
             yg_hint_view._touch_all_points()
             yg_hint_view._prepare_graphics()
             self.addItem(yg_hint_view)
         elif hint_type_num in [1, 3]:
             # With type 1, the target can be a set.
-            target = self.resolve_point_identifier(hint.target())
+            target = self.resolve_point_identifier(hint.target)
             if type(target) is ygSet:
                 gtarget = ygSetView(self, target, hint_type)
             else:
                 gtarget = self.yg_point_view_index[target.id]
             # *** If this is going to crash, need to catch it and recover. Maybe
             # mark the hint as invalid and skip it when drawing or compiling?
-            if hint.ref() == None:
+            if hint.ref == None:
                 print("Warning: ref is None (target is " + str(target) + ")")
-            ref = self.resolve_point_identifier(hint.ref())
+            ref = self.resolve_point_identifier(hint.ref)
             gref = self.yg_point_view_index[ref.id]
             ha = ygHintStem(
-                gref, gtarget, self.yg_glyph.current_axis(), hint_type, parent=self
+                gref, gtarget, self.yg_glyph.axis, hint_type, parent=self
             )
             hb = ygHintButton(self, ha.center_point(), hint)
             ah = ygArrowHead(
                 ha.endPoint(), ha.arrowhead_direction, hint_type, ha.id, parent=self
             )
             ah.setPos(ha.endPoint())
             glist = [ha, hb, ah]
@@ -2281,39 +2237,39 @@
                 glist.extend(gtarget.visible_objects())
             yg_hint_view = ygHintView(self, hint, glist)
             yg_hint_view._touch_all_points()
             yg_hint_view._prepare_graphics()
             self.addItem(yg_hint_view)
         elif hint_type_num == 2:
             # 2 = arrows from two reference points to one interpolated point or set
-            target = self.resolve_point_identifier(hint.target())
+            target = self.resolve_point_identifier(hint.target)
             if type(target) is ygSet:
                 gtarget = ygSetView(self, target, hint_type)
             else:
                 gtarget = self.yg_point_view_index[target.id]
-            ref_list = hint.ref()
+            ref_list = hint.ref
             if type(ref_list) is list:
                 ref_list = ygSet(ref_list)
-            if len(ref_list.point_list()) < 2:
+            if len(ref_list.point_list) < 2:
                 # This could come up with faulty code from the box, so handle it
                 # with an error dialog.
                 raise Exception(
                     "There must be two reference points for an interpolation hint"
                 )
             gref = []
-            ref_one = self.resolve_point_identifier(ref_list.point_list()[0])
-            ref_two = self.resolve_point_identifier(ref_list.point_list()[1])
+            ref_one = self.resolve_point_identifier(ref_list.point_list[0])
+            ref_two = self.resolve_point_identifier(ref_list.point_list[1])
             gref.append(self.yg_point_view_index[ref_one.id])
             gref.append(self.yg_point_view_index[ref_two.id])
             ha1 = ygHintStem(
-                gref[0], gtarget, self.yg_glyph.current_axis(), hint_type, parent=self
+                gref[0], gtarget, self.yg_glyph.axis, hint_type, parent=self
             )
             hb1 = ygHintButton(self, ha1.center_point(), hint)
             ha2 = ygHintStem(
-                gref[1], gtarget, self.yg_glyph.current_axis(), hint_type, parent=self
+                gref[1], gtarget, self.yg_glyph.axis, hint_type, parent=self
             )
             ah1 = ygArrowHead(
                 ha1.endPoint(), ha1.arrowhead_direction, hint_type, ha1.id, parent=self
             )
             hb2 = ygHintButton(self, ha2.center_point(), hint)
             ah2 = ygArrowHead(
                 ha2.endPoint(), ha2.arrowhead_direction, hint_type, ha2.id, parent=self
@@ -2325,19 +2281,19 @@
                 glist.extend(gtarget.visible_objects())
             yg_hint_view = ygHintView(self, hint, glist)
             yg_hint_view._touch_all_points()
             yg_hint_view._prepare_graphics()
             self.addItem(yg_hint_view)
         elif hint_type_num == 4:
             # Green anchors, surrounded by green border
-            gtarget = self.resolve_point_identifier(hint.target())
+            gtarget = self.resolve_point_identifier(hint.target)
             if type(gtarget) is ygParams:
-                gtarget.name = hint.macfunc_name()
+                gtarget.name = hint.macfunc_name
                 gtarget.hint_type = hint_type
-                gtarget.other_params = hint.macfunc_other_args()
+                gtarget.other_params = hint.macfunc_other_args
                 yg_params_view = ygPointCollectionView(self, gtarget)
                 yg_hint_view = ygHintView(self, hint, yg_params_view.visible_objects())
                 yg_hint_view._set_name(gtarget.name)
                 yg_hint_view._touch_all_points()
                 yg_hint_view._prepare_graphics()
                 self.addItem(yg_hint_view)
             else:
@@ -2353,15 +2309,15 @@
     def make_macfunc(self, _params: dict) -> None:
         hint_type = _params["hint_type"]
         name = _params["name"]
         self.make_macfunc_from_selection(hint_type, name=name)
         # Called function will send the signal to the model.
 
     def get_round_default(self, hint: ygHint) -> Optional[bool]:
-        t = hint.hint_type()
+        t = hint.hint_type
         l = self.yg_glyph.yg_font.defaults.get_default("round")
         if l != None:
             if t in l:
                 return True
         l = self.yg_glyph.yg_font.defaults.get_default("no-round")
         if l != None:
             if t in l:
@@ -2406,36 +2362,34 @@
                     print(e)
                 ref_name = ""
                 target_names = []
                 for ppp in pp:
                     if ppp.touched:
                         ref_name = self._model_point(ppp).preferred_label()
                     else:
-                        target_names.append(str(self._model_point(ppp).preferred_label()))
+                        target_names.append(self._model_point(ppp).preferred_label())
                 if len(target_names) == 1 or hint_type_num == 3:
                     tgt = target_names[0]
                 else:
                     tgt = target_names
                 # This should not happen if we've filtered properly before calling this.
-                if not ref_name or len(target_names) == 0:
+                if ref_name == "" or len(target_names) == 0:
                     return
                 h = {"ptid": tgt, "ref": ref_name, "rel": hint_type}
                 new_yg_hint = ygHint(self.yg_glyph, h)
                 dr = self.get_round_default(new_yg_hint)
                 if dr != None:
                     new_yg_hint.set_round(dr)
                 if ctrl and hint_type_num == 3:
                     self.guess_cv_for_hint(new_yg_hint)
                 if shift:
                     new_yg_hint.set_round(True)
                 self.sig_new_hint.emit(new_yg_hint)
         if hint_type_num == 2:
             if pplen >= 3:
-                #if pplen > 3:
-                #    del pp[3:]
                 # If two of the three selected points are touched, they are the
                 # reference points, and the untouched point is the target.
                 # Otherwise, sort the points by x or y position: the middle one
                 # is the target, and the ones on the ends are reference points.
                 # If the program makes the wrong choice, user can rearrange
                 # things in the editor.
                 touched_points = []
@@ -2460,15 +2414,15 @@
                     # Think about this more. Why does mypy not like it?
                     h = {"ptid": tgt, "ref": touched_names, "rel": hint_type}  # type: ignore
                     new_yg_hint = ygHint(self.yg_glyph, h)
                 else:
                     newlist = []
                     for p in pp:
                         newlist.append(self._model_point(p))
-                    sorter = ygPointSorter(self.yg_glyph.current_axis())
+                    sorter = ygPointSorter(self.yg_glyph.axis)
                     sorter.sort(newlist)
                     target = newlist.pop(1)
                     ref_names = [
                         newlist[0].preferred_label(),
                         newlist[1].preferred_label(),
                     ]
                     target_name = target.preferred_label()
@@ -2619,15 +2573,15 @@
         for v in unicode_cat_names.values():
             category_actions.append(set_category_menu.addAction(v))
 
         # "hint" will be None if the mouse pointer is not over a hint
 
         hint = self._mouse_over_hint(QPointF(event.scenePos()))
         try:
-            ntype = hint_type_nums[hint.yg_hint.hint_type()]
+            ntype = hint_type_nums[hint.yg_hint.hint_type]
         except Exception:
             ntype = 10
 
         cv_anchor_action_list = []
         cv_stem_action_list = []
         point_param_list = []
         black_space = white_space = gray_space = None
@@ -2638,25 +2592,25 @@
 
         round_hint = QAction("Round target point", checkable=True)  # type: ignore
         cmenu.addAction(round_hint)
         if hint == None or ntype == 4:
             round_hint.setEnabled(False)
             round_hint.setVisible(False)
         else:
-            if self._model_hint(hint).rounded():
+            if self._model_hint(hint).rounded:
                 round_hint.setChecked(True)
 
         min_dist_action = QAction("Minimum distance", checkable=True)  # type: ignore
         cmenu.addAction(min_dist_action)
         if hint == None or ntype != 3:
             min_dist_action.setEnabled(False)
             min_dist_action.setVisible(False)
         else:
             mh = self._model_hint(hint)
-            min_dist_action.setChecked(mh.min_dist())
+            min_dist_action.setChecked(mh.min_dist)
 
         # Set control value for anchor hint (ntype == 0)
 
         set_anchor_cv = cmenu.addMenu("Set control value...")
         cv_list = self.yg_glyph.yg_font.cvt.get_list(
             self.yg_glyph,
             type="pos",
@@ -2667,18 +2621,18 @@
         cv_list.sort()
         cv_list = ["None", "Guess"] + cv_list
 
         for c in cv_list:
             ccv = QAction(c, self, checkable=True)  # type: ignore
             if hint != None:
                 if ccv.text() == "None":
-                    if hint.yg_hint.cv() == None:
+                    if hint.yg_hint.cv == None:
                         ccv.setChecked(True)
                 else:
-                    if c == hint.yg_hint.cv():
+                    if c == hint.yg_hint.cv:
                         ccv.setChecked(True)
                 set_anchor_cv.addAction(ccv)
                 cv_anchor_action_list.append(ccv)
 
         if hint == None or ntype != 0:
             for c in cv_anchor_action_list:
                 c.setEnabled(False)
@@ -2700,18 +2654,18 @@
         cv_list.sort()
         cv_list = ["None", "Guess"] + cv_list
         # if len(cv_list) > 0:
         for c in cv_list:
             ccv = QAction(c, self, checkable=True)  # type: ignore
             if hint != None:
                 if ccv.text() == "None":
-                    if hint.yg_hint.cv() == None:
+                    if hint.yg_hint.cv == None:
                         ccv.setChecked(True)
                 else:
-                    if c == hint.yg_hint.cv():
+                    if c == hint.yg_hint.cv:
                         ccv.setChecked(True)
                 set_stem_cv.addAction(ccv)
                 cv_stem_action_list.append(ccv)
         if hint == None or ntype != 3:
             for c in cv_stem_action_list:
                 c.setEnabled(False)
                 c.setVisible(False)
@@ -2724,33 +2678,33 @@
 
         hint_color_menu = cmenu.addMenu("Set distance type...")
 
         no_color_menu = hint == None or ntype != 3
 
         black_space = QAction("Black", self, checkable=True)  # type: ignore
         if hint != None:
-            if hint.yg_hint.hint_type() in ["stem", "blackdist"]:
+            if hint.yg_hint.hint_type in ["stem", "blackdist"]:
                 black_space.setChecked(True)
         hint_color_menu.addAction(black_space)
         if no_color_menu:
             black_space.setEnabled(False)
             black_space.setVisible(False)
 
         white_space = QAction("White", self, checkable=True)  # type: ignore
         if hint != None:
-            if hint.yg_hint.hint_type() == "whitedist":
+            if hint.yg_hint.hint_type == "whitedist":
                 white_space.setChecked(True)
         hint_color_menu.addAction(white_space)
         if no_color_menu:
             white_space.setEnabled(False)
             white_space.setVisible(False)
 
         gray_space = QAction("Gray", self, checkable=True)  # type: ignore
         if hint != None:
-            if hint.yg_hint.hint_type() == "graydist":
+            if hint.yg_hint.hint_type == "graydist":
                 gray_space.setChecked(True)
         hint_color_menu.addAction(gray_space)
         if no_color_menu:
             gray_space.setEnabled(False)
             gray_space.setVisible(False)
 
         if no_color_menu:
@@ -2771,15 +2725,15 @@
         # Hide if no hint selected or hint is the wrong type or it has no non-
         # point parameters.
         if (
             hint == None
             or ntype != 4
             or len(
                 ygCaller(
-                    hint.yg_hint.hint_type(), hint.yg_hint.name, self.yg_glyph.yg_font
+                    hint.yg_hint.hint_type, hint.yg_hint.name, self.yg_glyph.yg_font
                 ).non_point_params()
             )
             == 0
         ):
             add_params.setEnabled(False)
             add_params.setVisible(False)
 
@@ -2790,20 +2744,20 @@
         # a ygPointView object.
         target_point = None
         swap_old_name = None
         point_list = []
         try:
             # mouse_over_point actually returns a ygPointMarker.
             target_point = hint.mouse_over_point(QPointF(event.scenePos()))
-            if hint.yg_hint.hint_type() == "macro":
+            if hint.yg_hint.hint_type == "macro":
                 mafu = ygMacro(hint.yg_hint.name, self.yg_glyph.yg_font)
-                point_list = mafu.point_list()
+                point_list = mafu.point_list
             else:
                 mafu = ygFunction(hint.yg_hint.name, self.yg_glyph.yg_font)  # type: ignore
-                point_list = mafu.point_list()
+                point_list = mafu.point_list
             swap_old_name = target_point.name
             point_list.remove(swap_old_name)
         except Exception as e:
             disable_point_params = True
         point_param_menu = cmenu.addMenu("Point params")
         for p in point_list:
             point_param_list.append(point_param_menu.addAction(p))
@@ -2817,46 +2771,23 @@
             a = point_param_menu.menuAction()
             a.setEnabled(False)
             a.setVisible(False)
 
         # Set a target or reference point for a function or macro. Only for use in ordering
         # hints: it has no effect on the rendering otherwise.
 
-        # The next few lines may be stranded. There used to be a "set target" menu item, but
-        # I removed it because it wasn't working, or was causing a crash, or something.
-
-        # if hint:
-        #     target_point = hint.mouse_over_point(QPointF(event.scenePos()))
-        #     if target_point != None:
-        #         target_point = target_point._get_model_point()
-        # else:
-        #     target_point = None
-        # new_target = target_point
-
-        # def tgt_pt_check(pt):
-        #    if pt == None:
-        #        return False
-        #    return self.resolve_point_identifier(pt) == target_point
-
-        # Make a set. Pointer can be anywhere for this.
-
-        # Test whether user can make a set. The rules are:
-        #    1. More than one point must be selected.
-        #    2. One selected point must be touched by a shift, align or
-        #       interpolate instruction (types 1 and 2).
-        #
         # Is this stranded code? We're no longer offering "Make Set" via the context menu,
         # and the point of this code seems to be to set a variable that's never consulted.
         touched_point = None
         num_of_selected_points = len(selected_points)
         try:
             if num_of_selected_points >= 2:
                 for p in selected_points:
                     if p.touched and len(p.owners) >= 1:
-                        if hint_type_nums[p.owners[0].yg_hint.hint_type()] in [1, 2]:
+                        if hint_type_nums[p.owners[0].yg_hint.hint_type] in [1, 2]:
                             touched_point = p
                             break
         except Exception:
             pass
 
         # Functions and macros. Each is marked for which params are points, which are control
         # values, and which are others. For each count up the point params and show only those
@@ -2958,18 +2889,14 @@
             self.sig_make_macfunc.emit({"hint_type": "macro", "name": action.text()})
         if action in function_actions:
             self.sig_make_macfunc.emit({"hint_type": "function", "name": action.text()})
         if action in point_param_list:
             self.sig_swap_macfunc_points.emit(
                 {"hint": hint, "new_pt": action.text(), "old_pt": swap_old_name}
             )
-        # if action == macfunc_target:
-        #    self.sig_macfunc_target.emit({"hint": hint, "pt": new_target})
-        # if action == macfunc_ref:
-        #    self.sig_macfunc_ref.emit({"hint": hint, "pt": new_target})
         if hint != None and action == round_hint:
             self.sig_round_hint.emit(hint)
         if hint != None and action == min_dist_action:
             self.sig_min_dist.emit(hint)
         if len(selected_points) > 0 and action == name_action:
             self.sig_name_points.emit(selected_points)
 
@@ -2977,15 +2904,15 @@
 class ygGlyphView(QGraphicsView):
     """The container for the graphical hint editor.
 
     It holds and displays an instance of ygGlyphScene; it will hold various
     buttons and controls, plus (I hope) a preview of the hinted glyph.
 
     Parameters:
-    viewer (ygGlyphScene): The QGraphicsScene that the user interacts with.
+    yg_glyph_scene (ygGlyphScene): The QGraphicsScene that the user interacts with.
 
     font (ygModel.ygFont): The font object, including both a fontTools Font
     object and the yaml file (as read by the Python yaml module). Has
     convenience functions supplying various kinds of information about the
     font.
 
     parent: Is this used at all?
@@ -2993,40 +2920,40 @@
 
     sig_goto = pyqtSignal(object)
     sig_toggle_drag_mode = pyqtSignal(object)
 
     def __init__(
         self,
         preferences: ygPreferences,
-        viewer: ygGlyphScene,
+        yg_glyph_scene: ygGlyphScene,
         font: ygFont,
         parent=None,
     ) -> None:
-        super(ygGlyphView, self).__init__(viewer, parent=parent)
+        super(ygGlyphView, self).__init__(yg_glyph_scene, parent=parent)
         self.setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
-        self.viewer = viewer
+        self.yg_glyph_scene = yg_glyph_scene
         self.yg_font = font
         self.preferences = preferences
         self.visited_glyphs: Dict[str, ygGlyphScene] = {}
         self.drag_mode_backup = QGraphicsView.DragMode.NoDrag
 
 
     @pyqtSlot()
     def make_control_value(self) -> None:
-        self.viewer.make_control_value()
+        self.yg_glyph_scene.make_control_value()
 
     def setup_goto_signal(self, o: Callable) -> None:
         self.sig_goto.connect(o)
 
     def setup_toggle_drag_mode_signal(self, o: Callable) -> None:
         self.sig_toggle_drag_mode.connect(o)
 
     def _current_index(self) -> int:
         return self.yg_font.get_glyph_index(
-            self.viewer.yg_glyph.gname, short_index=True
+            self.yg_glyph_scene.yg_glyph.gname, short_index=True
         )
 
     def go_to_glyph(self, g: str) -> None:
         self.preferences["top_window"].disconnect_editor_signals()
         try:
             self.yg_font.get_glyph_index(g, short_index=True)
             self.switch_to(g)
@@ -3058,67 +2985,66 @@
 
     def switch_from_font_viewer(self, gname: str) -> None:
         self.preferences["top_window"].disconnect_editor_signals()
         self.switch_to(gname)
         self.preferences["top_window"].connect_editor_signals()
 
     def switch_to(self, gname: str) -> None:
-        self.viewer.reset_scale()
-        self.viewer.yg_glyph.cleanup_glyph()
+        self.yg_glyph_scene.reset_scale()
+        self.yg_glyph_scene.yg_glyph.cleanup_glyph()
         # Store the current glyph if it is changed.
-        if not self.viewer.yg_glyph.undo_stack.isClean():
-            self.visited_glyphs[self.viewer.yg_glyph.gname] = self.viewer
+        if not self.yg_glyph_scene.yg_glyph.undo_stack.isClean():
+            self.visited_glyphs[self.yg_glyph_scene.yg_glyph.gname] = self.yg_glyph_scene
         if gname in self.visited_glyphs:
-            self.viewer = self.visited_glyphs[gname]
-            new_glyph = self.viewer.yg_glyph
+            self.yg_glyph_scene = self.visited_glyphs[gname]
+            new_glyph = self.yg_glyph_scene.yg_glyph
             # If we're returning to a glyph, we have to undo the cleanup
             # we did when we left it.
             new_glyph.undo_stack.setActive()
             new_glyph.restore_gsource()
         else:
             new_glyph = ygGlyph(self.preferences, self.yg_font, gname)
-            self.viewer = ygGlyphScene(self.preferences, new_glyph, owner = self)
-        self.preferences.set_current_glyph(self.yg_font.full_name(), gname)
-        self.setScene(self.viewer)
-        self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
+            self.yg_glyph_scene = ygGlyphScene(self.preferences, new_glyph, owner = self)
+        self.preferences.set_current_glyph(self.yg_font.full_name, gname)
+        self.setScene(self.yg_glyph_scene)
+        self.centerOn(self.yg_glyph_scene.center_x, self.sceneRect().center().y())
         self.parent().parent().set_window_title()  # type: ignore
         ed = self.preferences.top_window().source_editor
         new_glyph.set_yaml_editor(ed)
-        new_glyph.sig_hints_changed.emit(new_glyph.hints())
+        new_glyph.sig_hints_changed.emit(new_glyph.hints)
 
     @pyqtSlot()
     def guess_cv(self) -> None:
         try:
-            self.viewer.guess_cv()
+            self.yg_glyph_scene.guess_cv()
         except Exception:
             self.yg_font.send_error_message(
                 {"msg": "Error while looking for a control value.", "mode": "console"}
             )
 
     @pyqtSlot(bool)
     def switch_to_x(self, checked: bool) -> None:
-        if self.viewer:
-            if checked and self.viewer.yg_glyph.current_axis() != "x":
-                # self.viewer.axis = "x"
-                self.viewer.yg_glyph.switch_to_axis("x")
+        if self.yg_glyph_scene:
+            if checked and self.yg_glyph_scene.yg_glyph.axis != "x":
+                # self.yg_glyph_scene.axis = "x"
+                self.yg_glyph_scene.yg_glyph.switch_to_axis("x")
                 win = self.parent().parent()
                 win.set_window_title()  # type: ignore
 
     @pyqtSlot(bool)
     def switch_to_y(self, checked: bool) -> None:
-        if self.viewer:
-            if checked and self.viewer.yg_glyph.current_axis() != "y":
-                # self.viewer.axis = "y"
-                self.viewer.yg_glyph.switch_to_axis("y")
+        if self.yg_glyph_scene:
+            if checked and self.yg_glyph_scene.yg_glyph.axis != "y":
+                self.yg_glyph_scene.yg_glyph.switch_to_axis("y")
                 win = self.parent().parent()
                 win.set_window_title()  # type: ignore
 
     @pyqtSlot()
     def cleanup_yaml_code(self) -> None:
-        self.viewer.yg_glyph.rebuild_current_block()
+        self.yg_glyph_scene.yg_glyph.rebuild_current_block()
 
     @pyqtSlot()
     def make_hint_from_selection(self) -> None:
         menu_to_hint_type = {
             "Anchor (A)": "anchor",
             "Align (L)": "align",
             "Shift (H)": "shift",
@@ -3127,56 +3053,54 @@
         }
         with_ctrl = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ControlModifier
         ) == Qt.KeyboardModifier.ControlModifier
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
-        self.viewer.make_hint_from_selection(
+        self.yg_glyph_scene.make_hint_from_selection(
             menu_to_hint_type[self.sender().text()], ctrl=with_ctrl, shift=with_shift  # type: ignore
         )
 
-    #@pyqtSlot()
-    #def make_set(self) -> None:
-    #    self.viewer.make_set()
-
     # Why does sender return None when we use the decorator? What's best in this
     # situation? Here are problems: sender_text param is not consulted. Should it be
     # omitted? Make sure params match, esp. if we change them.
     # @pyqtSlot(object)
     def zoom(self, sender_text: str) -> None:
         sender_text = self.sender().text()  # type: ignore
         if sender_text == "Original Size":
-            self.viewer.set_zoom_factor(self.viewer.initial_zoom_factor)
+            self.yg_glyph_scene.set_zoom_factor(self.yg_glyph_scene.initial_zoom_factor)
         elif sender_text == "Zoom In":
-            if self.viewer.zoom_factor <= 5.75:
-                self.viewer.set_zoom_factor(self.viewer.zoom_factor + 0.25)
+            if self.yg_glyph_scene.zoom_factor <= 5.75:
+                self.yg_glyph_scene.set_zoom_factor(self.yg_glyph_scene.zoom_factor + 0.25)
         elif sender_text == "Zoom Out":
-            if self.viewer.zoom_factor >= 0.5:
-                self.viewer.set_zoom_factor(self.viewer.zoom_factor - 0.25)
-        self.centerOn(self.viewer.center_x, self.viewer.mid_point_y())
+            if self.yg_glyph_scene.zoom_factor >= 0.5:
+                self.yg_glyph_scene.set_zoom_factor(self.yg_glyph_scene.zoom_factor - 0.25)
+        self.centerOn(self.yg_glyph_scene.center_x, self.yg_glyph_scene.mid_point_y())
 
     def keyPressEvent(self, event) -> None:
         # 1. Delete key will delete any selected hints.
         # 2. Spacebar will shift Qt drag mode to ScrollHandDrag while it is
         #    down. For panning the screen.
+        # 3. Hyphen (minus) removes a target point from a hint.
+        # 4. Plus adds a point to a hint.
         if event.key() in [16777219, 16777223]:
-            self.viewer.delete_selected_hints()
+            self.yg_glyph_scene.delete_selected_hints()
         elif event.key() == Qt.Key.Key_Plus:
-            self.viewer.add_to_set()
+            self.yg_glyph_scene.add_to_set()
         elif event.key() == Qt.Key.Key_Minus:
-            self.viewer.delete_from_set()
+            self.yg_glyph_scene.delete_from_set()
         elif event.key() == 32 and not event.isAutoRepeat():
             self.drag_mode_backup = self.dragMode()
             if self.drag_mode_backup == QGraphicsView.DragMode.NoDrag:
                 self.sig_toggle_drag_mode.emit(QGraphicsView.DragMode.ScrollHandDrag)
 
     def keyReleaseEvent(self, event):
         # Releasting spacebar shifts Qt drag mode back to whatever it was before
         # spacebar was pressed.
         if event.key() == 32 and not event.isAutoRepeat():
             if self.drag_mode_backup != self.dragMode():
                 self.sig_toggle_drag_mode.emit(self.drag_mode_backup)
 
 
     def focusInEvent(self, event) -> None:
-        self.viewer.yg_glyph.undo_stack.setActive(True)
+        self.yg_glyph_scene.yg_glyph.undo_stack.setActive(True)
```

### Comparing `ygt-0.1.6/src/ygt/ygModel.py` & `ygt-0.2.0/src/ygt/ygModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,46 +84,46 @@
 unicode_cat_names = {
     "Lu": "Letter, uppercase",
     "Ll": "Letter, lowercase",
     "Lt": "Letter, titlecase",
     "LC": "Letter, cased",
     "Lm": "Letter, modifier",
     "Lo": "Letter, other",
-    "L": "Letter",
+    "L":  "Letter",
     "Mn": "Mark, nonspacing",
     "Mc": "Mark, spacing",
     "Me": "Mark, enclosing",
-    "M": "Mark",
+    "M":  "Mark",
     "Nd": "Number, decimal",
     "Nl": "Number, letter",
     "No": "Number, other",
-    "N": "Number",
+    "N":  "Number",
     "Pc": "Punctuation, connector",
     "Pd": "Punctuation, dash",
     "Ps": "Punctuation, open",
     "Pe": "Punctuation, close",
     "Pi": "Punctuation, initial quote",
     "Pf": "Punctuation, final quote",
     "Po": "Punctuation, other",
-    "P": "Punctuation",
+    "P":  "Punctuation",
     "Sm": "Symbol, math",
     "Sc": "Symbol, currency",
     "Sk": "Symbol, modifier",
     "So": "Symbol, other",
-    "S": "Symbol",
+    "S":  "Symbol",
     "Zs": "Separator, space",
     "Zl": "Separator, line",
     "Zp": "Separator, paragraph",
-    "Z": "Separator",
+    "Z":  "Separator",
     "Cc": "Other, control",
     "Cf": "Other, format",
     "Cs": "Other, surrogate",
     "Co": "Other, private use",
     "Cn": "Other, not assigned",
-    "C": "Other",
+    "C":  "Other",
 }
 
 INITIAL_CV_DELTA = {"size": 25, "distance": 0.0}
 
 reverse_unicode_cat_names = {v: k for k, v in unicode_cat_names.items()}
 
 # Error flags. These are set in the current ygGlyph when something has gone
@@ -188,26 +188,27 @@
 # setMacFuncOtherArgsCommand(glyphEditCommand): Glyph editing command.
 # swapMacFuncPointsCommand(glyphEditCommand): Glyph editing command.
 # cleanupGlyphCommand(glyphEditCommand): Glyph editing command.
 # changeDistanceTypeCommand(glyphEditCommand): Glyph editing command.
 # toggleMinDistCommand(glyphEditCommand): Glyph editing command.
 # changeCVCommand(glyphEditCommand): Glyph editing command.
 # toggleRoundingCommand(glyphEditCommand): Glyph editing command.
-# makeSetCommand(glyphEditCommand): Glyph editing command. (disabled -- perhaps not needed)
 # addHintCommand(glyphEditCommand): Glyph editing command.
 # deleteHintsCommand(glyphEditCommand): Glyph editing command.
 # reverseHintCommand(glyphEditCommand): Glyph editing command.
+# addPointsCommand(glyphEditCommand): Add point(s) to shift, align or interp. hint
+# deletePointsCommand(glyphEditCommand): Delete point(s) from shift, align or interp. hint
 # switchAxisCommand(QUndoCommand): Glyph editing command.
 # glyphAddPropertyCommand(QUndoCommand): Glyph editing command.
 # glyphDeletePropertyCommand(QUndoCommand): Glyph editing command.
 #
 #  Font objects (resumed):
 #
 # glyphSourceTester: Tests equality of object IDs.
-# ygGlyph(QObject): Keeps data for the current glyph.
+# ygGlyph(QObject): Keeps data for a glyph.
 # ygGlyphs: Collection of this font's glyphs.
 # Comparable: superclass for ygHintSource: for ordering hints.
 # ygHintSource(Comparable): Wrapper for hint source: use when sorting.
 # ygHint(QObject): One hint (including a function or macro call).
 # ygSourceable: Superclass for various chunks of ygt source code.
 # ygMasters: Collection of this font's masters
 # ygprep(ygSourceable): Holds the cvt program/pre-program.
@@ -270,15 +271,16 @@
                 y_stream.close()
             else:
                 ufo = ufoLib.UFOReader(self.filename)
                 if ufo.formatVersionTuple[0] == 3:
                     doc = ufo.readData("org.ygthinting/source.yaml")
                     self.y_doc = yaml.safe_load(doc)
 
-    def get_source(self) -> dict:
+    @property
+    def source(self) -> dict:
         return self.y_doc
 
     def save_source(self, top_window: Any = None) -> None:
         yy = yaml.dump(self.y_doc, sort_keys=False, width=float("inf"), Dumper=Dumper)
         if self.source_type == "yaml":
             f = open(self.filename, "w")
             f.write(yy)
@@ -301,23 +303,27 @@
 
     def __init__(self, source: dict) -> None:
         """Source is an internal representation of a yaml file, from which
         the names of the input and output font files can be retrieved.
         """
         self.data = source["font"]
 
+    @property
     def in_font(self) -> Optional[str]:
-        if "in" in self.data:
+        try:
             return self.data["in"]
-        return None
+        except KeyError:
+            return None
 
+    @property
     def out_font(self) -> Optional[str]:
-        if "out" in self.data:
+        try:
             return self.data["out"]
-        return None
+        except KeyError:
+            return None
 
 
 class ygFont(QObject):
     """Keeps all the font's data, including a fontTools representation of the
     font, the "source" structure built from the yaml file, and a structure
     for each section of the yaml file. All of the font data can be accessed
     through this class.
@@ -351,17 +357,17 @@
         if isinstance(source_file, str) and source_file:
             d = os.path.dirname(source_file)
         elif ygt_filename:
             d = os.path.dirname(ygt_filename)
         if d and os.path.isdir(d) and d != os.getcwd():
             os.chdir(d)
 
-        self.source = self.source_file.get_source()
+        self.source = self.source_file.source
         self.font_files = FontFiles(self.source)
-        fontfile = self.font_files.in_font()
+        fontfile = self.font_files.in_font
         if not fontfile:
             raise Exception("Need the name of an existing font")
             # Need to let user try again.
         split_fn = os.path.splitext(str(fontfile))
         extension = split_fn[1]
         ft_open_error = False
         if extension == ".ttf":
@@ -375,14 +381,19 @@
                 self.ft_font = compileTTF(ufo, useProductionNames=False, reverseDirection=False)
             except Exception as e:
                 print(e)
                 ft_open_error = True
         if ft_open_error:
             raise Exception("Can't find font file " + str(fontfile))
             # Fix this! Need a dialog box and a chance to try again for a valid font.
+            #
+            # Do this: open a file dialog for locating the font file, and place this
+            # in the SourceFile object. If user doesn't choose a font, then close
+            # this window (send signal to top_window?). The application can continue
+            # if other windows are open.
 
         # Making a deepcopy so we can always have a clean copy of the font to work with.
         self.preview_font = copy.deepcopy(self.ft_font)
 
         #
         # If it's a variable font, get instances and axes
         #
@@ -594,29 +605,31 @@
         self.sig_error.emit(d)
 
     @pyqtSlot()
     def refresh_variant_cvs(self):
         if self.is_variable_font:
             instanceChecker(self.preview_font, self.cvt, self.masters).refresh()
 
+    @property
     def default_instance(self) -> Optional[str]:
         if not self.is_variable_font:
             return None
         default_coordinates = {}
         for a in self.axes:
             default_coordinates[a.axisTag] = a.defaultValue
         def_inst = None
         kk = self.instances.keys()
         for k in kk:
             if self.instances[k] == default_coordinates:
                 def_inst = k
                 break
         return def_inst
 
-    def axis_tags(self):
+    @property
+    def axis_tags(self) -> list:
         result = []
         for a in self.axes:
             result.append(a.axisTag)
         return result
 
     def get_unicode(self, glyph_name: str, extended: bool = False) -> int:
         u: Optional[Union[set, int]] = None
@@ -646,22 +659,25 @@
                 pass
         return c
 
     def extreme_points(self, glyph_name: str) -> tuple[tuple, tuple]:
         """Helper for setting up an initial cvt."""
         return ygGlyph(ygPreferences(), self, glyph_name).extreme_points_y()
 
+    @property
     def family_name(self) -> str:
-        return self.ft_font["name"].getName(1, 3, 1, 0x409)
+        return str(self.ft_font["name"].getName(1, 3, 1, 0x409))
 
+    @property
     def style_name(self) -> str:
-        return self.ft_font["name"].getName(2, 3, 1, 0x409)
+        return str(self.ft_font["name"].getName(2, 3, 1, 0x409))
 
+    @property
     def full_name(self) -> str:
-        return str(self.family_name()) + "-" + str(self.style_name())
+        return self.family_name + "-" + self.style_name
 
     def set_dirty(self) -> None:
         self._clean = False
         self.main_window.set_window_title()
 
     def set_clean(self) -> None:
         self._clean = True
@@ -790,14 +806,15 @@
                 and "type" in self.data[k]
                 and not "val" in self.data[k]
             ):
                 if self.data[k]["type"] == "point":
                     min_count += 1
         return range(min_count, max_count + 1)
 
+    @property
     def point_list(self) -> list:
         """Get a list of points (identifiers, not objects) from the dict of
         this callable's parameters.
 
         """
         plist = []
         keys = self.data.keys()
@@ -895,23 +912,28 @@
 
     def preferred_label(
         self, normalized: bool = False, name_allowed: bool = True
     ) -> str | int:
         if name_allowed:
             if len(self.preferred_name) > 0:
                 return self.preferred_name
-        if self.label_pref == "coord":
+        # Coordinate IDs only allowed for on-curve points.
+        if self.label_pref == "coord" and self.on_curve:
             if normalized:
                 t = self.coord.replace("{", "")
                 t = t.replace("}", "")
                 t = t.replace(";", ",")
                 return t
             else:
                 return self.coord
-        return self.index
+        try:
+            return int(self.index)
+        except TypeError:
+            print("TypeError: " + str(self.index))
+            return str(self.index)
 
     def set_preferred_name(self, n: str) -> None:
         self.preferred_name = n
 
     def __eq__(self, other) -> bool:
         try:
             return self.id == other.id
@@ -937,14 +959,15 @@
         other_params: Optional[dict],
     ) -> None:
         self.hint_type = hint_type
         self.name = name
         self.point_dict = point_dict
         self.other_params = other_params
 
+    @property
     def point_list(self) -> list:
         result = []
         k = self.point_dict.keys()
         for kk in k:
             result.append(self.point_dict[kk])
         return result
 
@@ -976,22 +999,23 @@
         self._point_list = point_list
         self.id = uuid.uuid1()
         # The main point is the one the arrow is connected to. It shouldn't be
         # needed now, but the editor uses it against the possibility that a set
         # will contain another set. See if this can be safely removed.
         self._main_point: Optional[ygPoint] = None
 
+    @property
     def point_list(self) -> list:
         return self._point_list
 
-    def id_list(self) -> list:
-        l = []
-        for p in self._point_list:
-            l.append(p.preferred_label())
-        return l
+    #def id_list(self) -> list:
+    #    l = []
+    #    for p in self._point_list:
+    #        l.append(p.preferred_label())
+    #    return l
 
     def main_point(self) -> ygPoint:
         """Our use of an on-screen box may have made this useless. See if we
         can get rid of it.
 
         """
         if self._main_point:
@@ -1016,15 +1040,15 @@
                         return True
         return False
 
     def overlaps(self, tester: "ygSet") -> list:
         result: list = []
         if type(tester) is not ygSet:
             return result
-        pts = tester.point_list()
+        pts = tester.point_list
         for pt in pts:
             if pt in self:
                 result.append(pt)
         return result
     
     def __str__(self):
         result = "["
@@ -1034,39 +1058,29 @@
             result += str(p.index)
         result += "]"
         return result
 
 #
 # Undo / Redo
 #
-# One helper class(glyphSaver) and several subclasses of QUndoCommand. Each glyph has its
-# own QUndoStack, and these are coordinated at the app level by one QUndoGroup.
+# Two helper classes (glyphSaver and fontInfoSaver) and several subclasses of QUndoCommand.
+# Each glyph has its own QUndoStack, and these are coordinated at the app level by one
+# QUndoGroup.
 #
 # The regular sequence is: (1) The constructor takes a snapshot of the current state
-# of the glyph program (via glyphSaver); (2) An editing action is performed (in .redo(),
-# which Qt calls when a command is added to the stack--so the command's actual work is
-# done there) and another snapshot is taken of the result; (3) on undo, the snapshot
+# of the code (via glyphSaver or fontInfoSaver); (2) An editing action is performed (in
+# .redo, which Qt calls when a command is added to the stack--so the command's actual work
+# is done there) and another snapshot is taken of the result; (3) on undo, the snapshot
 # taken in (1) is swapped in for the current state of the glyph program; (4) on redo,
 # the snapshot taken in (2) is swapped in.
 #
 # As a typical glyph program takes up 200-400 bytes in memory, this isn't as wasteful of
 # memory as it sounds; and it definitely keeps things simple. There are some variations on
 # the sequence.
 #
-# At the glyph level, undos are all implemented.
-#
-# To do at the font level:
-#
-# Edit cvt
-# Edit prep
-# Edit fpgm
-# Edit cvar
-# Edit macros
-# Edit defaults
-#
 
 
 class glyphSaver:
     """Helper for many glyph commands."""
 
     def __init__(self, g: "ygGlyph") -> None:
         self.yg_glyph = g
@@ -1145,15 +1159,15 @@
         self.yg_glyph = self.yg_font.main_window.current_glyph()
         self.undo_state = fontInfoSaver(self.yg_font)
         self.redo_state: Union[fontInfoSaver, None] = None
 
     def send_signal(self) -> None:
         if self.yg_font.signal_connected:
             self.yg_font.sig_cvt_changed.emit()
-            self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints())
+            self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints)
 
     def redo(self) -> None:
         pass
 
     def undo(self) -> None:
         self.undo_state.restore()
         self.send_signal()
@@ -1171,15 +1185,15 @@
     def __init__(self, glyph: "ygGlyph") -> None:
         super().__init__()
         self.yg_glyph = glyph
         self.undo_state = glyphSaver(self.yg_glyph)
         self.redo_state: Union[glyphSaver, None] = None
 
     def send_signal(self) -> None:
-        self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints())
+        self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints)
         self.yg_glyph.send_yaml_to_editor()
 
     def redo(self) -> None:
         pass
 
     def undo(self) -> None:
         self.undo_state.restore()
@@ -1541,15 +1555,15 @@
             self.setText("Coords to Indices")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
             self.yg_glyph.sub_coords(
-                self.yg_glyph.current_block(), to_coords=self.to_coords
+                self.yg_glyph.current_block, to_coords=self.to_coords
             )
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "changePointNumbersCommand").test()
         self.send_signal()
 
 
 class updateSourceCommand(glyphEditCommand):
@@ -1560,21 +1574,21 @@
         self.setText("Compile Glyph Program")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
             try:
-                self.yg_glyph.gsource[self.yg_glyph.current_axis()]["points"].clear()
+                self.yg_glyph.gsource[self.yg_glyph.axis]["points"].clear()
                 for ss in self.s:
-                    self.yg_glyph.gsource[self.yg_glyph.current_axis()][
+                    self.yg_glyph.gsource[self.yg_glyph.axis][
                         "points"
                     ].append(ss)
-                self.yg_glyph._yaml_add_parents(self.yg_glyph.current_block())
-                self.yg_glyph._yaml_supply_refs(self.yg_glyph.current_block())
+                self.yg_glyph._yaml_add_parents(self.yg_glyph.current_block)
+                self.yg_glyph._yaml_supply_refs(self.yg_glyph.current_block)
             except Exception as e:
                 print(e)
                 self.undo_state.restore()
                 self.valid = False
         self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "updateSourceCommand").test()
         if self.valid:
@@ -1680,15 +1694,15 @@
         self.new_params = new_params
         self.setText("Edit parameters")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
-            self.hint._source[self.hint.hint_type()] = self.new_params
+            self.hint.source[self.hint.hint_type] = self.new_params
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "setMacFuncOtherArgsCommand").test()
         self.send_signal()
 
 
 class swapMacFuncPointsCommand(glyphEditCommand):
     def __init__(
@@ -1700,28 +1714,28 @@
         self.old_name = old_name
         self.setText("Swap Mac/Func points")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
-            if type(self.hint._source["ptid"]) is dict:
+            if type(self.hint.source["ptid"]) is dict:
                 try:
                     (
-                        self.hint._source["ptid"][self.new_name],
-                        self.hint._source["ptid"][self.old_name],
+                        self.hint.source["ptid"][self.new_name],
+                        self.hint.source["ptid"][self.old_name],
                     ) = (
-                        self.hint._source["ptid"][self.old_name],
-                        self.hint._source["ptid"][self.new_name],
+                        self.hint.source["ptid"][self.old_name],
+                        self.hint.source["ptid"][self.new_name],
                     )
                 except Exception as e:
-                    self.hint._source["ptid"][self.new_name] = self.hint._source[
+                    self.hint.source["ptid"][self.new_name] = self.hint._source[
                         "ptid"
                     ][self.old_name]
-                    del self.hint._source["ptid"][self.old_name]
+                    del self.hint.source["ptid"][self.old_name]
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "swapMacFuncPointsCommand").test()
         self.send_signal()
 
 
 class cleanupGlyphCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph") -> None:
@@ -1745,15 +1759,15 @@
         self.new_color = new_color
         self.setText("Change distance type")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
-            self.hint._source["rel"] = self.new_color
+            self.hint.source["rel"] = self.new_color
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "changeDistanceTypeCommand").test()
         self.send_signal()
 
 
 class toggleMinDistCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph", hint: "ygHint") -> None:
@@ -1761,20 +1775,20 @@
         self.hint = hint
         self.setText("Toggle Minimum Distance")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
-            current_min_dist = not self.hint.min_dist()
+            current_min_dist = not self.hint.min_dist
             if current_min_dist == self.hint.min_dist_is_default():
-                if "min" in self.hint._source:
-                    del self.hint._source["min"]
+                if "min" in self.hint.source:
+                    del self.hint.source["min"]
             else:
-                self.hint._source["min"] = current_min_dist
+                self.hint.source["min"] = current_min_dist
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "toggleMinDistCommand").test()
         self.send_signal()
 
 
 class changeCVCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph", hint: "ygHint", new_cv: str) -> None:
@@ -1796,73 +1810,42 @@
 class toggleRoundingCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph", hint: "ygHint") -> None:
         super().__init__(glyph)
         self.hint = hint
         self.setText("Toggle Rounding")
 
     def redo(self) -> None:
-        current_round = not self.hint.rounded()
+        current_round = not self.hint.rounded
         if self.redo_state:
             self.redo_state.restore()
         else:
             if current_round == self.hint.round_is_default():
-                if "round" in self.hint._source:
-                    del self.hint._source["round"]
+                if "round" in self.hint.source:
+                    del self.hint.source["round"]
             else:
-                self.hint._source["round"] = current_round
+                self.hint.source["round"] = current_round
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "toggleRoundingCommand").test()
         self.send_signal()
 
 
-#class makeSetCommand(glyphEditCommand):
-#    def __init__(
-#        self,
-#        glyph: "ygGlyph",
-#        hint: "ygHint",
-#        pt_list: list,
-#        touched_point: Optional[ygPoint],
-#        callback: Callable,
-#    ) -> None:
-#        super().__init__(glyph)
-#        self.hint = hint
-#        self.pt_list = pt_list
-#        self.touched_point = touched_point
-#        self.callback = callback
-#        self.setText("Make Set")
-#
-#    def redo(self) -> None:
-#        if self.redo_state:
-#            self.redo_state.restore()
-#        else:
-#            sorter = ygPointSorter(self.yg_glyph.current_axis())
-#            sorter.sort(self.pt_list)
-#            set = ygSet(self.pt_list)
-#            set._main_point = self.touched_point
-#            self.hint.set_target(set.id_list())
-#            self.callback()
-#            self.redo_state = glyphSaver(self.yg_glyph)
-#        glyphSourceTester(self.yg_glyph, "makeSetCommand").test()
-#        self.send_signal()
-
-
 class addHintCommand(glyphEditCommand):
     def __init__(
         self, glyph: "ygGlyph", hint: "ygHint", conditional: bool = False
     ) -> None:
         super().__init__(glyph)
         self.hint = hint
         self.conditional = conditional
         self.setText("Add Hint")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
-            self.yg_glyph._add_hint(self.hint, self.yg_glyph.current_block())
+            self.yg_glyph._add_hint(self.hint, self.yg_glyph.current_block)
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "addHintCommand").test()
         self.send_signal()
 
 
 class deleteHintsCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph", l: list) -> None:
@@ -1871,23 +1854,23 @@
         self.setText("Delete Hints")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
             for h in self.hint_list:
-                s = h._source
+                s = h.source
                 if "parent" in s:
                     try:
                         s["parent"]["points"].remove(s)
                     except Exception as e:
                         pass
                 else:
                     try:
-                        self.yg_glyph.current_block().remove(s)
+                        self.yg_glyph.current_block.remove(s)
                     except Exception as e:
                         pass
                 if "points" in s:
                     for hh in s["points"]:
                         try:
                             if not "rel" in hh or hint_type_nums[hh["rel"]] == 4:
                                 self.yg_glyph.add_hint(ygHint(self.yg_glyph, hh))
@@ -1904,17 +1887,17 @@
         self.hint = hint
         self.setText("Reverse Hint")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
-            self.hint._source["ptid"], self.hint._source["ref"] = (
-                self.hint._source["ref"],
-                self.hint._source["ptid"],
+            self.hint.source["ptid"], self.hint.source["ref"] = (
+                self.hint.source["ref"],
+                self.hint.source["ptid"],
             )
             self.yg_glyph._rebuild_current_block()
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "reverseHintCommand").test()
         self.send_signal()
 
 
@@ -1945,38 +1928,39 @@
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
             self.hint._delete_points(self.p_list)
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "deletePointsCommand").test()
+        #self.yg_glyph._hints_changed(self.yg_glyph.hints)
         self.send_signal()
 
 
 class switchAxisCommand(QUndoCommand):
     def __init__(self, g: "ygGlyph", prefs: ygPreferences, new_axis: str) -> None:
         super().__init__()
         self.yg_glyph = g
-        self.original_axis = self.yg_glyph.current_axis()
+        self.original_axis = self.yg_glyph.axis
         self.new_axis = new_axis
         self.top_window = prefs.top_window()
         self.setText("Change Axis")
 
     def redo(self) -> None:
-        if self.yg_glyph.current_axis() == self.new_axis:
+        if self.yg_glyph.axis == self.new_axis:
             return
-        self.top_window.current_axis = self.yg_glyph._current_axis = self.new_axis
-        self.yg_glyph._hints_changed(self.yg_glyph.hints(), dirty=False)
+        self.top_window.current_axis = self.yg_glyph.axis = self.new_axis
+        self.yg_glyph._hints_changed(self.yg_glyph.hints, dirty=False)
         self.yg_glyph.send_yaml_to_editor()
         self.top_window.set_window_title()
         self.top_window.check_axis_button()
 
     def undo(self) -> None:
-        self.top_window.current_axis = self.yg_glyph._current_axis = self.original_axis
-        self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints())
+        self.top_window.current_axis = self.yg_glyph.axis = self.original_axis
+        self.yg_glyph.sig_hints_changed.emit(self.yg_glyph.hints)
         self.yg_glyph.send_yaml_to_editor()
         self.top_window.set_window_title()
         self.top_window.check_axis_button()
 
 
 class glyphAddPropertyCommand(QUndoCommand):
     """redo() has got to be the action itself. It will get excecuted when the
@@ -2004,23 +1988,23 @@
     @pyqtSlot()
     def undo(self) -> None:
         if "props" in self.yg_glyph.gsource:
             if self.props:
                 self.yg_glyph.gsource["props"] = self.props
             else:
                 del self.yg_glyph.gsource["props"]
-        self.yg_glyph._hints_changed(self.yg_glyph.hints())
+        self.yg_glyph._hints_changed(self.yg_glyph.hints)
 
     @pyqtSlot()
     def redo(self) -> None:
         if not "props" in self.yg_glyph.gsource:
             self.yg_glyph.gsource["props"] = {}
         self.yg_glyph.gsource["props"][self.prop_name] = self.prop_value
         glyphSourceTester(self.yg_glyph, "glyphAddPropertyCommand").test()
-        self.yg_glyph._hints_changed(self.yg_glyph.hints())
+        self.yg_glyph._hints_changed(self.yg_glyph.hints)
 
 
 class glyphDeletePropertyCommand(QUndoCommand):
     def __init__(self, yg_glyph: "ygGlyph", prop_name: str) -> None:
         super().__init__()
         self.yg_glyph = yg_glyph
         # Make a backup copy of the "props" block. It should never be
@@ -2037,23 +2021,23 @@
         # with the former one.
         if self.props != None:
             if "props" in self.yg_glyph.gsource:
                 self.yg_glyph.gsource["props"] = self.props
         else:
             if "props" in self.yg_glyph.gsource:
                 del self.yg_glyph.gsource["props"]
-        self.yg_glyph._hints_changed(self.yg_glyph.hints())
+        self.yg_glyph._hints_changed(self.yg_glyph.hints)
 
     @pyqtSlot()
     def redo(self) -> None:
         try:
             del self.yg_glyph.gsource["props"][self.prop_name]
             if len(self.yg_glyph.gsource["props"]) == 0:
                 del self.yg_glyph.gsource["props"]
-            self.yg_glyph._hints_changed(self.yg_glyph.hints())
+            self.yg_glyph._hints_changed(self.yg_glyph.hints)
         except Exception:
             pass
         glyphSourceTester(self.yg_glyph, "glyphDeletePropertyCommand").test()
 
 
 class glyphSourceTester:
     def __init__(self, yg_glyph: "ygGlyph", caller: str):
@@ -2096,23 +2080,23 @@
 
     def __init__(self, preferences: ygPreferences, yg_font: ygFont, gname: str) -> None:
         """Requires a ygFont object and the name of the glyph. Also access to preferences
         as a convenience.
         """
         super().__init__()
         self.preferences = preferences
-        top_window = self.preferences.top_window()
-        if top_window != None:
+        self.top_window = self.preferences.top_window()
+        if self.top_window != None:
             self.undo_stack = QUndoStack()
-            self.preferences.top_window().add_undo_stack(self.undo_stack)
+            self.top_window.add_undo_stack(self.undo_stack)
             self.undo_stack.setActive(True)
         self.yaml_editor = None
-        self.yg_font = yg_font
+        self._yg_font = yg_font
         # The next few lines have to come *after* loading the ft_font (below)
-        self.gname = gname
+        self._gname = gname
 
         # Work with the glyph from the fontTools representation of the font.
 
         try:
             self.ft_glyph = yg_font.ft_font["glyf"][self.gname]
         except KeyError:
             l = list(yg_font.ft_font.getGlyphSet())
@@ -2122,15 +2106,15 @@
                 self.gname = l[1]
             else:
                 raise Exception("Tried to load nonexistent glyph " + self.gname)
             self.ft_glyph = yg_font.ft_font["glyf"][self.gname]
 
         # Initialize the source for this glyph.
 
-        self.gsource = yg_font.get_glyph(self.gname)
+        self._gsource = yg_font.get_glyph(self.gname)
         self.props = ygGlyphProperties(self)
         self.error = 0
 
         if not "y" in self.gsource:
             self.gsource["y"] = {"points": []}
         if not "x" in self.gsource:
             self.gsource["x"] = {"points": []}
@@ -2154,48 +2138,48 @@
 
         # Dict for looking up points by coordinates
         self.point_coord_dict = {}
         for p in self.point_list:
             self.point_coord_dict[p.coord] = p
 
         # Decide the initial axis.
-        if self.preferences and self.preferences.top_window() != None:
-            self._current_axis = self.preferences.top_window().current_axis
+        if self.preferences and self.top_window != None:
+            self._current_axis = self.top_window.current_axis
         else:
             self._current_axis = "y"
 
         # A little fix
 
-        backup_axis = self._current_axis
-        self._current_axis = "y"
-        self.fix_hint_types(self.current_block())
-        self._current_axis = "x"
-        self.fix_hint_types(self.current_block())
-        self._current_axis = backup_axis
+        backup_axis = self.axis
+        self.axis = "y"
+        self.fix_hint_types(self.current_block)
+        self.axis = "x"
+        self.fix_hint_types(self.current_block)
+        self.axis = backup_axis
 
         # Fix up the source to make it more usable.
-        self._yaml_add_parents(self.current_block())
-        self._yaml_supply_refs(self.current_block())
+        self._yaml_add_parents(self.current_block)
+        self._yaml_supply_refs(self.current_block)
 
         # This is the QGraphicsScene wrapper for this glyph object. But
         # do we need a reference here in the __init__? It's only used once,
         # in setting up a signal, and there are other ways to do that.
-        self.glyph_viewer = None
+        self.yg_glyph_scene = None
 
         self.sig_hints_changed.connect(self.hints_changed)
-        if self.preferences.top_window() != None:
+        if self.top_window != None:
             self.set_auto_preview_connection()
 
-    def report_vars(self) -> None:
-        print("Glyph name: " + self.gname)
-        print("Size of undo stack: " + str(self.undo_stack.count()))
-        print("Code for glyph:")
-        print(self.gsource)
-        print("Current block:")
-        print(self.current_block())
+    #def report_vars(self) -> None:
+    #    print("Glyph name: " + self.gname)
+    #    print("Size of undo stack: " + str(self.undo_stack.count()))
+    #    print("Code for glyph:")
+    #    print(self.gsource)
+    #    print("Current block:")
+    #    print(self.current_block)
 
     def send_error_message(self, d: dict):
         if self.yg_font:
             self.yg_font.send_error_message(d)
 
     #
     # Ordering and structuring YAML source
@@ -2252,23 +2236,23 @@
 
     def _rebuild_current_block(self) -> None:
         """Tears down the current source block and rebuilds it with proper
         regard for dependency and order. When this is reliable enough, it
         will be called every time the source is updated.
 
         """
-        flattened_tree = self._flatten_yaml_tree(copy.deepcopy(self.current_block()))
+        flattened_tree = self._flatten_yaml_tree(copy.deepcopy(self.current_block))
         for f in flattened_tree:
             if "points" in f:
                 del f["points"]
         new_tree = ygHintSorter(self.place_all(flattened_tree)).sort()
-        self.gsource[self.current_axis()]["points"].clear()
+        self.gsource[self.axis]["points"].clear()
         for t in new_tree:
-            self.gsource[self.current_axis()]["points"].append(t)
-        self.sig_hints_changed.emit(self.hints())
+            self.gsource[self.axis]["points"].append(t)
+        self.sig_hints_changed.emit(self.hints)
         self.send_yaml_to_editor()
 
     def rebuild_current_block(self) -> None:
         self.undo_stack.push(cleanupGlyphCommand(self))
 
     def _yaml_mk_hint_list(self, source: list, validate: bool = False) -> list:
         """'source' is a yaml "points" block."""
@@ -2325,15 +2309,15 @@
         """Walks the yaml tree, stripping out parent references and
         explicit statements of implicit refs.
 
         """
         for pt in node:
             if "parent" in pt:
                 h = ygHint(self, pt["parent"])
-                if (not h.hint_type() in ["function", "macro"]) and len(
+                if (not h.hint_type in ["function", "macro"]) and len(
                     h.target_list()
                 ) == 1:
                     del pt["ref"]
                 del pt["parent"]
             if "points" in pt:
                 self.yaml_strip_extraneous_nodes(pt["points"])
 
@@ -2392,15 +2376,15 @@
                 last_right = right
                 rightmost_point = i
             left = min(left, p.font_x)
             if left != last_left:
                 last_left = left
                 leftmost_point = i
         return (rightmost_point, right), (leftmost_point, left)
-    
+
     def dimensions(self):
         if len(self.point_list) == 0:
             return 0, 0
         x_right, x_left = self.extreme_points_x()
         y_top, y_bottom = self.extreme_points_y()
         x_dim = x_right[1] - x_left[1]
         y_dim = y_top[1] - y_bottom[1]
@@ -2410,30 +2394,53 @@
         cat = self.props.get_property("category")
         if cat == None:
             cat = self.yg_font.get_unicode_category(self.gname)
         if long_name:
             return unicode_cat_names[cat]
         return cat
 
-    def current_axis(self) -> str:
+    @property
+    def axis(self) -> str:
         return self._current_axis
+    
+    @axis.setter
+    def axis(self, a: str) -> None:
+        if a in ["y", "x"]:
+            self._current_axis = a
+        else:
+            raise ValueError("Axis must be 'y' or 'x'.")
+
+    @property
+    def yg_font(self) -> ygFont:
+        return self._yg_font
+    
+    @property
+    def gname(self) -> str:
+        return self._gname
+    
+    @property
+    def gsource(self) -> dict:
+        return self._gsource
 
+    @property
     def current_block(self) -> list:
-        if self._current_axis == "y":
+        if self.axis == "y":
             return self.gsource["y"]["points"]
         else:
             return self.gsource["x"]["points"]
 
+    @property
     def hints(self) -> list:
         """Get a list of hints for the current axis, wrapped in ygHint
         objects.
 
         """
-        return self._yaml_mk_hint_list(self.current_block(), validate=True)
+        return self._yaml_mk_hint_list(self.current_block, validate=True)
 
+    @property
     def points(self) -> list:
         return self.point_list
 
     def indices_to_coords(self) -> None:
         """Change coordinates in current block to point indices."""
         self.undo_stack.push(changePointNumbersCommand(self, True))
 
@@ -2541,15 +2548,15 @@
         block: list,
         pt: Union[ygPoint, ygSet, ygParams, int, str, None],
         ptype: str,
     ) -> list:
         """Search the yaml source for a point.
 
         Parameters:
-        block (list): At the top level, should be self.current_block().
+        block (list): At the top level, should be self.current_block.
 
         pt (ygPoint, ygSet, ygParams, int, or str): The point(s) we're
         searching for. If more than one point (ygSet, ygParams), any
         match at all is a positive result.
 
         ptype (str): "ptid" to search for target points, "ref" to search
         for ref points.
@@ -2596,23 +2603,25 @@
                 if tester:
                     if len(tester.overlaps(search_set)) > 0:
                         result.append(ppt)
             if "points" in ppt and len(ppt["points"]) > 0:
                 result.extend(self.search_source(ppt["points"], search_set, ptype))
         return result
 
-    def glyph_name(self) -> str:
-        return self.gname
+    #def glyph_name(self) -> str:
+    #    return self.gname
 
+    @property
     def xoffset(self) -> int:
         xo = self.props.get_property("xoffset")
         if xo != None:
             return xo
         return 0
 
+    @property
     def yoffset(self) -> int:
         yo = self.props.get_property("yoffset")
         if yo != None:
             return yo
         return 0
 
     def _yaml_hint_type(self, n) -> str:
@@ -2638,55 +2647,54 @@
         Returns:
         A list of ygPoint objects.
 
         """
         pt_list = []
         gl = self.ft_glyph.getCoordinates(self.yg_font.ft_font["glyf"])
         lpref = "index"
-        top_window = self.preferences.top_window()
-        if top_window != None and top_window.points_as_coords:
+        if self.top_window != None and self.top_window.points_as_coords:
             lpref = "coord"
         for point_index, p in enumerate(zip(gl[0], gl[2])):
             is_on_curve = p[1] & 0x01 == 0x01
             pt = ygPoint(
                 None,
                 point_index,
                 p[0][0],
                 p[0][1],
-                self.xoffset(),
-                self.yoffset(),
+                self.xoffset,
+                self.yoffset,
                 is_on_curve,
                 label_pref=lpref,
             )
             if point_index in gl[1]:
                 pt.end_of_contour = True
             pt_list.append(pt)
         return pt_list
 
     #
     # Navigation
     #
 
     def switch_to_axis(self, new_axis: str) -> None:
-        if self.current_axis() == "y":
+        if self.axis == "y":
             new_axis = "x"
         else:
             new_axis = "y"
         self.undo_stack.push(switchAxisCommand(self, self.preferences, new_axis))
 
     #
     # Saving
     #
 
     def save_editor_source(self, s: list) -> None:
         """When the user has typed Ctrl+R to compile the contents of the
         editor pane, this function gets called to do the rest. It
         massages the yaml source exactly as the __init__for this class
         does (calling the same functions) and installs new source
-        in self.current_block(). Finally it
+        in self.current_block. Finally it
         sends sig_hints_changed to notify that the hints are ready to
         render and sends reconstituted source back to the editor.
         """
         new_cmd = updateSourceCommand(self, s)
         self.undo_stack.push(new_cmd)
         if not new_cmd.valid:
             new_cmd.setObsolete(True)
@@ -2737,15 +2745,15 @@
         """If conditional=False, function will always place a hint somewhere
         in the tree (in the top level when it can't find another place).
         When True, function will return False when it fails to place the
         hint in the tree.
         """
         ref = None
         if type(h) is ygHint:
-            h = h.source()
+            h = h.source
         if "ref" in h:
             ref = h["ref"]
         if ref == None or type(ref) is list:
             block.append(h)
         else:
             matches = self.search_source(block, ref, "ptid")
             if len(matches) > 0:
@@ -2768,25 +2776,14 @@
         """l: a list of ygHint objects"""
         self.undo_stack.push(deleteHintsCommand(self, l))
 
     def set_dirty(self) -> None:
         self._clean = False
         self.yg_font.set_dirty()
 
-    #def make_set(
-    #    self,
-    #    hint: "ygHint",
-    #    pt_list: list,
-    #    touched_point: Optional[ygPoint],
-    #    callback: Callable,
-    #) -> None:
-    #    self.undo_stack.push(
-    #        makeSetCommand(self, hint, pt_list, touched_point, callback)
-    #    )
-
     def set_clean(self) -> None:
         self._clean = True
 
     def clean(self) -> bool:
         return self._clean
 
     @overload
@@ -2813,36 +2810,33 @@
         if type(pts) is list:
             result = []
             for p in pts:
                 if type(p) is ygPoint:
                     result.append(p.preferred_label())
             return result
         if type(pts) is ygSet:
-            return self.points_to_labels(pts.point_list())
+            return self.points_to_labels(pts.point_list)
         if type(pts) is ygParams:
-            pp = pts.point_list()
+            pp = pts.point_list
             result = []
             for p in pp:
                 if type(p) is ygPoint:
                     result.append(p.preferred_label())
                 elif type(p) is list:
                     result.extend(self.points_to_labels(p))
             return result
         if type(pts) is ygPoint:
             return pts.preferred_label()
         return 0
 
     def resolve_point_identifier(self, ptid: Any, depth: int = 0) -> Any:
         """Get the ygPoint object identified by ptid. ***Failures are very
         possible here, since there may be nonsense in a source file or in
-        the editor. Figure out how to handle failures gracefully.
-
-        (Instead of crashing, return None. Caller can respond by marking a
-        hint invalid, to be skipped over when generating xgf or rendering
-        on screen)
+        the editor. We handle obvious bad results (like None instead of an
+        object) by returning the zero point and issuing an error message.
 
         Parameters:
         ptid (int, str): An identifier for a point. Xgridfit allows them
         to be in any of three styles: int (the raw index of the point),
         coordinates (in the format "{100;100}"), or name (from the
         glyph's "names" section). The identifier may point to a single
         point, a list of points, or a dict (holding named parameters for
@@ -2918,57 +2912,65 @@
             return result
 
     #
     # Signals and slots
     #
 
     def set_auto_preview_connection(self) -> None:
-        if self.preferences.top_window().auto_preview_update:
+        if self.top_window.auto_preview_update:
             self.sig_hints_changed.connect(
-                self.preferences.top_window().preview_current_glyph
+                self.top_window.preview_current_glyph
             )
         else:
             try:
                 self.sig_hints_changed.disconnect(
-                    self.preferences.top_window().preview_current_glyph
+                    self.top_window.preview_current_glyph
                 )
             except Exception as e:
                 # print(e)
                 pass
 
     def set_yaml_editor(self, ed: Any) -> None:
         """Registers a slot in a ygYAMLEditor object, for installing source."""
         self.sig_glyph_source_ready.connect(ed.install_source)
         self.send_yaml_to_editor()
 
     def send_yaml_to_editor(self) -> None:
         """Sends yaml source for the current x or y block to the editor pane."""
-        new_yaml = copy.deepcopy(self.current_block())
+        new_yaml = copy.deepcopy(self.current_block)
         self.yaml_strip_extraneous_nodes(new_yaml)
         self.sig_glyph_source_ready.emit(
             yaml.dump(new_yaml, sort_keys=False, Dumper=Dumper)
         )
 
     def hint_changed(self, h: Union["ygHint", None]):
         """Called by signal from ygHint. Sends a list of hints in response."""
         self.set_dirty()
-        self.sig_hints_changed.emit(self.hints())
+        self.sig_hints_changed.emit(self.hints)
         self.send_yaml_to_editor()
 
     @pyqtSlot(object)
     def hints_changed(self, hint_list: list) -> None:
         self._hints_changed(hint_list)
 
-    def _hints_changed(self, hint_list: list, dirty: bool = True) -> None:
+    def _hints_changed(
+            self,
+            hint_list: list,
+            dirty: bool = True
+        ) -> None:
         if dirty:
             self.set_dirty()
         from .ygHintEditor import ygGlyphScene
 
-        if self.glyph_viewer:
-            self.glyph_viewer.install_hints(hint_list)
+        if self.yg_glyph_scene:
+            self.yg_glyph_scene.install_hints(hint_list)
+
+        if self.top_window != None:
+            if self.top_window.font_viewer:
+                self.top_window.font_viewer.update_cell(self.gname)
 
 
 class ygGlyphs:
     """The "glyphs" section of a yaml file."""
 
     def __init__(self, source: dict) -> None:
         try:
@@ -2978,16 +2980,16 @@
 
     def get_glyph(self, gname: str) -> dict:
         if gname in self.data:
             return self.data[gname]
         else:
             return {}
 
-    def glyph_list(self) -> list:
-        return list(self.data.keys())
+    #def glyph_list(self) -> list:
+    #    return list(self.data.keys())
 
     def del_glyph(self, gname: str) -> None:
         if gname in self.data:
             del self.data[gname]
 
 
 class Comparable(object):
@@ -3008,17 +3010,17 @@
     def _mk_point_list(self, obj: dict, key: str) -> list:
         """Helper for comparison functions. For target points, this will
         recurse into dependent hints to build a complete list.
 
         """
         hint = ygHint(None, obj) # type: ignore
         if key == "ptid":
-            p = hint.target()
+            p = hint.target
         else:
-            p = hint.ref()
+            p = hint.ref
         result = []
         if type(p) is dict:
             k = p.keys()
             for kk in k:
                 if type(p[kk]) is list:
                     result.extend(p[kk])
                 else:
@@ -3124,49 +3126,61 @@
 
     """
 
     hint_changed_signal = pyqtSignal(object)
 
     def __init__(self, glyph: ygGlyph, point: dict) -> None:
         super().__init__()
-        self.id = uuid.uuid1()
+        self._id = uuid.uuid1()
         self._source = point
         self.yg_glyph = glyph
         self.placed = False
 
         if self.yg_glyph != None:
             self.hint_changed_signal.connect(self.yg_glyph.hint_changed)
 
+    @property
     def source(self) -> dict:
         return self._source
 
     # The next two are not used right now. Note that parent() conflicts
     # with the superclass, so if we decide to use it, we have to
     # rename it.
 
     # def parent(self):
     #    if "parent" in self.source:
-    #        return self._source["parent"]
+    #        return self.source["parent"]
 
     # def children(self):
-    #    if "points" in self._source:
-    #        return self._source["points"]
+    #    if "points" in self.source:
+    #        return self.source["points"]
 
+    @property
+    def id(self):
+        return self._id
+
+    @property
     def target(self) -> Any:
         """May return a point identifier (index, name, coordinate-pair), a list,
         or a dict.
 
         """
         return self._source["ptid"]
 
+    # This is not used right now
+    # @target.setter
+    # def target(self, tgt: Any) -> None:
+    #     """tgt can be a point identifier or a set of them. no ygPoint objects."""
+    #     self.source["ptid"] = tgt
+
     def target_list(self, index_only: bool = False) -> list:
         """Always returns a list. Does not recurse."""
         if self.yg_glyph == None:
             return []
-        t = self.target()
+        t = self.target
         if type(t) is list:
             return t
         elif type(t) is dict:
             result = []
             v = t.values()
             for vv in v:
                 if type(vv) is list:
@@ -3209,15 +3223,15 @@
         Points in p must be type ygPoint."""
         current_points = self._ptid_to_objects()
         current_points.extend(p)
         labels = []
         for p in current_points:
             labels.append(p.preferred_label())
         if len(labels) > 1:
-            self._source["ptid"] = labels
+            self.source["ptid"] = labels
 
     def add_points(self, p: list) -> None:
         if self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(
                 addPointsCommand(self.yg_glyph, self, p)
             )
 
@@ -3237,120 +3251,122 @@
                 pass
         if len(pt_list) >= original_len:
             return
         labels = []
         for p in pt_list:
             labels.append(p.preferred_label())
         if len(labels) == 1:
-            self._source["ptid"] = labels[0]
+            self.source["ptid"] = labels[0]
         elif len(labels) > 1:
-            self._source["ptid"] = labels
+            self.source["ptid"] = labels
 
     def delete_points(self, p: list) -> None:
         if self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(
                 deletePointsCommand(self.yg_glyph, self, p)
             )
 
+    @property
     def ref(self) -> Any:
-        if "ref" in self._source:
-            return self._source["ref"]
+        if "ref" in self.source:
+            return self.source["ref"]
         return None
 
-    def set_target(self, tgt: Any) -> None:
-        """tgt can be a point identifier or a set of them. no ygPoint objects."""
-        self._source["ptid"] = tgt
-
+    @property
     def hint_type(self) -> str:
-        if "macro" in self._source:
+        if "macro" in self.source:
             return "macro"
-        if "function" in self._source:
+        if "function" in self.source:
             return "function"
-        if "rel" in self._source:
-            return self._source["rel"]
+        if "rel" in self.source:
+            return self.source["rel"]
         return "anchor"
 
-    def can_be_reversed(self) -> bool:
-        no_func = not "function" in self._source
-        no_macro = not "macro" in self._source
-        has_eligible_ref = "ref" in self._source and (
-            type(self._source["ref"]) is not list
+    @property
+    def reversible(self) -> bool:
+        no_func = not "function" in self.source
+        no_macro = not "macro" in self.source
+        has_eligible_ref = "ref" in self.source and (
+            type(self.source["ref"]) is not list
         )
-        has_eligible_target = "ptid" in self._source and (
-            type(self._source["ptid"]) is not list
+        has_eligible_target = "ptid" in self.source and (
+            type(self.source["ptid"]) is not list
         )
         return has_eligible_ref and has_eligible_target and no_func and no_macro
 
     def reverse_hint(self, h: Any) -> None:
-        if self.can_be_reversed() and self.yg_glyph != None:
+        if self.reversible and self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(reverseHintCommand(self.yg_glyph, self))
 
     def swap_macfunc_points(self, new_name: str, old_name: str) -> None:
         if self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(
                 swapMacFuncPointsCommand(self.yg_glyph, self, new_name, old_name)
             )
 
     def change_hint_color(self, new_color: str) -> None:
         if self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(
                 changeDistanceTypeCommand(self.yg_glyph, self, new_color)
             )
 
+    @property
     def rounded(self) -> bool:
-        if "round" in self._source:
-            if self._source["round"] == False:
+        if "round" in self.source:
+            if self.source["round"] == False:
                 return False
             return True
         else:
             return self.round_is_default()
 
     # Should make "min" handle a value.
+    @property
     def min_dist(self) -> bool:
         try:
-            m = self._source["min"]
+            m = self.source["min"]
             return m
         except Exception:
             return self.min_dist_is_default()
 
     def min_dist_is_default(self) -> bool:
-        return hint_type_nums[self.hint_type()] == 3
+        return hint_type_nums[self.hint_type] == 3
 
     def toggle_min_dist(self) -> None:
         if self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(toggleMinDistCommand(self.yg_glyph, self))
 
     def toggle_rounding(self) -> None:
         """Ignores rounding types."""
         if self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(toggleRoundingCommand(self.yg_glyph, self))
 
     def round_is_default(self) -> bool:
-        return hint_type_nums[self.hint_type()] in [0, 3]
+        return hint_type_nums[self.hint_type] in [0, 3]
 
     def set_round(self, b: bool, update: bool = False) -> None:
         if b != self.round_is_default():
-            self._source["round"] = b
+            self.source["round"] = b
         else:
-            if "round" in self._source:
-                del self._source["round"]
+            if "round" in self.source:
+                del self.source["round"]
         if update:
             self.hint_changed_signal.emit(self)
 
+    @property
     def cv(self) -> Optional[str]:
-        if "pos" in self._source:
-            return self._source["pos"]
-        if "dist" in self._source:
-            return self._source["dist"]
-        if "cv" in self._source:
-            return self._source["cv"]
+        if "pos" in self.source:
+            return self.source["pos"]
+        if "dist" in self.source:
+            return self.source["dist"]
+        if "cv" in self.source:
+            return self.source["cv"]
         return None
 
     def required_cv_type(self) -> Optional[str]:
-        hnum = hint_type_nums[self.hint_type()]
+        hnum = hint_type_nums[self.hint_type]
         if hnum == 0:
             return "pos"
         if hnum == 3:
             return "dist"
         return None
 
     def set_cv(self, new_cv: str) -> None:
@@ -3366,20 +3382,21 @@
         a command onto the undo stack. This is called from changeCVCommand, which does
         those things, and also from ygHintEditor.guess_cv_for_hint, which guesses at a cv
         as part of constructing a hint.
         """
         cvtype = self.required_cv_type()
         if cvtype:
             if new_cv == "None":
-                if cvtype in self._source:
-                    del self._source[cvtype]
+                if cvtype in self.source:
+                    del self.source[cvtype]
             else:
-                self._source[cvtype] = new_cv
+                self.source[cvtype] = new_cv
 
     # Placeholder. Need to provide an interface to control this.
+    @property
     def cut_in(self) -> bool:
         return True
 
     def hint_has_changed(self, h: "ygHint") -> None:
         self.hint_changed_signal.emit(h)
 
     def add_hint(self, hint: "ygHint") -> None:
@@ -3390,50 +3407,53 @@
     def delete_hints(self, hint_list: list) -> None:
         """Delete a hint from the hint tree. Just calls a function in ygGlyph."""
         if self.yg_glyph != None:
             self.yg_glyph.delete_hints(hint_list)
 
     def _hint_string(self) -> str:
         result = "Hint target: "
-        result += str(self._source["ptid"])
-        if "ref" in self._source:
+        result += str(self.source["ptid"])
+        if "ref" in self.source:
             result += "; ref: "
-            result += str(self._source["ref"])
-        if "parent" in self._source:
+            result += str(self.source["ref"])
+        if "parent" in self.source:
             result += "; parent: "
-            result += str(self._source["parent"]["ptid"])
+            result += str(self.source["parent"]["ptid"])
         return result
 
     def _get_macfunc(self) -> Optional[Union[str, dict]]:
-        if "function" in self._source:
-            return self._source["function"]
-        elif "macro" in self._source:
-            return self._source["macro"]
+        if "function" in self.source:
+            return self.source["function"]
+        elif "macro" in self.source:
+            return self.source["macro"]
         return None
 
+    @property
     def macfunc_name(self) -> Optional[str]:
         macfunc = self._get_macfunc()
         if type(macfunc) is dict:
             return macfunc["nm"]
         if type(macfunc) is str:
             return macfunc
         return None
 
+    @property
     def macfunc_other_args(self) -> Optional[dict]:
         macfunc = self._get_macfunc()
         other_params = {}
         if type(macfunc) is dict:
             other_params = {
                 key: val for key, val in macfunc.items() if not key in ["nm", "code"]
             }
         if len(other_params) > 0:
             return other_params
         return None
 
-    def set_macfunc_other_args(self, d: dict) -> None:
+    @macfunc_other_args.setter
+    def macfunc_other_args(self, d: dict) -> None:
         """d is a dictionary of params for this hint."""
         if len(d) > 1 and self.yg_glyph != None:
             self.yg_glyph.undo_stack.push(
                 setMacFuncOtherArgsCommand(self.yg_glyph, self, d)
             )
 
     def print(*args, **kwargs):
@@ -3489,31 +3509,33 @@
             self.source["masters"] = {}
         if len(self.source["masters"]) == 0:
             self.build_master_list()
 
     def create_master(self):
         master_id = random_id("master")
         d = {"name": master_id, "vars": {}}
-        at = self.yg_font.axis_tags()
+        at = self.yg_font.axis_tags
         for a in at:
             d["vars"][a] = 0.0
         return master_id, d
 
+    @property
     def keys(self):
         return self.source["masters"].keys()
 
+    @property
     def names(self):
         n_list = []
-        k = self.source["masters"].keys()
+        k = self.keys
         for kk in k:
             n_list.append(self.source["masters"][kk]["name"])
         return n_list
 
     def master_by_name(self, n):
-        k = self.source["masters"].keys()
+        k = self.keys
         for kk in k:
             if self.source["masters"][kk]["name"] == n:
                 return kk, self.source["masters"][kk]
         return None
 
     def master(self, m_id):
         try:
@@ -3823,14 +3845,15 @@
 
     def save(self, c: dict) -> None:
         self.yg_font.undo_stack.push(
             saveEditBoxCommand(self.yg_font, self, c, "Edit Control Values")
         )
         self.set_clean(True)
 
+    @property
     def keys(self) -> Iterable:
         return self.font_source["cvt"].keys()
 
     def get_cvs(self, glyph: ygGlyph, filters: dict) -> dict:
         """Get a list of control values filtered to match a particular
         environment.
 
@@ -3879,16 +3902,16 @@
         """Helper for get_closest_cv_action"""
         if v == None:
             return 0
         return lst[min(range(len(lst)), key=lambda i: abs(lst[i] - v))]
 
     def _get_val_from_hint(self, hint: ygHint, axis: str) -> Optional[int]:
         """Helper for get_closest_cv_action and get_closest_cv_name."""
-        tgt = hint.yg_glyph.resolve_point_identifier(hint.target())
-        ref = hint.ref()
+        tgt = hint.yg_glyph.resolve_point_identifier(hint.target)
+        ref = hint.ref
         if ref != None:
             ref = hint.yg_glyph.resolve_point_identifier(ref)
             if type(ref) is not ygPoint:
                 return None
         if type(tgt) is not ygPoint:
             return None
         if ref == None:
@@ -3900,15 +3923,15 @@
             if axis == "y":
                 return abs(tgt.font_y - ref.font_y)
             else:
                 return abs(tgt.font_x - ref.font_x)
 
     def get_closest_cv_name(self, cvlist: list, hint: ygHint) -> str:
         """cvlist is a list of cv names."""
-        axis = hint.yg_glyph.current_axis()
+        axis = hint.yg_glyph.axis
         val = self._get_val_from_hint(hint, axis)
         vlist = []
         for c in cvlist:
             vv = self.get_cv(c)
             if type(vv) is dict:
                 vlist.append(vv["val"])
             else:
@@ -3922,15 +3945,15 @@
 
         alst is a list of QActions; hint is the hint we're operating on.
         The hint must be type 0 (anchor) or 3 (single-point target, can take cv).
         Hint type should have been checked before we got here.
         """
         alst.pop(0)
         alst.pop(0)
-        axis = hint.yg_glyph.current_axis()
+        axis = hint.yg_glyph.axis
         val = self._get_val_from_hint(hint, axis)
         vlist = []
         for a in alst:
             vv = self.get_cv(a.text())
             if type(vv) is dict:
                 vlist.append(vv["val"])
             else:
```

### Comparing `ygt-0.1.6/src/ygt/ygPreferences.py` & `ygt-0.2.0/src/ygt/ygPreferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,17 @@
             winreg.REG_DWORD,
             int(prefs["points_as_coords"]),
         )
         winreg.SetValueEx(
             yg_key, "auto_preview", 0, winreg.REG_DWORD, int(prefs["auto_preview"])
         )
         winreg.SetValueEx(
+            yg_key, "recents", 0, winreg.REG_MULTI_SZ, prefs["recents"]
+        )
+        winreg.SetValueEx(
             yg_key, "top_window_pos_x", 0, winreg.REG_DWORD, prefs["top_window_pos_x"]
         )
         winreg.SetValueEx(
             yg_key, "top_window_pos_y", 0, winreg.REG_DWORD, prefs["top_window_pos_y"]
         )
         winreg.SetValueEx(
             yg_key, "top_window_height", 0, winreg.REG_DWORD, prefs["top_window_height"]
```

### Comparing `ygt-0.1.6/src/ygt/ygPreview.py` & `ygt-0.2.0/src/ygt/ygPreview.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     QWidget,
     QLabel,
     QLineEdit,
     QPushButton,
     QHBoxLayout,
     QVBoxLayout,
 )
-from PyQt6.QtGui import QPainter, QBrush, QColor, QPalette
+from PyQt6.QtGui import QPainter, QBrush, QColor, QPalette, QPixmap
 from PyQt6.QtCore import Qt, QRect, pyqtSignal, pyqtSlot, QLine
 
 
 PREVIEW_WIDTH = 450
 PREVIEW_HEIGHT = 700
 STRING_PREVIEW_HEIGHT = 150
 PREVIEW_HORI_MARGIN = 25
@@ -26,15 +26,15 @@
         self._layout.setSpacing(0)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(preview)
         self._layout.addWidget(string_preview)
         self.setLayout(self._layout)
 
 
-class ygPreview(QWidget):
+class ygPreview(QLabel):
 
     sig_preview_paint_done = pyqtSignal(object)
 
     def __init__(self, top_window) -> None:
         super().__init__()
         self.top_window = top_window
         self.face: Optional[freetypeFont] = None
@@ -72,32 +72,62 @@
         self.top_char_margin = 0
         self.show_grid = True
         # Two- or three-dimensional array shaped by numpy.
         self.Z: list = []
         self.instance_dict: Optional[dict] = None
         self.instance: Optional[str] = None
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
-        self.background_color = self.palette().color(QPalette.ColorRole.Base)
+        self.background_color = self.default_background = self.palette().color(QPalette.ColorRole.Base)
         bg_hsv_value = self.background_color.value()
-        #bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
         self.dark_theme = text_hsv_value > bg_hsv_value
-        self.colors = self.mk_color_list()
+        self.theme_choice = "auto"
+        self.colors = None
+        self.change_theme(self.theme_choice)
+
         self.render_mode = RENDER_LCD_1
         self.hinting_on = True
-        self.paintEvent = self.paintEvent_b # type: ignore
+        # We display the preview by painting on a QPixmap and adding that to this widget.
+        # There are three methods for grayscale, lcd1, and lcd2. These are assigned to
+        # self.make_pixmap, which can be called whenever display needs to be refreshed--
+        # but we don't call the actual methods directly.
+        self.make_pixmap = self.make_pixmap_lcd1
+
+        self.pixmap = None
 
     def set_up_signal(self, func: Callable) -> None:
         self.sig_preview_paint_done.connect(func)
 
+    def change_theme(self, new_theme):
+        self.theme_choice = new_theme
+        match self.theme_choice:
+            case "light":
+                palette = self.palette()
+                palette.setColor(QPalette.ColorRole.Base, QColor("white"))
+                self.setPalette(palette)
+            case "dark":
+                palette = self.palette()
+                palette.setColor(QPalette.ColorRole.Base, QColor("black"))
+                self.setPalette(palette)
+            case _:
+                palette = self.palette()
+                palette.setColor(QPalette.ColorRole.Base, self.default_background)
+                self.setPalette(palette)
+        self.background_color = self.palette().color(QPalette.ColorRole.Base)
+        self.colors = self.mk_color_list()
+
     def mk_color_list(self) -> List[QColor]:
         """Pre-build a list of grayscale colors--for the big preview."""
         l = [0] * 256
+
+        dark_theme = (self.theme_choice == "dark")
+        if self.theme_choice == "auto":
+            dark_theme = self.dark_theme
+
         for count, c in enumerate(l):
-            # Mypy complains about this, and I have no idea what is actually wrong.
-            if self.dark_theme:
+            if dark_theme:
                 l[count] = QColor(255, 255, 255, count) # type: ignore
             else:
                 l[count] = QColor(101, 53, 15, count) # type: ignore
         return l # type: ignore
 
     def fetch_glyph(self, font, glyph_index):
         """Get a temporary FreeType font, then build the specified glyph.
@@ -124,15 +154,14 @@
         self.face.set_char(self.glyph_index)
         gdata = self.face._get_bitmap_metrics()
 
         ft_bitmap = self.face.glyph_slot.bitmap
         ft_width = ft_bitmap.width
         ft_rows = ft_bitmap.rows
         self.current_glyph_height = ft_rows
-        # ft_pitch  = ft_bitmap.pitch
         self.bitmap_top = self.face.glyph_slot.bitmap_top
         self.grid_height = self.face.ascender + abs(self.face.descender)
         self.total_height = self.grid_height
         top_offset = self.face.ascender - self.bitmap_top
         if top_offset < 0:
             self.top_grid_offset = abs(top_offset)
             self.total_height += self.top_grid_offset
@@ -167,21 +196,38 @@
         self.Z = self.face.mk_array(gdata, self.render_mode)
         return True
 
     @pyqtSlot()
     def toggle_show_hints(self) -> None:
         self.hinting_on = not self.hinting_on
         self.face.set_hinting_on(self.hinting_on)
-        # self._build_glyph()
+        self.make_pixmap()
         self.update()
 
     @pyqtSlot()
     def toggle_grid(self) -> None:
         self.show_grid = not self.show_grid
-        # self._build_glyph()
+        self.make_pixmap()
+        self.update()
+
+    @pyqtSlot()
+    def set_theme_auto(self) -> None:
+        self.set_theme("auto")
+
+    @pyqtSlot()
+    def set_theme_light(self) -> None:
+        self.set_theme("light")
+
+    @pyqtSlot()
+    def set_theme_dark(self) -> None:
+        self.set_theme("dark")
+
+    def set_theme(self, t: str) -> None:
+        self.change_theme(t)
+        self.make_pixmap()
         self.update()
 
     @pyqtSlot()
     def render1(self) -> None:
         self.set_render_mode(RENDER_GRAYSCALE)
 
     @pyqtSlot()
@@ -191,42 +237,40 @@
     @pyqtSlot()
     def render3(self) -> None:
         self.set_render_mode(RENDER_LCD_2)
 
     def set_render_mode(self, m: int) -> None:
         self.render_mode = m
         if self.render_mode == RENDER_GRAYSCALE:
-            self.paintEvent = self.paintEvent_a # type: ignore
+            self.make_pixmap = self.make_pixmap_grayscale
         elif self.render_mode == RENDER_LCD_1:
-            self.paintEvent = self.paintEvent_b # type: ignore
+            self.make_pixmap = self.make_pixmap_lcd1
         else:
-            self.paintEvent = self.paintEvent_c # type: ignore
-        # self._build_glyph()
+            self.make_pixmap = self.make_pixmap_lcd2
+        self.make_pixmap()
         self.update()
 
     def set_size(self, n: str | int) -> None:
         n = int(n)
         if self.face != None:
             try:
                 self.char_size = n
                 if self.char_size < 10:
                     self.char_size = 10
                 self.face.set_size(self.char_size)
             except Exception as e:
                 return
-            # self.label.setText(str(self.char_size) + "ppem")
             self.set_label_text()
-            # self._build_glyph()
+            self.make_pixmap()
             self.update()
 
     def resize_by(self, n: int) -> None:
         if self.face != None and self.glyph_index != 0:
-            # self.char_size += n
-            # self.set_label_text()
             self.set_size(self.char_size + n)
+            self.make_pixmap()
             self.update()
 
     def set_label_text(self) -> None:
         t = str(self.char_size) + "ppem"
         if self.instance != None:
             t += " — " + self.instance
         self.label.setText(t)
@@ -273,15 +317,15 @@
     def set_instance(self) -> None:
         self.instance = self.sender().text() # type: ignore
         self._set_instance()
 
     def _set_instance(self) -> None:
         self.face.set_instance(self.instance)
         self.set_label_text()
-        # self._build_glyph()
+        self.make_pixmap()
         self.update()
 
     @pyqtSlot()
     def bigger_one(self) -> None:
         self.resize_by(1)
 
     @pyqtSlot()
@@ -308,140 +352,153 @@
 
         pen = painter.pen()
         pen.setWidth(1)
         line_length = self.face.glyph_slot.bitmap.width * self.pixel_size
         if self.render_mode != RENDER_GRAYSCALE:
             line_length = int(line_length / 3)
 
+        dark_theme = (self.theme_choice == "dark")
+        if self.theme_choice == "auto":
+            dark_theme = self.dark_theme
+
         for i, r in enumerate(range(height)):
             if i == baseline:
                 pen.setColor(QColor("red"))
             else:
-                if self.dark_theme:
+                if dark_theme:
                     pen.setColor(QColor(200, 200, 200, 50))
                 else:
                     pen.setColor(QColor(50, 50, 50, 50))
             painter.setPen(pen)
             painter.drawLine(QLine(left, top, left + line_length, top))
             top += self.pixel_size
 
         if self.render_mode in [RENDER_GRAYSCALE, RENDER_LCD_1]:
             grid_width = self.face.glyph_slot.bitmap.width + 1
             if self.render_mode == RENDER_LCD_1:
                 grid_width = round(grid_width / 3) + 1
             y_top = self.vertical_margin + (self.top_grid_offset * self.pixel_size)
             y_bot = top - self.pixel_size
-            if self.dark_theme:
+
+            if dark_theme:
                 pen.setColor(QColor(200, 200, 200, 50))
             else:
                 pen.setColor(QColor(50, 50, 50, 50))
             painter.setPen(pen)
             for i, r in enumerate(range(grid_width)):
                 painter.drawLine(QLine(left, y_top, left, y_bot))
                 left += self.pixel_size
 
-    def paintEvent_a(self, event) -> None:
+    def make_pixmap_grayscale(self) -> None:
         """Paint grayscale glyph."""
-        painter = QPainter(self)
-        brush = QBrush()
-        brush.setColor(self.background_color)
-        #if self.dark_theme:
-        #    brush.setColor(QColor("black"))
-        #else:
-        #    brush.setColor(QColor("white"))
-        brush.setStyle(Qt.BrushStyle.SolidPattern)
-        rect = QRect(0, 0, self.width(), self.height())
-        painter.fillRect(rect, brush)
+        dark_theme = (self.theme_choice == "dark")
+        if self.theme_choice == "auto":
+            dark_theme = self.dark_theme
+
+        if self.pixmap == None:
+            self.pixmap = QPixmap(self.width(), self.height())
+        self.pixmap.fill(self.background_color)
+        painter = QPainter(self.pixmap)
+
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
             painter.end()
             return
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
         for row in self.Z:
             for col in row:
                 qr = QRect(xposition, yposition, self.pixel_size, self.pixel_size)
-                # qb = QBrush(QColor(101,53,15,col))
                 painter.fillRect(qr, self.colors[col])
                 xposition += self.pixel_size
             yposition += self.pixel_size
             xposition = self.horizontal_margin
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
+        self.setPixmap(self.pixmap)
         self.sig_preview_paint_done.emit(None)
 
-    def paintEvent_b(self, event) -> None:
-        """Paint subpixel rendering with solid pixels."""
-        painter = QPainter(self)
-        brush = QBrush()
-        brush.setColor(self.background_color)
-        #if self.dark_theme:
-        #    brush.setColor(QColor("black"))
-        #else:
-        #    brush.setColor(QColor("white"))
-        brush.setStyle(Qt.BrushStyle.SolidPattern)
-        rect = QRect(0, 0, self.width(), self.height())
-        painter.fillRect(rect, brush)
+    def make_pixmap_lcd1(self) -> None:
+        dark_theme = (self.theme_choice == "dark")
+        if self.theme_choice == "auto":
+            dark_theme = self.dark_theme
+
+        if self.pixmap == None:
+            self.pixmap = QPixmap(self.width(), self.height())
+        self.pixmap.fill(self.background_color)
+        painter = QPainter(self.pixmap)
+
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
             painter.end()
             return
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
-        black = QColor("black")
+
+        if dark_theme:
+            skippable = QColor("black")
+        else:
+            skippable = QColor("white")
+
         for row in self.Z:
             for col in row:
                 rgb = []
                 for elem in col:
                     rgb.append(elem)
-                if self.dark_theme:
+                if dark_theme:
                     qc = QColor(rgb[0], rgb[1], rgb[2])
-                    if qc == black:
-                        qc == self.background_color
                 else:
                     qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
-                qr = QRect(xposition, yposition, self.pixel_size, self.pixel_size)
-                painter.fillRect(qr, qc)
+                if qc != skippable:
+                    qr = QRect(xposition, yposition, self.pixel_size, self.pixel_size)
+                    painter.fillRect(qr, qc)
                 xposition += self.pixel_size
             yposition += self.pixel_size
             xposition = self.horizontal_margin
+
         if self.show_grid:
             self.draw_grid(painter)
+
         painter.end()
+
+        self.setPixmap(self.pixmap)
+
         self.sig_preview_paint_done.emit(None)
 
-    def paintEvent_c(self, event) -> None:
+    def make_pixmap_lcd2(self) -> None:
         """Paint subpixel rendering with rgb pixel trios."""
-        painter = QPainter(self)
-        brush = QBrush()
-        brush.setColor(self.background_color)
-        #if self.dark_theme:
-        #    brush.setColor(QColor("black"))
-        #else:
-        #    brush.setColor(QColor("white"))
-        brush.setStyle(Qt.BrushStyle.SolidPattern)
-        rect = QRect(0, 0, self.width(), self.height())
-        painter.fillRect(rect, brush)
+        dark_theme = (self.theme_choice == "dark")
+        if self.theme_choice == "auto":
+            dark_theme = self.dark_theme
+
+        if self.pixmap == None:
+            self.pixmap = QPixmap(self.width(), self.height())
+        self.pixmap.fill(self.background_color)
+        painter = QPainter(self.pixmap)
+
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
             painter.end()
             return
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
+        dark_theme = (self.theme_choice == "dark")
+        if self.theme_choice == "auto":
+            dark_theme = self.dark_theme
         for row in self.Z:
             for col in row:
                 for n, elem in enumerate(col):
-                    if self.dark_theme:
+                    if dark_theme:
                         if n == 0:
                             qc = QColor(elem, 0, 0)
                         elif n == 1:
                             qc = QColor(0, elem, 0)
                         elif n == 2:
                             qc = QColor(0, 0, elem)
                     else:
@@ -460,14 +517,15 @@
                     painter.fillRect(qr, qc)
                     xposition += int(self.pixel_size / 3)
             yposition += self.pixel_size
             xposition = self.horizontal_margin
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
+        self.setPixmap(self.pixmap)
         self.sig_preview_paint_done.emit(None)
 
 
 class ygStringPreviewPanel(QWidget):
     sig_go_to_glyph = pyqtSignal(object)
 
     def __init__(self, yg_preview: ygPreview, top_window) -> None:
@@ -489,31 +547,27 @@
         self.face = face
 
     def set_text(self, t: str) -> None:
         self._text = t
 
     def string_to_glyph_list(self, s: str) -> list:
         """Get a list of glyph names needed for string s."""
-        yg_font = self.top_window.glyph_pane.viewer.yg_glyph.yg_font
+        yg_font = self.top_window.glyph_pane.yg_glyph_scene.yg_glyph.yg_font
         result = []
         for c in s:
             try:
                 if not c in result:
                     result.append(yg_font.unicode_to_name[ord(c)])
             except Exception:
                 result.append(".notdef")
         return result
 
     def _fill_background(self, painter: QPainter) -> None:
         brush = QBrush()
         brush.setColor(self.yg_preview.background_color)
-        #if self.yg_preview.dark_theme:
-        #    brush.setColor(QColor("black"))
-        #else:
-        #    brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
     def paintEvent_a(self, event) -> None:
         target_size = self.yg_preview.char_size
         painter = QPainter(self)
@@ -522,29 +576,34 @@
             painter.end()
             return
         if not self.yg_preview:
             return
         self.face.reset_rect_list()
         xposition = 25
         yposition = 66
+
+        dark_theme = (self.yg_preview.theme_choice == "dark")
+        if self.yg_preview.theme_choice == "auto":
+            dark_theme = self.yg_preview.dark_theme
+
         for s in range(10, 100):
             this_is_target = (s == target_size)
             self.face.set_params(
                 glyph=self.yg_preview.glyph_index,
                 render_mode=self.yg_preview.render_mode,
                 hinting_on=self.yg_preview.hinting_on,
                 size=s,
                 instance=self.yg_preview.instance,
             )
             advance = self.face.draw_char(
                 painter,
                 xposition,
                 yposition,
-                spacing_mark=True,
-                dark_theme=self.yg_preview.dark_theme,
+                spacing_mark = True,
+                dark_theme = dark_theme,
                 is_target=this_is_target
             )
             xposition += advance
             if xposition + advance > (PREVIEW_WIDTH - 50):
                 if yposition == 66:
                     xposition = 25
                     yposition = 133
@@ -557,21 +616,24 @@
         painter = QPainter(self)
         self._fill_background(painter)
         if not self.yg_preview:
             return
         xposition = 25
         yposition = 66
         self.face = self.yg_preview.face
+        dark_theme = (self.yg_preview.theme_choice == "dark")
+        if self.yg_preview.theme_choice == "auto":
+            dark_theme = self.yg_preview.dark_theme
         self.rect_list = self.face.draw_string(
             painter,
             self._text,
             xposition,
             yposition,
             x_limit = PREVIEW_WIDTH - 50,
-            dark_theme = self.yg_preview.dark_theme
+            dark_theme = dark_theme
         )
         painter.end()
 
     def mousePressEvent(self, event) -> None:
         qp = event.position()
         x = int(qp.x())
         y = int(qp.y())
```

### Comparing `ygt-0.1.6/src/ygt/ygSchema.py` & `ygt-0.2.0/src/ygt/ygSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,17 @@
     Optional("init-graphics"): bool,
     Optional("assume-always-y"): bool,
     Optional("cleartype"): bool,
     Optional("counterclockwise"): bool,
     Optional("round"): hint_types,
     Optional("no-round"): hint_types,
     Optional("cv_vars_generated"): bool,
+    Optional("merge-mode"): bool,
+    Optional("replace-prep"): bool,
+    Optional("function-base"): int,
 }
 
 properties_struct = {
     Optional("category"): Or(
         "Lu",
         "Ll",
         "Lt",
```

### Comparing `ygt-0.1.6/src/ygt/ygStems.py` & `ygt-0.2.0/src/ygt/ygStems.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 class stemFinder:
     def __init__(self, p1: ygPoint, p2: ygPoint, yg_glyph: ygGlyph) -> None:
         self.yg_glyph = yg_glyph
         self.counter_clockwise = bool(self.yg_glyph.yg_font.defaults.get_default("counterclockwise"))
         self.contours = []
         contour = []
-        points = yg_glyph.points()
+        points = yg_glyph.points
         for p in points:
             contour.append(p)
             if p.end_of_contour:
                 self.contours.append(contour)
                 contour = []
         self.high_point = p1
         self.low_point = p2
-        if self.yg_glyph.current_axis() == "y":
+        if self.yg_glyph.axis == "y":
             # self.high_point must have a higher y value than self.low_point.
             if self.high_point.font_y < self.low_point.font_y:
                 self.high_point, self.low_point = self.low_point, self.high_point
         else:
             # self.high_point must have a lower x value than self.low_point.
             if self.high_point.font_x > self.low_point.font_x:
                 self.high_point, self.low_point = self.low_point, self.high_point
@@ -132,15 +132,15 @@
         return "same"
         
     def get_color(self) -> str:
         """ Recommends a distance type for the stem formed by self.high_point
             and self.low_point, based on this class's analysis of the stem.
         """
         result = "graydist"
-        if self.yg_glyph.current_axis() == "x":
+        if self.yg_glyph.axis == "x":
             high_y_dir = self.y_direction(self.high_point)
             low_y_dir = self.y_direction(self.low_point)
             if high_y_dir == "up" and low_y_dir == "down":
                 result = "blackdist"
             elif high_y_dir == "down" and low_y_dir == "up":
                 result = "whitedist"
         else:
```

### Comparing `ygt-0.1.6/src/ygt/ygYAMLEditor.py` & `ygt-0.2.0/src/ygt/ygYAMLEditor.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.6/src/ygt.egg-info/PKG-INFO` & `ygt-0.2.0/src/ygt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.6
+Version: 0.2.0
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,25 +26,39 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
+### Verasion 0.2.0
+
+Enabled merge (Ygt can add its hints to existing hints).
+
+Added files supporting creation of executables.
+
+Changed shortcuts: Ctrl-P = Hint Preview; Ctrl-L: Set Resolution.
+
+Fixed a bug that left some untouched points with "touched" flags.
+
+Can override light or dark theme for the Preview panels.
+
+Various bug fixes, efficiencies, and other improvements in the code.
+
 ### Version 0.1.6 (2023-4-28)
 
 Select more than one untouched point when adding shift, align, or interpolate hints to create a hint with a set as target. This formerly had to be done with a separate “Make Set” command.
 
 “Make Set” command has been removed as unnecessary.
 
 To add a point to a shift, align, or interpolate hint, select the hint and at least one untouched point, and press the **plus** key.
 
 To delete a point or points from a shift, align, or interpolate hint, select one ore more points belonging to the hint and press the **hyphen** or **minus** key.
 
-Corrected background color of preview panels when dark theme is active.
+Corrected background color of preview panels when dark theme is active. New color scheme for dark theme.
 
 ### Version 0.1.5 (2023-4-25)
 
 Various UI refinements: initial scaling of glyphs, spacebar to temporarily switch to panning mode, and more.
 
 User now confronts only one kind of stem hint: Ygt guesses (more or less accurately) the distance type.
```

### Comparing `ygt-0.1.6/src/ygt.egg-info/SOURCES.txt` & `ygt-0.2.0/src/ygt.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/ygt.py
+src/hooks/hook-freetype.py
+src/hooks/hook-xgridfit.py
 src/ygt/__init__.py
 src/ygt/__main__.py
 src/ygt/autohint_trash.py
 src/ygt/cvGuesser.py
 src/ygt/fontViewDialog.py
 src/ygt/freetypeFont.py
+src/ygt/harfbuzzFont.py
 src/ygt/macfuncDialog.py
 src/ygt/makeCVDialog.py
 src/ygt/window.py
 src/ygt/ygError.py
 src/ygt/ygHintEditor.py
 src/ygt/ygModel.py
 src/ygt/ygPreferences.py
```


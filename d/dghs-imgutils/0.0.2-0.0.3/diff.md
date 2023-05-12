# Comparing `tmp/dghs-imgutils-0.0.2.tar.gz` & `tmp/dghs-imgutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.0.2.tar", last modified: Wed May  3 06:27:29 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.0.3.tar", last modified: Fri May 12 17:45:16 2023, max compression
```

## Comparing `dghs-imgutils-0.0.2.tar` & `dghs-imgutils-0.0.3.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/setup.py
```

### Comparing `dghs-imgutils-0.0.2/LICENSE` & `dghs-imgutils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/PKG-INFO` & `dghs-imgutils-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: gpu
+Provides-Extra: test
 License-File: LICENSE
 
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
@@ -94,30 +94,30 @@
 
 ### Object Detection
 
 Currently, object detection is supported for anime faces and person, as shown below
 
 * Face Detection
 
-![face detection](https://deepghs.github.io/imgutils/main/_images/face_detect.dat.svg)
+![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect.dat.svg)
 
 * Person Detection
 
-![person detection](https://deepghs.github.io/imgutils/main/_images/person_detect.dat.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.dat.svg)
 
 Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://deepghs.github.io/imgutils/main/_images/edge.dat.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.dat.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
```

### Comparing `dghs-imgutils-0.0.2/README.md` & `dghs-imgutils-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,30 +69,30 @@
 
 ### Object Detection
 
 Currently, object detection is supported for anime faces and person, as shown below
 
 * Face Detection
 
-![face detection](https://deepghs.github.io/imgutils/main/_images/face_detect.dat.svg)
+![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect.dat.svg)
 
 * Person Detection
 
-![person detection](https://deepghs.github.io/imgutils/main/_images/person_detect.dat.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.dat.svg)
 
 Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://deepghs.github.io/imgutils/main/_images/edge.dat.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.dat.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
```

### Comparing `dghs-imgutils-0.0.2/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.0.3/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: gpu
+Provides-Extra: test
 License-File: LICENSE
 
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
@@ -94,30 +94,30 @@
 
 ### Object Detection
 
 Currently, object detection is supported for anime faces and person, as shown below
 
 * Face Detection
 
-![face detection](https://deepghs.github.io/imgutils/main/_images/face_detect.dat.svg)
+![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect.dat.svg)
 
 * Person Detection
 
-![person detection](https://deepghs.github.io/imgutils/main/_images/person_detect.dat.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.dat.svg)
 
 Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://deepghs.github.io/imgutils/main/_images/edge.dat.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.dat.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
```

### Comparing `dghs-imgutils-0.0.2/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.0.3/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
 imgutils/segment/__init__.py
 imgutils/segment/isnetis.py
 imgutils/tagging/__init__.py
 imgutils/tagging/deepdanbooru.py
 imgutils/tagging/format.py
+imgutils/tagging/mldanbooru.py
 imgutils/tagging/wd14.py
 imgutils/utils/__init__.py
 imgutils/utils/onnxruntime.py
 imgutils/validate/__init__.py
 imgutils/validate/color.py
 imgutils/validate/monochrome.py
 imgutils/validate/truncate.py
```

### Comparing `dghs-imgutils-0.0.2/dghs_imgutils.egg-info/requires.txt` & `dghs-imgutils-0.0.3/dghs_imgutils.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 matplotlib
 natsort
 nbsphinx>=0.8.8
 ipython>=7.16.3
 psutil>=5.8.0
 ipykernel>=6.15
 py-cpuinfo>=8.0.0
+click>=7.0.0
 
 [gpu]
 onnxruntime-gpu
 
 [test]
 coverage>=5
 mock>=4.0.3
```

### Comparing `dghs-imgutils-0.0.2/imgutils/config/meta.py` & `dghs-imgutils-0.0.3/imgutils/config/meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,18 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.0.2'
+__VERSION__ = '0.0.3'
 
 #: Short description of the project, will be included in ``setup.py``.
-__DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.'
+__DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
+                  'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992'
 
 #: Email of the authors'.
 __AUTHOR_EMAIL__ = 'narugo@126.com'
```

### Comparing `dghs-imgutils-0.0.2/imgutils/data/background.py` & `dghs-imgutils-0.0.3/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/data/decode.py` & `dghs-imgutils-0.0.3/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/data/encode.py` & `dghs-imgutils-0.0.3/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/data/image.py` & `dghs-imgutils-0.0.3/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/data/layer.py` & `dghs-imgutils-0.0.3/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/detect/_yolo.py` & `dghs-imgutils-0.0.3/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/detect/face.py` & `dghs-imgutils-0.0.3/imgutils/detect/face.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 Overview:
     Detect human faces (including the entire head) in anime images.
 
     Trained on dataset `ani_face_detection <https://universe.roboflow.com/linog/ani_face_detection>`_ with YOLOv8.
 
     .. image:: face_detect.dat.svg
         :align: center
+
+    This is an overall benchmark of all the face detect models:
+
+    .. image:: face_detect.benchmark.py.svg
+        :align: center
+
 """
 from functools import lru_cache
 from typing import List, Tuple
 
 from huggingface_hub import hf_hub_download
 
 from ._yolo import _image_preprocess, _data_postprocess
```

### Comparing `dghs-imgutils-0.0.2/imgutils/detect/person.py` & `dghs-imgutils-0.0.3/imgutils/detect/person.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,20 @@
     Detect human bodies (including the entire body) in anime images.
 
     Trained on dataset `AniDet3 <https://universe.roboflow.com/university-of-michigan-ann-arbor/anidet3-ai42v>`_ \
         with YOLOv8.
 
     .. image:: person_detect.dat.svg
         :align: center
+
+    This is an overall benchmark of all the person detect models:
+
+    .. image:: person_detect.benchmark.py.svg
+        :align: center
+
 """
 from functools import lru_cache
 
 from huggingface_hub import hf_hub_download
 
 from ._yolo import _image_preprocess, _data_postprocess
 from ..data import ImageTyping, load_image, rgb_encode
@@ -28,16 +34,16 @@
 def detect_person(image: ImageTyping, level: str = 's', max_infer_size=1216,
                   conf_threshold: float = 0.3, iou_threshold: float = 0.5):
     """
     Overview:
         Detect human bodies (including the entire body) in anime images.
 
     :param image: Image to detect.
-    :param level: The model level being used can be either `s` or `n`.
-        The `n` model runs faster with smaller system overhead, while the `s` model achieves higher accuracy.
+    :param level: The model level being used can be either `s`, `m` or `x`.
+        The `s` model runs faster with smaller system overhead, while the `m` model achieves higher accuracy.
         The default value is `s`.
     :param max_infer_size: The maximum image size used for model inference, if the image size exceeds this limit,
         the image will be resized and used for inference. The default value is `1216` pixels.
     :param conf_threshold: The confidence threshold, only detection results with confidence scores above
         this threshold will be returned. The default value is `0.3`.
     :param iou_threshold: The detection area coverage overlap threshold, areas with overlaps above this threshold
         will be discarded. The default value is `0.5`.
```

### Comparing `dghs-imgutils-0.0.2/imgutils/detect/visual.py` & `dghs-imgutils-0.0.3/imgutils/detect/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     visual_image = image.copy()
     draw = ImageDraw.Draw(visual_image, mode='RGBA')
     font = _try_get_font_from_matplotlib(fontsize) or ImageFont.load_default()
 
     labels = sorted(labels or {label for _, label, _ in detection})
     _colors = list(map(str, rnd_colors(len(labels))))
     _color_map = dict(zip(labels, _colors))
-    for (xmin, ymin, xmax, ymax), label, score in detection:
+    for _, ((xmin, ymin, xmax, ymax), label, score) in sorted(enumerate(detection), key=lambda x: (x[1][2], x[0])):
         box_color = _color_map[label]
         draw.rectangle((xmin, ymin, xmax, ymax), outline=box_color, width=2)
 
         if not no_label:
             label_text = f'{label}: {score * 100:.2f}%'
             _t_x0, _t_y0, _t_x1, _t_y1 = draw.textbbox((xmin, ymin), label_text, font=font)
             _t_width, _t_height = _t_x1 - _t_x0, _t_y1 - _t_y0
```

### Comparing `dghs-imgutils-0.0.2/imgutils/edge/_base.py` & `dghs-imgutils-0.0.3/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/edge/canny.py` & `dghs-imgutils-0.0.3/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/edge/lineart.py` & `dghs-imgutils-0.0.3/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/edge/lineart_anime.py` & `dghs-imgutils-0.0.3/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/metrics/lpips.py` & `dghs-imgutils-0.0.3/imgutils/metrics/lpips.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 Overview:
     Useful utilities based on `richzhang/PerceptualSimilarity <https://github.com/richzhang/PerceptualSimilarity>`_, \
     tested with dataset `deepghs/chafen_arknights(private) <https://huggingface.co/datasets/deepghs/chafen_arknights>`_.
 
     When threshold is `0.45`, the `adjusted rand score <https://scikit-learn.org/stable/modules/generated/sklearn.metrics.adjusted_rand_score.html>`_ can reach `0.995`.
 
+    This is an overall benchmark of all the operations in LPIPS models:
+
+    .. image:: lpips.benchmark.py.svg
+        :align: center
+
 """
 from functools import lru_cache
 from typing import Tuple, Union, List
 
 import numpy as np
 from PIL import Image
 from huggingface_hub import hf_hub_download
```

### Comparing `dghs-imgutils-0.0.2/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.0.3/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/segment/isnetis.py` & `dghs-imgutils-0.0.3/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.0.3/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/tagging/format.py` & `dghs-imgutils-0.0.3/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/tagging/wd14.py` & `dghs-imgutils-0.0.3/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.0.3/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/validate/color.py` & `dghs-imgutils-0.0.3/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/imgutils/validate/monochrome.py` & `dghs-imgutils-0.0.3/imgutils/validate/monochrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
     A model for screening monochrome images, with the definition of monochrome images referring to Danbooru.
 
     The following are testing images. The top two rows are monochrome images, and the bottom two rows are color images.
     Please note that **monochrome images are not only those with all pixels in grayscale**.
 
     .. image:: monochrome.dat.svg
         :align: center
+
+    This is an overall benchmark of all the monochrome validation models:
+
+    .. image:: monochrome.benchmark.py.svg
+        :align: center
 """
 from functools import lru_cache
 from typing import Optional, Tuple, Mapping
 
 import numpy as np
 from PIL import Image
 from huggingface_hub import hf_hub_download
```

### Comparing `dghs-imgutils-0.0.2/imgutils/validate/truncate.py` & `dghs-imgutils-0.0.3/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.2/setup.py` & `dghs-imgutils-0.0.3/setup.py`

 * *Files identical despite different names*


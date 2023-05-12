# Comparing `tmp/fastfft-0.1.4.tar.gz` & `tmp/fastfft-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.1.4.tar", last modified: Fri May 12 11:25:02 2023, max compression
+gzip compressed data, was "fastfft-0.1.5.tar", last modified: Fri May 12 11:48:30 2023, max compression
```

## Comparing `fastfft-0.1.4.tar` & `fastfft-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629638 fastfft-0.1.4/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1069 2023-05-12 10:51:03.000000 fastfft-0.1.4/LICENSE.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:25:02.629704 fastfft-0.1.4/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.4/README.md
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      125 2023-05-11 20:07:27.000000 fastfft-0.1.4/pyproject.toml
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1477 2023-05-12 11:25:02.629976 fastfft-0.1.4/setup.cfg
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     3689 2023-05-12 11:09:35.000000 fastfft-0.1.4/setup.py
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.627877 fastfft-0.1.4/src/
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629137 fastfft-0.1.4/src/fastfft.egg-info/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      321 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:21:18.000000 fastfft-0.1.4/src/fastfft.egg-info/not-zip-safe
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       43 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/requires.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        5 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/top_level.txt
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629318 fastfft-0.1.4/src/fft2/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 10:56:37.000000 fastfft-0.1.4/src/fft2/__init__.py
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222791 2023-05-12 11:21:18.000000 fastfft-0.1.4/src/fft2/main.cpp
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629550 fastfft-0.1.4/tests/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      131 2023-05-12 11:18:47.000000 fastfft-0.1.4/tests/test_fft2.py
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.145175 fastfft-0.1.5/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1069 2023-05-12 10:51:03.000000 fastfft-0.1.5/LICENSE.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       45 2023-05-12 10:50:21.000000 fastfft-0.1.5/MANIFEST.in
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:48:30.145237 fastfft-0.1.5/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.5/README.md
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       27 2023-05-12 10:52:03.000000 fastfft-0.1.5/requirements-dev.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       13 2023-05-12 10:51:32.000000 fastfft-0.1.5/requirements.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1422 2023-05-12 11:48:30.145508 fastfft-0.1.5/setup.cfg
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     3689 2023-05-12 11:09:35.000000 fastfft-0.1.5/setup.py
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.143014 fastfft-0.1.5/src/
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.144641 fastfft-0.1.5/src/fastfft.egg-info/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      356 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/not-zip-safe
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       43 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/requires.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        5 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/top_level.txt
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.144837 fastfft-0.1.5/src/fft2/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 10:56:37.000000 fastfft-0.1.5/src/fft2/__init__.py
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222791 2023-05-12 11:48:14.000000 fastfft-0.1.5/src/fft2/main.cpp
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.145083 fastfft-0.1.5/tests/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      131 2023-05-12 11:18:47.000000 fastfft-0.1.5/tests/test_fft2.py
```

### Comparing `fastfft-0.1.4/LICENSE.txt` & `fastfft-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastfft-0.1.4/PKG-INFO` & `fastfft-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.1.4
+Version: 0.1.5
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.1.4/setup.cfg` & `fastfft-0.1.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fastfft
-version = 0.1.4
+version = 0.1.5
 description = Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = Maxim Movshin
 author_email = maxim-movshin@yandex.ru
 url = https://github.com/BSaaber/fastfft
@@ -38,15 +38,11 @@
 python_requires = >=3.4
 package_dir = =src
 packages = find:
 
 [options.packages.find]
 where = src
 
-[options.package_data]
-* = *.pxd, *.h
-cypack = data/*
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fastfft-0.1.4/setup.py` & `fastfft-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `fastfft-0.1.4/src/fastfft.egg-info/PKG-INFO` & `fastfft-0.1.5/src/fastfft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.1.4
+Version: 0.1.5
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.1.4/src/fft2/main.cpp` & `fastfft-0.1.5/src/fft2/main.cpp`

 * *Files identical despite different names*


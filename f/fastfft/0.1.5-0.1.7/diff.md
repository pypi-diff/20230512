# Comparing `tmp/fastfft-0.1.5.tar.gz` & `tmp/fastfft-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.1.5.tar", last modified: Fri May 12 11:48:30 2023, max compression
+gzip compressed data, was "fastfft-0.1.7.tar", last modified: Fri May 12 14:51:37 2023, max compression
```

## Comparing `fastfft-0.1.5.tar` & `fastfft-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.145175 fastfft-0.1.5/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1069 2023-05-12 10:51:03.000000 fastfft-0.1.5/LICENSE.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       45 2023-05-12 10:50:21.000000 fastfft-0.1.5/MANIFEST.in
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:48:30.145237 fastfft-0.1.5/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.5/README.md
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       27 2023-05-12 10:52:03.000000 fastfft-0.1.5/requirements-dev.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       13 2023-05-12 10:51:32.000000 fastfft-0.1.5/requirements.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1422 2023-05-12 11:48:30.145508 fastfft-0.1.5/setup.cfg
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     3689 2023-05-12 11:09:35.000000 fastfft-0.1.5/setup.py
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.143014 fastfft-0.1.5/src/
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.144641 fastfft-0.1.5/src/fastfft.egg-info/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      356 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/not-zip-safe
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       43 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/requires.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        5 2023-05-12 11:48:30.000000 fastfft-0.1.5/src/fastfft.egg-info/top_level.txt
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.144837 fastfft-0.1.5/src/fft2/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 10:56:37.000000 fastfft-0.1.5/src/fft2/__init__.py
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222791 2023-05-12 11:48:14.000000 fastfft-0.1.5/src/fft2/main.cpp
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:48:30.145083 fastfft-0.1.5/tests/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      131 2023-05-12 11:18:47.000000 fastfft-0.1.5/tests/test_fft2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.925797 fastfft-0.1.7/
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-05-12 12:16:40.000000 fastfft-0.1.7/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       45 2023-05-12 12:16:40.000000 fastfft-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 14:51:37.925797 fastfft-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-12 12:16:40.000000 fastfft-0.1.7/README.md
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-05-12 12:16:40.000000 fastfft-0.1.7/requirements-dev.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-05-12 12:16:40.000000 fastfft-0.1.7/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)     1543 2023-05-12 14:51:37.925797 fastfft-0.1.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1397 2023-05-12 12:22:07.000000 fastfft-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.921797 fastfft-0.1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.921797 fastfft-0.1.7/src/fastfft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.921797 fastfft-0.1.7/src/fft2/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-12 12:16:40.000000 fastfft-0.1.7/src/fft2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222791 2023-05-12 14:51:29.000000 fastfft-0.1.7/src/fft2/main.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.925797 fastfft-0.1.7/tests/
+-rw-rw-r--   0 root         (0) root         (0)      131 2023-05-12 12:16:40.000000 fastfft-0.1.7/tests/test_fft2.py
```

### Comparing `fastfft-0.1.5/LICENSE.txt` & `fastfft-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastfft-0.1.5/PKG-INFO` & `fastfft-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.1.5
+Version: 0.1.7
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
@@ -13,22 +13,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `fastfft-0.1.5/src/fastfft.egg-info/PKG-INFO` & `fastfft-0.1.7/src/fastfft.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.1.5
+Version: 0.1.7
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
@@ -13,22 +13,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `fastfft-0.1.5/src/fft2/main.cpp` & `fastfft-0.1.7/src/fft2/main.cpp`

 * *Files identical despite different names*


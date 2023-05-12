# Comparing `tmp/objc_types_decoder-0.0.4.tar.gz` & `tmp/objc_types_decoder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objc_types_decoder-0.0.4.tar", last modified: Mon Mar 15 07:40:16 2021, max compression
+gzip compressed data, was "objc_types_decoder-0.0.5.tar", last modified: Fri May 12 08:26:12 2023, max compression
```

## Comparing `objc_types_decoder-0.0.4.tar` & `objc_types_decoder-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 07:40:16.891678 objc_types_decoder-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-15 07:40:16.891678 objc_types_decoder-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-03-15 07:40:08.000000 objc_types_decoder-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 07:40:16.887678 objc_types_decoder-0.0.4/objc_types_decoder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-15 07:40:08.000000 objc_types_decoder-0.0.4/objc_types_decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-03-15 07:40:08.000000 objc_types_decoder-0.0.4/objc_types_decoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6429 2021-03-15 07:40:08.000000 objc_types_decoder-0.0.4/objc_types_decoder/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 07:40:16.891678 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-15 07:40:16.000000 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      373 2021-03-15 07:40:16.000000 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 07:40:16.000000 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-03-15 07:40:16.000000 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-03-15 07:40:16.000000 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-03-15 07:40:16.000000 objc_types_decoder-0.0.4/objc_types_decoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-03-15 07:40:16.891678 objc_types_decoder-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-15 07:40:08.000000 objc_types_decoder-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:26:12.297769 objc_types_decoder-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-12 08:26:12.297769 objc_types_decoder-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:26:12.297769 objc_types_decoder-0.0.5/objc_types_decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/objc_types_decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/objc_types_decoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/objc_types_decoder/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:26:12.297769 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-12 08:26:12.000000 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-12 08:26:12.000000 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:26:12.000000 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 08:26:12.000000 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 08:26:12.000000 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 08:26:12.000000 objc_types_decoder-0.0.5/objc_types_decoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:26:12.297769 objc_types_decoder-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:26:12.297769 objc_types_decoder-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/tests/test_decode_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-12 08:25:55.000000 objc_types_decoder-0.0.5/tests/test_decode_type_with_tail_sanity.py
```

### Comparing `objc_types_decoder-0.0.4/README.md` & `objc_types_decoder-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # objc-types-decoder
 
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/matan1008/objc-types-decoder.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/matan1008/objc-types-decoder/context:python)
+[![Python application](https://github.com/matan1008/objc-types-decoder/workflows/Python%20application/badge.svg)](https://github.com/matan1008/objc-types-decoder/actions/workflows/python-app.yml "Python application action")
+[![Pypi version](https://img.shields.io/pypi/v/objc-types-decoder.svg)](https://pypi.org/project/objc-types-decoder/ "PyPi package")
+[![Downloads](https://static.pepy.tech/personalized-badge/objc-types-decoder?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/objc-types-decoder)
 
 
 A type decoder for Objective-C types.
 
 It translates the encoded Objective-C type notation, the notation that the `@encode` function returns, into a readable
 form that tries to be as close as possible to the original type definition.
```

### Comparing `objc_types_decoder-0.0.4/objc_types_decoder/decode.py` & `objc_types_decoder-0.0.5/objc_types_decoder/decode.py`

 * *Files identical despite different names*


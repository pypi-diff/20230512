# Comparing `tmp/streaming-stt-nemo-0.1.1a1.tar.gz` & `tmp/streaming-stt-nemo-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming-stt-nemo-0.1.1a1.tar", last modified: Wed Mar 29 19:54:37 2023, max compression
+gzip compressed data, was "streaming-stt-nemo-0.1.2a0.tar", last modified: Fri May 12 18:44:24 2023, max compression
```

## Comparing `streaming-stt-nemo-0.1.1a1.tar` & `streaming-stt-nemo-0.1.2a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:54:37.098499 streaming-stt-nemo-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-29 19:54:37.098499 streaming-stt-nemo-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:54:32.000000 streaming-stt-nemo-0.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 19:54:37.098499 streaming-stt-nemo-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-29 19:54:32.000000 streaming-stt-nemo-0.1.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:54:37.094499 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-29 19:54:32.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-29 19:54:32.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:54:37.098499 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-29 19:54:37.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-29 19:54:37.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 19:54:37.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 19:54:37.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-29 19:54:37.000000 streaming-stt-nemo-0.1.1a1/streaming_stt_nemo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:44:24.833705 streaming-stt-nemo-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-12 18:44:24.833705 streaming-stt-nemo-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:44:20.000000 streaming-stt-nemo-0.1.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:44:24.833705 streaming-stt-nemo-0.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-12 18:44:20.000000 streaming-stt-nemo-0.1.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:44:24.833705 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-12 18:44:20.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-12 18:44:20.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:44:24.833705 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-12 18:44:24.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-12 18:44:24.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:44:24.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:44:24.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 18:44:24.000000 streaming-stt-nemo-0.1.2a0/streaming_stt_nemo.egg-info/top_level.txt
```

### Comparing `streaming-stt-nemo-0.1.1a1/setup.py` & `streaming-stt-nemo-0.1.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `streaming-stt-nemo-0.1.1a1/streaming_stt_nemo/configs.py` & `streaming-stt-nemo-0.1.2a0/streaming_stt_nemo/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,8 +51,14 @@
     },
     "pt": {
         "model": "neongeckocom/stt_pt_citrinet_512_gamma_0_25", 
     },
     "ca": {
         "model": "neongeckocom/stt_ca_citrinet_512_gamma_0_25", 
     },
-}
+}
+
+
+sample_rate = 16000
+
+
+subfolder_name = "onnx"
```


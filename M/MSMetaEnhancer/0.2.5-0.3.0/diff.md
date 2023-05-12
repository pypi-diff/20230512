# Comparing `tmp/MSMetaEnhancer-0.2.5.tar.gz` & `tmp/MSMetaEnhancer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MSMetaEnhancer-0.2.5.tar", last modified: Sat Oct 15 13:34:46 2022, max compression
+gzip compressed data, was "MSMetaEnhancer-0.3.0.tar", last modified: Fri May 12 07:35:50 2023, max compression
```

## Comparing `MSMetaEnhancer-0.2.5.tar` & `MSMetaEnhancer-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.298353 MSMetaEnhancer-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.282353 MSMetaEnhancer-0.2.5/MSMetaEnhancer/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.286353 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Annotator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Curator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Spectra.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.286353 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.290353 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/compute/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/compute/ComputeConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/compute/RDKit.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.290353 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/
--rw-r--r--   0 runner    (1001) docker     (121)     5743 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/BridgeDB.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/CIR.py
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/CTS.py
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/IDSM.py
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/NLM.py
--rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/PubChem.py
--rw-r--r--   0 runner    (1001) docker     (121)     4895 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/WebConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.294353 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/ConverterBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Job.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/LogRecord.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Throttler.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.282353 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-10-15 13:34:46.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-10-15 13:34:46.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-15 13:34:46.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-15 13:34:46.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-10-15 13:34:46.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-15 13:34:46.000000 MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-10-15 13:34:46.298353 MSMetaEnhancer-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:46.294353 MSMetaEnhancer-0.2.5/galaxy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/galaxy/generate_options.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-15 13:34:46.298353 MSMetaEnhancer-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-10-15 13:34:27.000000 MSMetaEnhancer-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.652687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.652687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/Annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/Curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.652687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.652687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/compute/ComputeConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/compute/RDKit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/BridgeDb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/CIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/IDSM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/PubChem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/WebConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/data/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/data/DataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/data/Spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/ConverterBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/LogRecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Throttler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.652687 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-12 07:35:50.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-12 07:35:50.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:35:50.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:35:50.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 07:35:50.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 07:35:50.000000 MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/galaxy/generate_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:35:50.656687 MSMetaEnhancer-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-12 07:35:38.000000 MSMetaEnhancer-0.3.0/setup.py
```

### Comparing `MSMetaEnhancer-0.2.5/LICENSE` & `MSMetaEnhancer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/app.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 import asyncio
 
 import aiohttp
 
 from MSMetaEnhancer.libs.Annotator import Annotator
 from MSMetaEnhancer.libs.Converter import Converter
 from MSMetaEnhancer.libs.Curator import Curator
-from MSMetaEnhancer.libs.Spectra import Spectra
+from MSMetaEnhancer.libs.data import Spectra, DataFrame
 from MSMetaEnhancer.libs.utils import logger
 from MSMetaEnhancer.libs.utils.ConverterBuilder import ConverterBuilder
 from MSMetaEnhancer.libs.utils.Errors import UnknownSpectraFormat
 from MSMetaEnhancer.libs.utils.Job import convert_to_jobs
 from MSMetaEnhancer.libs.utils.Monitor import Monitor
 
 
 class Application:
     def __init__(self, log_level='info', log_file=None):
-        self.spectra = Spectra()
+        self.data = None
         logger.setup(log_level, log_file)
 
-    def load_spectra(self, filename, file_format):
+    def load_data(self, filename, file_format):
         """
         High level method to load Spectra data from given file.
 
         :param filename: path to source spectra file
         :param file_format: format of spectra
         """
-        try:
-            getattr(self.spectra, f'load_from_{file_format}')(filename)
-        except AttributeError:
+        if file_format in ['msp', 'mgf', 'json']:
+            self.data = Spectra()
+        elif file_format in ['csv', 'tsv', 'xlsx']:
+            self.data = DataFrame()
+        else:
             raise UnknownSpectraFormat(f'Format {file_format} not supported.')
+        self.data.load_data(filename, file_format)
 
-    def save_spectra(self, filename, file_format):
+    def save_data(self, filename, file_format):
         """
         High level method to save Spectra data to given file.
 
         :param filename: path to target file
         :param file_format: desired format of spectra
         """
-        try:
-            getattr(self.spectra, f'save_to_{file_format}')(filename)
-        except Exception:
-            raise UnknownSpectraFormat(f'Format {file_format} not supported.')
+        self.data.save_data(filename, file_format)
 
-    def curate_spectra(self):
+    def curate_metadata(self):
         """
-        Updates current Spectra data by curation process.
+        Updates metadata by curation process.
 
         This includes e.g. normalisation of CAS numbers.
         """
-        self.spectra = Curator().curate_spectra(self.spectra)
+        curated_metadata = Curator().curate_metadata(self.data.get_metadata())
+        self.data.fuse_metadata(curated_metadata)
 
     async def annotate_spectra(self, converters, jobs=None, repeat=False, monitor=Monitor(), annotator=Annotator()):
         """
         Annotates current Spectra data by specified jobs.
 
         Used converters must be specified.
         Jobs do not have to be given, all available jobs will be executed instead.
@@ -80,16 +81,18 @@
                 if not jobs:
                     jobs = []
                     converter: Converter
                     for converter in converters.values():
                         jobs += converter.get_conversion_functions()
                 jobs = convert_to_jobs(jobs)
 
-                logger.set_target_attributes(jobs, len(self.spectra.spectrums))
+                metadata_list = self.data.get_metadata()
+
+                logger.set_target_attributes(jobs, len(metadata_list))
 
-                results = await asyncio.gather(*[annotator.annotate(spectra, jobs, repeat)
-                                                 for spectra in self.spectra.spectrums])
+                results = await asyncio.gather(*[annotator.annotate(metadata, jobs, repeat)
+                                                 for metadata in metadata_list])
             finally:
                 monitor.join()
 
-        self.spectra.spectrums = results
+        self.data.fuse_metadata(results)
         logger.write_metrics()
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Annotator.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/Annotator.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,27 @@
     def __init__(self):
         self.converters = dict()
         self.curator = Curator()
 
     def set_converters(self, converters):
         self.converters = converters
 
-    async def annotate(self, spectra, jobs, repeat=False):
+    async def annotate(self, metadata, jobs, repeat=False):
         """
         Runs all jobs to add annotations to given dictionary containing metadata
 
         The method goes through specified jobs of form (Source, Target, Converter)
         and tries to obtain 'Target' attribute based on 'Source' attribute using
         'Converter' converter.
 
-        :param spectra: given spectra metadata
+        :param metadata: given metadata
         :param jobs: specified list of jobs to be executed
         :param repeat: if some metadata was added, all jobs are executed again
         :return: annotated dictionary
         """
-        metadata = spectra.metadata
         cache = dict()
         log = LogRecord(dict(metadata))
         logger.add_coverage_before(metadata.keys())
 
         added_metadata = True
         while added_metadata:
             added_metadata = False
@@ -53,16 +52,15 @@
                         log.update(Exception(traceback.format_exc()), job, level=1)
                 else:
                     log.update(DataAlreadyPresent(f'Requested attribute {job.target} already present.'), job, level=2)
 
         logger.add_logs(log)
         logger.add_coverage_after(metadata.keys())
 
-        spectra.metadata = metadata
-        return spectra
+        return metadata
 
     async def execute_job_with_cache(self, job, metadata, cache, warning):
         """
         Execute given job in cached mode. Cache is converter specific
         and spectra specific.
 
         Raises TargetAttributeNotRetrieved
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Converter.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/Converter.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/Spectra.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/data/Spectra.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 from typing import List
-
 from matchms import Spectrum
-from matchms.exporting import save_as_msp
-from matchms.importing import load_from_msp
+import matchms.exporting
+import matchms.importing
+
+from MSMetaEnhancer.libs.data.Data import Data
+from MSMetaEnhancer.libs.utils.Errors import UnknownSpectraFormat
 
 
-class Spectra:
+class Spectra(Data):
     """
     Spectra class represents a single spectra dataset as a list.
     It is using `matchms` package to load and save MSP files.
     """
     def __init__(self):
         self.spectrums: List[Spectrum] = []
 
     def __eq__(self, other):
         if len(self.spectrums) == len(other.spectrums):
             return all([spectra_eq(self.spectrums[i], other.spectrums[i]) for i in range(len(self.spectrums))])
         else:
             return False
 
-    def load_from_msp(self, filename: str):
+    def load_data(self, filename: str, file_format: str):
         """
-        Loads given MSP filename as a list of matchms.Spectra objects and
-        stores them in self.spectrums attribute
+        Loads given file as a list of matchms.Spectra objects.
 
-        :param filename: given MSP file
+        Supported formats: msp, mgf, json
+
+        :param filename: given file
+        :param file_format: format of the input file
         """
-        self.spectrums = list(load_from_msp(filename))
+        self.spectrums = list(getattr(matchms.importing, f'load_from_{file_format}')(filename))
 
-    def save_to_msp(self, filename: str):
+    def save_data(self, filename: str, file_format: str):
         """
         Exports all matchms.Spectra objects stored in self.spectrums to
         a file given by filename
 
-        :param filename: target MSP file
+        Supported formats: msp, mgf, json
+
+        :param filename: target file
+        :param file_format: format of the output file
         """
-        save_as_msp(self.spectrums, filename)
+        try:
+            getattr(matchms.exporting, f'save_as_{file_format}')(self.spectrums, filename)
+        except Exception:
+            raise UnknownSpectraFormat(f'Format {file_format} not supported.')
+
+    def get_metadata(self):
+        return [spectra.metadata for spectra in self.spectrums]
+
+    def fuse_metadata(self, metadata):
+        for i in range(len(metadata)):
+            self.spectrums[i].metadata = metadata[i]
 
 
 def spectra_eq(first: Spectrum, second: Spectrum):
     """
     Compare two Spectra objects.
     Native __eq__ definition does not work properly.
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/BridgeDB.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/BridgeDb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from MSMetaEnhancer.libs.converters.web.WebConverter import WebConverter
 
 
-class BridgeDB(WebConverter):
+class BridgeDb(WebConverter):
     """
     BridgeDb is a framework to map identifiers between various biological databases. These mappings are provided for
     genes, proteins, genetic variants, metabolites, and metabolic reactions
 
     More info about the available conversions: https://bridgedb.github.io/
     """
     def __init__(self, session):
         super().__init__(session)
         # service URLs
-        self.endpoints = {'BridgeDB': 'https://webservice.bridgedb.org/Human/xrefs/'}
+        self.endpoints = {'BridgeDb': 'https://webservice.bridgedb.org/Human/xrefs/'}
 
         self.codes = {'hmdbid': 'Ch', 'pubchemid': 'Cpc', 'chemspiderid': 'Cs', 'wikidataid': 'Wd', 'chebiid': 'Ce',
                       'keggid': 'Ck'}
         self.identifiers = {'PubChem-compound': 'pubchemid', 'Chemspider': 'chemspiderid', 'ChEBI': 'chebiid',
                             'HMDB': 'hmdbid', 'Wikidata': 'wikidataid', 'KEGG Compound': 'keggid'}
 
         # generate top level methods defining allowed conversions
@@ -50,82 +50,82 @@
                        ('keggid', 'wikidataid', 'from_keggid'),
                        ('keggid', 'chebiid', 'from_keggid'),
                        ]
         self.create_top_level_conversion_methods(conversions)
 
     async def from_hmdbid(self, hmdbid):
         """
-        Convert HMDB ID to all possible IDs using BridgeDB web service
+        Convert HMDB ID to all possible IDs using BridgeDb web service
 
         :param hmdbid: given HMDB ID number
         :return: obtained IDs
         """
         args = f'{self.codes["hmdbid"]}/{hmdbid}'
         return await self.call_service(args)
 
     async def from_pubchemid(self, pubchemid):
         """
-        Convert PubChem ID to all possible IDs using BridgeDB web service
+        Convert PubChem ID to all possible IDs using BridgeDb web service
 
         :param pubchemid: given PubChem ID number
         :return: obtained IDs
         """
         args = f'{self.codes["pubchemid"]}/{pubchemid}'
         return await self.call_service(args)
 
     async def from_chemspiderid(self, chemspiderid):
         """
-        Convert ChemSpider ID to all possible IDs using BridgeDB web service
+        Convert ChemSpider ID to all possible IDs using BridgeDb web service
 
         :param chemspiderid: given ChemSpider ID number
         :return: obtained IDs
         """
         args = f'{self.codes["chemspiderid"]}/{chemspiderid}'
         return await self.call_service(args)
 
     async def from_wikidataid(self, wikidataid):
         """
-        Convert WikiData ID to all possible IDs using BridgeDB web service
+        Convert WikiData ID to all possible IDs using BridgeDb web service
 
         :param wikidataid: given WikiData ID number
         :return: obtained IDs
         """
         args = f'{self.codes["wikidataid"]}/{wikidataid}'
         return await self.call_service(args)
 
     async def from_chebiid(self, chebiid):
         """
-        Convert ChEBI ID to all possible IDs using BridgeDB web service
+        Convert ChEBI ID to all possible IDs using BridgeDb web service
 
         :param chebiid: given ChEBI ID number
         :return: obtained IDs
         """
         args = f'{self.codes["chebiid"]}/{chebiid}'
         return await self.call_service(args)
 
     async def from_keggid(self, keggid):
         """
-        Convert KEGG ID to all possible IDs using BridgeDB web service
+        Convert KEGG ID to all possible IDs using BridgeDb web service
 
         :param keggid: given KEGG ID number
         :return: obtained IDs
         """
         args = f'{self.codes["keggid"]}/{keggid}'
         return await self.call_service(args)
 
     async def call_service(self, args):
-        response = await self.query_the_service('BridgeDB', args)
+        response = await self.query_the_service('BridgeDb', args)
         if response:
             return self.parse_attributes(response)
 
     def parse_attributes(self, response):
         """
-        Parse all available attributes obtained using BridgeDB.
+        Parse all available attributes obtained using BridgeDb.
 
-        :param response: BridgeDB response to given ID
+        :param response: BridgeDb response to given ID
         :return: all parsed data
         """
         result = dict()
 
         lines = response.split('\n')
         for line in lines:
             if line:
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/CIR.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/CIR.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/CTS.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/CTS.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/IDSM.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/IDSM.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/PubChem.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/PubChem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import asyncio
 import json
-
-from MSMetaEnhancer.libs.converters.web.WebConverter import WebConverter
 from frozendict import frozendict
 
+from MSMetaEnhancer.libs.converters.web.WebConverter import WebConverter
+from MSMetaEnhancer.libs.utils.Generic import string_to_seconds
 from MSMetaEnhancer.libs.utils.Errors import UnknownResponse
 from MSMetaEnhancer.libs.utils.Throttler import Throttler
 
 
 class PubChem(WebConverter):
     """
     PubChem is the world's largest collection of freely accessible chemical information.
@@ -122,15 +123,17 @@
         :param response: given async response
         :param url: service URL
         :param method: GET/POST
         :return: processed response
         """
         result = await response.text()
         if 'X-Throttling-Control' in response.headers:
-            self.adjust_throttling(response.headers['X-Throttling-Control'])
+            sleep_time = self.adjust_throttling(response.headers['X-Throttling-Control'])
+            if sleep_time:
+                await asyncio.sleep(sleep_time)
         if response.ok:
             return result
         else:
             raise UnknownResponse(f'Unknown response {response.status}:{result} for {method} request on {url}.')
 
     def adjust_throttling(self, throttling_header):
         """
@@ -152,23 +155,30 @@
             Request Count status: Green (0%), Request Time status: Green (0%), WebConverter status: Green (20%)
 
             :param header: given PubChem header with Throttling info
             :return: most critical indicator value (maximum of three) with possible complete blacklist indicator
             """
             indicators = header.split(',')
             blocked = False
+            sleep_time = 0
             if 'too many requests per second or blacklisted' in indicators[-1]:
                 blocked = True
-            return {'load': max([parse_status(indicator) for indicator in indicators[:3]]), 'blocked': blocked}
+            if 'Remaining blocking time' in indicators[-1]:
+                sleep_time = string_to_seconds(indicators[-1].split(': ')[1])
+                blocked = True
+            return {'load': max([parse_status(indicator) for indicator in indicators[:3]]), 
+                    'blocked': blocked,
+                    'sleep_time': sleep_time}
 
         status = parse_pubchem_info(throttling_header)
         if status['blocked'] or status['load'] > 75:
             self.throttler.decrease_limit()
         elif status['load'] < 25:
             self.throttler.increase_limit()
+        return status['sleep_time']
 
     def parse_attributes(self, response):
         """
         Parse all available attributes (specified in self.attributes) from given response.
 
         Method does not return anything, instead stores data in local cache.
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/converters/web/WebConverter.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/converters/web/WebConverter.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/ConverterBuilder.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/ConverterBuilder.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Errors.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Errors.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Job.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Job.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/LogRecord.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/LogRecord.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Logger.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Metrics.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Metrics.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Monitor.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Monitor.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer/libs/utils/Throttler.py` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer/libs/utils/Throttler.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         if self.rate < self.rate_limit:
             self.rate += 1
 
     def decrease_limit(self):
         """
         Decrease rate (must be always positive).
         """
-        if self.rate > 0:
+        if self.rate > 1:
             self.rate -= 1
 
     def flush(self):
         now = time.monotonic()
         while self._task_logs:
             if now - self._task_logs[0] > self.period:
                 self._task_logs.popleft()
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/PKG-INFO` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSMetaEnhancer
-Version: 0.2.5
+Version: 0.3.0
 Summary: Repository for tool that adds more annotations (e.g. SMILES, InChI, CAS number) to MSP files (Python version).
 Home-page: https://github.com/RECETOX/MSMetaEnhancer
 Author: Matej Trojak
 Author-email: matej.trojak@recetox.muni.cz
 Maintainer: RECETOX
 Maintainer-email: GalaxyToolsDevelopmentandDeployment@space.muni.cz
 License: MIT
@@ -14,36 +14,40 @@
 License-File: LICENSE
 
 ## MSMetaEnhancer
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/msmetaenhancer/README.html)
 [![docs](https://readthedocs.org/projects/msmetaenhancer/badge/?version=latest)](https://msmetaenhancer.readthedocs.io/en/latest/)
 [![Conda](https://img.shields.io/conda/v/bioconda/msmetaenhancer)](https://anaconda.org/bioconda/msmetaenhancer)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04494/status.svg)](https://doi.org/10.21105/joss.04494)
 
 **MSMetaEnhancer** is a tool used for `.msp` files annotation.
-It adds metadata like SMILES, InChI, and CAS number fetched from the following services: [CIR](https://cactus.nci.nih.gov/chemical/structure_documentation), [CTS](https://cts.fiehnlab.ucdavis.edu/), [NLM](https://chem.nlm.nih.gov), [PubChem](https://pubchem.ncbi.nlm.nih.gov/), [IDSM](https://idsm.elixir-czech.cz/), and [BridgeDB](https://bridgedb.github.io/).
+It adds metadata like SMILES, InChI, and CAS number fetched from the following services: [CIR](https://cactus.nci.nih.gov/chemical/structure_documentation), [CTS](https://cts.fiehnlab.ucdavis.edu/), [PubChem](https://pubchem.ncbi.nlm.nih.gov/), [IDSM](https://idsm.elixir-czech.cz/), and [BridgeDb](https://bridgedb.github.io/).
 The app uses asynchronous implementation of annotation process allowing for optimal fetching speed.
 
+If you use MSMetaEnhancer in your work, please cite the following publication:
+
+Troják et al., (2022). MSMetaEnhancer: A Python package for mass spectra metadata annotation. Journal of Open Source Software, 7(79), 4494, https://doi.org/10.21105/joss.04494
 ### Usage
 
 ```python
 import asyncio
 
 from MSMetaEnhancer import Application
 
 app = Application()
 
 # import your .msp file
 app.load_spectra('tests/test_data/sample.msp', file_format='msp')
 
 # curate given metadata (e.g. fix CAS numbers)
-app.curate_spectra()
+app.curate_metadata()
 
 # specify requested services (these are supported)
-services = ['CTS', 'CIR', 'NLM', 'IDSM', 'PubChem', 'BridgeDB', 'RDKit']
+services = ['CTS', 'CIR', 'IDSM', 'PubChem', 'BridgeDb', 'RDKit']
 
 # specify requested jobs
 jobs = [('name', 'inchi', 'IDSM'), ('inchi', 'formula', 'IDSM'), ('inchi', 'inchikey', 'IDSM'),
         ('inchi', 'iupac_name', 'IDSM'), ('inchi', 'canonical_smiles', 'IDSM')]
 
 # run asynchronous annotations of spectra data
 asyncio.run(app.annotate_spectra(services, jobs))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MSMetaEnhancer-0.2.5/MSMetaEnhancer.egg-info/SOURCES.txt` & `MSMetaEnhancer-0.3.0/MSMetaEnhancer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 MSMetaEnhancer.egg-info/dependency_links.txt
 MSMetaEnhancer.egg-info/not-zip-safe
 MSMetaEnhancer.egg-info/requires.txt
 MSMetaEnhancer.egg-info/top_level.txt
 MSMetaEnhancer/libs/Annotator.py
 MSMetaEnhancer/libs/Converter.py
 MSMetaEnhancer/libs/Curator.py
-MSMetaEnhancer/libs/Spectra.py
 MSMetaEnhancer/libs/__init__.py
 MSMetaEnhancer/libs/converters/__init__.py
 MSMetaEnhancer/libs/converters/compute/ComputeConverter.py
 MSMetaEnhancer/libs/converters/compute/RDKit.py
 MSMetaEnhancer/libs/converters/compute/__init__.py
-MSMetaEnhancer/libs/converters/web/BridgeDB.py
+MSMetaEnhancer/libs/converters/web/BridgeDb.py
 MSMetaEnhancer/libs/converters/web/CIR.py
 MSMetaEnhancer/libs/converters/web/CTS.py
 MSMetaEnhancer/libs/converters/web/IDSM.py
-MSMetaEnhancer/libs/converters/web/NLM.py
 MSMetaEnhancer/libs/converters/web/PubChem.py
 MSMetaEnhancer/libs/converters/web/WebConverter.py
 MSMetaEnhancer/libs/converters/web/__init__.py
+MSMetaEnhancer/libs/data/Data.py
+MSMetaEnhancer/libs/data/DataFrame.py
+MSMetaEnhancer/libs/data/Spectra.py
+MSMetaEnhancer/libs/data/__init__.py
 MSMetaEnhancer/libs/utils/ConverterBuilder.py
 MSMetaEnhancer/libs/utils/Errors.py
 MSMetaEnhancer/libs/utils/Generic.py
 MSMetaEnhancer/libs/utils/Job.py
 MSMetaEnhancer/libs/utils/LogRecord.py
 MSMetaEnhancer/libs/utils/Logger.py
 MSMetaEnhancer/libs/utils/Metrics.py
```

### Comparing `MSMetaEnhancer-0.2.5/PKG-INFO` & `MSMetaEnhancer-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSMetaEnhancer
-Version: 0.2.5
+Version: 0.3.0
 Summary: Repository for tool that adds more annotations (e.g. SMILES, InChI, CAS number) to MSP files (Python version).
 Home-page: https://github.com/RECETOX/MSMetaEnhancer
 Author: Matej Trojak
 Author-email: matej.trojak@recetox.muni.cz
 Maintainer: RECETOX
 Maintainer-email: GalaxyToolsDevelopmentandDeployment@space.muni.cz
 License: MIT
@@ -14,36 +14,40 @@
 License-File: LICENSE
 
 ## MSMetaEnhancer
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/msmetaenhancer/README.html)
 [![docs](https://readthedocs.org/projects/msmetaenhancer/badge/?version=latest)](https://msmetaenhancer.readthedocs.io/en/latest/)
 [![Conda](https://img.shields.io/conda/v/bioconda/msmetaenhancer)](https://anaconda.org/bioconda/msmetaenhancer)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04494/status.svg)](https://doi.org/10.21105/joss.04494)
 
 **MSMetaEnhancer** is a tool used for `.msp` files annotation.
-It adds metadata like SMILES, InChI, and CAS number fetched from the following services: [CIR](https://cactus.nci.nih.gov/chemical/structure_documentation), [CTS](https://cts.fiehnlab.ucdavis.edu/), [NLM](https://chem.nlm.nih.gov), [PubChem](https://pubchem.ncbi.nlm.nih.gov/), [IDSM](https://idsm.elixir-czech.cz/), and [BridgeDB](https://bridgedb.github.io/).
+It adds metadata like SMILES, InChI, and CAS number fetched from the following services: [CIR](https://cactus.nci.nih.gov/chemical/structure_documentation), [CTS](https://cts.fiehnlab.ucdavis.edu/), [PubChem](https://pubchem.ncbi.nlm.nih.gov/), [IDSM](https://idsm.elixir-czech.cz/), and [BridgeDb](https://bridgedb.github.io/).
 The app uses asynchronous implementation of annotation process allowing for optimal fetching speed.
 
+If you use MSMetaEnhancer in your work, please cite the following publication:
+
+Troják et al., (2022). MSMetaEnhancer: A Python package for mass spectra metadata annotation. Journal of Open Source Software, 7(79), 4494, https://doi.org/10.21105/joss.04494
 ### Usage
 
 ```python
 import asyncio
 
 from MSMetaEnhancer import Application
 
 app = Application()
 
 # import your .msp file
 app.load_spectra('tests/test_data/sample.msp', file_format='msp')
 
 # curate given metadata (e.g. fix CAS numbers)
-app.curate_spectra()
+app.curate_metadata()
 
 # specify requested services (these are supported)
-services = ['CTS', 'CIR', 'NLM', 'IDSM', 'PubChem', 'BridgeDB', 'RDKit']
+services = ['CTS', 'CIR', 'IDSM', 'PubChem', 'BridgeDb', 'RDKit']
 
 # specify requested jobs
 jobs = [('name', 'inchi', 'IDSM'), ('inchi', 'formula', 'IDSM'), ('inchi', 'inchikey', 'IDSM'),
         ('inchi', 'iupac_name', 'IDSM'), ('inchi', 'canonical_smiles', 'IDSM')]
 
 # run asynchronous annotations of spectra data
 asyncio.run(app.annotate_spectra(services, jobs))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MSMetaEnhancer-0.2.5/README.md` & `MSMetaEnhancer-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 ## MSMetaEnhancer
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/msmetaenhancer/README.html)
 [![docs](https://readthedocs.org/projects/msmetaenhancer/badge/?version=latest)](https://msmetaenhancer.readthedocs.io/en/latest/)
 [![Conda](https://img.shields.io/conda/v/bioconda/msmetaenhancer)](https://anaconda.org/bioconda/msmetaenhancer)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04494/status.svg)](https://doi.org/10.21105/joss.04494)
 
 **MSMetaEnhancer** is a tool used for `.msp` files annotation.
-It adds metadata like SMILES, InChI, and CAS number fetched from the following services: [CIR](https://cactus.nci.nih.gov/chemical/structure_documentation), [CTS](https://cts.fiehnlab.ucdavis.edu/), [NLM](https://chem.nlm.nih.gov), [PubChem](https://pubchem.ncbi.nlm.nih.gov/), [IDSM](https://idsm.elixir-czech.cz/), and [BridgeDB](https://bridgedb.github.io/).
+It adds metadata like SMILES, InChI, and CAS number fetched from the following services: [CIR](https://cactus.nci.nih.gov/chemical/structure_documentation), [CTS](https://cts.fiehnlab.ucdavis.edu/), [PubChem](https://pubchem.ncbi.nlm.nih.gov/), [IDSM](https://idsm.elixir-czech.cz/), and [BridgeDb](https://bridgedb.github.io/).
 The app uses asynchronous implementation of annotation process allowing for optimal fetching speed.
 
+If you use MSMetaEnhancer in your work, please cite the following publication:
+
+Troják et al., (2022). MSMetaEnhancer: A Python package for mass spectra metadata annotation. Journal of Open Source Software, 7(79), 4494, https://doi.org/10.21105/joss.04494
 ### Usage
 
 ```python
 import asyncio
 
 from MSMetaEnhancer import Application
 
 app = Application()
 
 # import your .msp file
 app.load_spectra('tests/test_data/sample.msp', file_format='msp')
 
 # curate given metadata (e.g. fix CAS numbers)
-app.curate_spectra()
+app.curate_metadata()
 
 # specify requested services (these are supported)
-services = ['CTS', 'CIR', 'NLM', 'IDSM', 'PubChem', 'BridgeDB', 'RDKit']
+services = ['CTS', 'CIR', 'IDSM', 'PubChem', 'BridgeDb', 'RDKit']
 
 # specify requested jobs
 jobs = [('name', 'inchi', 'IDSM'), ('inchi', 'formula', 'IDSM'), ('inchi', 'inchikey', 'IDSM'),
         ('inchi', 'iupac_name', 'IDSM'), ('inchi', 'canonical_smiles', 'IDSM')]
 
 # run asynchronous annotations of spectra data
 asyncio.run(app.annotate_spectra(services, jobs))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MSMetaEnhancer-0.2.5/galaxy/generate_options.py` & `MSMetaEnhancer-0.3.0/galaxy/generate_options.py`

 * *Files identical despite different names*

### Comparing `MSMetaEnhancer-0.2.5/setup.py` & `MSMetaEnhancer-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(name='MSMetaEnhancer',
-      version='0.2.5',
+      version='0.3.0',
       description='Repository for tool that adds more annotations '
                   '(e.g. SMILES, InChI, CAS number) to MSP files (Python version).',
       long_description=readme,
       long_description_content_type="text/markdown",
       url='https://github.com/RECETOX/MSMetaEnhancer',
       author='Matej Trojak',
       author_email='matej.trojak@recetox.muni.cz',
```


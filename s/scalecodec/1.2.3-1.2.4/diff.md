# Comparing `tmp/scalecodec-1.2.3.tar.gz` & `tmp/scalecodec-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalecodec-1.2.3.tar", last modified: Mon May  8 12:30:38 2023, max compression
+gzip compressed data, was "scalecodec-1.2.4.tar", last modified: Fri May 12 10:42:01 2023, max compression
```

## Comparing `scalecodec-1.2.3.tar` & `scalecodec-1.2.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:30:38.874609 scalecodec-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 12:29:24.000000 scalecodec-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-05-08 12:30:38.874609 scalecodec-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-05-08 12:29:24.000000 scalecodec-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:30:38.866609 scalecodec-1.2.3/scalecodec/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:30:38.870609 scalecodec-1.2.3/scalecodec/type_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/acala.json
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/canvas.json
--rw-r--r--   0 runner    (1001) docker     (123)    66503 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/core.json
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/crust.json
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/development.json
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/karura.json
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/kusama.json
--rw-r--r--   0 runner    (1001) docker     (123)   208220 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/moonbase-alpha.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/moonbeam.json
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/moonriver.json
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/polkadot.json
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/polymesh-mainnet.json
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/polymesh-testnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/rococo.json
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/statemine.json
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/statemint.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/substrate-node-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/type_registry/westend.json
--rw-r--r--   0 runner    (1001) docker     (123)   105662 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:30:38.870609 scalecodec-1.2.3/scalecodec/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-05-08 12:29:24.000000 scalecodec-1.2.3/scalecodec/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:30:38.866609 scalecodec-1.2.3/scalecodec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-05-08 12:30:38.000000 scalecodec-1.2.3/scalecodec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 12:30:38.000000 scalecodec-1.2.3/scalecodec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:30:38.000000 scalecodec-1.2.3/scalecodec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 12:30:38.000000 scalecodec-1.2.3/scalecodec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 12:30:38.000000 scalecodec-1.2.3/scalecodec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:30:38.874609 scalecodec-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-08 12:29:24.000000 scalecodec-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:30:38.874609 scalecodec-1.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    89166 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_extrinsic_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_runtime_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_scale_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    36470 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_scale_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_scalebytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_type_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)   179798 2023-05-08 12:29:24.000000 scalecodec-1.2.3/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:01.911039 scalecodec-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 10:40:42.000000 scalecodec-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-05-12 10:42:01.911039 scalecodec-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-05-12 10:40:42.000000 scalecodec-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:01.907039 scalecodec-1.2.4/scalecodec/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:01.911039 scalecodec-1.2.4/scalecodec/type_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/acala.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/canvas.json
+-rw-r--r--   0 runner    (1001) docker     (123)    66678 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/crust.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/development.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/karura.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/kusama.json
+-rw-r--r--   0 runner    (1001) docker     (123)   208220 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/moonbase-alpha.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/moonbeam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/moonriver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/polkadot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/polymesh-mainnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/polymesh-testnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/rococo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/statemine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/statemint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/substrate-node-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/type_registry/westend.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105662 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:01.911039 scalecodec-1.2.4/scalecodec/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-05-12 10:40:42.000000 scalecodec-1.2.4/scalecodec/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:01.907039 scalecodec-1.2.4/scalecodec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-05-12 10:42:01.000000 scalecodec-1.2.4/scalecodec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-12 10:42:01.000000 scalecodec-1.2.4/scalecodec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:42:01.000000 scalecodec-1.2.4/scalecodec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 10:42:01.000000 scalecodec-1.2.4/scalecodec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 10:42:01.000000 scalecodec-1.2.4/scalecodec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:42:01.911039 scalecodec-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-12 10:40:42.000000 scalecodec-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:01.911039 scalecodec-1.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    89166 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_extrinsic_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_runtime_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_scale_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36470 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_scale_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_scalebytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_type_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179798 2023-05-12 10:40:42.000000 scalecodec-1.2.4/test/test_type_registry.py
```

### Comparing `scalecodec-1.2.3/LICENSE` & `scalecodec-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/PKG-INFO` & `scalecodec-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalecodec
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python SCALE Codec Library
 Home-page: https://github.com/polkascan/py-scale-codec
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 Keywords: scale codec polkascan polkadot substrate blockchain kusama
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scalecodec-1.2.3/README.md` & `scalecodec-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/__init__.py` & `scalecodec-1.2.4/scalecodec/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/base.py` & `scalecodec-1.2.4/scalecodec/base.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/exceptions.py` & `scalecodec-1.2.4/scalecodec/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/__init__.py` & `scalecodec-1.2.4/scalecodec/type_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/canvas.json` & `scalecodec-1.2.4/scalecodec/type_registry/canvas.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/core.json` & `scalecodec-1.2.4/scalecodec/type_registry/core.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993489583333334%*

 * *Differences: {"'runtime_api'": "{'TransactionPaymentCallApi': {'types': {'DispatchClass': OrderedDict([('type', "*

 * *                  "'enum'), ('value_list', ['Normal', 'Operational', 'Mandatory'])])}}}"}*

```diff
@@ -1701,14 +1701,22 @@
                             "type": "u32"
                         }
                     ],
                     "type": "RuntimeDispatchInfo"
                 }
             },
             "types": {
+                "DispatchClass": {
+                    "type": "enum",
+                    "value_list": [
+                        "Normal",
+                        "Operational",
+                        "Mandatory"
+                    ]
+                },
                 "FeeDetails": {
                     "type": "struct",
                     "type_mapping": [
                         [
                             "inclusion_fee",
                             "Option<InclusionFee>"
                         ],
```

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/crust.json` & `scalecodec-1.2.4/scalecodec/type_registry/crust.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/development.json` & `scalecodec-1.2.4/scalecodec/type_registry/development.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/karura.json` & `scalecodec-1.2.4/scalecodec/type_registry/karura.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/kusama.json` & `scalecodec-1.2.4/scalecodec/type_registry/kusama.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/legacy.json` & `scalecodec-1.2.4/scalecodec/type_registry/legacy.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/moonriver.json` & `scalecodec-1.2.4/scalecodec/type_registry/moonriver.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/polkadot.json` & `scalecodec-1.2.4/scalecodec/type_registry/polkadot.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/polymesh-mainnet.json` & `scalecodec-1.2.4/scalecodec/type_registry/polymesh-mainnet.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/polymesh-testnet.json` & `scalecodec-1.2.4/scalecodec/type_registry/polymesh-testnet.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/rococo.json` & `scalecodec-1.2.4/scalecodec/type_registry/rococo.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/substrate-node-template.json` & `scalecodec-1.2.4/scalecodec/type_registry/substrate-node-template.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/test.json` & `scalecodec-1.2.4/scalecodec/type_registry/test.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/type_registry/westend.json` & `scalecodec-1.2.4/scalecodec/type_registry/westend.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/types.py` & `scalecodec-1.2.4/scalecodec/types.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/updater.py` & `scalecodec-1.2.4/scalecodec/updater.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/utils/__init__.py` & `scalecodec-1.2.4/scalecodec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/utils/math.py` & `scalecodec-1.2.4/scalecodec/utils/math.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec/utils/ss58.py` & `scalecodec-1.2.4/scalecodec/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/scalecodec.egg-info/PKG-INFO` & `scalecodec-1.2.4/scalecodec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalecodec
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python SCALE Codec Library
 Home-page: https://github.com/polkascan/py-scale-codec
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 Keywords: scale codec polkascan polkadot substrate blockchain kusama
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scalecodec-1.2.3/scalecodec.egg-info/SOURCES.txt` & `scalecodec-1.2.4/scalecodec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/setup.py` & `scalecodec-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_extrinsic_payload.py` & `scalecodec-1.2.4/test/test_extrinsic_payload.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_metadata.py` & `scalecodec-1.2.4/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_runtime_call.py` & `scalecodec-1.2.4/test/test_runtime_call.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_runtime_configuration.py` & `scalecodec-1.2.4/test/test_runtime_configuration.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_scale_info.py` & `scalecodec-1.2.4/test/test_scale_info.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_scale_types.py` & `scalecodec-1.2.4/test/test_scale_types.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_scalebytes.py` & `scalecodec-1.2.4/test/test_scalebytes.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_ss58.py` & `scalecodec-1.2.4/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_type_encoding.py` & `scalecodec-1.2.4/test/test_type_encoding.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.3/test/test_type_registry.py` & `scalecodec-1.2.4/test/test_type_registry.py`

 * *Files identical despite different names*


# Comparing `tmp/substrate-interface-1.7.0.tar.gz` & `tmp/substrate-interface-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-interface-1.7.0.tar", last modified: Mon May  8 13:57:05 2023, max compression
+gzip compressed data, was "substrate-interface-1.7.1.tar", last modified: Fri May 12 10:59:50 2023, max compression
```

## Comparing `substrate-interface-1.7.0.tar` & `substrate-interface-1.7.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.595689 substrate-interface-1.7.0/substrate_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/substrateinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31151 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/substrateinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/ecdsa_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/encrypted_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_create_extrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_extension_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_rpc_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.565325 substrate-interface-1.7.1/substrate_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 10:59:50.000000 substrate-interface-1.7.1/substrate_interface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.565325 substrate-interface-1.7.1/substrateinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31151 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.565325 substrate-interface-1.7.1/substrateinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/ecdsa_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/encrypted_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/substrateinterface/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:59:50.569325 substrate-interface-1.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_create_extrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_extension_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_rpc_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-12 10:53:53.000000 substrate-interface-1.7.1/test/test_type_registry.py
```

### Comparing `substrate-interface-1.7.0/LICENSE` & `substrate-interface-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/PKG-INFO` & `substrate-interface-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.0
+Version: 1.7.1
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.0/README.md` & `substrate-interface-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/setup.py` & `substrate-interface-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         'requests>=2.21.0,<3',
         'xxhash>=1.3.0,<4',
         'ecdsa>=0.17.0,<1',
         'eth-keys>=0.2.1,<1',
         'eth_utils>=1.3.0,<3',
         'pycryptodome>=3.11.0,<4',
         'PyNaCl>=1.0.1,<2',
-        'scalecodec>=1.2.3,<1.3',
+        'scalecodec>=1.2.4,<1.3',
         'py-sr25519-bindings>=0.2.0,<1',
         'py-ed25519-zebra-bindings>=1.0,<2',
         'py-bip39-bindings>=0.1.9,<1'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
```

### Comparing `substrate-interface-1.7.0/substrate_interface.egg-info/PKG-INFO` & `substrate-interface-1.7.1/substrate_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.0
+Version: 1.7.1
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.0/substrate_interface.egg-info/SOURCES.txt` & `substrate-interface-1.7.1/substrate_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/__init__.py` & `substrate-interface-1.7.1/substrateinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/base.py` & `substrate-interface-1.7.1/substrateinterface/base.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/constants.py` & `substrate-interface-1.7.1/substrateinterface/constants.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/contracts.py` & `substrate-interface-1.7.1/substrateinterface/contracts.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/exceptions.py` & `substrate-interface-1.7.1/substrateinterface/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/extensions.py` & `substrate-interface-1.7.1/substrateinterface/extensions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/interfaces.py` & `substrate-interface-1.7.1/substrateinterface/interfaces.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/key.py` & `substrate-interface-1.7.1/substrateinterface/key.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/keypair.py` & `substrate-interface-1.7.1/substrateinterface/keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/storage.py` & `substrate-interface-1.7.1/substrateinterface/storage.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/utils/__init__.py` & `substrate-interface-1.7.1/substrateinterface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/utils/caching.py` & `substrate-interface-1.7.1/substrateinterface/utils/caching.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/utils/ecdsa_helpers.py` & `substrate-interface-1.7.1/substrateinterface/utils/ecdsa_helpers.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/utils/encrypted_json.py` & `substrate-interface-1.7.1/substrateinterface/utils/encrypted_json.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/utils/hasher.py` & `substrate-interface-1.7.1/substrateinterface/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/substrateinterface/utils/ss58.py` & `substrate-interface-1.7.1/substrateinterface/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_block.py` & `substrate-interface-1.7.1/test/test_block.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_contracts.py` & `substrate-interface-1.7.1/test/test_contracts.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_create_extrinsics.py` & `substrate-interface-1.7.1/test/test_create_extrinsics.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_extension_interface.py` & `substrate-interface-1.7.1/test/test_extension_interface.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_helper_functions.py` & `substrate-interface-1.7.1/test/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_init.py` & `substrate-interface-1.7.1/test/test_init.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_keypair.py` & `substrate-interface-1.7.1/test/test_keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_query.py` & `substrate-interface-1.7.1/test/test_query.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_query_map.py` & `substrate-interface-1.7.1/test/test_query_map.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_rpc_compatibility.py` & `substrate-interface-1.7.1/test/test_rpc_compatibility.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_runtime_call.py` & `substrate-interface-1.7.1/test/test_runtime_call.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_ss58.py` & `substrate-interface-1.7.1/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_subscriptions.py` & `substrate-interface-1.7.1/test/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.0/test/test_type_registry.py` & `substrate-interface-1.7.1/test/test_type_registry.py`

 * *Files identical despite different names*


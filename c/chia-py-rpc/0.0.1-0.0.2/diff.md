# Comparing `tmp/chia_py_rpc-0.0.1.tar.gz` & `tmp/chia_py_rpc-0.0.2.tar.gz`

## Comparing `chia_py_rpc-0.0.1.tar` & `chia_py_rpc-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/src/chia_py_rpc/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/src/chia_py_rpc/rpc_connect.py
--rw-r--r--   0        0        0    80547 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/src/chia_py_rpc/wallet.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/LICENSE
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/src/chia_py_rpc/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/src/chia_py_rpc/rpc_connect.py
+-rw-r--r--   0        0        0    80547 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/src/chia_py_rpc/wallet.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 chia_py_rpc-0.0.2/PKG-INFO
```

### Comparing `chia_py_rpc-0.0.1/src/chia_py_rpc/rpc_connect.py` & `chia_py_rpc-0.0.2/src/chia_py_rpc/rpc_connect.py`

 * *Files identical despite different names*

### Comparing `chia_py_rpc-0.0.1/src/chia_py_rpc/wallet.py` & `chia_py_rpc-0.0.2/src/chia_py_rpc/wallet.py`

 * *Files identical despite different names*

### Comparing `chia_py_rpc-0.0.1/LICENSE` & `chia_py_rpc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chia_py_rpc-0.0.1/README.md` & `chia_py_rpc-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 pip install chia-py-rpc
 ```
 
 ## Usage
 Here's an example of how you can use Chia-Py-RPC to send transactions to multiple recipients in a single transaction:
 
 ```
-from chia_py_rpc import ChiaWallet
+from chia_py_rpc import Wallet
 
 # Create an instance of ChiaWallet
-chia_wallet = ChiaWallet()
+wallet = Wallet()
 
 # Specify the wallet ID, additions (recipients), fee, and optional parameters
 wallet_id = 1
 additions = [
     {'amount': 1000000000000, 'puzzle_hash': '0x...'},  # Recipient 1
     {'amount': 500000000000, 'puzzle_hash': '0x...'},  # Recipient 2
 ]
```

### Comparing `chia_py_rpc-0.0.1/pyproject.toml` & `chia_py_rpc-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chia_py_rpc"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="L4bb3rs", email="king@the300.net" },
 ]
 description = "Chia-Py-RPC is a Python library that provides a convenient way to interact with the Chia blockchain using the Chia RPC (Remote Procedure Call) protocol."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `chia_py_rpc-0.0.1/PKG-INFO` & `chia_py_rpc-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: chia_py_rpc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Chia-Py-RPC is a Python library that provides a convenient way to interact with the Chia blockchain using the Chia RPC (Remote Procedure Call) protocol.
 Project-URL: Homepage, https://github.com/L4bb3rs/Chia-Py-RPC
 Project-URL: Bug Tracker, https://github.com/L4bb3rs/Chia-Py-RPC
 Author-email: L4bb3rs <king@the300.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Chia-Py-RPC
 
 Chia-Py-RPC is a Python library that provides a convenient way to interact with the Chia blockchain using the Chia RPC (Remote Procedure Call) protocol. It allows you to send transactions, check balances, and perform other Chia-related operations programmatically from Python.
 
 ## Features
@@ -33,18 +33,18 @@
 pip install chia-py-rpc
 ```
 
 ## Usage
 Here's an example of how you can use Chia-Py-RPC to send transactions to multiple recipients in a single transaction:
 
 ```
-from chia_py_rpc import ChiaWallet
+from chia_py_rpc import Wallet
 
 # Create an instance of ChiaWallet
-chia_wallet = ChiaWallet()
+wallet = Wallet()
 
 # Specify the wallet ID, additions (recipients), fee, and optional parameters
 wallet_id = 1
 additions = [
     {'amount': 1000000000000, 'puzzle_hash': '0x...'},  # Recipient 1
     {'amount': 500000000000, 'puzzle_hash': '0x...'},  # Recipient 2
 ]
```


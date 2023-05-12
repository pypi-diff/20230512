# Comparing `tmp/cyberutils-0.0.3.tar.gz` & `tmp/cyberutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberutils-0.0.3.tar", max compression
+gzip compressed data, was "cyberutils-0.0.4.tar", max compression
```

## Comparing `cyberutils-0.0.3.tar` & `cyberutils-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1075 2023-05-11 06:23:14.946521 cyberutils-0.0.3/LICENSE
--rw-r--r--   0        0        0     3603 2023-05-11 06:23:14.946521 cyberutils-0.0.3/README.md
--rw-r--r--   0        0        0      166 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/__init__.py
--rw-r--r--   0        0        0       77 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/bash/__init__.py
--rw-r--r--   0        0        0     2268 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/bash/execution.py
--rw-r--r--   0        0        0       40 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/contract/__init__.py
--rw-r--r--   0        0        0     1671 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/contract/execution.py
--rw-r--r--   0        0        0       93 2023-05-11 06:23:14.946521 cyberutils-0.0.3/cyberutils/graphql/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-11 06:23:14.950521 cyberutils-0.0.3/cyberutils/graphql/execution.py
--rw-r--r--   0        0        0     1895 2023-05-11 06:23:14.950521 cyberutils-0.0.3/cyberutils/graphql/queries.py
--rw-r--r--   0        0        0     1818 2023-05-11 06:23:14.950521 cyberutils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 cyberutils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-12 07:27:50.772962 cyberutils-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3603 2023-05-12 07:27:50.772962 cyberutils-0.0.4/README.md
+-rw-r--r--   0        0        0      166 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/__init__.py
+-rw-r--r--   0        0        0       77 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/bash/__init__.py
+-rw-r--r--   0        0        0     2268 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/bash/execution.py
+-rw-r--r--   0        0        0       40 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/contract/__init__.py
+-rw-r--r--   0        0        0     2739 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/contract/execution.py
+-rw-r--r--   0        0        0       93 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/graphql/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/graphql/execution.py
+-rw-r--r--   0        0        0     2032 2023-05-12 07:27:50.776963 cyberutils-0.0.4/cyberutils/graphql/queries.py
+-rw-r--r--   0        0        0     1818 2023-05-12 07:27:50.776963 cyberutils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 cyberutils-0.0.4/PKG-INFO
```

### Comparing `cyberutils-0.0.3/LICENSE` & `cyberutils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.3/README.md` & `cyberutils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.3/cyberutils/bash/execution.py` & `cyberutils-0.0.4/cyberutils/bash/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.3/cyberutils/graphql/execution.py` & `cyberutils-0.0.4/cyberutils/graphql/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.3/cyberutils/graphql/queries.py` & `cyberutils-0.0.4/cyberutils/graphql/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,21 @@
                 order_by: {transaction: {block: {height: desc}}}
               ) {
                     message_type: type
                     message_value: value
                     message_involved_addresses: involved_accounts_addresses
                     transaction_hash
                     transaction {
-                      success
-                      memo
-                      signer_infos
+                        success
+                        memo
+                        signer_infos
+                        block {
+                            height
+                            timestamp
+                        }
                     }
                 }
             }
             """,
         variable_values={
             "address": f"{{{address}}}",
             "types": f"{{{msg_type}}}",
```

### Comparing `cyberutils-0.0.3/pyproject.toml` & `cyberutils-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-description = "The Toolset for cyber protocol and cosmos ecosystem"
+description = "the toolset for cyber protocol and cosmos ecosystem"
 documentation = "https://github.com/Snedashkovsky/cyberutils"
 homepage = "https://github.com/Snedashkovsky/cyberutils"
 keywords = ["bostrom", "cyber", "knowledge-graph", "dex", "swap", "defi", "crypto", "blockchain", ]
 license = "MIT"
 packages = [{ include = "cyberutils" }]
 readme = "README.md"
 repository = "https://github.com/Snedashkovsky/cyberutils.git"
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.poetry.dependencies]
 pandas = "^1.0.0"
 numpy = "^1.0.0"
 python-dotenv = "^0.20.0"
 tqdm = "^4.0.0"
 ipython = "^8.0.0"
```

### Comparing `cyberutils-0.0.3/PKG-INFO` & `cyberutils-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cyberutils
-Version: 0.0.3
-Summary: The Toolset for cyber protocol and cosmos ecosystem
+Version: 0.0.4
+Summary: the toolset for cyber protocol and cosmos ecosystem
 Home-page: https://github.com/Snedashkovsky/cyberutils
 License: MIT
 Keywords: bostrom,cyber,knowledge-graph,dex,swap,defi,crypto,blockchain
 Author: Snedashkovsky,
 Author-email: sn@cyberdrop.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberutils Version: 0.0.3 Summary: The Toolset for
+Metadata-Version: 2.1 Name: cyberutils Version: 0.0.4 Summary: the toolset for
 cyber protocol and cosmos ecosystem Home-page: https://github.com/
 Snedashkovsky/cyberutils License: MIT Keywords: bostrom,cyber,knowledge-
 graph,dex,swap,defi,crypto,blockchain Author: Snedashkovsky, Author-email:
 sn@cyberdrop.ai Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```


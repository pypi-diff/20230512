# Comparing `tmp/genochain-0.0.6.tar.gz` & `tmp/genochain-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genochain-0.0.6.tar", last modified: Tue May  9 17:45:08 2023, max compression
+gzip compressed data, was "genochain-0.0.7.tar", last modified: Fri May 12 16:58:44 2023, max compression
```

## Comparing `genochain-0.0.6.tar` & `genochain-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:45:08.369904 genochain-0.0.6/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:45:08.369615 genochain-0.0.6/PKG-INFO
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:45:08.365831 genochain-0.0.6/genochain/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       45 2023-05-09 17:43:36.000000 genochain-0.0.6/genochain/__init__.py
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)     4201 2023-05-09 17:33:17.000000 genochain-0.0.6/genochain/genochain.py
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:45:08.368964 genochain-0.0.6/genochain.egg-info/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:45:08.000000 genochain-0.0.6/genochain.egg-info/PKG-INFO
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      185 2023-05-09 17:45:08.000000 genochain-0.0.6/genochain.egg-info/SOURCES.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)        1 2023-05-09 17:45:08.000000 genochain-0.0.6/genochain.egg-info/dependency_links.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       10 2023-05-09 17:45:08.000000 genochain-0.0.6/genochain.egg-info/top_level.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       38 2023-05-09 17:45:08.370012 genochain-0.0.6/setup.cfg
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)     1154 2023-05-09 17:43:08.000000 genochain-0.0.6/setup.py
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-12 16:58:44.612386 genochain-0.0.7/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-12 16:58:44.612081 genochain-0.0.7/PKG-INFO
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-12 16:58:44.606335 genochain-0.0.7/genochain/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       45 2023-05-09 17:43:36.000000 genochain-0.0.7/genochain/__init__.py
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)     4669 2023-05-12 16:53:46.000000 genochain-0.0.7/genochain/genochain.py
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-12 16:58:44.611387 genochain-0.0.7/genochain.egg-info/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-12 16:58:44.000000 genochain-0.0.7/genochain.egg-info/PKG-INFO
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      185 2023-05-12 16:58:44.000000 genochain-0.0.7/genochain.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)        1 2023-05-12 16:58:44.000000 genochain-0.0.7/genochain.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       10 2023-05-12 16:58:44.000000 genochain-0.0.7/genochain.egg-info/top_level.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       38 2023-05-12 16:58:44.612497 genochain-0.0.7/setup.cfg
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)     1154 2023-05-12 16:56:13.000000 genochain-0.0.7/setup.py
```

### Comparing `genochain-0.0.6/PKG-INFO` & `genochain-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genochain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Storing and versioning genomics data on a blockchain
 Author: GenoChain(Sanjana Sharma)
 Author-email: <sharmasanjana1947@gmail.com>
 Keywords: python,blockchain,genomics,fasta,block,biology
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genochain-0.0.6/genochain/genochain.py` & `genochain-0.0.7/genochain/genochain.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         self.previous_hash = previous_hash
         self.version_changes = version_changes
         self.hash = self.calculate_hash()
 
     def calculate_hash(self):
         return hashlib.sha256(str(self.index).encode() + str(self.timestamp).encode() + str(self.data).encode() + str(self.previous_hash).encode() + str(self.version_changes).encode()).hexdigest()
 
+
 class BlockChain:
     def __init__(self, genesis_fasta):
         self.chain = [self.create_genesis_block(genesis_fasta)]
 
     def create_genesis_block(self, genesis_fasta):
         return Block(0, time.time(), {"id": "Genesis Block", "fasta": genesis_fasta}, "0", {"version-1": "Initial version"})
 
@@ -37,25 +38,35 @@
         version_changes.update(block.version_changes)
         block = Block(index, timestamp, data, previous_hash, version_changes)
         self.chain.append(block)
 
     def check_version(self, id, fasta):
         prev_fasta = ""
         found = False
+        last_version = -1  # initialize last_version to -1
         for block in self.chain[::-1]:
             if block.data['id'] == id:
                 found = True
                 prev_fasta = self.get_latest_version(id)
+                last_version = int(max(block.version_changes.keys()).split("-")[-1])
                 break
         version = "version-1"
         change = f"Added new sequence: {fasta}"
         version_changes = {"version-1": change}
         if found:
             diff = set(prev_fasta).symmetric_difference(set(fasta))
-            version = "version-" + str(int(max(block.version_changes.keys()).split("-")[-1]) + 1)
+            last_version = max(block.version_changes.keys(), key=lambda v: [int(x) for x in v.split('-')[1:]])
+            last_version_num = int(last_version.split("-")[-1])
+            if last_version_num == 10:
+                version = "version-11"
+            elif last_version_num == -1000:
+                version = "version-1001"
+            else:
+                version = "version-" + str(last_version_num + 1)
+
             if len(fasta) > len(prev_fasta):
                 for i in range(len(prev_fasta)):
                     if prev_fasta[i] != fasta[i]:
                         change = f"Replaced {prev_fasta[i]} with {fasta[i]} at position {i+1}"
                         break
                 if not diff:
                     change = f"{fasta[len(prev_fasta):]} has been added at position {len(prev_fasta)+1}"
@@ -76,14 +87,16 @@
                         change = f"Replaced {prev_fasta[i]} with {fasta[i]} at position {i+1}"
                         break
             version_changes = block.version_changes.copy()
             version_changes[version] = change
         self.add_block({"id": id, "fasta": fasta}, version_changes)
         return f"ID: {id}, Previous fasta: {prev_fasta}, Current fasta: {fasta}, Change:{change}, Version: {version}"
 
+
+
     def get_latest_version(self, id):
         for block in self.chain[::-1]:
             if block.data['id'] == id:
                 return block.data['fasta']
         return ""
 
     def print_blockchain(self):
@@ -93,10 +106,7 @@
             print("Data: ", block.data)
             print("Previous Hash: ", block.previous_hash)
             print("Hash: ", block.hash)
             print("Version Changes: ", block.version_changes)
             print()
 
 
-
-
-
```

### Comparing `genochain-0.0.6/genochain.egg-info/PKG-INFO` & `genochain-0.0.7/genochain.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genochain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Storing and versioning genomics data on a blockchain
 Author: GenoChain(Sanjana Sharma)
 Author-email: <sharmasanjana1947@gmail.com>
 Keywords: python,blockchain,genomics,fasta,block,biology
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genochain-0.0.6/setup.py` & `genochain-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Storing and versioning genomics data on a blockchain'
 LONG_DESCRIPTION = 'The provided code is a Python implementation of a simple blockchain. It allows for the creation of a genesis block with a given FASTA sequence, addition of new blocks with a given FASTA sequence and associated ID, and versioning of FASTA sequences. The blockchain can also be checked and printed. This code is licensed under the MIT License.'
 
 # Setting up
 setup(
     name="genochain",
     version=VERSION,
```


# Comparing `tmp/pyln_proto-23.2.tar.gz` & `tmp/pyln-proto-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_proto-23.2.tar", max compression
+gzip compressed data, was "pyln-proto-23.5.tar", max compression
```

## Comparing `pyln_proto-23.2.tar` & `pyln-proto-23.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      976 2023-03-03 15:54:49.821873 pyln_proto-23.2/README.md
--rw-r--r--   0        0        0      490 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/__init__.py
--rw-r--r--   0        0        0     4698 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/bech32.py
--rwxr-xr-x   0        0        0    15493 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/invoice.py
--rw-r--r--   0        0        0       68 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/message/Makefile
--rw-r--r--   0        0        0      668 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/message/__init__.py
--rw-r--r--   0        0        0     8647 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/message/array_types.py
--rw-r--r--   0        0        0    11192 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/message/fundamental_types.py
--rw-r--r--   0        0        0    27875 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/message/message.py
--rw-r--r--   0        0        0    18733 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/onion.py
--rw-r--r--   0        0        0     4473 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/primitives.py
--rw-r--r--   0        0        0    12025 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/wire.py
--rw-r--r--   0        0        0     3915 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyln/proto/zbase32.py
--rw-r--r--   0        0        0      737 2023-03-03 15:54:49.821873 pyln_proto-23.2/pyproject.toml
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 pyln_proto-23.2/setup.py
--rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 pyln_proto-23.2/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-05-11 17:43:49.805160 pyln-proto-23.5/README.md
+-rw-r--r--   0        0        0      490 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/__init__.py
+-rw-r--r--   0        0        0     4698 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/bech32.py
+-rwxr-xr-x   0        0        0    15493 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/invoice.py
+-rw-r--r--   0        0        0       68 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/Makefile
+-rw-r--r--   0        0        0      668 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/__init__.py
+-rw-r--r--   0        0        0     8647 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/array_types.py
+-rw-r--r--   0        0        0    11192 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/fundamental_types.py
+-rw-r--r--   0        0        0    27875 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/message.py
+-rw-r--r--   0        0        0    18733 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/onion.py
+-rw-r--r--   0        0        0     4368 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/primitives.py
+-rw-r--r--   0        0        0    12025 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/wire.py
+-rw-r--r--   0        0        0     3915 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/zbase32.py
+-rw-r--r--   0        0        0      737 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 pyln-proto-23.5/setup.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyln-proto-23.5/PKG-INFO
```

### Comparing `pyln_proto-23.2/README.md` & `pyln-proto-23.5/README.md`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/bech32.py` & `pyln-proto-23.5/pyln/proto/bech32.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/invoice.py` & `pyln-proto-23.5/pyln/proto/invoice.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/message/__init__.py` & `pyln-proto-23.5/pyln/proto/message/__init__.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/message/array_types.py` & `pyln-proto-23.5/pyln/proto/message/array_types.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/message/fundamental_types.py` & `pyln-proto-23.5/pyln/proto/message/fundamental_types.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/message/message.py` & `pyln-proto-23.5/pyln/proto/message/message.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/onion.py` & `pyln-proto-23.5/pyln/proto/onion.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/primitives.py` & `pyln-proto-23.5/pyln/proto/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,15 @@
         block = (i >> 40) & 0xFFFFFF
         txnum = (i >> 16) & 0xFFFFFF
         outnum = (i >> 0) & 0xFFFF
         return cls(block=block, txnum=txnum, outnum=outnum)
 
     @classmethod
     def from_str(self, s):
-        block, txnum, outnum = s.split('x')
-        return ShortChannelId(block=int(block), txnum=int(txnum),
-                              outnum=int(outnum))
+        return ShortChannelId(*map(int, s.split('x')))
 
     def to_int(self):
         return self.block << 40 | self.txnum << 16 | self.outnum
 
     def to_bytes(self):
         return struct.pack("!Q", self.to_int())
```

### Comparing `pyln_proto-23.2/pyln/proto/wire.py` & `pyln-proto-23.5/pyln/proto/wire.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyln/proto/zbase32.py` & `pyln-proto-23.5/pyln/proto/zbase32.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-23.2/pyproject.toml` & `pyln-proto-23.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyln-proto"
-version = "23.02"
+version = "23.05"
 description = "This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!)."
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/proto" },
```

### Comparing `pyln_proto-23.2/setup.py` & `pyln-proto-23.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'base58>=2.1.1,<3.0.0',
  'bitstring>=3.1.9,<4.0.0',
  'coincurve>=17.0.0,<18.0.0',
  'cryptography>=36.0.1,<37.0.0']
 
 setup_kwargs = {
     'name': 'pyln-proto',
-    'version': '23.2',
+    'version': '23.5',
     'description': 'This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!).',
     'long_description': '# pyln-proto: Lightning Network protocol implementation\n\nThis package implements some of the Lightning Network protocol in pure\npython. It is intended for protocol testing and some minor tooling only. It is\nnot deemed secure enough to handle any amount of real funds (you have been\nwarned!).\n\n\n## Installation\n\n`pyln-proto` is available on `pip`:\n\n```\npip install pyln-proto\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-proto\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n',
     'author': 'Christian Decker',
     'author_email': 'decker.christian@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyln_proto-23.2/PKG-INFO` & `pyln-proto-23.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyln-proto
-Version: 23.2
+Version: 23.5
 Summary: This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!).
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PySocks (>=1.7.1,<2.0.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: bitstring (>=3.1.9,<4.0.0)
 Requires-Dist: coincurve (>=17.0.0,<18.0.0)
 Requires-Dist: cryptography (>=36.0.1,<37.0.0)
 Description-Content-Type: text/markdown
```


# Comparing `tmp/pyqrack-1.9.0.tar.gz` & `tmp/pyqrack-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqrack-1.9.0.tar", last modified: Thu May 11 21:47:08 2023, max compression
+gzip compressed data, was "pyqrack-1.9.1.tar", last modified: Fri May 12 10:30:58 2023, max compression
```

## Comparing `pyqrack-1.9.0.tar` & `pyqrack-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-11 21:47:08.522640 pyqrack-1.9.0/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.9.0/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-11 21:47:08.522640 pyqrack-1.9.0/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-05-11 21:46:48.000000 pyqrack-1.9.0/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.9.0/pyproject.toml
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-11 21:47:08.522640 pyqrack-1.9.0/pyqrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      532 2023-05-11 21:37:54.000000 pyqrack-1.9.0/pyqrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      594 2023-05-01 22:49:53.000000 pyqrack-1.9.0/pyqrack/neuron_activation_fn.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.9.0/pyqrack/pauli.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3676 2023-05-11 21:37:54.000000 pyqrack-1.9.0/pyqrack/qrack_circuit.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     8677 2023-05-01 22:27:13.000000 pyqrack-1.9.0/pyqrack/qrack_neuron.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-05-11 21:37:54.000000 pyqrack-1.9.0/pyqrack/qrack_simulator.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-11 21:47:08.522640 pyqrack-1.9.0/pyqrack/qrack_system/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.9.0/pyqrack/qrack_system/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    28788 2023-05-11 21:46:48.000000 pyqrack-1.9.0/pyqrack/qrack_system/qrack_system.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-11 21:47:08.522640 pyqrack-1.9.0/pyqrack/util/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.9.0/pyqrack/util/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.9.0/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-11 21:47:08.522640 pyqrack-1.9.0/pyqrack.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-11 21:47:08.000000 pyqrack-1.9.0/pyqrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      493 2023-05-11 21:47:08.000000 pyqrack-1.9.0/pyqrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-11 21:47:08.000000 pyqrack-1.9.0/pyqrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-11 21:47:08.000000 pyqrack-1.9.0/pyqrack.egg-info/not-zip-safe
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-05-11 21:47:08.000000 pyqrack-1.9.0/pyqrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-11 21:47:08.522640 pyqrack-1.9.0/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-05-11 21:37:54.000000 pyqrack-1.9.0/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-12 10:30:58.325772 pyqrack-1.9.1/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.9.1/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-12 10:30:58.325772 pyqrack-1.9.1/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-05-12 10:30:49.000000 pyqrack-1.9.1/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.9.1/pyproject.toml
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-12 10:30:58.321772 pyqrack-1.9.1/pyqrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      532 2023-05-11 21:37:54.000000 pyqrack-1.9.1/pyqrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      594 2023-05-01 22:49:53.000000 pyqrack-1.9.1/pyqrack/neuron_activation_fn.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.9.1/pyqrack/pauli.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3676 2023-05-11 21:37:54.000000 pyqrack-1.9.1/pyqrack/qrack_circuit.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     8677 2023-05-01 22:27:13.000000 pyqrack-1.9.1/pyqrack/qrack_neuron.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-05-11 21:37:54.000000 pyqrack-1.9.1/pyqrack/qrack_simulator.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-12 10:30:58.325772 pyqrack-1.9.1/pyqrack/qrack_system/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.9.1/pyqrack/qrack_system/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    28788 2023-05-12 10:30:49.000000 pyqrack-1.9.1/pyqrack/qrack_system/qrack_system.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-12 10:30:58.325772 pyqrack-1.9.1/pyqrack/util/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.9.1/pyqrack/util/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.9.1/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-12 10:30:58.325772 pyqrack-1.9.1/pyqrack.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-12 10:30:58.000000 pyqrack-1.9.1/pyqrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      493 2023-05-12 10:30:58.000000 pyqrack-1.9.1/pyqrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-12 10:30:58.000000 pyqrack-1.9.1/pyqrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-12 10:30:58.000000 pyqrack-1.9.1/pyqrack.egg-info/not-zip-safe
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-05-12 10:30:58.000000 pyqrack-1.9.1/pyqrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-12 10:30:58.325772 pyqrack-1.9.1/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-05-12 10:30:39.000000 pyqrack-1.9.1/setup.py
```

### Comparing `pyqrack-1.9.0/LICENSE` & `pyqrack-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/PKG-INFO` & `pyqrack-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.9.0
+Version: 1.9.1
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.9.0/README.md` & `pyqrack-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/__init__.py` & `pyqrack-1.9.1/pyqrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/neuron_activation_fn.py` & `pyqrack-1.9.1/pyqrack/neuron_activation_fn.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/pauli.py` & `pyqrack-1.9.1/pyqrack/pauli.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/qrack_circuit.py` & `pyqrack-1.9.1/pyqrack/qrack_circuit.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/qrack_neuron.py` & `pyqrack-1.9.1/pyqrack/qrack_neuron.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/qrack_simulator.py` & `pyqrack-1.9.1/pyqrack/qrack_simulator.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/qrack_system/qrack_system.py` & `pyqrack-1.9.1/pyqrack/qrack_system/qrack_system.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py` & `pyqrack-1.9.1/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.9.0/pyqrack.egg-info/PKG-INFO` & `pyqrack-1.9.1/pyqrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.9.0
+Version: 1.9.1
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.9.0/setup.py` & `pyqrack-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 
 requirements = []
 
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
 
 setup(
```


# Comparing `tmp/ansys-tools-path-0.2.1.tar.gz` & `tmp/ansys-tools-path-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-tools-path-0.2.1.tar", last modified: Tue May  9 15:14:34 2023, max compression
+gzip compressed data, was "ansys-tools-path-0.2.2.tar", last modified: Fri May 12 15:37:59 2023, max compression
```

## Comparing `ansys-tools-path-0.2.1.tar` & `ansys-tools-path-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/LICENSE
--rw-r--r--   0        0        0     4701 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/README.rst
--rw-r--r--   0        0        0     1849 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      919 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      648 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    25892 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-12 15:37:46.028437 ansys-tools-path-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4701 2023-05-12 15:37:46.028437 ansys-tools-path-0.2.2/README.rst
+-rw-r--r--   0        0        0     1849 2023-05-12 15:37:46.032437 ansys-tools-path-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      919 2023-05-12 15:37:46.032437 ansys-tools-path-0.2.2/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      648 2023-05-12 15:37:46.032437 ansys-tools-path-0.2.2/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    25986 2023-05-12 15:37:46.032437 ansys-tools-path-0.2.2/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.2.2/PKG-INFO
```

### Comparing `ansys-tools-path-0.2.1/LICENSE` & `ansys-tools-path-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.1/README.rst` & `ansys-tools-path-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.1/pyproject.toml` & `ansys-tools-path-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.2.1"
+version = "0.2.2"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys-tools-path-0.2.1/src/ansys/tools/path/__init__.py` & `ansys-tools-path-0.2.2/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.1/src/ansys/tools/path/misc.py` & `ansys-tools-path-0.2.2/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.1/src/ansys/tools/path/path.py` & `ansys-tools-path-0.2.2/src/ansys/tools/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,16 @@
         ansys_bin = os.path.join(ans_path, "ansys", "bin", f"ansys{version}")
     return ansys_bin, int(version) / 10
 
 
 def _find_installation(product: str, version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
     if product == "mapdl":
         return find_mapdl(version, supported_versions)
+    elif product == "mechanical":
+        return find_mechanical(version, supported_versions)
     raise Exception("unexpected product")
 
 
 def find_ansys(version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
     """Obsolete method, use find_mapdl."""
     warnings.warn(
         "This method is going to be deprecated in future versions. Please use 'find_mapdl'.",
```

### Comparing `ansys-tools-path-0.2.1/PKG-INFO` & `ansys-tools-path-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```


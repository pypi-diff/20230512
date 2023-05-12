# Comparing `tmp/dict-toolbox-3.1.0.tar.gz` & `tmp/dict-toolbox-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dict-toolbox-3.1.0.tar", last modified: Mon Mar 20 21:12:58 2023, max compression
+gzip compressed data, was "dict-toolbox-3.1.1.tar", last modified: Fri May 12 20:21:26 2023, max compression
```

## Comparing `dict-toolbox-3.1.0.tar` & `dict-toolbox-3.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:12:58.605941 dict-toolbox-3.1.0/
--rw-r--r--   0 root         (0) root         (0)    19053 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6417 2023-03-20 21:12:58.605941 dict-toolbox-3.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5499 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:12:58.601941 dict-toolbox-3.1.0/dict_toolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6417 2023-03-20 21:12:58.000000 dict-toolbox-3.1.0/dict_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2023-03-20 21:12:58.000000 dict-toolbox-3.1.0/dict_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:12:58.000000 dict-toolbox-3.1.0/dict_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-20 21:12:58.000000 dict-toolbox-3.1.0/dict_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-20 21:12:58.000000 dict-toolbox-3.1.0/dict_toolbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-20 21:12:58.000000 dict-toolbox-3.1.0/dict_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:12:58.605941 dict-toolbox-3.1.0/dict_tools/
--rw-r--r--   0 root         (0) root         (0)      269 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/args.py
--rw-r--r--   0 root         (0) root         (0)    27595 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/data.py
--rw-r--r--   0 root         (0) root         (0)    15032 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/differ.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/mysql.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/trim.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/typing.py
--rw-r--r--   0 root         (0) root         (0)     9583 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/update.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/xml.py
--rw-r--r--   0 root         (0) root         (0)    12072 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/dict_tools/yamlex.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-20 21:12:58.605941 dict-toolbox-3.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2730 2023-03-20 21:12:44.000000 dict-toolbox-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/
+-rw-r--r--   0 root         (0) root         (0)    19053 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6418 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5499 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/dict_toolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6418 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/dict_tools/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/args.py
+-rw-r--r--   0 root         (0) root         (0)    28208 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/data.py
+-rw-r--r--   0 root         (0) root         (0)    15032 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/differ.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/trim.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/typing.py
+-rw-r--r--   0 root         (0) root         (0)     9583 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/update.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/xml.py
+-rw-r--r--   0 root         (0) root         (0)    12072 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/yamlex.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/setup.py
```

### Comparing `dict-toolbox-3.1.0/LICENSE` & `dict-toolbox-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/PKG-INFO` & `dict-toolbox-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 3.1.0
+Version: 3.1.1
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 DICT-TOOLBOX
```

### Comparing `dict-toolbox-3.1.0/README.rst` & `dict-toolbox-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_toolbox.egg-info/PKG-INFO` & `dict-toolbox-3.1.1/dict_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 3.1.0
+Version: 3.1.1
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 DICT-TOOLBOX
```

### Comparing `dict-toolbox-3.1.0/dict_tools/aggregation.py` & `dict-toolbox-3.1.1/dict_tools/aggregation.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/args.py` & `dict-toolbox-3.1.1/dict_tools/args.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/data.py` & `dict-toolbox-3.1.1/dict_tools/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,59 +154,73 @@
 
 
 class NamespaceDict(dict):
     """
     A dictionary that can access its string keys through the namespace
     """
 
-    def __init__(self, seq: Mapping = None, **kwargs):
+    def __init__(self, *args, **kwargs):
         """
         NamespaceDict() -> new empty namespaced dictionary
         NamespaceDict(mapping) -> new namespaced dictionary initialized from a mapping object's
             (key, value) pairs
         NamespaceDict(iterable) -> new namespaced dictionary initialized as if via:
             d = {}
             for k, v in iterable:
                 d[k] = v
         NamespaceDict(**kwargs) -> new namespaced dictionary initialized with the name=value pairs
             in the keyword argument list.  For example:  NamespaceDict(one=1, two=2)
         """
-        if seq:
-            super().__init__(seq)
+        super().__init__(*args, **kwargs)
+        for key, value in self.items():
+            if isinstance(value, dict):
+                super().__setitem__(key, NamespaceDict(value))
+
+    def __setitem__(self, k, v):
+        if isinstance(v, Mapping):
+            v = NamespaceDict(v)
+        super().__setitem__(k, v)
+
+    def update(self, *args, **kwargs):
+        other = dict(*args, **kwargs)
+        for k, v in other.items():
+            self[k] = v
+
+    def __setattr__(self, k, v):
+        if k in self.__dict__ or k in self.__class__.__dict__:
+            # if the attribute already exists in the instance dictionary or in the class dictionary
+            super().__setattr__(k, v)
         else:
-            super().__init__()
-
-        self.update(**kwargs)
-
-    def __setattr__(self, k: str, v: Any):
-        self[k] = v
+            self[k] = v
 
     def __getattr__(self, k: str):
         # Swap key errors for attribute errors so that we don't blow up on "hasattr" checks
-        try:
-            value = self[k]
-        except KeyError as e:
-            raise AttributeError(e)
-
-        # Allow chain-getting namespaced values
-        if isinstance(value, Mapping):
-            return NamespaceDict(value)
-        return value
+        if k not in self:
+            raise AttributeError(
+                f"'{self.__class__.__name__}' object has no attribute '{k}'"
+            )
+        return self[k]
 
     def __copy__(self):
         return NamespaceDict(dict(**self).copy())
 
     def __deepcopy__(self, memodict=None):
         return NamespaceDict(copy.deepcopy(dict(self), memo=memodict))
 
     def __getstate__(self):
         return dict(self)
 
     def __setstate__(self, state):
-        self.update(**state)
+        self.update(state)
+
+    def pop(self, key, *args):
+        value = super().pop(key, *args)
+        if isinstance(value, dict):
+            value = NamespaceDict(value)
+        return value
 
 
 class SafeNamespaceDict(NamespaceDict, metaclass=DictMeta):
     """
     A Dict that does not expose values when represented as a string
     """
```

### Comparing `dict-toolbox-3.1.0/dict_tools/differ.py` & `dict-toolbox-3.1.1/dict_tools/differ.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/mysql.py` & `dict-toolbox-3.1.1/dict_tools/mysql.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/trim.py` & `dict-toolbox-3.1.1/dict_tools/trim.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/typing.py` & `dict-toolbox-3.1.1/dict_tools/typing.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/update.py` & `dict-toolbox-3.1.1/dict_tools/update.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/utils.py` & `dict-toolbox-3.1.1/dict_tools/utils.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/xml.py` & `dict-toolbox-3.1.1/dict_tools/xml.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/dict_tools/yamlex.py` & `dict-toolbox-3.1.1/dict_tools/yamlex.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.0/setup.py` & `dict-toolbox-3.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import Command
 from setuptools import setup
 
 NAME = "dict_tools"
 DESC = "Dict tools for Python projects"
 
 # Version info -- read without importing
-VERSION = "3.1.0"
+VERSION = "3.1.1"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
@@ -76,18 +76,17 @@
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
-    entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
 )
```


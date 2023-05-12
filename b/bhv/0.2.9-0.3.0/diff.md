# Comparing `tmp/bhv-0.2.9.tar.gz` & `tmp/bhv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.9.tar", last modified: Wed May 10 11:55:51 2023, max compression
+gzip compressed data, was "bhv-0.3.0.tar", last modified: Fri May 12 19:31:57 2023, max compression
```

## Comparing `bhv-0.2.9.tar` & `bhv-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-10 11:55:51.051033 bhv-0.2.9/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.9/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-10 11:55:51.051033 bhv-0.2.9/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.9/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-10 11:55:51.047700 bhv-0.2.9/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.9/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12173 2023-05-08 14:41:53.000000 bhv-0.2.9/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.2.9/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11610 2023-05-10 11:54:44.000000 bhv-0.2.9/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.9/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.9/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.2.9/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.2.9/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.9/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    24158 2023-05-05 11:23:02.000000 bhv-0.2.9/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3503 2023-05-10 11:50:50.000000 bhv-0.2.9/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.9/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-10 11:55:51.047700 bhv-0.2.9/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-10 11:55:51.051033 bhv-0.2.9/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-05-10 11:54:44.000000 bhv-0.2.9/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-12 19:31:57.589482 bhv-0.3.0/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.3.0/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-12 19:31:57.589482 bhv-0.3.0/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.3.0/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-12 19:31:57.589482 bhv-0.3.0/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.3.0/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    12914 2023-05-12 19:21:11.000000 bhv-0.3.0/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.3.0/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11610 2023-05-10 11:54:44.000000 bhv-0.3.0/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.3.0/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.3.0/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.3.0/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.3.0/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.3.0/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    24158 2023-05-05 11:23:02.000000 bhv-0.3.0/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3503 2023-05-10 11:50:50.000000 bhv-0.3.0/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.3.0/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-12 19:31:57.589482 bhv-0.3.0/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-12 19:31:57.589482 bhv-0.3.0/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1290 2023-05-12 19:25:11.000000 bhv-0.3.0/setup.py
```

### Comparing `bhv-0.2.9/LICENSE` & `bhv-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/PKG-INFO` & `bhv-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.9
+Version: 0.3.0
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,12 +16,11 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
-Provides-Extra: torch-hd
 Provides-Extra: numpy
 License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
```

### Comparing `bhv-0.2.9/README.md` & `bhv-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/abstract.py` & `bhv-0.3.0/bhv/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,27 +170,47 @@
 
     def hamming(self, other: Self) -> int:
         return (self ^ other).active()
 
     def bit_error_rate(self, other: Self) -> float:
         return (self ^ other).active_fraction()
 
-    def jaccard(self, other: Self) -> float:
-        return 1. - float((self & other).active()) / float((self | other).active() + 1E-7)
-
-    def cosine(self, other: Self) -> float:
-        return 1 - float((self & other).active()) / float(self.active() * other.active() + 1E-7)**.5
+    def jaccard(self, other: Self, distance=False) -> float:
+        union_active = (self | other).active()
+        if union_active == 0:
+            raise RuntimeError("Jaccard index where both vectors are zero")
+        res = (self & other).active() / union_active
+        return 1. - res if distance else res
+
+    def cosine(self, other: Self, distance=False) -> float:
+        s_active = self.active()
+        o_active = other.active()
+        if not s_active or not o_active:
+            raise RuntimeError("Cosine similarity where one of the two vectors is zero")
+        res = (self & other).active() / (s_active*o_active)**.5
+        return 1. - res if distance else res
 
     def std_apart(self, other: Self, invert=False) -> float:
+        return self.frac_to_std(self.bit_error_rate(other), invert)
+
+    @staticmethod
+    def frac_to_std(frac, invert=False):
         p = 0.5
         n = NormalDist(0, (DIMENSION*p*(1 - p))**.5)
         estdvs = n.zscore(p*DIMENSION)
-        stdvs = n.zscore(self.hamming(other))
+        stdvs = n.zscore(frac*DIMENSION)
         return estdvs - stdvs if invert else stdvs
 
+    @staticmethod
+    def std_to_frac(std, invert=False):
+        p = 0.5
+        n = NormalDist(0, (DIMENSION*p*(1 - p))**.5)
+        frac = (std*n.stdev + n.mean)/DIMENSION
+        return 1. - frac if invert else frac
+
     def zscore(self) -> float:
         p = 0.5
         n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
         return n.zscore(self.active())
 
     def pvalue(self) -> float:
         p = 0.5
```

### Comparing `bhv-0.2.9/bhv/embedding.py` & `bhv-0.3.0/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/np.py` & `bhv-0.3.0/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/poibin.py` & `bhv-0.3.0/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/positions.py` & `bhv-0.3.0/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/pytorch.py` & `bhv-0.3.0/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/shared.py` & `bhv-0.3.0/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/slice.py` & `bhv-0.3.0/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/symbolic.py` & `bhv-0.3.0/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/vanilla.py` & `bhv-0.3.0/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv/visualization.py` & `bhv-0.3.0/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.9/bhv.egg-info/PKG-INFO` & `bhv-0.3.0/bhv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.9
+Version: 0.3.0
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,12 +16,11 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
-Provides-Extra: torch-hd
 Provides-Extra: numpy
 License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
```

### Comparing `bhv-0.2.9/setup.py` & `bhv-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.9'
+VERSION = '0.3.0'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
     author_email="contact@adamv.be",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     extras_require={
         "torch": ["torch>=2.0.0"],
-        "torch-hd": ["torch-hd~=5.0.1"],
         "numpy": ["numpy>=1.24.2"],
     },
     keywords='ai binary hypervector hdc bsc',
     python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
```


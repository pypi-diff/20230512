# Comparing `tmp/DoSser-1.0.tar.gz` & `tmp/DoSser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DoSser-1.0.tar", last modified: Thu May 11 21:29:36 2023, max compression
+gzip compressed data, was "DoSser-1.0.1.tar", last modified: Thu May 11 22:27:56 2023, max compression
```

## Comparing `DoSser-1.0.tar` & `DoSser-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 21:29:36.223793 DoSser-1.0/
-drwxrwxrwx   0        0        0        0 2023-05-11 21:29:36.210741 DoSser-1.0/DoSser/
--rw-rw-rw-   0        0        0     6468 2023-05-11 20:32:04.000000 DoSser-1.0/DoSser/DoSser.py
--rw-rw-rw-   0        0        0       73 2023-05-10 17:33:17.000000 DoSser-1.0/DoSser/__init__.py
--rw-rw-rw-   0        0        0     2138 2023-05-11 20:27:02.000000 DoSser-1.0/DoSser/teardropAttack.py
--rw-rw-rw-   0        0        0     3617 2023-05-11 20:32:04.000000 DoSser-1.0/DoSser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:29:36.221782 DoSser-1.0/DoSser.egg-info/
--rw-rw-rw-   0        0        0     2474 2023-05-11 21:29:36.000000 DoSser-1.0/DoSser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-11 21:29:36.000000 DoSser-1.0/DoSser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 21:29:36.000000 DoSser-1.0/DoSser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 21:29:36.000000 DoSser-1.0/DoSser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 21:29:36.000000 DoSser-1.0/DoSser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-05-10 16:34:02.000000 DoSser-1.0/LICENSE
--rw-rw-rw-   0        0        0     2474 2023-05-11 21:29:36.223295 DoSser-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1797 2023-05-11 21:13:16.000000 DoSser-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 21:29:36.223793 DoSser-1.0/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-05-11 21:27:23.000000 DoSser-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 22:27:56.133371 DoSser-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-11 22:27:56.122341 DoSser-1.0.1/DoSser/
+-rw-rw-rw-   0        0        0     6468 2023-05-11 20:32:04.000000 DoSser-1.0.1/DoSser/DoSser.py
+-rw-rw-rw-   0        0        0       73 2023-05-10 17:33:17.000000 DoSser-1.0.1/DoSser/__init__.py
+-rw-rw-rw-   0        0        0     2138 2023-05-11 20:27:02.000000 DoSser-1.0.1/DoSser/teardropAttack.py
+-rw-rw-rw-   0        0        0     3617 2023-05-11 20:32:04.000000 DoSser-1.0.1/DoSser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 22:27:56.132371 DoSser-1.0.1/DoSser.egg-info/
+-rw-rw-rw-   0        0        0     2476 2023-05-11 22:27:56.000000 DoSser-1.0.1/DoSser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-11 22:27:56.000000 DoSser-1.0.1/DoSser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 22:27:56.000000 DoSser-1.0.1/DoSser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 22:27:56.000000 DoSser-1.0.1/DoSser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 22:27:56.000000 DoSser-1.0.1/DoSser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-05-10 16:34:02.000000 DoSser-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2476 2023-05-11 22:27:56.132873 DoSser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1797 2023-05-11 21:13:16.000000 DoSser-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 22:27:56.133371 DoSser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      954 2023-05-11 22:27:36.000000 DoSser-1.0.1/setup.py
```

### Comparing `DoSser-1.0/DoSser/DoSser.py` & `DoSser-1.0.1/DoSser/DoSser.py`

 * *Files identical despite different names*

### Comparing `DoSser-1.0/DoSser/teardropAttack.py` & `DoSser-1.0.1/DoSser/teardropAttack.py`

 * *Files identical despite different names*

### Comparing `DoSser-1.0/DoSser/utils.py` & `DoSser-1.0.1/DoSser/utils.py`

 * *Files identical despite different names*

### Comparing `DoSser-1.0/DoSser.egg-info/PKG-INFO` & `DoSser-1.0.1/DoSser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoSser
-Version: 1.0
+Version: 1.0.1
 Summary: A layer 4 python Denial of Service tool.
 Home-page: https://github.com/BigSlugger/DoSser
 Author: Joe Whalley
 Author-email: 19095271@stu.mmu.ac.uk
 Keywords: python,denial of service,DoS,DDoS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `DoSser-1.0/LICENSE` & `DoSser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DoSser-1.0/PKG-INFO` & `DoSser-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoSser
-Version: 1.0
+Version: 1.0.1
 Summary: A layer 4 python Denial of Service tool.
 Home-page: https://github.com/BigSlugger/DoSser
 Author: Joe Whalley
 Author-email: 19095271@stu.mmu.ac.uk
 Keywords: python,denial of service,DoS,DDoS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `DoSser-1.0/README.md` & `DoSser-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `DoSser-1.0/setup.py` & `DoSser-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="DoSser",
-    version="1.0",
+    version="1.0.1",
     author="Joe Whalley",
     author_email="19095271@stu.mmu.ac.uk",
     description="A layer 4 python Denial of Service tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BigSlugger/DoSser",
     packages=find_packages(),
```


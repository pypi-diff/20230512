# Comparing `tmp/HoodHod-0.1.0.tar.gz` & `tmp/HoodHod-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HoodHod-0.1.0.tar", last modified: Fri May 12 19:26:18 2023, max compression
+gzip compressed data, was "HoodHod-0.2.0.tar", last modified: Fri May 12 20:11:40 2023, max compression
```

## Comparing `HoodHod-0.1.0.tar` & `HoodHod-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 aicha     (1000) aicha     (1000)        0 2023-05-12 19:26:18.088471 HoodHod-0.1.0/
-drwxrwxr-x   0 aicha     (1000) aicha     (1000)        0 2023-05-12 19:26:18.088471 HoodHod-0.1.0/HoodHod/
--rw-rw-r--   0 aicha     (1000) aicha     (1000)     6948 2023-05-12 18:58:46.000000 HoodHod-0.1.0/HoodHod/HoodHod.py
--rw-rw-r--   0 aicha     (1000) aicha     (1000)       52 2023-05-12 19:25:00.000000 HoodHod-0.1.0/HoodHod/__init__.py
-drwxrwxr-x   0 aicha     (1000) aicha     (1000)        0 2023-05-12 19:26:18.088471 HoodHod-0.1.0/HoodHod.egg-info/
--rw-rw-r--   0 aicha     (1000) aicha     (1000)      462 2023-05-12 19:26:18.000000 HoodHod-0.1.0/HoodHod.egg-info/PKG-INFO
--rw-rw-r--   0 aicha     (1000) aicha     (1000)      201 2023-05-12 19:26:18.000000 HoodHod-0.1.0/HoodHod.egg-info/SOURCES.txt
--rw-rw-r--   0 aicha     (1000) aicha     (1000)        1 2023-05-12 19:26:18.000000 HoodHod-0.1.0/HoodHod.egg-info/dependency_links.txt
--rw-rw-r--   0 aicha     (1000) aicha     (1000)       27 2023-05-12 19:26:18.000000 HoodHod-0.1.0/HoodHod.egg-info/requires.txt
--rw-rw-r--   0 aicha     (1000) aicha     (1000)        8 2023-05-12 19:26:18.000000 HoodHod-0.1.0/HoodHod.egg-info/top_level.txt
--rw-rw-r--   0 aicha     (1000) aicha     (1000)      462 2023-05-12 19:26:18.088471 HoodHod-0.1.0/PKG-INFO
--rw-rw-r--   0 aicha     (1000) aicha     (1000)       38 2023-05-12 19:26:18.088471 HoodHod-0.1.0/setup.cfg
--rw-rw-r--   0 aicha     (1000) aicha     (1000)      605 2023-05-12 19:23:16.000000 HoodHod-0.1.0/setup.py
+drwxrwxr-x   0 aicha     (1000) aicha     (1000)        0 2023-05-12 20:11:39.997772 HoodHod-0.2.0/
+drwxrwxr-x   0 aicha     (1000) aicha     (1000)        0 2023-05-12 20:11:39.993772 HoodHod-0.2.0/HoodHod/
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)     7088 2023-05-12 20:10:45.000000 HoodHod-0.2.0/HoodHod/HoodHod.py
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)       52 2023-05-12 19:25:00.000000 HoodHod-0.2.0/HoodHod/__init__.py
+drwxrwxr-x   0 aicha     (1000) aicha     (1000)        0 2023-05-12 20:11:39.997772 HoodHod-0.2.0/HoodHod.egg-info/
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)      462 2023-05-12 20:11:39.000000 HoodHod-0.2.0/HoodHod.egg-info/PKG-INFO
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)      201 2023-05-12 20:11:39.000000 HoodHod-0.2.0/HoodHod.egg-info/SOURCES.txt
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)        1 2023-05-12 20:11:39.000000 HoodHod-0.2.0/HoodHod.egg-info/dependency_links.txt
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)       27 2023-05-12 20:11:39.000000 HoodHod-0.2.0/HoodHod.egg-info/requires.txt
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)        8 2023-05-12 20:11:39.000000 HoodHod-0.2.0/HoodHod.egg-info/top_level.txt
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)      462 2023-05-12 20:11:39.997772 HoodHod-0.2.0/PKG-INFO
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)       38 2023-05-12 20:11:39.997772 HoodHod-0.2.0/setup.cfg
+-rw-rw-r--   0 aicha     (1000) aicha     (1000)      605 2023-05-12 20:11:10.000000 HoodHod-0.2.0/setup.py
```

### Comparing `HoodHod-0.1.0/HoodHod/HoodHod.py` & `HoodHod-0.2.0/HoodHod/HoodHod.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,22 @@
         
 
       def fit(self, X, y):
         n = len(X)
         mean_x, mean_y = sum(X) / n, sum(y) / n
         numer = sum([(xi - mean_x) * (yi - mean_y) for xi, yi in zip(X, y)])
         denom = sum([(xi - mean_x) ** 2 for xi in X])
-        self.slope = numer / denom
-        self.intercept = mean_y - self.slope * mean_x
+        if denom == 0:
+            self.slope = 0
+        else:
+            self.slope = numer / denom
+        if numer == 0:
+            self.intercept = 0
+        else:
+            self.intercept = mean_y - self.slope * mean_x
 
       def predict(self, X):
         return [self.slope * xi + self.intercept for xi in X]
 
       def r_squared(self, X, y):
         y_mean = sum(y) / len(y)
         y_pred = self.predict(X)
```

### Comparing `HoodHod-0.1.0/setup.py` & `HoodHod-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HoodHod',
-    version='0.1.0',
+    version='0.2.0',
     description='A package for performing simple linear regression and binary decision tree classification and visualize the tree.',
     author="Derradji Aicha Elbatoul",
     author_email="derradjiaichaelbatoul@gmail.com",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'graphviz',
```


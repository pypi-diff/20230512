# Comparing `tmp/noisy_outlier-0.1.5.tar.gz` & `tmp/noisy_outlier-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noisy_outlier-0.1.5.tar", max compression
+gzip compressed data, was "noisy_outlier-0.1.6.tar", max compression
```

## Comparing `noisy_outlier-0.1.5.tar` & `noisy_outlier-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1086 2023-05-12 10:41:05.182897 noisy_outlier-0.1.5/LICENSE
--rw-r--r--   0        0        0      218 2023-05-12 10:41:05.182897 noisy_outlier-0.1.5/noisy_outlier/__init__.py
--rw-r--r--   0        0        0      128 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/hyperopt/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/hyperopt/hyperopt.py
--rw-r--r--   0        0        0       79 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/model/__init__.py
--rw-r--r--   0        0        0     3915 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/model/model.py
--rw-r--r--   0        0        0     2060 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/model/transformer.py
--rw-r--r--   0        0        0      391 2023-05-12 10:47:05.826222 noisy_outlier-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      718 2023-05-12 10:47:09.839386 noisy_outlier-0.1.5/setup.py
--rw-r--r--   0        0        0      477 2023-05-12 10:47:09.840384 noisy_outlier-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-12 10:41:05.182897 noisy_outlier-0.1.6/LICENSE
+-rw-r--r--   0        0        0      218 2023-05-12 10:41:05.182897 noisy_outlier-0.1.6/noisy_outlier/__init__.py
+-rw-r--r--   0        0        0      128 2023-05-12 10:41:05.198521 noisy_outlier-0.1.6/noisy_outlier/hyperopt/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-12 10:41:05.198521 noisy_outlier-0.1.6/noisy_outlier/hyperopt/hyperopt.py
+-rw-r--r--   0        0        0       79 2023-05-12 10:41:05.198521 noisy_outlier-0.1.6/noisy_outlier/model/__init__.py
+-rw-r--r--   0        0        0     3915 2023-05-12 10:41:05.198521 noisy_outlier-0.1.6/noisy_outlier/model/model.py
+-rw-r--r--   0        0        0     2060 2023-05-12 10:41:05.198521 noisy_outlier-0.1.6/noisy_outlier/model/transformer.py
+-rw-r--r--   0        0        0      550 2023-05-12 10:52:53.587512 noisy_outlier-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4287 2023-05-12 10:41:05.182897 noisy_outlier-0.1.6/README.md
+-rw-r--r--   0        0        0     5052 2023-05-12 10:53:23.141003 noisy_outlier-0.1.6/setup.py
+-rw-r--r--   0        0        0     4855 2023-05-12 10:53:23.141003 noisy_outlier-0.1.6/PKG-INFO
```

### Comparing `noisy_outlier-0.1.5/LICENSE` & `noisy_outlier-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `noisy_outlier-0.1.5/noisy_outlier/hyperopt/hyperopt.py` & `noisy_outlier-0.1.6/noisy_outlier/hyperopt/hyperopt.py`

 * *Files identical despite different names*

### Comparing `noisy_outlier-0.1.5/noisy_outlier/model/model.py` & `noisy_outlier-0.1.6/noisy_outlier/model/model.py`

 * *Files identical despite different names*

### Comparing `noisy_outlier-0.1.5/noisy_outlier/model/transformer.py` & `noisy_outlier-0.1.6/noisy_outlier/model/transformer.py`

 * *Files identical despite different names*


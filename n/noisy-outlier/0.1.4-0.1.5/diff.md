# Comparing `tmp/noisy_outlier-0.1.4.tar.gz` & `tmp/noisy_outlier-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ta46kof\PycharmProjects\self-supervised-outlier\dist\tmpe_5inzma\noisy_outlier-0.1.4.tar", last modified: Thu Aug 19 15:20:04 2021, max compression
+gzip compressed data, was "noisy_outlier-0.1.5.tar", max compression
```

## Comparing `noisy_outlier-0.1.4.tar` & `noisy_outlier-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,10 @@
-drwxrwxrwx   0        0        0        0 2021-08-19 15:20:04.882728 noisy_outlier-0.1.4/
--rw-rw-rw-   0        0        0     1086 2020-08-17 11:59:52.000000 noisy_outlier-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4805 2021-08-19 15:20:04.882728 noisy_outlier-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4287 2021-08-19 14:49:58.000000 noisy_outlier-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2021-08-19 15:20:04.725103 noisy_outlier-0.1.4/noisy_outlier/
--rw-rw-rw-   0        0        0      218 2021-08-19 15:17:19.000000 noisy_outlier-0.1.4/noisy_outlier/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-19 15:20:04.757472 noisy_outlier-0.1.4/noisy_outlier/hyperopt/
--rw-rw-rw-   0        0        0      128 2020-08-19 08:54:22.000000 noisy_outlier-0.1.4/noisy_outlier/hyperopt/__init__.py
--rw-rw-rw-   0        0        0     2036 2021-08-19 15:12:09.000000 noisy_outlier-0.1.4/noisy_outlier/hyperopt/hyperopt.py
-drwxrwxrwx   0        0        0        0 2021-08-19 15:20:04.882728 noisy_outlier-0.1.4/noisy_outlier/model/
--rw-rw-rw-   0        0        0       79 2020-08-19 08:54:22.000000 noisy_outlier-0.1.4/noisy_outlier/model/__init__.py
--rw-rw-rw-   0        0        0     3915 2020-08-19 08:54:22.000000 noisy_outlier-0.1.4/noisy_outlier/model/model.py
--rw-rw-rw-   0        0        0     2060 2020-08-19 08:54:22.000000 noisy_outlier-0.1.4/noisy_outlier/model/transformer.py
-drwxrwxrwx   0        0        0        0 2021-08-19 15:20:04.757472 noisy_outlier-0.1.4/noisy_outlier.egg-info/
--rw-rw-rw-   0        0        0     4805 2021-08-19 15:20:04.000000 noisy_outlier-0.1.4/noisy_outlier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2021-08-19 15:20:04.000000 noisy_outlier-0.1.4/noisy_outlier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-19 15:20:04.000000 noisy_outlier-0.1.4/noisy_outlier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2021-08-19 15:20:04.000000 noisy_outlier-0.1.4/noisy_outlier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-08-19 15:20:04.000000 noisy_outlier-0.1.4/noisy_outlier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-19 15:20:04.882728 noisy_outlier-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      867 2021-08-19 15:19:53.000000 noisy_outlier-0.1.4/setup.py
+-rw-r--r--   0        0        0     1086 2023-05-12 10:41:05.182897 noisy_outlier-0.1.5/LICENSE
+-rw-r--r--   0        0        0      218 2023-05-12 10:41:05.182897 noisy_outlier-0.1.5/noisy_outlier/__init__.py
+-rw-r--r--   0        0        0      128 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/hyperopt/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/hyperopt/hyperopt.py
+-rw-r--r--   0        0        0       79 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/model/__init__.py
+-rw-r--r--   0        0        0     3915 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/model/model.py
+-rw-r--r--   0        0        0     2060 2023-05-12 10:41:05.198521 noisy_outlier-0.1.5/noisy_outlier/model/transformer.py
+-rw-r--r--   0        0        0      391 2023-05-12 10:47:05.826222 noisy_outlier-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      718 2023-05-12 10:47:09.839386 noisy_outlier-0.1.5/setup.py
+-rw-r--r--   0        0        0      477 2023-05-12 10:47:09.840384 noisy_outlier-0.1.5/PKG-INFO
```

### Comparing `noisy_outlier-0.1.4/LICENSE` & `noisy_outlier-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `noisy_outlier-0.1.4/noisy_outlier/hyperopt/hyperopt.py` & `noisy_outlier-0.1.5/noisy_outlier/hyperopt/hyperopt.py`

 * *Files identical despite different names*

### Comparing `noisy_outlier-0.1.4/noisy_outlier/model/model.py` & `noisy_outlier-0.1.5/noisy_outlier/model/model.py`

 * *Files identical despite different names*

### Comparing `noisy_outlier-0.1.4/noisy_outlier/model/transformer.py` & `noisy_outlier-0.1.5/noisy_outlier/model/transformer.py`

 * *Files identical despite different names*


# Comparing `tmp/up_ibacop-0.0.1.tar.gz` & `tmp/up_ibacop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_ibacop-0.0.1.tar", last modified: Wed May 10 09:49:40 2023, max compression
+gzip compressed data, was "up_ibacop-0.0.2.tar", last modified: Thu May 11 20:39:28 2023, max compression
```

## Comparing `up_ibacop-0.0.1.tar` & `up_ibacop-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-10 09:49:40.846640 up_ibacop-0.0.1/
--rw-rw-r--   0 gio       (1000) gio       (1000)    11357 2023-05-10 09:40:09.000000 up_ibacop-0.0.1/LICENSE
--rw-rw-r--   0 gio       (1000) gio       (1000)      281 2023-05-10 09:49:40.846640 up_ibacop-0.0.1/PKG-INFO
--rw-rw-r--   0 gio       (1000) gio       (1000)     2243 2023-05-10 09:40:09.000000 up_ibacop-0.0.1/README.md
--rw-rw-r--   0 gio       (1000) gio       (1000)       38 2023-05-10 09:49:40.846640 up_ibacop-0.0.1/setup.cfg
--rw-rw-r--   0 gio       (1000) gio       (1000)      365 2023-05-10 09:49:37.000000 up_ibacop-0.0.1/setup.py
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-10 09:49:40.842640 up_ibacop-0.0.1/up_ibacop/
--rw-rw-r--   0 gio       (1000) gio       (1000)       27 2023-05-10 09:40:09.000000 up_ibacop-0.0.1/up_ibacop/__init__.py
--rw-rw-r--   0 gio       (1000) gio       (1000)    12060 2023-05-10 09:40:09.000000 up_ibacop-0.0.1/up_ibacop/ibacop.py
-drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-10 09:49:40.846640 up_ibacop-0.0.1/up_ibacop.egg-info/
--rw-rw-r--   0 gio       (1000) gio       (1000)      281 2023-05-10 09:49:40.000000 up_ibacop-0.0.1/up_ibacop.egg-info/PKG-INFO
--rw-rw-r--   0 gio       (1000) gio       (1000)      232 2023-05-10 09:49:40.000000 up_ibacop-0.0.1/up_ibacop.egg-info/SOURCES.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-10 09:49:40.000000 up_ibacop-0.0.1/up_ibacop.egg-info/dependency_links.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)       25 2023-05-10 09:49:40.000000 up_ibacop-0.0.1/up_ibacop.egg-info/requires.txt
--rw-rw-r--   0 gio       (1000) gio       (1000)       10 2023-05-10 09:49:40.000000 up_ibacop-0.0.1/up_ibacop.egg-info/top_level.txt
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-11 20:39:28.842048 up_ibacop-0.0.2/
+-rw-rw-r--   0 gio       (1000) gio       (1000)    11357 2023-05-11 20:36:33.000000 up_ibacop-0.0.2/LICENSE
+-rw-rw-r--   0 gio       (1000) gio       (1000)      328 2023-05-11 20:39:28.842048 up_ibacop-0.0.2/PKG-INFO
+-rw-rw-r--   0 gio       (1000) gio       (1000)     2243 2023-05-11 20:36:33.000000 up_ibacop-0.0.2/README.md
+-rw-rw-r--   0 gio       (1000) gio       (1000)       38 2023-05-11 20:39:28.842048 up_ibacop-0.0.2/setup.cfg
+-rw-rw-r--   0 gio       (1000) gio       (1000)      392 2023-05-11 20:36:33.000000 up_ibacop-0.0.2/setup.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-11 20:39:28.842048 up_ibacop-0.0.2/up_ibacop/
+-rw-rw-r--   0 gio       (1000) gio       (1000)       27 2023-05-11 20:36:33.000000 up_ibacop-0.0.2/up_ibacop/__init__.py
+-rw-rw-r--   0 gio       (1000) gio       (1000)    12060 2023-05-11 20:36:33.000000 up_ibacop-0.0.2/up_ibacop/ibacop.py
+drwxrwxr-x   0 gio       (1000) gio       (1000)        0 2023-05-11 20:39:28.842048 up_ibacop-0.0.2/up_ibacop.egg-info/
+-rw-rw-r--   0 gio       (1000) gio       (1000)      328 2023-05-11 20:39:28.000000 up_ibacop-0.0.2/up_ibacop.egg-info/PKG-INFO
+-rw-rw-r--   0 gio       (1000) gio       (1000)      200 2023-05-11 20:39:28.000000 up_ibacop-0.0.2/up_ibacop.egg-info/SOURCES.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)        1 2023-05-11 20:39:28.000000 up_ibacop-0.0.2/up_ibacop.egg-info/dependency_links.txt
+-rw-rw-r--   0 gio       (1000) gio       (1000)       10 2023-05-11 20:39:28.000000 up_ibacop-0.0.2/up_ibacop.egg-info/top_level.txt
```

### Comparing `up_ibacop-0.0.1/LICENSE` & `up_ibacop-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `up_ibacop-0.0.1/README.md` & `up_ibacop-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `up_ibacop-0.0.1/up_ibacop/ibacop.py` & `up_ibacop-0.0.2/up_ibacop/ibacop.py`

 * *Files identical despite different names*


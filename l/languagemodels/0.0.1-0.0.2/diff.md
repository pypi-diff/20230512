# Comparing `tmp/languagemodels-0.0.1.tar.gz` & `tmp/languagemodels-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.0.1.tar", last modified: Sun May  7 01:54:20 2023, max compression
+gzip compressed data, was "languagemodels-0.0.2.tar", last modified: Thu May 11 23:45:36 2023, max compression
```

## Comparing `languagemodels-0.0.1.tar` & `languagemodels-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-07 01:54:20.285622 languagemodels-0.0.1/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      581 2023-05-07 01:54:20.285622 languagemodels-0.0.1/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-07 01:54:20.281621 languagemodels-0.0.1/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       32 2023-05-07 01:42:38.000000 languagemodels-0.0.1/languagemodels/__init__.py
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)      764 2023-05-07 01:50:29.000000 languagemodels-0.0.1/languagemodels/languagemodels.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-07 01:54:20.285622 languagemodels-0.0.1/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      581 2023-05-07 01:54:20.000000 languagemodels-0.0.1/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      220 2023-05-07 01:54:20.000000 languagemodels-0.0.1/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-07 01:54:20.000000 languagemodels-0.0.1/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-07 01:54:20.000000 languagemodels-0.0.1/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-07 01:54:20.285622 languagemodels-0.0.1/setup.cfg
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)      692 2023-05-07 01:53:56.000000 languagemodels-0.0.1/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-11 23:45:36.584200 languagemodels-0.0.2/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3014 2023-05-11 23:45:36.584200 languagemodels-0.0.2/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-11 23:45:36.580199 languagemodels-0.0.2/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4469 2023-05-11 23:45:12.000000 languagemodels-0.0.2/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2265 2023-05-09 19:09:44.000000 languagemodels-0.0.2/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1908 2023-05-11 23:45:12.000000 languagemodels-0.0.2/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-11 23:45:36.584200 languagemodels-0.0.2/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3014 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       52 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-11 23:45:36.584200 languagemodels-0.0.2/setup.cfg
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)      788 2023-05-11 23:45:20.000000 languagemodels-0.0.2/setup.py
```


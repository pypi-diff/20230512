# Comparing `tmp/example-sulthan4-0.0.8.tar.gz` & `tmp/example-sulthan4-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example-sulthan4-0.0.8.tar", last modified: Fri May 12 14:00:35 2023, max compression
+gzip compressed data, was "example-sulthan4-0.0.9.tar", last modified: Fri May 12 15:26:51 2023, max compression
```

## Comparing `example-sulthan4-0.0.8.tar` & `example-sulthan4-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 14:00:35.599073 example-sulthan4-0.0.8/
--rw-rw-rw-   0        0        0      161 2023-05-12 14:00:35.597073 example-sulthan4-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-05-12 13:59:53.000000 example-sulthan4-0.0.8/example.cpp
-drwxrwxrwx   0        0        0        0 2023-05-12 14:00:35.594000 example-sulthan4-0.0.8/example_sulthan4.egg-info/
--rw-rw-rw-   0        0        0      161 2023-05-12 14:00:35.000000 example-sulthan4-0.0.8/example_sulthan4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-12 14:00:35.000000 example-sulthan4-0.0.8/example_sulthan4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 14:00:35.000000 example-sulthan4-0.0.8/example_sulthan4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-12 14:00:35.000000 example-sulthan4-0.0.8/example_sulthan4.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-12 14:00:35.000000 example-sulthan4-0.0.8/example_sulthan4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 14:00:35.599073 example-sulthan4-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1750 2023-05-12 14:00:06.000000 example-sulthan4-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:26:51.759865 example-sulthan4-0.0.9/
+-rw-rw-rw-   0        0        0      160 2023-05-12 15:26:51.759865 example-sulthan4-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-05-12 13:59:53.000000 example-sulthan4-0.0.9/example.cpp
+drwxrwxrwx   0        0        0        0 2023-05-12 15:26:51.759865 example-sulthan4-0.0.9/example_sulthan4.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-05-12 15:26:51.000000 example-sulthan4-0.0.9/example_sulthan4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-12 15:26:51.000000 example-sulthan4-0.0.9/example_sulthan4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 15:26:51.000000 example-sulthan4-0.0.9/example_sulthan4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 15:26:51.000000 example-sulthan4-0.0.9/example_sulthan4.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-12 15:26:51.000000 example-sulthan4-0.0.9/example_sulthan4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 15:26:51.759865 example-sulthan4-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-05-12 15:24:40.000000 example-sulthan4-0.0.9/setup.py
```

### Comparing `example-sulthan4-0.0.8/example.cpp` & `example-sulthan4-0.0.9/example.cpp`

 * *Files identical despite different names*


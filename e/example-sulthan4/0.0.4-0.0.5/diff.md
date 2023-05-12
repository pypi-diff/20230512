# Comparing `tmp/example-sulthan4-0.0.4.tar.gz` & `tmp/example-sulthan4-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example-sulthan4-0.0.4.tar", last modified: Fri May 12 10:33:27 2023, max compression
+gzip compressed data, was "example-sulthan4-0.0.5.tar", last modified: Fri May 12 13:23:44 2023, max compression
```

## Comparing `example-sulthan4-0.0.4.tar` & `example-sulthan4-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:33:27.635420 example-sulthan4-0.0.4/
--rw-rw-rw-   0        0        0      158 2023-05-12 10:33:27.634419 example-sulthan4-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-12 10:17:20.000000 example-sulthan4-0.0.4/example.cpp
-drwxrwxrwx   0        0        0        0 2023-05-12 10:33:27.632238 example-sulthan4-0.0.4/example_sulthan4.egg-info/
--rw-rw-rw-   0        0        0      158 2023-05-12 10:33:27.000000 example-sulthan4-0.0.4/example_sulthan4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-12 10:33:27.000000 example-sulthan4-0.0.4/example_sulthan4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:33:27.000000 example-sulthan4-0.0.4/example_sulthan4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-12 10:33:27.000000 example-sulthan4-0.0.4/example_sulthan4.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-12 10:33:27.000000 example-sulthan4-0.0.4/example_sulthan4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 10:33:27.635420 example-sulthan4-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1104 2023-05-12 10:33:01.000000 example-sulthan4-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:23:44.025498 example-sulthan4-0.0.5/
+-rw-rw-rw-   0        0        0      158 2023-05-12 13:23:44.024498 example-sulthan4-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-05-12 13:22:00.000000 example-sulthan4-0.0.5/example.cpp
+drwxrwxrwx   0        0        0        0 2023-05-12 13:23:44.021489 example-sulthan4-0.0.5/example_sulthan4.egg-info/
+-rw-rw-rw-   0        0        0      158 2023-05-12 13:23:43.000000 example-sulthan4-0.0.5/example_sulthan4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-12 13:23:43.000000 example-sulthan4-0.0.5/example_sulthan4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 13:23:43.000000 example-sulthan4-0.0.5/example_sulthan4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 13:23:43.000000 example-sulthan4-0.0.5/example_sulthan4.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-12 13:23:43.000000 example-sulthan4-0.0.5/example_sulthan4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 13:23:44.026497 example-sulthan4-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2023-05-12 13:23:17.000000 example-sulthan4-0.0.5/setup.py
```

### Comparing `example-sulthan4-0.0.4/setup.py` & `example-sulthan4-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='example-sulthan4',
-    version='0.0.4',
+    version='0.0.5',
     author='Your Name',
     author_email='your.email@example.com',
     description='Example project using numpy',
     ext_modules=ext_modules,
     zip_safe=False,
 )
```


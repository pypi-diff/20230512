# Comparing `tmp/pybuilder-docker-too-42.tar.gz` & `tmp/pybuilder-docker-too-43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-docker-too-42.tar", last modified: Tue Feb  7 17:27:03 2023, max compression
+gzip compressed data, was "pybuilder-docker-too-43.tar", last modified: Fri May 12 17:54:07 2023, max compression
```

## Comparing `pybuilder-docker-too-42.tar` & `pybuilder-docker-too-43.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:27:03.254730 pybuilder-docker-too-42/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-07 17:27:03.254730 pybuilder-docker-too-42/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:27:03.254730 pybuilder-docker-too-42/pybuilder_docker_too/
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-02-07 17:26:47.000000 pybuilder-docker-too-42/pybuilder_docker_too/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:27:03.254730 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-07 17:27:03.000000 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-07 17:27:03.000000 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 17:27:03.000000 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 17:27:03.000000 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-07 17:27:03.000000 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 17:27:03.000000 pybuilder-docker-too-42/pybuilder_docker_too.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 17:27:03.254730 pybuilder-docker-too-42/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-02-07 17:27:02.000000 pybuilder-docker-too-42/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:07.224499 pybuilder-docker-too-43/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 17:54:07.224499 pybuilder-docker-too-43/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:07.220499 pybuilder-docker-too-43/pybuilder_docker_too/
+-rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-05-12 17:53:43.000000 pybuilder-docker-too-43/pybuilder_docker_too/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:07.224499 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 17:54:07.000000 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-12 17:54:07.000000 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:07.000000 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:07.000000 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 17:54:07.000000 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:07.000000 pybuilder-docker-too-43/pybuilder_docker_too.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:54:07.224499 pybuilder-docker-too-43/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-05-12 17:54:05.000000 pybuilder-docker-too-43/setup.py
```

### Comparing `pybuilder-docker-too-42/PKG-INFO` & `pybuilder-docker-too-43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-docker-too
-Version: 42
+Version: 43
 Summary: A pybuilder plugin that stages a python package into a docker container and optionally publishes it to a registry.
 Home-page: https://github.com/rspitler/pybuilder-docker
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-docker-too-42/pybuilder_docker_too/__init__.py` & `pybuilder-docker-too-43/pybuilder_docker_too/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-docker-too-42/pybuilder_docker_too.egg-info/PKG-INFO` & `pybuilder-docker-too-43/pybuilder_docker_too.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-docker-too
-Version: 42
+Version: 43
 Summary: A pybuilder plugin that stages a python package into a docker container and optionally publishes it to a registry.
 Home-page: https://github.com/rspitler/pybuilder-docker
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-docker-too-42/setup.py` & `pybuilder-docker-too-43/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-docker-too',
-        version = '42',
+        version = '43',
         description = 'A pybuilder plugin that stages a python package into a docker container and optionally publishes it to a registry.',
         long_description = 'A pybuilder plugin that stages a python package into a docker container and optionally publishes it to a registry.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```


# Comparing `tmp/doeloe-0.1.tar.gz` & `tmp/doeloe-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doeloe-0.1.tar", last modified: Fri May 12 05:18:44 2023, max compression
+gzip compressed data, was "doeloe-0.2.tar", last modified: Fri May 12 05:20:42 2023, max compression
```

## Comparing `doeloe-0.1.tar` & `doeloe-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-12 05:18:44.557140 doeloe-0.1/
--rw-r--r--   0 david     (1000) david     (1000)      848 2023-05-12 05:18:44.557140 doeloe-0.1/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      487 2023-05-12 05:14:57.000000 doeloe-0.1/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-12 05:18:44.557140 doeloe-0.1/doeloe.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      848 2023-05-12 05:18:44.000000 doeloe-0.1/doeloe.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      163 2023-05-12 05:18:44.000000 doeloe-0.1/doeloe.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-12 05:18:44.000000 doeloe-0.1/doeloe.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-12 05:18:44.000000 doeloe-0.1/doeloe.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       98 2023-05-12 05:07:32.000000 doeloe-0.1/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)      106 2023-05-12 05:18:44.557140 doeloe-0.1/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      844 2023-05-12 05:18:36.000000 doeloe-0.1/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-12 05:20:42.357140 doeloe-0.2/
+-rw-r--r--   0 david     (1000) david     (1000)      848 2023-05-12 05:20:42.357140 doeloe-0.2/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      487 2023-05-12 05:14:57.000000 doeloe-0.2/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-12 05:20:42.357140 doeloe-0.2/doeloe.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      848 2023-05-12 05:20:42.000000 doeloe-0.2/doeloe.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      163 2023-05-12 05:20:42.000000 doeloe-0.2/doeloe.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-12 05:20:42.000000 doeloe-0.2/doeloe.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-12 05:20:42.000000 doeloe-0.2/doeloe.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       98 2023-05-12 05:07:32.000000 doeloe-0.2/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)      106 2023-05-12 05:20:42.357140 doeloe-0.2/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      844 2023-05-12 05:20:39.000000 doeloe-0.2/setup.py
```

### Comparing `doeloe-0.1/PKG-INFO` & `doeloe-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doeloe
-Version: 0.1
+Version: 0.2
 Summary: A tool to convert old Indonesian language into EYD (Ejaan yang Disempurnakan)
 Home-page: https://github.com/bookbot-hive/doeloe
 Author: David Samuel
 Author-email: davidsamuel.7878@gmail.com
 License: Apache License
 Platform: linux
 Platform: unix
```

### Comparing `doeloe-0.1/doeloe.egg-info/PKG-INFO` & `doeloe-0.2/doeloe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doeloe
-Version: 0.1
+Version: 0.2
 Summary: A tool to convert old Indonesian language into EYD (Ejaan yang Disempurnakan)
 Home-page: https://github.com/bookbot-hive/doeloe
 Author: David Samuel
 Author-email: davidsamuel.7878@gmail.com
 License: Apache License
 Platform: linux
 Platform: unix
```

### Comparing `doeloe-0.1/setup.py` & `doeloe-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = readme_path.read_text(encoding="utf-8")
 
 data_dir = module_dir / "dict"
 
 if __name__ == "__main__":
     setup(
         name="doeloe",
-        version='0.1',
+        version='0.2',
         description="A tool to convert old Indonesian language into EYD (Ejaan yang Disempurnakan)",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="David Samuel",
         author_email="davidsamuel.7878@gmail.com",
         url="https://github.com/bookbot-hive/doeloe",
         license="Apache License",
```


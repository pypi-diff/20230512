# Comparing `tmp/element-optogenetics-0.1.1.tar.gz` & `tmp/element-optogenetics-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-optogenetics-0.1.1.tar", last modified: Mon May  8 19:05:07 2023, max compression
+gzip compressed data, was "element-optogenetics-0.1.3.tar", last modified: Fri May 12 21:49:13 2023, max compression
```

## Comparing `element-optogenetics-0.1.1.tar` & `element-optogenetics-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:07.062668 element-optogenetics-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 19:05:04.000000 element-optogenetics-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 19:05:07.062668 element-optogenetics-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 19:05:04.000000 element-optogenetics-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:07.062668 element-optogenetics-0.1.1/element_optogenetics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:04.000000 element-optogenetics-0.1.1/element_optogenetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-08 19:05:04.000000 element-optogenetics-0.1.1/element_optogenetics/optogenetics.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 19:05:04.000000 element-optogenetics-0.1.1/element_optogenetics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:07.062668 element-optogenetics-0.1.1/element_optogenetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 19:05:06.000000 element-optogenetics-0.1.1/element_optogenetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 19:05:06.000000 element-optogenetics-0.1.1/element_optogenetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:05:06.000000 element-optogenetics-0.1.1/element_optogenetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 19:05:06.000000 element-optogenetics-0.1.1/element_optogenetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 19:05:06.000000 element-optogenetics-0.1.1/element_optogenetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:05:07.062668 element-optogenetics-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 19:05:04.000000 element-optogenetics-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:49:13.389887 element-optogenetics-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 21:49:09.000000 element-optogenetics-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-12 21:49:13.389887 element-optogenetics-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 21:49:09.000000 element-optogenetics-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:49:13.389887 element-optogenetics-0.1.3/element_optogenetics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:49:09.000000 element-optogenetics-0.1.3/element_optogenetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-12 21:49:09.000000 element-optogenetics-0.1.3/element_optogenetics/optogenetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 21:49:09.000000 element-optogenetics-0.1.3/element_optogenetics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:49:13.389887 element-optogenetics-0.1.3/element_optogenetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-12 21:49:13.000000 element-optogenetics-0.1.3/element_optogenetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-12 21:49:13.000000 element-optogenetics-0.1.3/element_optogenetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:49:13.000000 element-optogenetics-0.1.3/element_optogenetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 21:49:13.000000 element-optogenetics-0.1.3/element_optogenetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 21:49:13.000000 element-optogenetics-0.1.3/element_optogenetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:49:13.389887 element-optogenetics-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-12 21:49:09.000000 element-optogenetics-0.1.3/setup.py
```

### Comparing `element-optogenetics-0.1.1/LICENSE` & `element-optogenetics-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `element-optogenetics-0.1.1/PKG-INFO` & `element-optogenetics-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-optogenetics
-Version: 0.1.1
+Version: 0.1.3
 Summary: DataJoint Element for Optogenetics
 Home-page: https://github.com/datajoint/element-optogenetics
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience optogenetics science datajoint
 Platform: UNKNOWN
@@ -35,8 +35,12 @@
      pip install element-optogenetics
      ```
 
 + [Interactive tutorial on GitHub Codespaces](https://github.com/datajoint/workflow-optogenetics#interactive-tutorial)
 
 + [Documentation](https://datajoint.com/docs/elements/element-optogenetics)
 
+## Support
+
++ If you need help getting started or run into any errors, please contact our team by email at support@datajoint.com.
+
```

### Comparing `element-optogenetics-0.1.1/README.md` & `element-optogenetics-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,7 +21,11 @@
      ```bash
      pip install element-optogenetics
      ```
 
 + [Interactive tutorial on GitHub Codespaces](https://github.com/datajoint/workflow-optogenetics#interactive-tutorial)
 
 + [Documentation](https://datajoint.com/docs/elements/element-optogenetics)
+
+## Support
+
++ If you need help getting started or run into any errors, please contact our team by email at support@datajoint.com.
```

### Comparing `element-optogenetics-0.1.1/element_optogenetics/optogenetics.py` & `element-optogenetics-0.1.3/element_optogenetics/optogenetics.py`

 * *Files identical despite different names*

### Comparing `element-optogenetics-0.1.1/element_optogenetics.egg-info/PKG-INFO` & `element-optogenetics-0.1.3/element_optogenetics.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-optogenetics
-Version: 0.1.1
+Version: 0.1.3
 Summary: DataJoint Element for Optogenetics
 Home-page: https://github.com/datajoint/element-optogenetics
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience optogenetics science datajoint
 Platform: UNKNOWN
@@ -35,8 +35,12 @@
      pip install element-optogenetics
      ```
 
 + [Interactive tutorial on GitHub Codespaces](https://github.com/datajoint/workflow-optogenetics#interactive-tutorial)
 
 + [Documentation](https://datajoint.com/docs/elements/element-optogenetics)
 
+## Support
+
++ If you need help getting started or run into any errors, please contact our team by email at support@datajoint.com.
+
```

### Comparing `element-optogenetics-0.1.1/setup.py` & `element-optogenetics-0.1.3/setup.py`

 * *Files identical despite different names*


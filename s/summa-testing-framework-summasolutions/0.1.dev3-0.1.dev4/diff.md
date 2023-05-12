# Comparing `tmp/summa-testing-framework-summasolutions-0.1.dev3.tar.gz` & `tmp/summa-testing-framework-summasolutions-0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/summa-testing-framework-summasolutions-0.1.dev3.tar", last modified: Fri Sep 11 21:20:58 2020, max compression
+gzip compressed data, was "dist/summa-testing-framework-summasolutions-0.1.dev4.tar", last modified: Fri Sep 11 21:25:53 2020, max compression
```

## Comparing `summa-testing-framework-summasolutions-0.1.dev3.tar` & `summa-testing-framework-summasolutions-0.1.dev4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/
--rw-rw-rw-   0 root         (0) root         (0)     2668 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      557 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       20 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      156 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      729 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      154 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       43 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/setup.cfg 
--rw-rw-rw-   0 root         (0) root         (0)      985 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/assets/
--rw-rw-rw-   0 root         (0) root         (0)      114 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/assets/config.base.yml
--rw-rw-rw-   0 root         (0) root         (0)      493 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/assets/docker-compose.base.yml
--rw-rw-rw-   0 root         (0) root         (0)      591 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/command/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/command/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/command/suite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/common/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/common/docker.py
--rw-rw-rw-   0 root         (0) root         (0)      680 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/common/filesystem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)       32 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test/fixtures/basic_config_file.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test/fixtures/empty_config_file.yml
--rw-rw-rw-   0 root         (0) root         (0)     1590 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test/test_common_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/magento.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/sample/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/sample/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/sample/magento.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2020-09-11 21:20:49.000000 summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/sample/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       62 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2020-09-11 21:20:58.000000 summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      557 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       20 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      156 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       43 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/setup.cfg 
+-rw-rw-rw-   0 root         (0) root         (0)      985 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/assets/config.base.yml
+-rw-rw-rw-   0 root         (0) root         (0)      493 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/assets/docker-compose.base.yml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/command/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/command/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/command/suite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/common/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/common/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)      680 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/common/filesystem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test/fixtures/basic_config_file.yml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test/fixtures/empty_config_file.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test/test_common_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/magento.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/sample/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/sample/magento.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2020-09-11 21:25:43.000000 summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/sample/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2020-09-11 21:25:53.000000 summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/top_level.txt
```

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/.gitignore` & `summa-testing-framework-summasolutions-0.1.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/LICENSE` & `summa-testing-framework-summasolutions-0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/PKG-INFO` & `summa-testing-framework-summasolutions-0.1.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summa-testing-framework-summasolutions
-Version: 0.1.dev3
+Version: 0.1.dev4
 Summary: Summa Solutions Testing Framework
 Home-page: https://bitbucket.org/summasolutions/summa-testing-framework
 Author: Summa Solutions
 Author-email: coreteam@summasoutions.net
 License: UNKNOWN
 Description: # Summa Solutions Testing Framework
```

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/setup.py` & `summa-testing-framework-summasolutions-0.1.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/cli.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/cli.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/command/config.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/command/config.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/command/grid.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/command/grid.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/command/suite.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/command/suite.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/common/config.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/common/config.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/common/docker.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/common/docker.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/common/filesystem.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/common/filesystem.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/test/test_common_config.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/test/test_common_config.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/base.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/base.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/stf/test_case/magento.py` & `summa-testing-framework-summasolutions-0.1.dev4/stf/test_case/magento.py`

 * *Files identical despite different names*

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/PKG-INFO` & `summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summa-testing-framework-summasolutions
-Version: 0.1.dev3
+Version: 0.1.dev4
 Summary: Summa Solutions Testing Framework
 Home-page: https://bitbucket.org/summasolutions/summa-testing-framework
 Author: Summa Solutions
 Author-email: coreteam@summasoutions.net
 License: UNKNOWN
 Description: # Summa Solutions Testing Framework
```

### Comparing `summa-testing-framework-summasolutions-0.1.dev3/summa_testing_framework_summasolutions.egg-info/SOURCES.txt` & `summa-testing-framework-summasolutions-0.1.dev4/summa_testing_framework_summasolutions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


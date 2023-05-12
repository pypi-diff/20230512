# Comparing `tmp/jadecobra-0.3.67.tar.gz` & `tmp/jadecobra-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadecobra-0.3.67.tar", last modified: Fri May 12 14:10:50 2023, max compression
+gzip compressed data, was "jadecobra-0.3.7.tar", last modified: Mon Apr  3 00:47:12 2023, max compression
```

## Comparing `jadecobra-0.3.67.tar` & `jadecobra-0.3.7.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.595638 jadecobra-0.3.67/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.67/LICENSE
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-12 14:10:50.595492 jadecobra-0.3.67/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.67/README.md
--rw-r--r--   0 johnnyblase   (501) staff       (20)      534 2023-05-12 14:10:41.000000 jadecobra-0.3.67/pyproject.toml
--rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-05-12 14:10:50.595676 jadecobra-0.3.67/setup.cfg
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.586453 jadecobra-0.3.67/src/
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.587279 jadecobra-0.3.67/src/None/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-04-20 16:05:17.000000 jadecobra-0.3.67/src/None/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.589408 jadecobra-0.3.67/src/jadecobra/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       22 2023-05-12 14:10:41.000000 jadecobra-0.3.67/src/jadecobra/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.67/src/jadecobra/aws_environment.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.590386 jadecobra-0.3.67/src/jadecobra/aws_lambda/
--rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.67/src/jadecobra/aws_lambda/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.591718 jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/deploy.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3888 2023-04-28 20:18:57.000000 jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.67/src/jadecobra/cloudformation_deployer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.67/src/jadecobra/setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     4788 2023-05-11 13:19:21.000000 jadecobra-0.3.67/src/jadecobra/tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3265 2023-04-20 18:35:14.000000 jadecobra-0.3.67/src/jadecobra/toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1947 2023-04-20 18:29:33.000000 jadecobra-0.3.67/src/jadecobra/versioning.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.590253 jadecobra-0.3.67/src/jadecobra.egg-info/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1878 2023-05-12 14:10:50.000000 jadecobra-0.3.67/src/jadecobra.egg-info/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1050 2023-05-12 14:10:50.000000 jadecobra-0.3.67/src/jadecobra.egg-info/SOURCES.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-05-12 14:10:50.000000 jadecobra-0.3.67/src/jadecobra.egg-info/dependency_links.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-05-12 14:10:50.000000 jadecobra-0.3.67/src/jadecobra.egg-info/requires.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       15 2023-05-12 14:10:50.000000 jadecobra-0.3.67/src/jadecobra.egg-info/top_level.txt
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-05-12 14:10:50.595104 jadecobra-0.3.67/tests/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.67/tests/test_aws_deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.67/tests/test_aws_deploy_lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.67/tests/test_aws_deploy_lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.67/tests/test_aws_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.67/tests/test_environment.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.67/tests/test_jadecobra.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     5677 2023-05-11 13:20:02.000000 jadecobra-0.3.67/tests/test_jadecobra_tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1477 2023-04-20 01:08:32.000000 jadecobra-0.3.67/tests/test_jadecobra_toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1949 2023-04-03 02:04:42.000000 jadecobra-0.3.67/tests/test_jadecobra_versioning.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       72 2023-04-03 02:57:17.000000 jadecobra-0.3.67/tests/test_setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      977 2023-05-04 15:16:26.000000 jadecobra-0.3.67/tests/test_z_build_publish.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.943803 jadecobra-0.3.7/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.7/LICENSE
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1877 2023-04-03 00:47:12.943654 jadecobra-0.3.7/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.7/README.md
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      533 2023-04-03 00:46:54.000000 jadecobra-0.3.7/pyproject.toml
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-04-03 00:47:12.943847 jadecobra-0.3.7/setup.cfg
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.935666 jadecobra-0.3.7/src/
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.938315 jadecobra-0.3.7/src/jadecobra/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       21 2023-04-03 00:46:54.000000 jadecobra-0.3.7/src/jadecobra/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.7/src/jadecobra/aws_environment.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.939323 jadecobra-0.3.7/src/jadecobra/aws_lambda/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/__init__.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.940897 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     3731 2023-03-31 22:35:26.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.7/src/jadecobra/cloudformation_deployer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.7/src/jadecobra/setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1960 2023-04-03 00:40:54.000000 jadecobra-0.3.7/src/jadecobra/tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1784 2023-04-03 00:06:36.000000 jadecobra-0.3.7/src/jadecobra/toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1694 2023-04-03 00:36:26.000000 jadecobra-0.3.7/src/jadecobra/versioning.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.939189 jadecobra-0.3.7/src/jadecobra.egg-info/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1877 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1029 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/requires.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       10 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/top_level.txt
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.943448 jadecobra-0.3.7/tests/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.7/tests/test_aws_deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.7/tests/test_aws_deploy_lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.7/tests/test_aws_deploy_lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.7/tests/test_aws_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.7/tests/test_environment.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.7/tests/test_jadecobra.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     4806 2023-04-03 00:16:06.000000 jadecobra-0.3.7/tests/test_jadecobra_tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1195 2023-04-03 00:32:43.000000 jadecobra-0.3.7/tests/test_jadecobra_toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1832 2023-04-03 00:46:48.000000 jadecobra-0.3.7/tests/test_jadecobra_versioning.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:47:21.000000 jadecobra-0.3.7/tests/test_setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      598 2023-04-03 00:46:57.000000 jadecobra-0.3.7/tests/test_z_build_publish.py
```

### Comparing `jadecobra-0.3.67/LICENSE` & `jadecobra-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/PKG-INFO` & `jadecobra-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.67
+Version: 0.3.7
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.67/pyproject.toml` & `jadecobra-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jadecobra"
-version = "0.3.67"
+version = "0.3.7"
 authors = [
   { name="johnnyblase", email="johnnyblasin@gmail.com" },
 ]
 description = "DRY"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `jadecobra-0.3.67/src/jadecobra/aws_environment.py` & `jadecobra-0.3.7/src/jadecobra/aws_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/deploy.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/deploy_lambda.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/lambda_function.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/src/jadecobra/aws_lambda/deploy/lambda_layer.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
 import shutil
 
 from . import deploy_lambda
 
 
 class LambdaLayer(deploy_lambda.LambdaDeployer):
+
     def __init__(
-        self, dependencies=None, bucket_name=None, profile_name=os.getenv('AWS_PROFILE', 'DEV'), name=None
+        self,
+        dependencies=None,
+        bucket_name=None,
+        profile_name="DEV",
+        name=None
     ):
         super().__init__(bucket_name=bucket_name, profile_name=profile_name)
         self.dependencies = dependencies
         self.set_name(name)
         self.delete_directory()
         self.package_layer()
         # self.upload_to_s3()
@@ -55,32 +60,26 @@
     def runtime(self):
         return "python"
 
     def install_dependencies(self):
         try:
             for dependency in self.dependencies:
                 os.system(
-                    "pip install "
-                    "--upgrade "
-                    f"--target ./{self.directory()}/{self.runtime()} "
-                    "--platform manylinux2014_x86_64 --only-binary=:all: "
-                    "--platform manylinux2014_aarch64 --only-binary=:all: "
-                    f"--implementation cp {dependency}"
+                    f"pip install --target ./{self.directory()}/{self.runtime()} {dependency} --upgrade --platform linux_x86_64 --only-binary=:all: --platform linux_aarch64 --only-binary=:all:"
                 )
         except TypeError:
             print("No dependencies to install")
 
     def package_layer(self):
         self.delimiter()
         print(f"Creating Archive for {self.name} Layer")
         os.system("python -m pip install -U pip")
         self.install_dependencies()
         shutil.make_archive(
-            self.name,
-            "zip",
+            self.name, "zip",
             root_dir=self.directory(),
             # base_dir=self.runtime()
         )
 
     def zip_filename(self):
         return f"{self.name}.zip"
```

### Comparing `jadecobra-0.3.67/src/jadecobra.egg-info/PKG-INFO` & `jadecobra-0.3.7/src/jadecobra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.67
+Version: 0.3.7
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.67/src/jadecobra.egg-info/SOURCES.txt` & `jadecobra-0.3.7/src/jadecobra.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-src/None/__init__.py
 src/jadecobra/__init__.py
 src/jadecobra/aws_environment.py
 src/jadecobra/cloudformation_deployer.py
 src/jadecobra/setup_tdd.py
 src/jadecobra/tester.py
 src/jadecobra/toolkit.py
 src/jadecobra/versioning.py
```

### Comparing `jadecobra-0.3.67/tests/test_aws_deploy_lambda.py` & `jadecobra-0.3.7/tests/test_aws_deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/tests/test_aws_deploy_lambda_function.py` & `jadecobra-0.3.7/tests/test_aws_deploy_lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/tests/test_aws_deploy_lambda_layer.py` & `jadecobra-0.3.7/tests/test_aws_deploy_lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/tests/test_aws_lambda.py` & `jadecobra-0.3.7/tests/test_aws_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/tests/test_environment.py` & `jadecobra-0.3.7/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/tests/test_jadecobra.py` & `jadecobra-0.3.7/tests/test_jadecobra.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.67/tests/test_jadecobra_toolkit.py` & `jadecobra-0.3.7/tests/test_jadecobra_versioning.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-import src.jadecobra
 import src.jadecobra.tester
-import src.jadecobra.toolkit
 import src.jadecobra.versioning
 
 
-class TestJadeCobraToolkit(src.jadecobra.tester.TestCase):
+class TestJadeCobraVersioning(src.jadecobra.tester.TestCase):
 
-    def test_toolkit(self):
+    def test_version_attributes(self):
         self.assert_attributes_equal(
-            src.jadecobra.toolkit,
+            src.jadecobra.versioning,
             [
+                'Version',
                 '__builtins__',
                 '__cached__',
                 '__doc__',
                 '__file__',
                 '__loader__',
                 '__name__',
                 '__package__',
                 '__spec__',
-                'datetime',
-                'delete',
-                'delimiter',
-                'error',
-                'file_exists',
-                'get_commit_message',
-                'get_latest_published_version',
-                'git_commit',
-                'git_diff',
-                'header',
-                'json',
-                'log_performance',
-                'logger',
-                'make_parent_directory',
                 'os',
-                'package',
-                'pathlib',
-                'publish',
-                'read_json',
-                'run_in_shell',
-                'subprocess',
-                'time',
-                'time_it',
-                'to_camel_case',
-                'write_config',
-                'write_file'
+                're',
+                'toolkit',
             ]
         )
 
-    def test_to_camel_case(self):
-        self.assertEqual(
-            src.jadecobra.toolkit.to_camel_case('abc-def-hij'),
-            'AbcDefHij'
-        )
+    def test_version_class_attributes(self):
+        self.assert_attributes_equal(
+            src.jadecobra.versioning.Version,
+            [
+                '__class__',
+                '__delattr__',
+                '__dict__',
+                '__dir__',
+                '__doc__',
+                '__eq__',
+                '__format__',
+                '__ge__',
+                '__getattribute__',
+                '__getstate__',
+                '__gt__',
+                '__hash__',
+                '__init__',
+                '__init_subclass__',
+                '__le__',
+                '__lt__',
+                '__module__',
+                '__ne__',
+                '__new__',
+                '__reduce__',
+                '__reduce_ex__',
+                '__repr__',
+                '__setattr__',
+                '__sizeof__',
+                '__str__',
+                '__subclasshook__',
+                '__weakref__',
+                'get_pyproject_version',
+                'git_push',
+                'pyproject',
+                'read_pyproject',
+                'semantic_version_pattern',
+                'update_module_version',
+                'update_pyproject_version'
+            ]
+        )
+
+
```


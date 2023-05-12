# Comparing `tmp/aws_console_url-0.7.4.tar.gz` & `tmp/aws_console_url-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_console_url-0.7.4.tar", last modified: Tue May  9 19:41:36 2023, max compression
+gzip compressed data, was "aws_console_url-0.7.5.tar", last modified: Fri May 12 17:57:30 2023, max compression
```

## Comparing `aws_console_url-0.7.4.tar` & `aws_console_url-0.7.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.026028 aws_console_url-0.7.4/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-09 19:41:36.025890 aws_console_url-0.7.4/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)    15928 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/Public-API.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     2905 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.022227 aws_console_url-0.7.4/aws_console_url/
--rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-09 19:39:37.000000 aws_console_url-0.7.4/aws_console_url/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/compat.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3555 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/console.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.022886 aws_console_url-0.7.4/aws_console_url/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6437 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/model.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1213 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/resource.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.025198 aws_console_url-0.7.4/aws_console_url/srv/
--rw-r--r--   0 sanhehu    (501) staff       (20)       45 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2769 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/a2i.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5747 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/awslambda.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    14455 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/cloudformation.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4619 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/cloudwatch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5455 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/codebuild.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4116 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/codecommit.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1831 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1553 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/ecr.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4386 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/glue.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1596 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/ground_truth.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4917 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/iam.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2502 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/s3.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1207 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/sagemaker.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/secretmanager.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1834 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/sqs.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1607 2023-05-09 19:38:31.000000 aws_console_url-0.7.4/aws_console_url/srv/ssm.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5552 2023-05-09 19:36:47.000000 aws_console_url-0.7.4/aws_console_url/srv/step_function.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2810 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/vpc.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.025515 aws_console_url-0.7.4/aws_console_url/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/tests/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.022776 aws_console_url-0.7.4/aws_console_url.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-09 19:41:35.000000 aws_console_url-0.7.4/aws_console_url.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1322 2023-05-09 19:41:36.000000 aws_console_url-0.7.4/aws_console_url.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-09 19:41:35.000000 aws_console_url-0.7.4/aws_console_url.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      300 2023-05-09 19:41:36.000000 aws_console_url-0.7.4/aws_console_url.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-09 19:41:36.000000 aws_console_url-0.7.4/aws_console_url.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2424 2023-05-09 19:41:20.000000 aws_console_url-0.7.4/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      297 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      117 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-09 19:41:36.026066 aws_console_url-0.7.4/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7661 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.025724 aws_console_url-0.7.4/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      290 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/tests/test_builder.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1658 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.234783 aws_console_url-0.7.5/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-12 17:57:30.234646 aws_console_url-0.7.5/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15928 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/Public-API.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2905 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.229656 aws_console_url-0.7.5/aws_console_url/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 01:36:58.000000 aws_console_url-0.7.5/aws_console_url/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3555 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/console.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.230399 aws_console_url-0.7.5/aws_console_url/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6758 2023-05-12 01:33:30.000000 aws_console_url-0.7.5/aws_console_url/model.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1213 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/resource.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.233652 aws_console_url-0.7.5/aws_console_url/srv/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       45 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2769 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/a2i.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5747 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/awslambda.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14455 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/cloudformation.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4619 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/cloudwatch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5455 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/codebuild.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4116 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/codecommit.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1831 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1553 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/ecr.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4386 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/glue.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1596 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/ground_truth.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4917 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/iam.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2502 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1207 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/sagemaker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/secretmanager.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1834 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/sqs.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1607 2023-05-09 19:38:31.000000 aws_console_url-0.7.5/aws_console_url/srv/ssm.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5552 2023-05-09 19:36:47.000000 aws_console_url-0.7.5/aws_console_url/srv/step_function.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2810 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/vpc.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.234043 aws_console_url-0.7.5/aws_console_url/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.230275 aws_console_url-0.7.5/aws_console_url.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1322 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      300 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2606 2023-05-12 01:36:51.000000 aws_console_url-0.7.5/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      297 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      117 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 17:57:30.234824 aws_console_url-0.7.5/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7661 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.234386 aws_console_url-0.7.5/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      290 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/tests/test_builder.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1658 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/tests/test_import.py
```

### Comparing `aws_console_url-0.7.4/LICENSE.txt` & `aws_console_url-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/PKG-INFO` & `aws_console_url-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_console_url
-Version: 0.7.4
+Version: 0.7.5
 Summary: Build AWS Console Url for debugging.
 Home-page: https://github.com/MacHu-GWU/aws_console_url-project
-Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.4#downloads
+Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.5#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_console_url-0.7.4/Public-API.rst` & `aws_console_url-0.7.5/Public-API.rst`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/README.rst` & `aws_console_url-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/console.py` & `aws_console_url-0.7.5/aws_console_url/console.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/model.py` & `aws_console_url-0.7.5/aws_console_url/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,22 +72,33 @@
             name=name,
             _service_name=cls._SERVICE_NAME,
             _resource_type=cls._RESOURCE_TYPE,
         )
 
     @property
     def arn(self) -> str:
-        return f"arn:aws:{self._service_name}:{self.aws_region}:{self.aws_account_id}:{self._resource_type}/{self.name}"
+        if self.name.startswith("/"):
+            name = self.name[1:]
+        else:
+            name = self.name
+        return f"arn:aws:{self._service_name}:{self.aws_region}:{self.aws_account_id}:{self._resource_type}/{name}"
 
     @classmethod
     def from_arn(cls, arn: str) -> "BaseServiceResourceV1":
         parts = arn.split(":")
         aws_account_id = parts[4]
         aws_region = parts[3]
-        name = parts[5].split("/")[-1]
+        name = parts[5].replace(cls._RESOURCE_TYPE, "")
+        slash_count = name.count("/")
+        if slash_count == 0:
+            raise NotImplementedError
+        elif slash_count == 1:
+            name = name[1:]
+        else:
+            pass
         return cls.make(aws_account_id, aws_region, name)
 
 
 @dataclasses.dataclass(frozen=True)
 class Service:
     """
     Represent an AWS Service. This class is mainly for creating AWS console urls.
```

### Comparing `aws_console_url-0.7.4/aws_console_url/resource.py` & `aws_console_url-0.7.5/aws_console_url/resource.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/a2i.py` & `aws_console_url-0.7.5/aws_console_url/srv/a2i.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/awslambda.py` & `aws_console_url-0.7.5/aws_console_url/srv/awslambda.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/cloudformation.py` & `aws_console_url-0.7.5/aws_console_url/srv/cloudformation.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/cloudwatch.py` & `aws_console_url-0.7.5/aws_console_url/srv/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/codebuild.py` & `aws_console_url-0.7.5/aws_console_url/srv/codebuild.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/codecommit.py` & `aws_console_url-0.7.5/aws_console_url/srv/codecommit.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/dynamodb.py` & `aws_console_url-0.7.5/aws_console_url/srv/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/ec2.py` & `aws_console_url-0.7.5/aws_console_url/srv/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/ecr.py` & `aws_console_url-0.7.5/aws_console_url/srv/ecr.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/glue.py` & `aws_console_url-0.7.5/aws_console_url/srv/glue.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/ground_truth.py` & `aws_console_url-0.7.5/aws_console_url/srv/ground_truth.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/iam.py` & `aws_console_url-0.7.5/aws_console_url/srv/iam.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/s3.py` & `aws_console_url-0.7.5/aws_console_url/srv/s3.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/sagemaker.py` & `aws_console_url-0.7.5/aws_console_url/srv/sagemaker.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/secretmanager.py` & `aws_console_url-0.7.5/aws_console_url/srv/secretmanager.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/sqs.py` & `aws_console_url-0.7.5/aws_console_url/srv/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/ssm.py` & `aws_console_url-0.7.5/aws_console_url/srv/ssm.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/step_function.py` & `aws_console_url-0.7.5/aws_console_url/srv/step_function.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/srv/vpc.py` & `aws_console_url-0.7.5/aws_console_url/srv/vpc.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url/tests/helper.py` & `aws_console_url-0.7.5/aws_console_url/tests/helper.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/aws_console_url.egg-info/PKG-INFO` & `aws_console_url-0.7.5/aws_console_url.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-console-url
-Version: 0.7.4
+Version: 0.7.5
 Summary: Build AWS Console Url for debugging.
 Home-page: https://github.com/MacHu-GWU/aws_console_url-project
-Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.4#downloads
+Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.5#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_console_url-0.7.4/aws_console_url.egg-info/SOURCES.txt` & `aws_console_url-0.7.5/aws_console_url.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/release-history.rst` & `aws_console_url-0.7.5/release-history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.7.5 (2023-05-10)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- add support to those resource name may have slash (SSM parameter)
+
+
 0.7.4 (2023-05-09)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that when SSM parameter has a prefix "/", the console url is not correct.
```

### Comparing `aws_console_url-0.7.4/requirements-doc.txt` & `aws_console_url-0.7.5/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/setup.py` & `aws_console_url-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.4/tests/test_import.py` & `aws_console_url-0.7.5/tests/test_import.py`

 * *Files identical despite different names*


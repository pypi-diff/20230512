# Comparing `tmp/cdk-extensions-0.0.60.tar.gz` & `tmp/cdk-extensions-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.60.tar", last modified: Fri May 12 17:41:05 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.61.tar", last modified: Fri May 12 20:37:43 2023, max compression
```

## Comparing `cdk-extensions-0.0.60.tar` & `cdk-extensions-0.0.61.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.926235 cdk-extensions-0.0.60/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1593138 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/_jsii/cdk-extensions@0.0.60.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   257720 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.934235 cdk-extensions-0.0.60/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.938235 cdk-extensions-0.0.60/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-12 17:40:53.000000 cdk-extensions-0.0.60/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:41:05.930235 cdk-extensions-0.0.60/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-12 17:41:05.000000 cdk-extensions-0.0.60/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-12 17:41:05.000000 cdk-extensions-0.0.60/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:41:05.000000 cdk-extensions-0.0.60/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 17:41:05.000000 cdk-extensions-0.0.60/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 17:41:05.000000 cdk-extensions-0.0.60/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.835818 cdk-extensions-0.0.61/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.839819 cdk-extensions-0.0.61/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.839819 cdk-extensions-0.0.61/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1594052 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/_jsii/cdk-extensions@0.0.61.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702552 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.843819 cdk-extensions-0.0.61/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   261565 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.847819 cdk-extensions-0.0.61/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215302 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.851820 cdk-extensions-0.0.61/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-05-12 20:37:29.000000 cdk-extensions-0.0.61/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:37:43.839819 cdk-extensions-0.0.61/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-12 20:37:43.000000 cdk-extensions-0.0.61/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-12 20:37:43.000000 cdk-extensions-0.0.61/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:37:43.000000 cdk-extensions-0.0.61/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 20:37:43.000000 cdk-extensions-0.0.61/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 20:37:43.000000 cdk-extensions-0.0.61/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.60/LICENSE` & `cdk-extensions-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/PKG-INFO` & `cdk-extensions-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.60
+Version: 0.0.61
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.60/README.md` & `cdk-extensions-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/setup.py` & `cdk-extensions-0.0.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.60",
+    "version": "0.0.61",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -43,15 +43,15 @@
         "cdk_extensions.route53",
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.60.jsii.tgz"
+            "cdk-extensions@0.0.61.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,14 +546,73 @@
     def __repr__(self) -> str:
         return "AddIsolatedClientVpnEndpointOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="cdk-extensions.ec2_patterns.AddMultiSubnetRouteOptions",
+    jsii_struct_bases=[],
+    name_mapping={"cidr": "cidr", "description": "description", "scope": "scope"},
+)
+class AddMultiSubnetRouteOptions:
+    def __init__(
+        self,
+        *,
+        cidr: builtins.str,
+        description: typing.Optional[builtins.str] = None,
+        scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+    ) -> None:
+        '''
+        :param cidr: 
+        :param description: 
+        :param scope: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2888f6c29133d3bfecf96140b79c8780f82cf2cc72ed0d79419b5f5ddc3772ee)
+            check_type(argname="argument cidr", value=cidr, expected_type=type_hints["cidr"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "cidr": cidr,
+        }
+        if description is not None:
+            self._values["description"] = description
+        if scope is not None:
+            self._values["scope"] = scope
+
+    @builtins.property
+    def cidr(self) -> builtins.str:
+        result = self._values.get("cidr")
+        assert result is not None, "Required property 'cidr' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def scope(self) -> typing.Optional[_constructs_77d1e7e8.IConstruct]:
+        result = self._values.get("scope")
+        return typing.cast(typing.Optional[_constructs_77d1e7e8.IConstruct], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "AddMultiSubnetRouteOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="cdk-extensions.ec2_patterns.AddNetworkOptions",
     jsii_struct_bases=[],
     name_mapping={
         "availability_zones": "availabilityZones",
         "max_azs": "maxAzs",
         "netmask": "netmask",
     },
@@ -3548,14 +3607,38 @@
             environment_from_arn=environment_from_arn,
             physical_name=physical_name,
             region=region,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="addMultiSubnetRoute")
+    def add_multi_subnet_route(
+        self,
+        id: builtins.str,
+        *,
+        cidr: builtins.str,
+        description: typing.Optional[builtins.str] = None,
+        scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+    ) -> typing.Any:
+        '''
+        :param id: -
+        :param cidr: 
+        :param description: 
+        :param scope: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__474ff1f3d7805ad25fb8ef0d62e9d0b5e3c0c8fa7c0d5a895288ab6abd22e207)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        options = AddMultiSubnetRouteOptions(
+            cidr=cidr, description=description, scope=scope
+        )
+
+        return typing.cast(typing.Any, jsii.invoke(self, "addMultiSubnetRoute", [id, options]))
+
     @jsii.python.classproperty
     @jsii.member(jsii_name="DEFAULT_VPN_CIDR")
     def DEFAULT_VPN_CIDR(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "DEFAULT_VPN_CIDR"))
 
     @builtins.property
     @jsii.member(jsii_name="clientVpnEndpoint")
@@ -4285,14 +4368,15 @@
 
 
 __all__ = [
     "AddCidrBlockOptions",
     "AddClientVpnEndpointOptions",
     "AddHubOptions",
     "AddIsolatedClientVpnEndpointOptions",
+    "AddMultiSubnetRouteOptions",
     "AddNetworkOptions",
     "AddPoolOptions",
     "AddSpokeNetworkProps",
     "AllocatePrivateNetworkOptions",
     "FlowLogOptions",
     "FourTierNetwork",
     "FourTierNetworkHub",
@@ -4368,14 +4452,23 @@
     transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
     user_based_authentication: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnUserBasedAuthentication] = None,
     vpn_cidr: typing.Optional[_IIpv4CidrAssignment_b412e3a5] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__2888f6c29133d3bfecf96140b79c8780f82cf2cc72ed0d79419b5f5ddc3772ee(
+    *,
+    cidr: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+    scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__24d3c1346e4e259fee32303499f123223b892ff23852cdfdf5a57bf21cad7680(
     *,
     availability_zones: typing.Optional[typing.Sequence[builtins.str]] = None,
     max_azs: typing.Optional[jsii.Number] = None,
     netmask: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
@@ -4920,14 +5013,24 @@
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__474ff1f3d7805ad25fb8ef0d62e9d0b5e3c0c8fa7c0d5a895288ab6abd22e207(
+    id: builtins.str,
+    *,
+    cidr: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+    scope: typing.Optional[_constructs_77d1e7e8.IConstruct] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__3802025d1d451c01388cfc739e97c163e6f87b2af20266ee60e0b8b5f0be1607(
     *,
     account: typing.Optional[builtins.str] = None,
     environment_from_arn: typing.Optional[builtins.str] = None,
     physical_name: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
     server_certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
```

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.61/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.61/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.60
+Version: 0.0.61
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.60/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.61/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.60.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.61.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```


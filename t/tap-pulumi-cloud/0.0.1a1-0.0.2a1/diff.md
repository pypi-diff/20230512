# Comparing `tmp/tap_pulumi_cloud-0.0.1a1.tar.gz` & `tmp/tap_pulumi_cloud-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_pulumi_cloud-0.0.1a1.tar", max compression
+gzip compressed data, was "tap_pulumi_cloud-0.0.2a1.tar", max compression
```

## Comparing `tap_pulumi_cloud-0.0.1a1.tar` & `tap_pulumi_cloud-0.0.2a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     3087 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/README.md
--rw-r--r--   0        0        0     2131 2023-04-17 18:30:37.509409 tap_pulumi_cloud-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/__init__.py
--rw-r--r--   0        0        0      129 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/__main__.py
--rw-r--r--   0        0        0     2027 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/client.py
--rw-r--r--   0        0        0     7957 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/streams.py
--rw-r--r--   0        0        0     2496 2023-04-17 18:30:15.367941 tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/tap.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 tap_pulumi_cloud-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0     3087 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/README.md
+-rw-r--r--   0        0        0     2131 2023-05-12 18:12:36.079154 tap_pulumi_cloud-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/__main__.py
+-rw-r--r--   0        0        0     2027 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/client.py
+-rw-r--r--   0        0        0     7957 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/streams.py
+-rw-r--r--   0        0        0     2496 2023-05-12 18:12:16.675037 tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/tap.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 tap_pulumi_cloud-0.0.2a1/PKG-INFO
```

### Comparing `tap_pulumi_cloud-0.0.1a1/LICENSE` & `tap_pulumi_cloud-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.1a1/README.md` & `tap_pulumi_cloud-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.1a1/pyproject.toml` & `tap_pulumi_cloud-0.0.2a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1,<2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tap-pulumi-cloud"
-version = "0.0.1a1"
+version = "0.0.2a1"
 description = "`tap-pulumi-cloud` is a Singer tap for Pulumi Cloud, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Pulumi Cloud",
 ]
@@ -18,18 +18,18 @@
 repository = "https://github.com/edgarrmondragon/tap-pulumi-cloud"
 documentation = "https://github.com/edgarrmondragon/tap-pulumi-cloud#readme"
 
 [tool.poetry.dependencies]
 pyhumps = "^3.8.0"
 python = "<3.12,>=3.7.1"
 requests-cache = "^1.0.1"
-singer-sdk = "0.24.0"
+singer-sdk = "0.27.0"
 
 [tool.poetry.group.dev.dependencies]
-singer-sdk = { version = "0.24.0", extras = ["testing"] }
+singer-sdk = { version = "0.27.0", extras = ["testing"] }
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-pulumi-cloud" = "tap_pulumi_cloud.tap:TapPulumiCloud.cli"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/client.py` & `tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/client.py`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/streams.py` & `tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/streams.py`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.1a1/tap_pulumi_cloud/tap.py` & `tap_pulumi_cloud-0.0.2a1/tap_pulumi_cloud/tap.py`

 * *Files identical despite different names*

### Comparing `tap_pulumi_cloud-0.0.1a1/PKG-INFO` & `tap_pulumi_cloud-0.0.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-pulumi-cloud
-Version: 0.0.1a1
+Version: 0.0.2a1
 Summary: `tap-pulumi-cloud` is a Singer tap for Pulumi Cloud, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-pulumi-cloud
 License: Apache-2.0
 Keywords: ELT,singer.io,Pulumi Cloud
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: singer-sdk (==0.24.0)
+Requires-Dist: singer-sdk (==0.27.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-pulumi-cloud#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-pulumi-cloud
 Description-Content-Type: text/markdown
 
 # `tap-pulumi-cloud`
 
 Singer tap for Pulumi Cloud.
```


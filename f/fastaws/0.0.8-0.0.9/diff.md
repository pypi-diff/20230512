# Comparing `tmp/fastaws-0.0.8.tar.gz` & `tmp/fastaws-0.0.9.tar.gz`

## Comparing `fastaws-0.0.8.tar` & `fastaws-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastaws-0.0.8/Makefile
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/auth.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/core.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/enums.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/exceptions.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/s3/client.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/s3/models.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/ses/client.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/sqs/client.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/sqs/models.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastaws-0.0.8/src/fastaws/sqs/utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastaws-0.0.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fastaws-0.0.8/LICENSE
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastaws-0.0.8/README.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 fastaws-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 fastaws-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastaws-0.0.9/Makefile
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/auth.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/core.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/enums.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/exceptions.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/s3/client.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/s3/models.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/ses/client.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/sqs/client.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/sqs/models.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastaws-0.0.9/src/fastaws/sqs/utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastaws-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fastaws-0.0.9/LICENSE
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastaws-0.0.9/README.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 fastaws-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 fastaws-0.0.9/PKG-INFO
```

### Comparing `fastaws-0.0.8/src/fastaws/auth.py` & `fastaws-0.0.9/src/fastaws/auth.py`

 * *Files identical despite different names*

### Comparing `fastaws-0.0.8/src/fastaws/core.py` & `fastaws-0.0.9/src/fastaws/core.py`

 * *Files identical despite different names*

### Comparing `fastaws-0.0.8/src/fastaws/s3/client.py` & `fastaws-0.0.9/src/fastaws/s3/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import date, datetime
 from typing import Any, Literal
+from urllib.parse import urlparse
 
 from bs4 import BeautifulSoup, Tag
 
 from fastaws.core import AwsClient
 from fastaws.enums import Service
 
 from .models import S3ListObjectsRes, S3Object, S3ObjectOwner
@@ -121,17 +122,22 @@
         self,
         bucket: str,
         *,
         data: Any,
         remote_filepath: str,
         access: AmzAcl = "private",
     ):
+        """
+        `remote_filepath` must start with a "/"
+        """
+        f_remote_filepath = urlparse(remote_filepath).path
+
         res = await self._make_request(
             method="PUT",
             action="PutObject",
             host=f"{bucket}.{self.host}",
-            endpoint=remote_filepath,
+            endpoint=f_remote_filepath,
             extra_headers={"x-amz-acl": access},
             data=data,
         )
 
         return res
```

### Comparing `fastaws-0.0.8/src/fastaws/ses/client.py` & `fastaws-0.0.9/src/fastaws/ses/client.py`

 * *Files identical despite different names*

### Comparing `fastaws-0.0.8/src/fastaws/sqs/client.py` & `fastaws-0.0.9/src/fastaws/sqs/client.py`

 * *Files identical despite different names*

### Comparing `fastaws-0.0.8/LICENSE` & `fastaws-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastaws-0.0.8/pyproject.toml` & `fastaws-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastaws"
-version = "0.0.8"
+version = "0.0.9"
 description = "A fast, simple, async Python library for some AWS services (S3, SES, SQS)"
 readme = "README.md"
 requires-python = ">=3.10.4"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "aws", "asyncio"]
 classifiers = [
```

### Comparing `fastaws-0.0.8/PKG-INFO` & `fastaws-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastaws
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fast, simple, async Python library for some AWS services (S3, SES, SQS)
 Project-URL: Homepage, https://github.com/waydegg/fastaws
 Project-URL: Source, https://github.com/waydegg/fastaws
 Author-email: Wayde Gilliam <waydegilliam@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: asyncio,aws,python
```


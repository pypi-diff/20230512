# Comparing `tmp/pysecret-2.2.2.tar.gz` & `tmp/pysecret-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysecret-2.2.2.tar", last modified: Sun Feb 12 06:22:37 2023, max compression
+gzip compressed data, was "pysecret-2.2.3.tar", last modified: Fri May 12 17:56:56 2023, max compression
```

## Comparing `pysecret-2.2.2.tar` & `pysecret-2.2.3.tar`

### file list

```diff
@@ -1,45 +1,52 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-12 06:22:37.430225 pysecret-2.2.2/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2023-02-11 22:09:52.000000 pysecret-2.2.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1118 2021-10-07 16:11:09.000000 pysecret-2.2.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      316 2023-02-10 15:08:00.000000 pysecret-2.2.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     4958 2023-02-12 06:22:37.430051 pysecret-2.2.2/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     3881 2023-02-12 04:24:32.000000 pysecret-2.2.2/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-12 06:22:37.426147 pysecret-2.2.2/pysecret/
--rw-r--r--   0 sanhehu    (505) staff       (20)     1704 2023-02-12 05:35:36.000000 pysecret-2.2.2/pysecret/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-02-12 06:22:28.000000 pysecret-2.2.2/pysecret/_version.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-12 06:22:37.428777 pysecret-2.2.2/pysecret/aws/
--rw-r--r--   0 sanhehu    (505) staff       (20)      376 2023-02-12 05:35:04.000000 pysecret-2.2.2/pysecret/aws/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      786 2023-02-11 20:55:39.000000 pysecret-2.2.2/pysecret/aws/kms.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    19575 2023-02-10 16:56:42.000000 pysecret-2.2.2/pysecret/aws/main.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    18894 2023-02-12 06:20:45.000000 pysecret-2.2.2/pysecret/aws/parameter_store.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    11438 2023-02-11 20:23:34.000000 pysecret-2.2.2/pysecret/aws/secret_manager.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      321 2023-02-12 05:06:06.000000 pysecret-2.2.2/pysecret/aws/tagging.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      336 2023-02-10 17:14:29.000000 pysecret-2.2.2/pysecret/compat.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-12 06:22:37.429010 pysecret-2.2.2/pysecret/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2021-10-07 16:11:09.000000 pysecret-2.2.2/pysecret/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2462 2023-02-11 21:15:45.000000 pysecret-2.2.2/pysecret/env.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      329 2023-02-10 21:58:26.000000 pysecret-2.2.2/pysecret/helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1298 2023-02-10 15:34:48.000000 pysecret-2.2.2/pysecret/js.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3385 2023-02-10 15:41:21.000000 pysecret-2.2.2/pysecret/js_helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      190 2023-02-11 20:52:50.000000 pysecret-2.2.2/pysecret/paths.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      698 2023-02-11 21:04:38.000000 pysecret-2.2.2/pysecret/sh.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2653 2023-02-11 21:05:27.000000 pysecret-2.2.2/pysecret/sh_helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1483 2021-10-07 16:11:09.000000 pysecret-2.2.2/pysecret/singleton.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1236 2021-10-07 16:11:09.000000 pysecret-2.2.2/pysecret/singleton_alternative.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-12 06:22:37.429693 pysecret-2.2.2/pysecret/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      359 2023-02-11 20:40:33.000000 pysecret-2.2.2/pysecret/tests/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1241 2023-02-10 15:19:45.000000 pysecret-2.2.2/pysecret/tests/covtest.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      370 2023-01-02 00:03:52.000000 pysecret-2.2.2/pysecret/tests/paths.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-12 06:22:37.427044 pysecret-2.2.2/pysecret.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     4958 2023-02-12 06:22:37.000000 pysecret-2.2.2/pysecret.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      815 2023-02-12 06:22:37.000000 pysecret-2.2.2/pysecret.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-12 06:22:37.000000 pysecret-2.2.2/pysecret.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      221 2023-02-12 06:22:37.000000 pysecret-2.2.2/pysecret.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        9 2023-02-12 06:22:37.000000 pysecret-2.2.2/pysecret.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     5672 2023-02-12 06:22:14.000000 pysecret-2.2.2/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      139 2023-02-11 21:15:06.000000 pysecret-2.2.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      620 2022-03-27 03:45:41.000000 pysecret-2.2.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       98 2023-02-11 21:15:06.000000 pysecret-2.2.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       47 2023-02-12 03:57:47.000000 pysecret-2.2.2/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-12 06:22:37.430278 pysecret-2.2.2/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7488 2023-02-10 15:16:26.000000 pysecret-2.2.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.626958 pysecret-2.2.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 17:04:24.000000 pysecret-2.2.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1118 2023-05-12 17:04:24.000000 pysecret-2.2.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      316 2023-05-12 17:04:24.000000 pysecret-2.2.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4958 2023-05-12 17:56:56.626817 pysecret-2.2.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3881 2023-05-12 17:04:24.000000 pysecret-2.2.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.623519 pysecret-2.2.3/pysecret/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1704 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 17:37:14.000000 pysecret-2.2.3/pysecret/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.625090 pysecret-2.2.3/pysecret/aws/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      376 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/aws/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      786 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/aws/kms.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    19575 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/aws/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    19211 2023-05-12 17:17:27.000000 pysecret-2.2.3/pysecret/aws/parameter_store.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11588 2023-05-12 17:29:28.000000 pysecret-2.2.3/pysecret/aws/secret_manager.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/aws/tagging.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.625238 pysecret-2.2.3/pysecret/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2462 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/env.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1298 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/js.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3385 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/js_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      190 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      698 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/sh.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2653 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/sh_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1483 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/singleton.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1236 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/singleton_alternative.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.625769 pysecret-2.2.3/pysecret/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      359 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1241 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/tests/covtest.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-12 17:04:24.000000 pysecret-2.2.3/pysecret/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.624222 pysecret-2.2.3/pysecret.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4958 2023-05-12 17:56:56.000000 pysecret-2.2.3/pysecret.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      961 2023-05-12 17:56:56.000000 pysecret-2.2.3/pysecret.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 17:56:56.000000 pysecret-2.2.3/pysecret.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      221 2023-05-12 17:56:56.000000 pysecret-2.2.3/pysecret.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        9 2023-05-12 17:56:56.000000 pysecret-2.2.3/pysecret.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5885 2023-05-12 17:30:55.000000 pysecret-2.2.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      139 2023-05-12 17:04:24.000000 pysecret-2.2.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      620 2023-05-12 17:04:24.000000 pysecret-2.2.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-05-12 17:04:24.000000 pysecret-2.2.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       47 2023-05-12 17:04:24.000000 pysecret-2.2.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 17:56:56.627004 pysecret-2.2.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7488 2023-05-12 17:04:24.000000 pysecret-2.2.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:56:56.626614 pysecret-2.2.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1160 2023-05-12 17:04:24.000000 pysecret-2.2.3/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1055 2023-05-12 17:04:24.000000 pysecret-2.2.3/tests/test_js.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1557 2023-05-12 17:04:24.000000 pysecret-2.2.3/tests/test_js_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1308 2023-05-12 17:04:24.000000 pysecret-2.2.3/tests/test_sh_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2002 2023-05-12 17:04:24.000000 pysecret-2.2.3/tests/test_singleton.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1546 2023-05-12 17:04:24.000000 pysecret-2.2.3/tests/test_singleton_alternative.py
```

### Comparing `pysecret-2.2.2/LICENSE.txt` & `pysecret-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/PKG-INFO` & `pysecret-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysecret
-Version: 2.2.2
+Version: 2.2.3
 Summary: utility tool that load secret information safely.
 Home-page: https://github.com/MacHu-GWU/pysecret-project
-Download-URL: https://pypi.python.org/pypi/pysecret/2.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/pysecret/2.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `pysecret-2.2.2/README.rst` & `pysecret-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/__init__.py` & `pysecret-2.2.3/pysecret/__init__.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/aws/kms.py` & `pysecret-2.2.3/pysecret/aws/kms.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/aws/main.py` & `pysecret-2.2.3/pysecret/aws/main.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/aws/parameter_store.py` & `pysecret-2.2.3/pysecret/aws/parameter_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,19 +149,19 @@
     - if you know what data type to expect in the parameter, please use
         :meth:`Parameter.string`, :meth:`Parameter.string_list`,
         :meth:`Parameter.json_dict`, :meth:`Parameter.json_list`,
         :meth:`Parameter.py_object` to access the data.
     """
 
     Name: str = dataclasses.field()
-    Type: str = dataclasses.field()
     Value: str = dataclasses.field()
-    Version: int = dataclasses.field()
-    LastModifiedDate: datetime = dataclasses.field()
-    DataType: str = dataclasses.field()
+    Type: T.Optional[str] = dataclasses.field(default=None)
+    Version: T.Optional[int] = dataclasses.field(default=None)
+    LastModifiedDate: T.Optional[datetime] = dataclasses.field(default=None)
+    DataType: T.Optional[str] = dataclasses.field(default=None)
     ARN: T.Optional[str] = dataclasses.field(default=None)
     Selector: T.Optional[str] = dataclasses.field(default=None)
     SourceResult: T.Optional[str] = dataclasses.field(default=None)
     Tags: T.Dict[str, str] = dataclasses.field(default_factory=dict)
     Labels: T.List[str] = dataclasses.field(default_factory=list)
 
     @classmethod
@@ -234,23 +234,30 @@
 
     @classmethod
     def _from_put_parameter_response(
         cls,
         put_parameter_kwargs: dict,
         put_parameter_response: dict,
     ):
+        last_modified_date = (
+            put_parameter_response.get("ResponseMetadata", {})
+            .get("HTTPHeaders", {})
+            .get("date")
+        )
+        if last_modified_date is not None:
+            last_modified_date = datetime.strptime(
+                last_modified_date,
+                "%a, %d %b %Y %H:%M:%S %Z",
+            )
         return Parameter(
             Name=put_parameter_kwargs["Name"],
-            Type=put_parameter_kwargs["Type"],
+            Type=put_parameter_kwargs.get("Type"),
             Value=put_parameter_kwargs["Value"],
-            Version=put_parameter_response["Version"],
-            LastModifiedDate=datetime.strptime(
-                put_parameter_response["ResponseMetadata"]["HTTPHeaders"]["date"],
-                "%a, %d %b %Y %H:%M:%S %Z",
-            ),
+            Version=put_parameter_response.get("Version"),
+            LastModifiedDate=last_modified_date,
             ARN=None,
             DataType="text",
         )
 
     @property
     def string(self) -> str:
         """
```

### Comparing `pysecret-2.2.2/pysecret/aws/secret_manager.py` & `pysecret-2.2.3/pysecret/aws/secret_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     - only one of ``SecretBinary`` or ``SecretString`` could exist.
     - if you know what data type to expect in the secret, please use
         :meth:`Secret.binary`, :meth:`Secret.string`, :meth:`Secret.json_dict`,
         :meth:`Secret.json_list` to access the data.
     """
     ARN: str = dataclasses.field()
     Name: str = dataclasses.field()
-    VersionId: str = dataclasses.field()
-    CreatedDate: datetime = dataclasses.field()
+    VersionId: T.Optional[str] = dataclasses.field(default=None)
+    CreatedDate: T.Optional[datetime] = dataclasses.field(default=None)
     SecretBinary: T.Optional[bytes] = dataclasses.field(default=None)
     SecretString: T.Optional[str] = dataclasses.field(default=None)
     VersionStages: T.List[str] = dataclasses.field(default_factory=list)
 
     @cached_property
     def fingerprint(self) -> bytes:
         """
@@ -87,26 +87,28 @@
 
     @classmethod
     def _from_create_or_update_secret_response(
         cls,
         create_or_update_secret_kwargs: dict,
         create_or_update_secret_response: dict,
     ):
+        created_date = (
+            create_or_update_secret_response.get("ResponseMetadata", {})
+            .get("HTTPHeaders", {})
+            .get("date")
+        )
+        if created_date is not None:
+            created_date = datetime.strptime(created_date, "%a, %d %b %Y %H:%M:%S %Z")
         return Secret(
             ARN=create_or_update_secret_response["ARN"],
             Name=create_or_update_secret_response["Name"],
-            VersionId=create_or_update_secret_response["VersionId"],
+            VersionId=create_or_update_secret_response.get("VersionId"),
             SecretBinary=create_or_update_secret_kwargs.get("SecretBinary"),
             SecretString=create_or_update_secret_kwargs.get("SecretString"),
-            CreatedDate=datetime.strptime(
-                create_or_update_secret_response["ResponseMetadata"]["HTTPHeaders"][
-                    "date"
-                ],
-                "%a, %d %b %Y %H:%M:%S %Z",
-            ),
+            CreatedDate=created_date,
         )
 
     @property
     def binary(self) -> bytes:
         """
         The binary user data.
         """
```

### Comparing `pysecret-2.2.2/pysecret/env.py` & `pysecret-2.2.3/pysecret/env.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/js.py` & `pysecret-2.2.3/pysecret/js.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/js_helper.py` & `pysecret-2.2.3/pysecret/js_helper.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/sh.py` & `pysecret-2.2.3/pysecret/sh.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/sh_helper.py` & `pysecret-2.2.3/pysecret/sh_helper.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/singleton.py` & `pysecret-2.2.3/pysecret/singleton.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/singleton_alternative.py` & `pysecret-2.2.3/pysecret/singleton_alternative.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret/tests/covtest.py` & `pysecret-2.2.3/pysecret/tests/covtest.py`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/pysecret.egg-info/PKG-INFO` & `pysecret-2.2.3/pysecret.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysecret
-Version: 2.2.2
+Version: 2.2.3
 Summary: utility tool that load secret information safely.
 Home-page: https://github.com/MacHu-GWU/pysecret-project
-Download-URL: https://pypi.python.org/pypi/pysecret/2.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/pysecret/2.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `pysecret-2.2.2/release-history.rst` & `pysecret-2.2.3/release-history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+2.2.3 (2023-05-12)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that sometime certain attributes are not available in AWS Parameter and Secret object.
+
+
 2.2.2 (2023-02-12)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that ``pysecret.deploy_parameter`` should not use ``tags`` and ``overwrite`` together when creating a new parameter.
```

### Comparing `pysecret-2.2.2/requirements-doc.txt` & `pysecret-2.2.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `pysecret-2.2.2/setup.py` & `pysecret-2.2.3/setup.py`

 * *Files identical despite different names*


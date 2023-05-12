# Comparing `tmp/braincube-aws-core-alpha-0.0.26.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.26.tar", last modified: Fri May 12 06:58:03 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.27.tar", last modified: Fri May 12 21:31:14 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.26.tar` & `braincube-aws-core-alpha-0.0.27.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.900180 braincube-aws-core-alpha-0.0.26/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9107 2023-05-12 06:58:03.900439 braincube-aws-core-alpha-0.0.26/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8354 2023-05-10 17:06:13.000000 braincube-aws-core-alpha-0.0.26/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-12 06:58:03.901927 braincube-aws-core-alpha-0.0.26/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.883983 braincube-aws-core-alpha-0.0.26/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.888391 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9107 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.888799 braincube-aws-core-alpha-0.0.26/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.892049 braincube-aws-core-alpha-0.0.26/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-11 11:52:40.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3354 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    31143 2023-05-11 16:43:27.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.894425 braincube-aws-core-alpha-0.0.26/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.26/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.26/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.897294 braincube-aws-core-alpha-0.0.26/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.899565 braincube-aws-core-alpha-0.0.26/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-10 14:02:40.000000 braincube-aws-core-alpha-0.0.26/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.26/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.164129 braincube-aws-core-alpha-0.0.27/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-12 21:31:14.164417 braincube-aws-core-alpha-0.0.27/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8338 2023-05-12 07:04:00.000000 braincube-aws-core-alpha-0.0.27/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-12 21:31:14.166020 braincube-aws-core-alpha-0.0.27/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.147251 braincube-aws-core-alpha-0.0.27/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.153547 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      769 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.153855 braincube-aws-core-alpha-0.0.27/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.157563 braincube-aws-core-alpha-0.0.27/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-11 11:52:40.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3362 2023-05-12 12:29:46.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    31571 2023-05-12 08:16:44.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_repository.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      226 2023-05-12 11:56:51.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/transaction_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.159103 braincube-aws-core-alpha-0.0.27/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.27/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.27/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.161511 braincube-aws-core-alpha-0.0.27/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.163469 braincube-aws-core-alpha-0.0.27/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-10 14:02:40.000000 braincube-aws-core-alpha-0.0.27/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.27/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.26/LICENSE` & `braincube-aws-core-alpha-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/PKG-INFO` & `braincube-aws-core-alpha-0.0.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.26
+Version: 0.0.27
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -164,35 +164,35 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
+await repo.find_by_pk(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
-await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
+await repo.exists_by_pk(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
 await repo.find_all(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
-await repo.find_all_by_id([
+await repo.find_all_by_pk([
     Key("9448a57b-f686-4935-b152-566baab712db"),
     Key("43c8ec37-9a59-44eb-be90-def391ba2f02")],
     aliases=request.query_parameters.fields,
     order=request.query_parameters.order)
 
-await repo.find_all_page(
+await repo.find_many(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     page=request.query_parameters.page,
     order=request.query_parameters.order)
 
 await repo.insert(
     data={
@@ -219,34 +219,34 @@
     data={
         "type": 1,
         "isin": 40,
     },
     conditions=request.query_parameters.conditions,
     returning_aliases=request.query_parameters.fields)
 
-await repo.update_by_id(
+await repo.update_by_pk(
     Key("9448a57b-f686-4935-b152-566baab712db"),
     data={
         "type": 1,
         "isin": 40,
     }, returning_aliases=[])
 
 await repo.delete(
     conditions=request.query_parameters.conditions,
     returning_aliases=["id", "name", "type"])
 
-await repo.delete_by_id(
+await repo.delete_by_pk(
     Key("9448a57b-f686-4935-b152-566baab712db"),
     returning_aliases=["id", "name", "type"])
 
-await repo.fetch_raw("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
+await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
-await repo.fetch_one_raw("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
+await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
-await repo.execute_raw("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
+await repo.execute("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
```

### Comparing `braincube-aws-core-alpha-0.0.26/README.md` & `braincube-aws-core-alpha-0.0.27/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,35 +144,35 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
+await repo.find_by_pk(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
-await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
+await repo.exists_by_pk(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
 await repo.find_all(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
-await repo.find_all_by_id([
+await repo.find_all_by_pk([
     Key("9448a57b-f686-4935-b152-566baab712db"),
     Key("43c8ec37-9a59-44eb-be90-def391ba2f02")],
     aliases=request.query_parameters.fields,
     order=request.query_parameters.order)
 
-await repo.find_all_page(
+await repo.find_many(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     page=request.query_parameters.page,
     order=request.query_parameters.order)
 
 await repo.insert(
     data={
@@ -199,34 +199,34 @@
     data={
         "type": 1,
         "isin": 40,
     },
     conditions=request.query_parameters.conditions,
     returning_aliases=request.query_parameters.fields)
 
-await repo.update_by_id(
+await repo.update_by_pk(
     Key("9448a57b-f686-4935-b152-566baab712db"),
     data={
         "type": 1,
         "isin": 40,
     }, returning_aliases=[])
 
 await repo.delete(
     conditions=request.query_parameters.conditions,
     returning_aliases=["id", "name", "type"])
 
-await repo.delete_by_id(
+await repo.delete_by_pk(
     Key("9448a57b-f686-4935-b152-566baab712db"),
     returning_aliases=["id", "name", "type"])
 
-await repo.fetch_raw("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
+await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
-await repo.fetch_one_raw("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
+await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
-await repo.execute_raw("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
+await repo.execute("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
```

### Comparing `braincube-aws-core-alpha-0.0.26/setup.cfg` & `braincube-aws-core-alpha-0.0.27/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.26
+version = 0.0.27
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.26
+Version: 0.0.27
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -164,35 +164,35 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
+await repo.find_by_pk(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
-await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
+await repo.exists_by_pk(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
 await repo.find_all(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
-await repo.find_all_by_id([
+await repo.find_all_by_pk([
     Key("9448a57b-f686-4935-b152-566baab712db"),
     Key("43c8ec37-9a59-44eb-be90-def391ba2f02")],
     aliases=request.query_parameters.fields,
     order=request.query_parameters.order)
 
-await repo.find_all_page(
+await repo.find_many(
     aliases=request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     page=request.query_parameters.page,
     order=request.query_parameters.order)
 
 await repo.insert(
     data={
@@ -219,34 +219,34 @@
     data={
         "type": 1,
         "isin": 40,
     },
     conditions=request.query_parameters.conditions,
     returning_aliases=request.query_parameters.fields)
 
-await repo.update_by_id(
+await repo.update_by_pk(
     Key("9448a57b-f686-4935-b152-566baab712db"),
     data={
         "type": 1,
         "isin": 40,
     }, returning_aliases=[])
 
 await repo.delete(
     conditions=request.query_parameters.conditions,
     returning_aliases=["id", "name", "type"])
 
-await repo.delete_by_id(
+await repo.delete_by_pk(
     Key("9448a57b-f686-4935-b152-566baab712db"),
     returning_aliases=["id", "name", "type"])
 
-await repo.fetch_raw("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
+await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
-await repo.fetch_one_raw("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
+await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
-await repo.execute_raw("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
+await repo.execute("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
```

### Comparing `braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/braincube_aws_core_alpha.egg-info/top_level.txt
 src/core/__init__.py
 src/core/dal/__init__.py
 src/core/dal/data.py
 src/core/dal/database_errors.py
 src/core/dal/postgres_connection.py
 src/core/dal/postgres_repository.py
+src/core/dal/transaction_manager.py
 src/core/di/__init__.py
 src/core/di/data.py
 src/core/di/injector.py
 src/core/rest/__init__.py
 src/core/rest/app_controller.py
 src/core/rest/app_module.py
 src/core/rest/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.27/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,25 @@
                              min_size=min_size, max_size=max_size,
                              max_inactive_connection_lifetime=max_inactive_connection_lifetime,
                              init=__init)
 
 
 @asynccontextmanager
 async def transactional(pool: Pool = None, connection: Connection = None):
-    """Create a database transaction. If connection is provided then a transaction is created immediately, if not then
-    a transaction established using a connection acquired from provided connection pool.
+    """Create a database transaction conditionally. If connection is provided then this
+    connection is returned immediately without creating any transaction, if not then a
+    transaction is established using a connection acquired from provided connection pool.
     :param pool: (asyncpg) Connection pool.
     :param connection: (asyncpg) Connection.
     :raise DatabaseError: If nor connection neither connection pool are specified.
     :return: Transactional connection.
     """
 
     if connection:
-        async with connection.transaction():
-            yield connection
+        yield connection
     elif pool:
         async with pool.acquire() as connection, connection.transaction():
             yield connection
     else:
         raise DatabaseError("nor connection neither connection pool are specified")
```

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,119 +297,42 @@
                            count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
 
         fields = self._aliases_to_fields(aliases)
         order_ = self._order_to_fields(order) if order else (self._order_by if set_order else None)
 
         return self.__init_select_query(fields, criterion, order_, count_query)
 
+    ####################################
+    # Retrieve
+    ####################################
+
     async def _find_one(self, aliases: list[str] = None,
                         criterion: Criterion = None,
                         order: list[Order] = None,
                         connection: Connection = None) -> dict[str, any] | None:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch_one(q.limit(1), connection=connection)
 
-    async def _find_all(self, aliases: list[str] = None,
-                        criterion: Criterion = None,
-                        order: list[Order] = None,
-                        connection: Connection = None) -> list[dict[str, any]]:
-
-        q, _ = self._init_select_query(aliases, criterion, order)
-
-        return await self._fetch(q, connection=connection)
-
-    async def _find_many(self, aliases: list[str] = None,
-                         criterion: Criterion = None,
-                         page: Pageable = Pageable(),
-                         order: list[Order] = None,
-                         connection: Connection = None) -> Page | Top:
-
-        if connection:
-            return await self.__find_many(connection, aliases, criterion, page, order)
-        async with self._pool.acquire() as connection_:
-            return await self.__find_many(connection_, aliases, criterion, page, order)
-
-    async def __find_many(self, connection: Connection,
-                          aliases: list[str] = None,
-                          criterion: Criterion = None,
-                          page: Pageable = Pageable(),
-                          order: list[Order] = None) -> Page | Top:
-
-        if page.top_size < 0:
-            data = await self._find_all(aliases, criterion, order, connection)
-            return Top(data, page.top_size, False)
-
-        start = time.time()
-
-        calc_top = page.top_size > 0
-        q, cq = self._init_select_query(aliases, criterion, order, count_query=not calc_top)
-
-        # top implementation
-        if calc_top:
-            records = await self._fetch(q.limit(page.top_size + 1), connection=connection)
-            has_more = len(records) > page.top_size
-            return Top(records[:-1] if has_more else records, page.top_size, has_more)
-
-        # paging implementation
-        page_no = page.page_no if page.page_no > 0 else 1
-        records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
-                                    connection=connection)
-
-        # retrieve count only if we do not mention page ether we are not on
-        # first page and there are no records from first retrieve
-        count = None
-        total_pages = None
-        retrieve_pre_page = len(records) == 0 and page.page_no > 1
-
-        if retrieve_pre_page or page.page_no == 0:
-            record = await self._fetch_one(cq, connection=connection)
-            count = record["count"] if record.get("count") else 0
-            total_pages = math.ceil(count / page.page_size)
-
-        if retrieve_pre_page and total_pages > 0:
-            page_no = total_pages
-            records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
-                                        connection=connection)
-
-        return Page(records, Paging(page_no, page.page_size, total_pages, count),
-                    Metadata(int((time.time() - start) * 1000)))
-
-    async def _update(self, data: BaseModel | dict[str, any],
-                      criterion: Criterion,
-                      returning_aliases: list[str] = None,
-                      connection: Connection = None) -> list[dict[str, any]] | None:
-
-        if isinstance(criterion, EmptyCriterion):
-            raise SaveError("update without conditions is not allowed")
-
-        uq = PostgreSQLQuery.update(self._master_table.name)
-
-        data_ = data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy()
-
-        for v, k in self._filter_save_data(data_, SaveType.update).items():
-            uq = uq.set(v, k)
-        uq = uq.where(criterion)
-
-        return await self._execute(uq, returning_aliases, connection)
-
-    async def _delete(self, criterion: Criterion,
-                      returning_aliases: list[str] = None,
-                      connection: Connection = None) -> list[dict[str, any]] | None:
-
-        if isinstance(criterion, EmptyCriterion):
-            raise DeleteError("delete without conditions is not allowed")
+    async def find_one(self, aliases: list[str] = None,
+                       conditions: list[Condition] = None,
+                       order: list[Order] = None,
+                       connection: Connection = None) -> dict[str, any] | None:
+        """Find one record from passed filters.
+        :param aliases: List of fields that will be selected by the query.
+        :param conditions: List of filters that will be applied to query.
+        :param order: Order that will be applied to query.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Record as dictionary.
+        """
 
-        dq = PostgreSQLQuery \
-            .from_(self._master_table.name) \
-            .delete() \
-            .where(criterion)
+        criterion = self._conditions_to_criterion(conditions)
 
-        return await self._execute(dq, returning_aliases, connection)
+        return await self._find_one(aliases, criterion, order, connection)
 
     async def find_by_pk(self, key: Key,
                          aliases: list[str] = None,
                          connection: Connection = None) -> dict[str, any] | None:
         """Find the record from passed key.
         :param key: Record identifier.
         :param aliases: List of fields that will be selected by the query.
@@ -430,29 +353,22 @@
         :return: Record existence.
         """
 
         aliases = [pk.field.alias for pk in self._primary_key.values()]
 
         return await self.find_by_pk(key, aliases, connection) is not None
 
-    async def find_one(self, aliases: list[str] = None,
-                       conditions: list[Condition] = None,
-                       order: list[Order] = None,
-                       connection: Connection = None) -> dict[str, any] | None:
-        """Find one record from passed filters.
-        :param aliases: List of fields that will be selected by the query.
-        :param conditions: List of filters that will be applied to query.
-        :param order: Order that will be applied to query.
-        :param connection: (asyncpg) Connection that will execute the generated query.
-        :return: Record as dictionary.
-        """
+    async def _find_all(self, aliases: list[str] = None,
+                        criterion: Criterion = None,
+                        order: list[Order] = None,
+                        connection: Connection = None) -> list[dict[str, any]]:
 
-        criterion = self._conditions_to_criterion(conditions)
+        q, _ = self._init_select_query(aliases, criterion, order)
 
-        return await self._find_one(aliases, criterion, order, connection)
+        return await self._fetch(q, connection=connection)
 
     async def find_all(self, aliases: list[str] = None,
                        conditions: list[Condition] = None,
                        order: list[Order] = None,
                        connection: Connection = None) -> list[dict[str, any]]:
         """Find all records from passed filters.
         :param aliases: List of fields that will be selected by the query.
@@ -481,14 +397,70 @@
         if not keys:
             raise DatabaseError("no keys provided")
 
         criterion = Criterion.any([self._create_primary_key_criterion(key) for key in keys])
 
         return await self._find_all(aliases, criterion, order, connection)
 
+    async def __find_many(self, connection: Connection,
+                          aliases: list[str] = None,
+                          criterion: Criterion = None,
+                          page: Pageable = Pageable(),
+                          order: list[Order] = None) -> Page | Top:
+
+        if page.top_size < 0:
+            data = await self._find_all(aliases, criterion, order, connection)
+            return Top(data, page.top_size, False)
+
+        start = time.time()
+
+        calc_top = page.top_size > 0
+        q, cq = self._init_select_query(aliases, criterion, order, count_query=not calc_top)
+
+        # top implementation
+        if calc_top:
+            records = await self._fetch(q.limit(page.top_size + 1), connection=connection)
+            has_more = len(records) > page.top_size
+            return Top(records[:-1] if has_more else records, page.top_size, has_more)
+
+        # paging implementation
+        page_no = page.page_no if page.page_no > 0 else 1
+        records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
+                                    connection=connection)
+
+        # retrieve count only if we do not mention page ether we are not on
+        # first page and there are no records from first retrieve
+        count = None
+        total_pages = None
+        retrieve_pre_page = len(records) == 0 and page.page_no > 1
+
+        if retrieve_pre_page or page.page_no == 0:
+            record = await self._fetch_one(cq, connection=connection)
+            count = record["count"] if record.get("count") else 0
+            total_pages = math.ceil(count / page.page_size)
+
+        if retrieve_pre_page and total_pages > 0:
+            page_no = total_pages
+            records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
+                                        connection=connection)
+
+        return Page(records, Paging(page_no, page.page_size, total_pages, count),
+                    Metadata(int((time.time() - start) * 1000)))
+
+    async def _find_many(self, aliases: list[str] = None,
+                         criterion: Criterion = None,
+                         page: Pageable = Pageable(),
+                         order: list[Order] = None,
+                         connection: Connection = None) -> Page | Top:
+
+        if connection:
+            return await self.__find_many(connection, aliases, criterion, page, order)
+        async with self._pool.acquire() as connection_:
+            return await self.__find_many(connection_, aliases, criterion, page, order)
+
     async def find_many(self, aliases: list[str] = None,
                         conditions: list[Condition] = None,
                         page: Pageable = Pageable(),
                         order: list[Order] = None,
                         connection: Connection = None) -> Page | Top:
         """Find records from passed filters using paging.
         :param aliases: List of fields that will be selected by the query.
@@ -499,14 +471,18 @@
         :return: Records wrapped by Page or Top dataclass.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_many(aliases, criterion, page, order, connection)
 
+    ####################################
+    # Create
+    ####################################
+
     async def insert(self, data: BaseModel | dict[str, any],
                      returning_aliases: list[str] = None,
                      connection: Connection = None) -> dict[str, any]:
         """Insert one record from dictionary.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
@@ -588,14 +564,36 @@
             .columns(list(column_names.keys()))
 
         for d in data:
             iq = iq.insert([d[i] for i in column_names.values()])
 
         return await self._execute(iq, returning_aliases, connection)
 
+    ####################################
+    # Update
+    ####################################
+
+    async def _update(self, data: BaseModel | dict[str, any],
+                      criterion: Criterion,
+                      returning_aliases: list[str] = None,
+                      connection: Connection = None) -> list[dict[str, any]] | None:
+
+        if isinstance(criterion, EmptyCriterion):
+            raise SaveError("update without conditions is not allowed")
+
+        uq = PostgreSQLQuery.update(self._master_table.name)
+
+        data_ = data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy()
+
+        for v, k in self._filter_save_data(data_, SaveType.update).items():
+            uq = uq.set(v, k)
+        uq = uq.where(criterion)
+
+        return await self._execute(uq, returning_aliases, connection)
+
     async def update(self, data: BaseModel | dict[str, any],
                      conditions: list[Condition],
                      returning_aliases: list[str] = None,
                      connection: Connection = None) -> list[dict[str, any]] | None:
         """Update records with new data according conditions.
         :param data: Master column aliases with values.
         :param conditions: List of filters that will be applied into the query.
@@ -605,14 +603,33 @@
         :return: Execution results as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._update(data, criterion, returning_aliases, connection)
 
+    # _update_data: criterion: Criterion
+
+    async def update_data(self, data: BaseModel | dict[str, any],
+                          conditions: list[Condition],
+                          returning: type[T],
+                          connection: Connection = None) -> list[T] | None:
+        """Update records with new data according conditions using model.
+        :param data: Model which contains master table column properties.
+        :param conditions: List of filters that will be applied into the query.
+        :param returning: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
+        :return: Execution results with returning type.
+        """
+
+        results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
+
+        return [returning(**r) for r in results] if results else None
+
     async def update_by_pk(self, key: Key,
                            data: BaseModel | dict[str, any],
                            returning_aliases: list[str] = None,
                            connection: Connection = None) -> dict[str, any] | None:
         """Update record with new data according to passed key.
         :param key: Record identifier.
         :param data: Master column aliases with values.
@@ -624,31 +641,14 @@
 
         criterion = self._create_primary_key_criterion(key, select=False)
 
         records = await self._update(data, criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
-    async def update_data(self, data: BaseModel | dict[str, any],
-                          conditions: list[Condition],
-                          returning: type[T],
-                          connection: Connection = None) -> list[T] | None:
-        """Update records with new data according conditions using model.
-        :param data: Model which contains master table column properties.
-        :param conditions: List of filters that will be applied into the query.
-        :param returning: Result type.
-        :param connection: (asyncpg) Connection that will execute the generated query.
-        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
-        :return: Execution results with returning type.
-        """
-
-        results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
-
-        return [returning(**r) for r in results] if results else None
-
     async def update_data_by_pk(self, key: Key,
                                 data: BaseModel | dict[str, any],
                                 returning: type[T],
                                 connection: Connection = None) -> T | None:
         """Update record with new data according to passed key using model.
         :param key: Record identifier.
         :param data: Model which contains master table column properties.
@@ -658,14 +658,32 @@
         :return: Execution result with returning type.
         """
 
         result = await self.update_by_pk(key, data, self.__base_model_aliases(returning), connection)
 
         return returning(**result) if result else None
 
+    ####################################
+    # Delete
+    ####################################
+
+    async def _delete(self, criterion: Criterion,
+                      returning_aliases: list[str] = None,
+                      connection: Connection = None) -> list[dict[str, any]] | None:
+
+        if isinstance(criterion, EmptyCriterion):
+            raise DeleteError("delete without conditions is not allowed")
+
+        dq = PostgreSQLQuery \
+            .from_(self._master_table.name) \
+            .delete() \
+            .where(criterion)
+
+        return await self._execute(dq, returning_aliases, connection)
+
     async def delete(self, conditions: list[Condition],
                      returning_aliases: list[str] = None,
                      connection: Connection = None) -> list[dict[str, any]] | None:
         """Delete records according conditions.
         :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
```

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.27/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.27/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.27/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.27/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.27/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.27/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.26/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.27/src/core/utils/data.py`

 * *Files identical despite different names*


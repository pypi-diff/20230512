# Comparing `tmp/pm_food_lib-0.2.4.tar.gz` & `tmp/pm_food_lib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm_food_lib-0.2.4.tar", max compression
+gzip compressed data, was "pm_food_lib-0.2.5.tar", max compression
```

## Comparing `pm_food_lib-0.2.4.tar` & `pm_food_lib-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       15 2023-05-11 09:45:34.366566 pm_food_lib-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.366566 pm_food_lib-0.2.4/pm-food-lib/__init__.py
--rw-r--r--   0        0        0     5968 2023-05-11 09:45:34.366566 pm_food_lib-0.2.4/pm-food-lib/db/LogDbBase.py
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.366566 pm_food_lib-0.2.4/pm-food-lib/db/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-11 09:45:34.366566 pm_food_lib-0.2.4/pm-food-lib/db/dynamo_db_base_class.py
--rw-r--r--   0        0        0    16370 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/db/sql_db_base_class.py
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/mail/__init__.py
--rw-r--r--   0        0        0     3539 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/mail/aws_ses.py
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/__init__.py
--rw-r--r--   0        0        0     7709 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/PM.py
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/__init__.py
--rw-r--r--   0        0        0     5369 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/error_codes.py
--rw-r--r--   0        0        0      113 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/log_levels.py
--rw-r--r--   0        0        0      525 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/parameters.py
--rw-r--r--   0        0        0     1101 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/platforms.py
--rw-r--r--   0        0        0      374 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/constants/products.py
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/formats/__init__.py
--rw-r--r--   0        0        0     7173 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/formats/order.py
--rw-r--r--   0        0        0        0 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/functions/__init__.py
--rw-r--r--   0        0        0    22794 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/functions/general.py
--rw-r--r--   0        0        0     2785 2023-05-11 09:45:34.370566 pm_food_lib-0.2.4/pm-food-lib/utils/functions/regions.py
--rw-r--r--   0        0        0     1417 2023-05-11 09:45:59.914735 pm_food_lib-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 pm_food_lib-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/__init__.py
+-rw-r--r--   0        0        0     5968 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/db/LogDbBase.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/db/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/db/dynamo_db_base_class.py
+-rw-r--r--   0        0        0    16370 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/db/sql_db_base_class.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/mail/__init__.py
+-rw-r--r--   0        0        0     3539 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/mail/aws_ses.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/__init__.py
+-rw-r--r--   0        0        0     7709 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/PM.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/__init__.py
+-rw-r--r--   0        0        0     5369 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/error_codes.py
+-rw-r--r--   0        0        0      113 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/log_levels.py
+-rw-r--r--   0        0        0      525 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/parameters.py
+-rw-r--r--   0        0        0     1101 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/platforms.py
+-rw-r--r--   0        0        0      374 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/constants/products.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/formats/__init__.py
+-rw-r--r--   0        0        0     7173 2023-05-12 08:26:38.501434 pm_food_lib-0.2.5/pm-food-lib/utils/formats/order.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:26:38.505434 pm_food_lib-0.2.5/pm-food-lib/utils/functions/__init__.py
+-rw-r--r--   0        0        0    22794 2023-05-12 08:26:38.505434 pm_food_lib-0.2.5/pm-food-lib/utils/functions/general.py
+-rw-r--r--   0        0        0     2785 2023-05-12 08:26:38.505434 pm_food_lib-0.2.5/pm-food-lib/utils/functions/regions.py
+-rw-r--r--   0        0        0     1397 2023-05-12 08:27:13.441808 pm_food_lib-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 pm_food_lib-0.2.5/PKG-INFO
```

### Comparing `pm_food_lib-0.2.4/pm-food-lib/db/LogDbBase.py` & `pm_food_lib-0.2.5/pm-food-lib/db/LogDbBase.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/db/dynamo_db_base_class.py` & `pm_food_lib-0.2.5/pm-food-lib/db/dynamo_db_base_class.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/db/sql_db_base_class.py` & `pm_food_lib-0.2.5/pm-food-lib/db/sql_db_base_class.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/mail/aws_ses.py` & `pm_food_lib-0.2.5/pm-food-lib/mail/aws_ses.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/constants/PM.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/constants/PM.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/constants/error_codes.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/constants/error_codes.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/constants/parameters.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/constants/parameters.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/constants/platforms.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/constants/platforms.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/formats/order.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/formats/order.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/functions/general.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/functions/general.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pm-food-lib/utils/functions/regions.py` & `pm_food_lib-0.2.5/pm-food-lib/utils/functions/regions.py`

 * *Files identical despite different names*

### Comparing `pm_food_lib-0.2.4/pyproject.toml` & `pm_food_lib-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pm-food-lib"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Yasin Beyazlı <89048757+ysnbyzli@users.noreply.github.com>"]
 readme = "README.md"
 packages = [
     { include = "pm-food-lib" },
 ]
 
@@ -26,24 +26,23 @@
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = true                       # don't auto-upload to PyPI
 remove_dist = true                          # don't remove dists
 patch_without_tag = true                    # patch release by default
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python="^3.7"
 requests = "^2.28.2"
 boto3 = "^1.26.115"
 uuid = "^1.30"
 datetime = "^5.1"
 slugify = "^0.0.1"
 pyjwt = "^2.6.0"
 beartype = "^0.13.1"
 flask = "^2.2.3"
-flake8 = "^6.0.0"
 iso8601="^1.1.0"
 mysql-connector="^2.2.9"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.971"
 black = "^22.8.0"
 python-semantic-release = "^7.32.1"
```

### Comparing `pm_food_lib-0.2.4/PKG-INFO` & `pm_food_lib-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pm-food-lib
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Yasin Beyazlı
 Author-email: 89048757+ysnbyzli@users.noreply.github.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beartype (>=0.13.1,<0.14.0)
 Requires-Dist: boto3 (>=1.26.115,<2.0.0)
 Requires-Dist: datetime (>=5.1,<6.0)
-Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: iso8601 (>=1.1.0,<2.0.0)
 Requires-Dist: mysql-connector (>=2.2.9,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: slugify (>=0.0.1,<0.0.2)
 Requires-Dist: uuid (>=1.30,<2.0)
```


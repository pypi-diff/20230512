# Comparing `tmp/dbt-impala-1.3.1.tar.gz` & `tmp/dbt-impala-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-impala-1.3.1.tar", last modified: Sat Dec  3 14:42:32 2022, max compression
+gzip compressed data, was "dbt-impala-1.3.2.tar", last modified: Thu May 11 04:58:01 2023, max compression
```

## Comparing `dbt-impala-1.3.1.tar` & `dbt-impala-1.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.964269 dbt-impala-1.3.1/
--rw-r--r--   0 jenkins   (1001) users      (100)    10837 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)       83 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) users      (100)     1861 2022-12-03 14:42:32.963269 dbt-impala-1.3.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1243 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.954270 dbt-impala-1.3.1/dbt/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.954270 dbt-impala-1.3.1/dbt/adapters/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.957270 dbt-impala-1.3.1/dbt/adapters/impala/
--rw-------   0 jenkins   (1001) users      (100)      227 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt/adapters/impala/.env
--rw-r--r--   0 jenkins   (1001) users      (100)     1069 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      594 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/__version__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     8422 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/cloudera_tracking.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2840 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/column.py
--rw-r--r--   0 jenkins   (1001) users      (100)    14843 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/connections.py
--rw-r--r--   0 jenkins   (1001) users      (100)    14704 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/impl.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2329 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/adapters/impala/relation.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.954270 dbt-impala-1.3.1/dbt/include/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.958269 dbt-impala-1.3.1/dbt/include/impala/
--rw-r--r--   0 jenkins   (1001) users      (100)      629 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      651 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/dbt_project.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.959269 dbt-impala-1.3.1/dbt/include/impala/macros/
--rw-r--r--   0 jenkins   (1001) users      (100)    15044 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/adapters.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1591 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/apply_grants.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      678 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/catalog.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     6289 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/incremental.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2837 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/insertoverwrite.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1877 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/seed.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.962269 dbt-impala-1.3.1/dbt/include/impala/macros/utils/
--rw-r--r--   0 jenkins   (1001) users      (100)      721 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/any_value.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      157 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/array_append.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      155 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/array_concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      159 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/array_construct.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      751 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/bool_or.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      672 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      750 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/dateadd.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     5905 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/datediff.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      695 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      825 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/hash.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1211 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/last_day.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1106 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/listagg.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      727 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/position.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      863 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/split_part.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      665 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/macros/utils/timestamps.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      779 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/dbt/include/impala/sample_profiles.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2022-12-03 14:42:32.963269 dbt-impala-1.3.1/dbt_impala.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)     1861 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt_impala.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1544 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt_impala.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt_impala.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt_impala.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) users      (100)       66 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt_impala.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        4 2022-12-03 14:42:32.000000 dbt-impala-1.3.1/dbt_impala.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       38 2022-12-03 14:42:32.964269 dbt-impala-1.3.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)     3039 2022-12-03 14:42:06.000000 dbt-impala-1.3.1/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/
+-rw-r--r--   0 jenkins   (1001) users      (100)    10837 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)       83 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) users      (100)     3101 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     2433 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.625726 dbt-impala-1.3.2/dbt/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.625726 dbt-impala-1.3.2/dbt/adapters/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.629726 dbt-impala-1.3.2/dbt/adapters/impala/
+-rw-------   0 jenkins   (1001) users      (100)      227 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt/adapters/impala/.env
+-rw-r--r--   0 jenkins   (1001) users      (100)     1062 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      596 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/__version__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     8443 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/cloudera_tracking.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2771 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/column.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15342 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/connections.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15388 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/impl.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2406 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/relation.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.625726 dbt-impala-1.3.2/dbt/include/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.629726 dbt-impala-1.3.2/dbt/include/impala/
+-rw-r--r--   0 jenkins   (1001) users      (100)      630 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      651 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/dbt_project.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.633726 dbt-impala-1.3.2/dbt/include/impala/macros/
+-rw-r--r--   0 jenkins   (1001) users      (100)    15268 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/adapters.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1591 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/apply_grants.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      676 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/catalog.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     6282 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/incremental.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1899 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/insertoverwrite.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1877 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/seed.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.633726 dbt-impala-1.3.2/dbt/include/impala/macros/utils/
+-rw-r--r--   0 jenkins   (1001) users      (100)      721 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/any_value.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      157 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/array_append.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      155 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/array_concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      159 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/array_construct.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      751 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/bool_or.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      672 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      750 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/dateadd.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     5905 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/datediff.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      696 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      825 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/hash.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1208 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/last_day.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1106 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/listagg.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      727 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/position.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      863 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/split_part.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      665 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/timestamps.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      779 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/sample_profiles.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/dbt_impala.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)     3101 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1544 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) users      (100)       50 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        4 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       38 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)     3118 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/setup.py
```

### Comparing `dbt-impala-1.3.1/LICENSE` & `dbt-impala-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/__init__.py` & `dbt-impala-1.3.2/dbt/adapters/impala/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,10 +19,9 @@
 from dbt.adapters.impala.impl import ImpalaAdapter
 
 from dbt.adapters.base import AdapterPlugin
 from dbt.include import impala
 
 
 Plugin = AdapterPlugin(
-    adapter=ImpalaAdapter,
-    credentials=ImpalaCredentials,
-    include_path=impala.PACKAGE_PATH)
+    adapter=ImpalaAdapter, credentials=ImpalaCredentials, include_path=impala.PACKAGE_PATH
+)
```

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/__version__.py` & `dbt-impala-1.3.2/dbt/adapters/impala/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version="1.3.1"
+version = "1.3.2"
```

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/cloudera_tracking.py` & `dbt-impala-1.3.2/dbt/adapters/impala/cloudera_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,26 @@
 import threading
 from dbt.tracking import active_user
 
 from dbt.adapters.base import Credentials
 from dbt.events import AdapterLogger
 from decouple import config
 
+
 # all event types
 class TrackingEventType:
     DEBUG = "debug_and_fetch_permission"
     OPEN = "open"
     CLOSE = "close"
     START_QUERY = "start_query"
     END_QUERY = "end_query"
     INCREMENTAL = "incremental"
     MODEL_ACCESS = "model_access"
 
+
 # global logger
 logger = AdapterLogger("Tracker")
 
 # global switch to turn on/off the usage tracking
 usage_tracking: bool = True
 
 # Json object to store OS and platform related information
@@ -52,15 +54,16 @@
 # Json object to store dbt profile(profile.yml) related information
 profile_info = {}
 
 # Json object to store dbt deployment environment variables
 dbt_deployment_env_info = {}
 
 # Json object for warehouse information
-warehouse_info = { "warehouse_version": { "version": "NA", "build": "NA" } }
+warehouse_info = {"warehouse_version": {"version": "NA", "build": "NA"}}
+
 
 def populate_platform_info(cred: Credentials, ver):
     """
     populate platform info to be passed on for tracking
     @param cred DBT cred object, representing the dbt profile
     @param ver DBT adapter version
     """
@@ -69,104 +72,113 @@
     # Underlying system e.g. : Linux, Darwin(Mac), Windows
     platform_info["system"] = platform.system()
     # Architecture e.g. x86_64 ,arm, AMD64
     platform_info["machine"] = platform.machine()
     # Full platform info e.g Linux-2.6.32-32-server-x86_64-with-Ubuntu-10.04-lucid,Windows-2008ServerR2-6.1.7601-SP1
     platform_info["platform"] = platform.platform()
     # dbt core version
-    platform_info[
-        "dbt_version"
-    ] = dbt.version.get_installed_version().to_version_string(skip_matcher=True)
+    platform_info["dbt_version"] = dbt.version.get_installed_version().to_version_string(
+        skip_matcher=True
+    )
     # dbt adapter info e.g. impala-1.2.0
     platform_info["dbt_adapter_type"] = f"{cred.type}"
     platform_info["dbt_adapter_version"] = f"{ver.version}"
 
+
 def populate_dbt_deployment_env_info():
     """
     populate dbt deployment environment variables if available to be passed on for tracking
     """
     default_value = "{}"  # if environment variables doesn't exist add empty json as default
-    dbt_deployment_env_info["dbt_deployment_env"] = json.loads(os.environ.get('DBT_DEPLOYMENT_ENV', default_value))
+    dbt_deployment_env_info["dbt_deployment_env"] = json.loads(
+        os.environ.get("DBT_DEPLOYMENT_ENV", default_value)
+    )
+
 
 def populate_unique_ids(cred: Credentials, userkey="username"):
     host = str(cred.host).encode()
     user = str(getattr(cred, userkey)).encode()
     timestamp = str(time.time()).encode()
 
     # dbt invocation id
     if active_user:
-       unique_ids["id"] = active_user.invocation_id
+        unique_ids["id"] = active_user.invocation_id
     else:
-       unique_ids["id"] = "N/A"
+        unique_ids["id"] = "N/A"
 
     # hashed host name
     unique_ids["unique_host_hash"] = hashlib.md5(host).hexdigest()
     # hashed username
     unique_ids["unique_user_hash"] = hashlib.md5(user).hexdigest()
     # hashed session
     unique_ids["unique_session_hash"] = hashlib.md5(host + user + timestamp).hexdigest()
 
+
 def generate_profile_info(self):
     if not profile_info:
         # name of dbt project in profiles
         profile_info["project_name"] = self.profile.profile_name
         # dbt target in profiles
         profile_info["target_name"] = self.profile.target_name
         # number of threads in profiles
         profile_info["no_of_threads"] = self.profile.threads
 
+
 def populate_warehouse_info(w_info):
     warehouse_info["warehouse_version"]["version"] = w_info["version"]
     warehouse_info["warehouse_version"]["build"] = w_info["build"]
 
+
 def _merge_keys(source_dict, dest_dict):
     for key, value in source_dict.items():
         dest_dict[key] = value
     return dest_dict
 
+
 def _get_sql_type(sql):
     if not sql:
         return ""
 
     words = sql.split("*/")
 
     if len(words) > 1:
         sql_words = words[1].strip().split()
     else:
         sql_words = words[0].strip().split()
 
-    sql_type = " ".join(sql_words[:min(2, len(sql_words))]).lower()
+    sql_type = " ".join(sql_words[: min(2, len(sql_words))]).lower()
 
     return sql_type
 
+
 def fix_tracking_payload(given_payload):
     """
     The payload for an event
     @param given_payload: Payload sent from events
     @return desired_payload: Payload in desired schema
     """
     desired_payload = {}
     # merge valid keys from source to desired payload first
     desired_payload = _merge_keys(given_payload, desired_payload)
 
     # handle sql redaction - convert to sql type from full sql statement
     if "sql" in desired_payload:
         desired_payload["sql_type"] = _get_sql_type(desired_payload["sql"])
         del desired_payload["sql"]
-   
+
     desired_keys = [
         "auth",
         "connection_state",
         "elapsed_time",
         "incremental_strategy",
         "model_name",
         "model_type",
         "permissions",
         "profile_name",
-        "sql_type"
+        "sql_type",
     ]
 
     for key in desired_keys:
         if key not in desired_payload:
             # indicate that the key doesn't have valid data for the event
             desired_payload[key] = "N/A"
 
@@ -184,15 +196,17 @@
             payload["unique_hash"] = hashlib.md5(credentials.host.encode()).hexdigest()
             payload["auth"] = auth_type
             payload["connection_state"] = connection.state
     """
 
     global usage_tracking
 
-    logger.debug(f"Usage tracking flag {usage_tracking}. To turn on/off use usage_tracking flag in profiles.yml")
+    logger.debug(
+        f"Usage tracking flag {usage_tracking}. To turn on/off use usage_tracking flag in profiles.yml"
+    )
 
     # if usage_tracking is disabled, quit
     if not usage_tracking:
         logger.debug(f"Skipping Event {tracking_payload}")
         return
 
     # fix the schema of tracking payload to be common for all events
@@ -243,11 +257,9 @@
             logger.debug(f"Usage tracking error. {err}")
             logger.debug("Disabling usage tracking due to error.")
             usage_tracking = False
 
         return res
 
     # call the tracking function in a Thread
-    the_track_thread = threading.Thread(
-        target=_tracking_func, kwargs={"data": tracking_data}
-    )
+    the_track_thread = threading.Thread(target=_tracking_func, kwargs={"data": tracking_data})
     the_track_thread.start()
```

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/column.py` & `dbt-impala-1.3.2/dbt/adapters/impala/column.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dataclasses import dataclass
 from typing import TypeVar, Optional, Dict, Any
 
 from dbt.adapters.base.column import Column
 from dbt.dataclass_schema import dbtClassMixin
 from hologram import JsonDict
 
-Self = TypeVar('Self', bound='ImpalaColumn')
+Self = TypeVar("Self", bound="ImpalaColumn")
 
 
 @dataclass
 class ImpalaColumn(dbtClassMixin, Column):
     table_database: Optional[str] = None
     table_schema: Optional[str] = None
     table_name: Optional[str] = None
@@ -37,46 +37,43 @@
         return dtype
 
     def can_expand_to(self: Self, other_column: Self) -> bool:
         """returns True if both columns are strings"""
         return self.is_string() and other_column.is_string()
 
     def literal(self, value):
-        return "cast({} as {})".format(value, self.dtype)
+        return f"cast({value} as {self.dtype})"
 
     @property
     def quoted(self) -> str:
-        return '"{}"'.format(self.column)
+        return f'"{self.column}"'
 
     @property
     def data_type(self) -> str:
         return self.dtype
 
     def __repr__(self) -> str:
-        return "<ImpalaColumn {} ({})>".format(self.name, self.data_type)
+        return f"<ImpalaColumn {self.name} ({self.data_type})>"
 
     @staticmethod
     def convert_table_stats(raw_stats: Optional[str]) -> Dict[str, Any]:
         table_stats = {}
         if raw_stats:
             # format: 1109049927 bytes, 14093476 rows
             stats = {
-                stats.split(" ")[1]: int(stats.split(" ")[0])
-                for stats in raw_stats.split(', ')
+                stats.split(" ")[1]: int(stats.split(" ")[0]) for stats in raw_stats.split(", ")
             }
             for key, val in stats.items():
-                table_stats[f'stats:{key}:label'] = key
-                table_stats[f'stats:{key}:value'] = val
-                table_stats[f'stats:{key}:description'] = ''
-                table_stats[f'stats:{key}:include'] = True
+                table_stats[f"stats:{key}:label"] = key
+                table_stats[f"stats:{key}:value"] = val
+                table_stats[f"stats:{key}:description"] = ""
+                table_stats[f"stats:{key}:include"] = True
         return table_stats
 
-    def to_column_dict(
-            self, omit_none: bool = True, validate: bool = False
-    ) -> JsonDict:
+    def to_column_dict(self, omit_none: bool = True, validate: bool = False) -> JsonDict:
         original_dict = self.to_dict(omit_none=omit_none)
-       
+
         # If there are stats, merge them into the root of the dict
-        original_stats = original_dict.pop('table_stats', None)
+        original_stats = original_dict.pop("table_stats", None)
         if original_stats:
             original_dict.update(original_stats)
         return original_dict
```

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/connections.py` & `dbt-impala-1.3.2/dbt/adapters/impala/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 DEFAULT_IMPALA_HOST = "localhost"
 DEFAULT_IMPALA_PORT = 21050
 DEFAULT_MAX_RETRIES = 3
 
 logger = AdapterLogger("Impala")
 
+
 @dataclass
 class ImpalaCredentials(Credentials):
     host: str = DEFAULT_IMPALA_HOST
     schema: str = None
     database: Optional[str] = None
     port: Optional[int] = DEFAULT_IMPALA_PORT
     username: Optional[str] = None
@@ -104,38 +105,39 @@
         return "host", "port", "schema", "username"
 
     @property
     def unique_field(self) -> str:
         # adapter anonymous adoption
         return self.host
 
-class ImpalaConnectionWrapper(object):
+
+class ImpalaConnectionWrapper:
     def __init__(self, handle):
         self.handle = handle
         self._cursor = self.handle.cursor()
 
     def cursor(self):
         if not self._cursor:
             self._cursor = self.handle.cursor()
         return self
 
     def cancel(self):
         if self._cursor:
             try:
                 self._cursor.cancel()
-            except EnvironmentError as exc:
-                logger.debug("Exception while cancelling query: {}".format(exc))
+            except OSError as exc:
+                logger.debug(f"Exception while cancelling query: {exc}")
 
     def close(self):
         if self._cursor:
             try:
                 self._cursor.close()
                 self._cursor = None
-            except EnvironmentError as exc:
-                logger.debug("Exception while closing cursor: {}".format(exc))
+            except OSError as exc:
+                logger.debug(f"Exception while closing cursor: {exc}")
 
     def rollback(self, *args, **kwargs):
         logger.debug("NotImplemented: rollback")
 
     def fetchall(self):
         return self._cursor.fetchall()
 
@@ -146,14 +148,15 @@
         result = self._cursor.execute(sql, bindings, configuration)
         return result
 
     @property
     def description(self):
         return self._cursor.description
 
+
 class ImpalaConnectionManager(SQLConnectionManager):
     TYPE = "impala"
 
     impala_version = None
 
     def __init__(self, profile: AdapterRequiredConfig):
         super().__init__(profile)
@@ -161,24 +164,28 @@
         tracker.generate_profile_info(self)
 
     @contextmanager
     def exception_handler(self, sql: str):
         try:
             yield
         except HttpError as httpError:
-            logger.debug("Authorization error: {}".format(httpError))
-            raise dbt.exceptions.RuntimeException ("HTTP Authorization error: " + str(httpError) + ", please check your credentials")
+            logger.debug(f"Authorization error: {httpError}")
+            raise dbt.exceptions.RuntimeException(
+                "HTTP Authorization error: " + str(httpError) + ", please check your credentials"
+            )
         except HiveServer2Error as servError:
-            logger.debug("Server connection error: {}".format(servError))
-            raise dbt.exceptions.RuntimeException ("Unable to establish connection to Impala server: " + str(servError))
+            logger.debug(f"Server connection error: {servError}")
+            raise dbt.exceptions.RuntimeException(
+                "Unable to establish connection to Impala server: " + str(servError)
+            )
         except DatabaseError as dbError:
-            logger.debug("Database connection error: {}".format(str(dbError)))
+            logger.debug(f"Database connection error: {str(dbError)}")
             raise dbt.exceptions.DatabaseException("Database Connection error: " + str(dbError))
         except Exception as exc:
-            logger.debug("Error running SQL: {}".format(sql))
+            logger.debug(f"Error running SQL: {sql}")
             raise dbt.exceptions.RuntimeException(str(exc))
 
     @classmethod
     def open(cls, connection):
         if connection.state == ConnectionState.OPEN:
             logger.debug("Connection is already open, skipping open.")
             return connection
@@ -188,77 +195,88 @@
 
         auth_type = "insecure"
 
         try:
             connection_start_time = time.time()
             # the underlying dbapi supports retries, so this is directly used instead to support retries
             if (
-                    credentials.auth_type == "LDAP" or credentials.auth_type == "ldap"
+                credentials.auth_type == "LDAP" or credentials.auth_type == "ldap"
             ):  # ldap connection
-                custom_user_agent = 'dbt/cloudera-impala-v' + ADAPTER_VERSION
-                logger.debug("Using user agent: {}".format(custom_user_agent))
+                custom_user_agent = "dbt/cloudera-impala-v" + ADAPTER_VERSION
+                logger.debug(f"Using user agent: {custom_user_agent}")
                 handle = impala.dbapi.connect(
                     host=credentials.host,
                     port=credentials.port,
                     auth_mechanism="LDAP",
                     use_http_transport=credentials.use_http_transport,
                     user=credentials.username,
                     password=credentials.password,
                     use_ssl=credentials.use_ssl,
                     http_path=credentials.http_path,
                     retries=credentials.retries,
-                    user_agent=custom_user_agent
+                    user_agent=custom_user_agent,
                 )
                 auth_type = "ldap"
             elif (
-                    credentials.auth_type == "GSSAPI"
-                    or credentials.auth_type == "gssapi"
-                    or credentials.auth_type == "kerberos"
+                credentials.auth_type == "GSSAPI"
+                or credentials.auth_type == "gssapi"
+                or credentials.auth_type == "kerberos"
             ):  # kerberos based connection
                 handle = impala.dbapi.connect(
                     host=credentials.host,
                     port=credentials.port,
                     auth_mechanism="GSSAPI",
                     kerberos_service_name=credentials.kerberos_service_name,
                     use_http_transport=credentials.use_http_transport,
                     use_ssl=credentials.use_ssl,
                     retries=credentials.retries,
                 )
                 auth_type = "kerberos"
+            elif (
+                credentials.auth_type == "PLAIN" or credentials.auth_type == "plain"
+            ):  # plain type connection
+                handle = impala.dbapi.connect(
+                    host=credentials.host,
+                    port=credentials.port,
+                    auth_mechanism="PLAIN",
+                    use_ssl=credentials.use_ssl,
+                    user=credentials.username,
+                    password=credentials.password,
+                    retries=credentials.retries,
+                )
+                auth_type = "plain"
             else:  # default, insecure connection
                 handle = impala.dbapi.connect(
                     host=credentials.host,
                     port=credentials.port,
                     retries=credentials.retries,
                 )
             connection_end_time = time.time()
 
             connection.state = ConnectionState.OPEN
             connection.handle = ImpalaConnectionWrapper(handle)
 
             ImpalaConnectionManager.fetch_impala_version(connection.handle)
         except Exception as ex:
-            logger.debug("Connection error {}".format(ex))
+            logger.debug(f"Connection error {ex}")
             connection_ex = ex
             connection.state = ConnectionState.FAIL
             connection.handle = None
             connection_end_time = time.time()
 
         # track usage
         payload = {
             "event_type": tracker.TrackingEventType.OPEN,
             "auth": auth_type,
             "connection_state": connection.state,
-            "elapsed_time": "{:.2f}".format(
-                connection_end_time - connection_start_time
-            ),
+            "elapsed_time": f"{connection_end_time - connection_start_time:.2f}",
         }
 
         if connection.state == ConnectionState.FAIL:
-            payload["connection_exception"] = "{}".format(connection_ex)
+            payload["connection_exception"] = f"{connection_ex}"
 
         tracker.track_usage(payload)
 
         return connection
 
     @classmethod
     def close(cls, connection):
@@ -283,34 +301,37 @@
 
             return connection
         except Exception as err:
             logger.debug(f"Error closing connection {err}")
 
     @classmethod
     def fetch_impala_version(cls, connection):
-
-        if ImpalaConnectionManager.impala_version: 
+        if ImpalaConnectionManager.impala_version:
             return ImpalaConnectionManager.impala_version
 
         try:
             sql = "select version()"
             cursor = connection.cursor()
             cursor.execute(sql)
 
             res = cursor.fetchall()
 
             ImpalaConnectionManager.impala_version = res[0][0].split("RELEASE")[0].strip()
 
-            tracker.populate_warehouse_info({ "version": ImpalaConnectionManager.impala_version, "build": res[0][0] })
+            tracker.populate_warehouse_info(
+                {"version": ImpalaConnectionManager.impala_version, "build": res[0][0]}
+            )
         except Exception as ex:
             # we couldn't get the impala warehouse version
             logger.debug(f"Cannot get impala version. Error: {ex}")
             ImpalaConnectionManager.impala_version = "NA"
 
-            tracker.populate_warehouse_info({ "version": ImpalaConnectionManager.impala_version, "build": "NA" })
+            tracker.populate_warehouse_info(
+                {"version": ImpalaConnectionManager.impala_version, "build": "NA"}
+            )
 
         logger.debug(f"IMPALA VERSION {'ImpalaConnectionManager.impala_version'}")
 
     @classmethod
     def get_response(cls, cursor):
         message = "OK"
         return AdapterResponse(_message=message)
@@ -327,19 +348,19 @@
     def commit(self, *args, **kwargs):
         logger.debug("NotImplemented: commit")
 
     def rollback(self, *args, **kwargs):
         logger.debug("NotImplemented: rollback")
 
     def add_query(
-            self,
-            sql: str,
-            auto_begin: bool = True,
-            bindings: Optional[Any] = None,
-            abridge_sql_log: bool = False,
+        self,
+        sql: str,
+        auto_begin: bool = True,
+        bindings: Optional[Any] = None,
+        abridge_sql_log: bool = False,
     ) -> Tuple[Connection, Any]:
         connection = self.get_thread_connection()
         if auto_begin and connection.transaction_open is False:
             self.begin()
         fire_event(ConnectionUsed(conn_type=self.TYPE, conn_name=connection.name))
 
         additional_info = {}
@@ -348,23 +369,23 @@
                 additional_info = json.loads(self.query_header.comment.query_comment.strip())
             except Exception as ex:  # silently ignore error for parsing
                 additional_info = {}
                 logger.debug(f"Unable to get query header {ex}")
 
         with self.exception_handler(sql):
             if abridge_sql_log:
-                log_sql = "{}...".format(sql[:512])
+                log_sql = f"{sql[:512]}..."
             else:
                 log_sql = sql
 
             # track usage
             payload = {
                 "event_type": tracker.TrackingEventType.START_QUERY,
                 "sql": log_sql,
-                "profile_name": self.profile.profile_name
+                "profile_name": self.profile.profile_name,
             }
 
             for key, value in additional_info.items():
                 if key == "node_id":
                     payload["model_name"] = value
                 else:
                     payload[key] = value
@@ -389,23 +410,23 @@
                 query_exception = ex
 
             elapsed_time = time.time() - pre
 
             payload = {
                 "event_type": tracker.TrackingEventType.END_QUERY,
                 "sql": log_sql,
-                "elapsed_time": "{:.2f}".format(elapsed_time),
+                "elapsed_time": f"{elapsed_time:.2f}",
                 "status": query_status,
-                "profile_name": self.profile.profile_name
+                "profile_name": self.profile.profile_name,
             }
 
             tracker.track_usage(payload)
 
             # re-raise query exception so that it propogates to dbt
-            if (query_exception):
+            if query_exception:
                 raise query_exception
 
             fire_event(
                 SQLQueryStatus(
                     status=query_status,
                     elapsed=round(elapsed_time, 2),
                 )
```

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/impl.py` & `dbt-impala-1.3.2/dbt/adapters/impala/impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import re
 from collections import OrderedDict
-from concurrent.futures import Future, as_completed
-from typing import Any, Dict, Iterable, List, Tuple
+from concurrent.futures import Future
+from typing import Any, Dict, Iterable, List
 
 import agate
 import dbt.exceptions
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.adapters.sql import SQLAdapter
 from dbt.clients import agate_helper
 from dbt.clients.agate_helper import ColumnTypeBuilder, NullableAgateType, _NullMarker
@@ -31,39 +30,36 @@
 import dbt.adapters.impala.cloudera_tracking as tracker
 from dbt.adapters.impala import ImpalaConnectionManager
 from dbt.adapters.impala.column import ImpalaColumn
 from dbt.adapters.impala.relation import ImpalaRelation
 
 logger = AdapterLogger("Impala")
 
-LIST_SCHEMAS_MACRO_NAME = 'list_schemas'
-LIST_RELATIONS_MACRO_NAME = 'list_relations_without_caching'
+LIST_SCHEMAS_MACRO_NAME = "list_schemas"
+LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
+
+KEY_TABLE_OWNER = "Owner"
+KEY_TABLE_STATISTICS = "Statistics"
 
-KEY_TABLE_OWNER = 'Owner'
-KEY_TABLE_STATISTICS = 'Statistics'
 
 class ImpalaAdapter(SQLAdapter):
     Relation = ImpalaRelation
     Column = ImpalaColumn
     ConnectionManager = ImpalaConnectionManager
 
-    INFORMATION_COLUMNS_REGEX = re.compile(
-        r"^ \|-- (.*): (.*) \(nullable = (.*)\b", re.MULTILINE)
+    INFORMATION_COLUMNS_REGEX = re.compile(r"^ \|-- (.*): (.*) \(nullable = (.*)\b", re.MULTILINE)
     INFORMATION_OWNER_REGEX = re.compile(r"^Owner: (.*)$", re.MULTILINE)
-    INFORMATION_STATISTICS_REGEX = re.compile(
-        r"^Statistics: (.*)$", re.MULTILINE)
+    INFORMATION_STATISTICS_REGEX = re.compile(r"^Statistics: (.*)$", re.MULTILINE)
 
     @classmethod
     def date_function(cls):
-        return 'now()'
+        return "now()"
 
     @classmethod
-    def convert_datetime_type(
-            cls, agate_table: agate.Table, col_idx: int
-    ) -> str:
+    def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "timestamp"
 
     @classmethod
     def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "date"
 
     @classmethod
@@ -71,267 +67,279 @@
         return "time"
 
     @classmethod
     def convert_text_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "string"
 
     def quote(self, identifier):
-        return identifier # no quote
+        return identifier  # no quote
 
     @classmethod
     def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))  # type: ignore[attr-defined]
         return "real" if decimals else "integer"
-        
+
     def check_schema_exists(self, database, schema):
-        results = self.execute_macro(
-            LIST_SCHEMAS_MACRO_NAME,
-            kwargs={'database': database}
-        )
+        results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
 
         exists = True if schema in [row[0] for row in results] else False
-        
+
         return exists
 
     def list_schemas(self, database: str) -> List[str]:
-        results = self.execute_macro(
-            LIST_SCHEMAS_MACRO_NAME,
-            kwargs={'database': database}
-        )
-        
+        results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
+
         schemas = []
 
         for row in results:
             _schema = row[0]
             schemas.append(_schema)
 
         return schemas
 
     def list_relations_without_caching(
         self, schema_relation: ImpalaRelation
     ) -> List[ImpalaRelation]:
-        kwargs = {'schema_relation': schema_relation}
+        kwargs = {"schema_relation": schema_relation}
 
         try:
-            results = self.execute_macro(
-                LIST_RELATIONS_MACRO_NAME,
-                kwargs=kwargs
-            )
+            results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
         except dbt.exceptions.RuntimeException as e:
-            errmsg = getattr(e, 'msg', '')
+            errmsg = getattr(e, "msg", "")
             if f"Database '{schema_relation}' not found" in errmsg:
                 return []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation}: {e.msg}")
                 return []
 
         relations = []
         for row in results:
             if len(row) != 2:
                 raise dbt.exceptions.RuntimeException(
                     f'Invalid value from "show table extended ...", '
-                    f'got {len(row)} values, expected 4'
+                    f"got {len(row)} values, expected 4"
                 )
             _identifier = row[0]
-            _rel_type   = row[1]
+            _rel_type = row[1]
 
             relation = self.Relation.create(
-                database=None, 
+                database=None,
                 schema=schema_relation.schema,
                 identifier=_identifier,
                 type=_rel_type,
                 information=_identifier,
             )
             relations.append(relation)
 
         return relations
 
     def get_columns_in_relation(self, relation: Relation) -> List[ImpalaColumn]:
         cached_relations = self.cache.get_relations(relation.database, relation.schema)
-        cached_relation = next((cached_relation
-                                for cached_relation in cached_relations
-                                if str(cached_relation) == str(relation)),
-                               None)
+        cached_relation = next(
+            (
+                cached_relation
+                for cached_relation in cached_relations
+                if str(cached_relation) == str(relation)
+            ),
+            None,
+        )
         columns = []
         if cached_relation and cached_relation.information:
             columns = self.parse_columns_from_information(cached_relation)
 
         # execute the macro and parse the data
-        if not columns:       
+        if not columns:
             try:
                 rows: List[agate.Row] = super().get_columns_in_relation(relation)
                 columns = self.parse_describe_extended(relation, rows)
             except dbt.exceptions.RuntimeException as e:
                 # impala would throw error when table doesn't exist
                 errmsg = getattr(e, "msg", "")
-                if "Table or view not found" in errmsg or "NoSuchTableException" in errmsg:
-                    pass
+                if (
+                    "Table or view not found" in errmsg
+                    or "NoSuchTableException" in errmsg
+                    or "Could not resolve path" in errmsg
+                ):
+                    return []
                 else:
                     raise e
 
         return columns
 
     def parse_describe_extended(
-            self,
-            relation: Relation,
-            raw_rows: List[agate.Row]
+        self, relation: Relation, raw_rows: List[agate.Row]
     ) -> List[ImpalaColumn]:
-
         # TODO: this method is largely from dbt-spark, sample test with impala works (test_dbt_base: base)
-        # need deeper testing 
+        # need deeper testing
 
         # Convert the Row to a dict
         dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
+        # Find the separator between columns and partitions information
+        # by the DESCRIBE EXTENDED {{relation}} statement
+        partition_separator_pos = ImpalaAdapter.find_partition_information_separator(
+            dict_rows
+        )  # ensure that the class method is called
+
         # Find the separator between the rows and the metadata provided
         # by the DESCRIBE EXTENDED {{relation}} statement
-        pos = ImpalaAdapter.find_table_information_separator(dict_rows)  # ensure that the class method is called
+        table_separator_pos = ImpalaAdapter.find_table_information_separator(
+            dict_rows
+        )  # ensure that the class method is called
 
+        column_separator_pos = (
+            partition_separator_pos if partition_separator_pos > 0 else table_separator_pos
+        )
         # Remove rows that start with a hash, they are comments
         rows = [
-            row for row in raw_rows[0:pos]
-            if not row['name'].startswith('#') and not row['name'] == ''
+            row
+            for row in raw_rows[0:column_separator_pos]
+            if not row["name"].startswith("#") and not row["name"] == ""
         ]
         # trim the fields so that these are clean key,value pairs and metadata.get() correctly returns the values
         metadata = {
-            col['name'].split(":")[0].strip(): col['type'].strip() for col in raw_rows[pos + 1:]
-            if col['name'] and not col['name'].startswith('#') and not col['name'] == '' and col['type']
+            col["name"].split(":")[0].strip(): col["type"].strip()
+            for col in raw_rows[table_separator_pos + 1 :]
+            if col["name"]
+            and not col["name"].startswith("#")
+            and not col["name"] == ""
+            and col["type"]
         }
 
         raw_table_stats = metadata.get(KEY_TABLE_STATISTICS)
         table_stats = ImpalaColumn.convert_table_stats(raw_table_stats)
 
-        return [ImpalaColumn(
-            table_database=None,
-            table_schema=relation.schema,
-            table_name=relation.name,
-            table_type=relation.type,
-            table_owner=str(metadata.get(KEY_TABLE_OWNER)),
-            table_stats=table_stats,
-            column=column['name'],
-            column_index=idx,
-            dtype=column['type'],
-        ) for idx, column in enumerate(rows)]
+        return [
+            ImpalaColumn(
+                table_database=None,
+                table_schema=relation.schema,
+                table_name=relation.name,
+                table_type=relation.type,
+                table_owner=str(metadata.get(KEY_TABLE_OWNER)),
+                table_stats=table_stats,
+                column=column["name"],
+                column_index=idx,
+                dtype=column["type"],
+            )
+            for idx, column in enumerate(rows)
+        ]
+
+    @staticmethod
+    def find_partition_information_separator(rows: List[dict]) -> int:
+        pos = 0
+        for row in rows:
+            if row["name"].startswith("# Partition Transform Information"):
+                break
+            pos += 1
+        result = 0 if (pos == len(rows)) else pos
+        return result
 
     @staticmethod
     def find_table_information_separator(rows: List[dict]) -> int:
         pos = 0
         for row in rows:
-            if row['name'].startswith('# Detailed Table Information'):
+            if row["name"].startswith("# Detailed Table Information"):
                 break
             pos += 1
         return pos
 
-    def parse_columns_from_information(
-            self, relation: ImpalaRelation
-    ) -> List[ImpalaColumn]:
-
+    def parse_columns_from_information(self, relation: ImpalaRelation) -> List[ImpalaColumn]:
         # TODO: this method is largely from dbt-spark, sample test with impala works (test_dbt_base: base)
         # need deeper testing
 
-        owner_match = re.findall(
-            self.INFORMATION_OWNER_REGEX, relation.information)
+        owner_match = re.findall(self.INFORMATION_OWNER_REGEX, relation.information)
         owner = owner_match[0] if owner_match else None
-        matches = re.finditer(
-            self.INFORMATION_COLUMNS_REGEX, relation.information)
+        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, relation.information)
         columns = []
-        stats_match = re.findall(
-            self.INFORMATION_STATISTICS_REGEX, relation.information)
+        stats_match = re.findall(self.INFORMATION_STATISTICS_REGEX, relation.information)
         raw_table_stats = stats_match[0] if stats_match else None
         table_stats = ImpalaColumn.convert_table_stats(raw_table_stats)
         for match_num, match in enumerate(matches):
             column_name, column_type, nullable = match.groups()
             column = ImpalaColumn(
                 table_database=None,
                 table_schema=relation.schema,
                 table_name=relation.table,
                 table_type=relation.type,
                 column_index=match_num,
                 table_owner=owner,
                 column=column_name,
                 dtype=column_type,
-                table_stats=table_stats
+                table_stats=table_stats,
             )
             columns.append(column)
 
         return columns
 
     def get_catalog(self, manifest):
         schema_map = self._get_catalog_schemas(manifest)
 
-
         with executor(self.config) as tpe:
             futures: List[Future[agate.Table]] = []
             for info, schemas in schema_map.items():
                 for schema in schemas:
-                    futures.append(tpe.submit_connected(
-                            self, schema,
-                            self._get_one_catalog, info, [schema], manifest
-                        ))
-            catalogs, exceptions = catch_as_completed(futures) # call the default implementation 
+                    futures.append(
+                        tpe.submit_connected(
+                            self, schema, self._get_one_catalog, info, [schema], manifest
+                        )
+                    )
+            catalogs, exceptions = catch_as_completed(futures)  # call the default implementation
 
         return catalogs, exceptions
 
-    def _get_one_catalog(
-        self, information_schema, schemas, manifest
-    ) -> agate.Table:
-
+    def _get_one_catalog(self, information_schema, schemas, manifest) -> agate.Table:
         if len(schemas) != 1:
             dbt.exceptions.raise_compiler_error(
-                f'Expected only one schema in ImpalaAdapter._get_one_catalog, found '
-                f'{schemas}'
+                f"Expected only one schema in ImpalaAdapter._get_one_catalog, found " f"{schemas}"
             )
 
         schema = list(schemas)[0]
-        
+
         columns: List[Dict[str, Any]] = []
 
         relation_list = self.list_relations(None, schema)
 
         for relation in relation_list:
             columns.extend(self._get_columns_for_catalog(relation))
 
         if len(columns) > 0:
-            text_types = agate_helper.build_type_tester(["table_database", "table_schema", "table_name"])
+            text_types = agate_helper.build_type_tester(
+                ["table_database", "table_schema", "table_name"]
+            )
         else:
             text_types = []
 
-        return agate.Table.from_object(
-            columns,
-            column_types = text_types
-        )
+        return agate.Table.from_object(columns, column_types=text_types)
 
-    def _get_columns_for_catalog(
-        self, relation: ImpalaRelation
-    ) -> Iterable[Dict[str, Any]]:
+    def _get_columns_for_catalog(self, relation: ImpalaRelation) -> Iterable[Dict[str, Any]]:
         columns = self.get_columns_in_relation(relation)
 
         for column in columns:
             # convert ImpalaColumns into catalog dicts
             as_dict = column.to_column_dict()
-            
-            as_dict['column_name'] = as_dict.pop('column', None)
-            as_dict['column_type'] = as_dict.pop('dtype')
-            as_dict['table_database'] = None
+
+            as_dict["column_name"] = as_dict.pop("column", None)
+            as_dict["column_type"] = as_dict.pop("dtype")
+            as_dict["table_database"] = None
 
             yield as_dict
- 
+
     def timestamp_add_sql(self, add_to: str, number: int = 1, interval: str = "hour") -> str:
-        # We override this from base dbt adapter because impala doesn't need to escape interval 
+        # We override this from base dbt adapter because impala doesn't need to escape interval
         # duration string like postgres/redshift.
         return f"{add_to} + interval {number} {interval}"
 
     def debug_query(self) -> None:
         self.execute("select 1 as id")
         username = ""
 
         # query user permissions where available
         try:
             username = self.config.credentials.username
-            if not username: # username is not available when auth_type is insecure or kerberos
+            if not username:  # username is not available when auth_type is insecure or kerberos
                 logger.debug("No username available to fetch permissions")
                 payload = {
                     "event_type": tracker.TrackingEventType.DEBUG,
                     "permissions": "NA",
                 }
                 tracker.track_usage(payload)
             else:
@@ -348,17 +356,15 @@
 
                 payload = {
                     "event_type": tracker.TrackingEventType.DEBUG,
                     "permissions": permissions_json,
                 }
                 tracker.track_usage(payload)
         except Exception as ex:
-            logger.error(
-                f"Failed to fetch permissions for user: {username}. Exception: {ex}"
-            )
+            logger.error(f"Failed to fetch permissions for user: {username}. Exception: {ex}")
 
         self.connections.get_thread_connection().handle.close()
 
     ###
     # Methods about grants
     ###
     def standardize_grants_dict(self, grants_table: agate.Table) -> dict:
@@ -392,8 +398,7 @@
         return grants_dict
 
     def valid_incremental_strategies(self):
         """The set of standard builtin strategies which this adapter supports out-of-the-box.
         Not used to validate custom strategies defined by end users.
         """
         return ["append", "insert_overwrite"]
-
```

### Comparing `dbt-impala-1.3.1/dbt/adapters/impala/relation.py` & `dbt-impala-1.3.2/dbt/adapters/impala/relation.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 from dataclasses import dataclass
 
 from dbt.adapters.base.relation import BaseRelation, Policy
 from dbt.exceptions import RuntimeException
 
 import dbt.adapters.impala.cloudera_tracking as tracker
 
+
 @dataclass
 class ImpalaQuotePolicy(Policy):
     database: bool = False
     schema: bool = False
     identifier: bool = False
 
+
 @dataclass
 class ImpalaIncludePolicy(Policy):
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
@@ -36,36 +38,40 @@
 class ImpalaRelation(BaseRelation):
     quote_policy: ImpalaQuotePolicy = ImpalaQuotePolicy()
     include_policy: ImpalaIncludePolicy = ImpalaIncludePolicy()
     quote_character: str = None
     information: str = None
 
     def __post_init__(self):
-        if (self.type):
-            tracker.track_usage({
-                "event_type": tracker.TrackingEventType.MODEL_ACCESS,
-                "model_name": self.render(),
-                "model_type": self.type,
-                "incremental_strategy": ""
-            })
-    
+        if self.type:
+            tracker.track_usage(
+                {
+                    "event_type": tracker.TrackingEventType.MODEL_ACCESS,
+                    "model_name": self.render(),
+                    "model_type": self.type,
+                    "incremental_strategy": "",
+                }
+            )
+
     def render(self):
         return super().render()
 
     def log_relation(self, incremental_strategy):
-        if (self.type):
-            tracker.track_usage({
-                "event_type": tracker.TrackingEventType.INCREMENTAL,
-                "model_name": self.render(),
-                "model_type": self.type,
-                "incremental_strategy": incremental_strategy
-            })
+        if self.type:
+            tracker.track_usage(
+                {
+                    "event_type": tracker.TrackingEventType.INCREMENTAL,
+                    "model_name": self.render(),
+                    "model_type": self.type,
+                    "incremental_strategy": incremental_strategy,
+                }
+            )
 
     def new_copy(self, name, identifier):
         new_relation = ImpalaRelation.create(
-                database=None, # since include policy of database is False, this should be None
-                schema=name,
-                identifier=identifier,
-                information=identifier,
-            )
+            database=None,  # since include policy of database is False, this should be None
+            schema=name,
+            identifier=identifier,
+            information=identifier,
+        )
 
         return new_relation
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/__init__.py` & `dbt-impala-1.3.2/dbt/include/impala/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+
 PACKAGE_PATH = os.path.dirname(__file__)
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/dbt_project.yml` & `dbt-impala-1.3.2/dbt/include/impala/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/adapters.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -145,29 +145,35 @@
   {{ return(objects_with_type) }}
 {% endmacro %}
 
 {% macro impala__create_table_as(temporary, relation, sql) -%}
 
   {%- set sql_header = config.get('sql_header', none) -%}
   {%- set is_external = config.get('external') -%}
+  {%- set table_type = config.get('table_type') -%}
 
   {{ sql_header if sql_header is not none }}
 
   create {% if is_external == true -%}external{%- endif %} table
     {{ relation.include(schema=true) }}
-    {{ ct_option_partition_cols(label="partitioned by") }}
+    {% if table_type == 'iceberg' -%}
+      {{ ct_option_partition_cols(label="partitioned by spec") }}
+    {% else %}
+      {{ ct_option_partition_cols(label="partitioned by") }}
+    {%- endif %}
     {{ ct_option_sort_cols(label="sort by") }}
     {{ ct_option_comment_relation(label="comment") }}
     {{ ct_option_row_format(label="row format") }}
     {{ ct_option_with_serdeproperties(label="with serdeproperties") }}
+    {%- if table_type == 'iceberg' -%} STORED BY ICEBERG {%- endif -%}
     {{ ct_option_stored_as(label="stored as") }}
-    {{ ct_option_location_clause(label="location") }} 
+    {{ ct_option_location_clause(label="location") }}
     {{ ct_option_cached_in(label="cached in") }}
     {{ ct_option_tbl_properties(label="tblproperties") }}
-  as 
+  as
     {{ sql }}
   ;
 {%- endmacro %}
 
 {% macro impala__create_view_as(relation, sql) -%}
 
   {%- set sql_header = config.get('sql_header', none) -%}
@@ -208,25 +214,25 @@
   {% set result_set = run_query('show tables in ' ~ relation.schema ~ ' like "' ~ relation.identifier.lower() ~ '"') %}
 
   {% if execute %}
     {%- for rs in result_set -%}
       {% do return(true) %}
     {%- endfor -%}
   {%- endif -%}
-  
+
   {% do return(false) %}
 {% endmacro %}
 
 {% macro get_relation_type(relation) -%}
   {% set rel_type = 'table' %}
   {% set relation_exists = is_relation_present(relation) %}
 
   {%- if relation_exists -%}
     {% set result_set = run_query('describe extended ' ~ relation) %}
-  
+
     {% if execute %}
       {%- for rs in result_set -%}
         {%- if rs[0].startswith('Table Type') -%}
           {%- if rs[1].startswith('VIRTUAL_VIEW') -%}
             {% set rel_type = 'view' %}
             {% do return(rel_type) %}
           {%- elif rs[1].startswith('MANAGED_TABLE') -%}
@@ -236,21 +242,21 @@
             {% set rel_type = 'table' %}
             {% do return(rel_type) %}
           {%- endif -%}
         {%- endif -%}
       {%- endfor -%}
     {%- endif -%}
   {%- endif -%}
-  
+
   {% do return(rel_type) %}
 {% endmacro %}
 
 {% macro impala__rename_relation(from_relation, to_relation) -%}
   {% set from_rel_type = get_relation_type(from_relation) %}
-  
+
   {% call statement('drop_relation_if_exists_table') %}
     drop table if exists {{ to_relation }}
   {% endcall %}
   {% call statement('drop_relation_if_exists_view') %}
     drop view if exists {{ to_relation }};
   {% endcall %}
   {% call statement('rename_relation') -%}
@@ -281,15 +287,15 @@
 
 {% macro impala__truncate_relation(relation) -%}
     {% call statement('truncate_relation') -%}
       truncate table if exists {{ relation }}
     {%- endcall %}
 {% endmacro %}
 
-/* impala has two hash functions, both are not perfect hash function: fnv_hash and murmur_hash, 
+/* impala has two hash functions, both are not perfect hash function: fnv_hash and murmur_hash,
    the earlier one seems be available from older version and hence is being used here */
 {% macro impala__snapshot_hash_arguments(args) -%}
     hex(fnv_hash(concat({%- for arg in args -%}
         coalesce(cast({{ arg }} as varchar ), '')
         {% if not loop.last %} , '|',  {% endif %}
     {%- endfor -%})))
 {%- endmacro %}
@@ -307,24 +313,24 @@
 
 {% macro get_row_count(relation_name) %}
     {% call statement('row_count', fetch_result=True) %}
         select count(*) as count from {{relation_name}}
     {% endcall %}
     {%- set row_count = load_result('row_count') -%}
 
-    {% do return(row_count['data'][0][0]) %}    
+    {% do return(row_count['data'][0][0]) %}
 {% endmacro %}
 
 {% macro get_new_inserts_count(relation_name) %}
     {% call statement('inserts_count', fetch_result=True) %}
         select count(*) as count from {{relation_name}} where {{relation_name}}.dbt_change_type='insert'
     {% endcall %}
     {%- set inserts_count = load_result('inserts_count') -%}
 
-    {% do return(inserts_count['data'][0][0]) %}    
+    {% do return(inserts_count['data'][0][0]) %}
 {% endmacro %}
 
 {% macro fetch_rows_to_insert(target_relation, staging_table, insert_cols) %}
     {%- set insert_cols_csv = insert_cols | join(', ') -%}
 
     insert into {{target_relation}} ({{insert_cols_csv}}) select {{insert_cols_csv}} from {{staging_table}}
 {% endmacro %}
@@ -372,42 +378,42 @@
 
       {{ adapter.valid_snapshot_target(target_relation) }}
 
       {% set staging_table = build_snapshot_staging_table(strategy, sql, target_relation) %}
 
       /*
       1. if the staging table has no entries, then simply do nothing
-      2. if the staging table has entries, drop the existing snapshot table, build a new one 
+      2. if the staging table has entries, drop the existing snapshot table, build a new one
        */
 
       {% set row_count = get_row_count(staging_table) %}
       {% set insert_count = get_new_inserts_count(staging_table) %}
 
       /* if the change includes anything apart from insert, rebuild the snapshot */
       {% if row_count > 0 and row_count != insert_count %}
         {% call statement('drop_snapshot') %}
             drop table {{target_relation}}
         {% endcall %}
 
         {% set build_sql = build_snapshot_table(strategy, model['compiled_sql']) %}
         {% set final_sql = create_table_as(False, target_relation, build_sql) %}
       {% elif row_count > 0 and row_count == insert_count %} /* insert, if all changes are of that type */
-        
+
         {% set source_columns = adapter.get_columns_in_relation(staging_table)
                                    | rejectattr('name', 'equalto', 'dbt_change_type')
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
                                    | rejectattr('name', 'equalto', 'DBT_UNIQUE_KEY')
                                    | list %}
 
         {% set quoted_source_columns = [] %}
         {% for column in source_columns %}
           {% do quoted_source_columns.append(adapter.quote(column.name)) %}
         {% endfor %}
-        
+
         {% set final_sql = fetch_rows_to_insert(target_relation, staging_table, quoted_source_columns) %}
       {% else %}
         {% set final_sql = 'select 1' %} /* dummy sql */
       {% endif %}
 
   {% endif %}
 
@@ -432,8 +438,7 @@
   {{ adapter.commit() }}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
-
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/apply_grants.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/catalog.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/catalog.sql`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 # limitations under the License.
 #}
 
 {% macro impala__get_catalog(information_schema, schemas) -%}
 
   {# no-op #}
 {% endmacro %}
-
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/incremental.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   {% do return(incremental_strategy) %}
 {% endmacro %}
 
 {% macro incremental_validate_on_schema_change(on_schema_change, default='ignore') %}
    {% if on_schema_change not in ['fail', 'ignore'] %}
      {% set log_message = 'Invalid value for on_schema_change (%s) specified. Setting default value of %s.' % (on_schema_change, default) %}
      {% do log(log_message) %}
-     
+
      {% do exceptions.raise_compiler_error(log_message) %}
 
      {{ return(default) }}
    {% else %}
      {{ return(on_schema_change) }}
    {% endif %}
 {% endmacro %}
@@ -67,15 +67,15 @@
   {% if incremental_strategy == None %}
     {% set incremental_strategy = 'append' %}
   {% endif %}
   {% set incremental_strategy = validate_get_incremental_strategy(incremental_strategy) %}
   {%- set full_refresh_mode = (should_full_refresh()  or existing_relation.is_view) -%}
   {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
 
-  -- log incremental strategy 
+  -- log incremental strategy
   {% do target_relation.log_relation(incremental_strategy) %}
 
   -- the temp_ and backup_ relations should not already exist in the database; get_relation
   -- will return None in that case. Otherwise, we get a relation that we can drop
   -- later, before we try to use this name for the current operation. This has to happen before
   -- BEGIN, in a separate transaction
   {%- set preexisting_intermediate_relation = load_cached_relation(intermediate_relation)-%}
@@ -143,8 +143,7 @@
       {% do adapter.drop_relation(rel) %}
   {% endfor %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
   {{ return({'relations': [target_relation]}) }}
 {%- endmaterialization %}
-
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/insertoverwrite.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/insertoverwrite.sql`

 * *Files 24% similar despite different names*

```diff
@@ -10,66 +10,48 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #}
 
-{% macro get_quoted_csv_exclude(column_names, exclude_name) %}
-
-    {% set quoted = [] %}
-    {% for col in column_names -%}
-        {% if exclude_name|string() != col|string() %}
-           {%- do quoted.append(adapter.quote(col)) -%}
-        {% endif %}
-    {%- endfor %}
-
-    {%- set dest_cols_csv = quoted | join(', ') -%}
-    {{ return(dest_cols_csv) }}
-
-{% endmacro %}
-
 {% macro get_insert_overwrite_sql(target, source, dest_columns) -%}
 
-    {%- set raw_strategy = config.get('incremental_strategy', default='append')  -%}
+    {% set raw_strategy = config.get('incremental_strategy') or 'append' %}
     {%- set partition_cols = config.get('partition_by', validator=validation.any[list]) -%}
-    
-    {% if partition_cols is not none and raw_strategy == 'insert_overwrite' %}
-        {% if partition_cols is string %}
-           {%- set partition_col = partition_cols -%}
-        {% else %}
-           {%- set partition_col = partition_cols[0] -%}
-        {% endif %}
-
-        {%- set dest_cols_csv = get_quoted_csv_exclude(dest_columns | map(attribute="name"), "") -%}
-        {%- set dest_cols_csv_exclude = get_quoted_csv_exclude(dest_columns | map(attribute="name"), partition_col) -%}
+    {%- set dest_cols_csv = dest_columns | map(attribute="name") | join(", ") -%}
 
-        insert overwrite {{ target }} ({{ dest_cols_csv_exclude }}) partition({{ partition_col }})
-            select {{ dest_cols_csv }}
-            from {{ source }}
-    {% elif partition_cols is not none and raw_strategy == 'append' %}
+    {% if partition_cols is not none %}
         {% if partition_cols is string %}
-           {%- set partition_col = partition_cols -%}
+            {%- set partition_cols_csv = partition_cols -%}
         {% else %}
-           {%- set partition_col = partition_cols[0] -%}
+            {%- set partition_cols_csv = partition_cols | join(", ") -%}
         {% endif %}
+        {{ print("partition_cols_csv = " + partition_cols_csv) }}
 
-        {%- set dest_cols_csv = get_quoted_csv_exclude(dest_columns | map(attribute="name"), "") -%}
-        {%- set dest_cols_csv_exclude = get_quoted_csv_exclude(dest_columns | map(attribute="name"), partition_col) -%}
+        {% if raw_strategy == 'insert_overwrite' %}
 
-        insert into {{ target }} ({{ dest_cols_csv_exclude }}) partition({{ partition_col }})
-        (
-            select {{ dest_cols_csv }}
-            from {{ source }}
-        )
+            insert overwrite {{ target }} partition({{ partition_cols_csv }})
+            (
+                select {{ dest_cols_csv }}
+                from {{ source }}
+            )
+
+        {% elif raw_strategy == 'append' %}
+
+            insert into {{ target }} partition({{ partition_cols_csv }})
+            (
+                select {{ dest_cols_csv }}
+                from {{ source }}
+            )
+
+        {% endif %}
     {% else %}
-        {%- set dest_cols_csv = get_quoted_csv_exclude(dest_columns | map(attribute="name"), "") -%}
 
         insert into {{ target }} ({{ dest_cols_csv }})
         (
             select {{ dest_cols_csv }}
             from {{ source }}
         )
     {% endif %}
 
 {%- endmacro %}
-
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/seed.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/any_value.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/bool_or.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/concat.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/dateadd.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/datediff.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/escape_single_quotes.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/escape_single_quotes.sql`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #}
 
 {% macro impala__escape_single_quotes(expression) -%}
     {{ expression | replace("'","\\'") }}
-{%- endmacro %}
+{%- endmacro %}
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/hash.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/last_day.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/last_day.sql`

 * *Files 12% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 # limitations under the License.
 #}
 
 {%- macro impala__last_day(date, datepart) -%}
     {% if datepart == 'quarter' %}
         cast(
             {{
-                dbt.dateadd('day', '-1', 
-                    dbt.dateadd('month', '3', 
+                dbt.dateadd('day', '-1',
+                    dbt.dateadd('month', '3',
                         dbt.date_trunc('month', date)
                     )
                 )
             }}
             as date)
     {% else %}
         cast(
             {{
-                dbt.dateadd('day', '-1', 
-                    dbt.dateadd(datepart, '1', 
+                dbt.dateadd('day', '-1',
+                    dbt.dateadd(datepart, '1',
                         dbt.date_trunc(datepart, date)
                     )
                 )
             }}
             as date)
     {% endif %}
-{%- endmacro -%}
+{%- endmacro -%}
```

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/listagg.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/position.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/split_part.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/macros/utils/timestamps.sql` & `dbt-impala-1.3.2/dbt/include/impala/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt/include/impala/sample_profiles.yml` & `dbt-impala-1.3.2/dbt/include/impala/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/dbt_impala.egg-info/SOURCES.txt` & `dbt-impala-1.3.2/dbt_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.1/setup.py` & `dbt-impala-1.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,68 +15,69 @@
 
 import os
 import re
 from setuptools import find_namespace_packages, setup
 
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md'), 'r', encoding='utf8') as f:
+with open(os.path.join(this_directory, "README.md"), encoding="utf8") as f:
     long_description = f.read()
 
+
 # get this package's version from dbt/adapters/<name>/__version__.py
 def _get_plugin_version_dict():
-    _version_path = os.path.join(
-        this_directory, 'dbt', 'adapters', 'impala', '__version__.py'
-    )
-    _semver = r'''(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)'''
-    _pre = r'''((?P<prekind>a|b|rc)(?P<pre>\d+))?'''
-    _version_pattern = fr'''version\s*=\s*["']{_semver}{_pre}["']'''
+    _version_path = os.path.join(this_directory, "dbt", "adapters", "impala", "__version__.py")
+    _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
+    _pre = r"""((?P<prekind>a|b|rc)(?P<pre>\d+))?"""
+    _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}["']"""
     with open(_version_path) as f:
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
-            raise ValueError(f'invalid version at {_version_path}')
+            raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
 # require a compatible minor version (~=), prerelease if this is a prerelease
 def _get_dbt_core_version():
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
-    pre = (parts["prekind"]+"1" if parts["prekind"] else "")
+    pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
+
 package_name = "dbt-impala"
 # make sure this always matches dbt/adapters/dbt_impala/__version__.py
-package_version = "1.3.1"
+package_version = "1.3.2"
 description = """The Impala adapter plugin for dbt"""
 
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
     description="Impala adapter for DBT",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="Cloudera",
     author_email="innovation-feedback@cloudera.com",
     url="https://github.com/cloudera/dbt-impala",
-    packages=find_namespace_packages(include=['dbt', 'dbt.*']),
-    data_files=[('', ['dbt/adapters/impala/.env'])],
+    packages=find_namespace_packages(include=["dbt", "dbt.*"]),
+    data_files=[("", ["dbt/adapters/impala/.env"])],
     include_package_data=True,
     install_requires=[
-        'dbt-core~={}'.format(dbt_core_version),
+        f"dbt-core~={dbt_core_version}",
         "impyla==0.18",
         "python-decouple>=3.6",
-        "kerberos>=1.3.0",
+        # "kerberos>=1.3.0", # Not required per README, doesn't work on Windows
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "License :: OSI Approved :: Apache Software License"
+        "License :: OSI Approved :: Apache Software License",
     ],
-    zip_safe=False
+    zip_safe=False,
 )
```


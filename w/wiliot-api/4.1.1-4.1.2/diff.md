# Comparing `tmp/wiliot-api-4.1.1.tar.gz` & `tmp/wiliot-api-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.1.1.tar", last modified: Wed May 10 03:45:39 2023, max compression
+gzip compressed data, was "wiliot-api-4.1.2.tar", last modified: Thu May 11 23:02:51 2023, max compression
```

## Comparing `wiliot-api-4.1.1.tar` & `wiliot-api-4.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2891 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11124 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13640 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14095 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35636 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.750939 wiliot-api-4.1.2/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11124 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13640 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    14095 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35660 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7223 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.1.1/LICENSE` & `wiliot-api-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/PKG-INFO` & `wiliot-api-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.1.1
+Version: 4.1.2
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,15 +57,15 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
-Version 4.1.1:
+Version 4.1.2:
 -----------------
 * Changed additional functions use the metadataFetch API to support larger returned data sets:
     * Get Locations
     * Get zones
     * Get location associations
     * Get zone associations
 * Added the ability to associate pixels to zones
```

### Comparing `wiliot-api-4.1.1/README.md` & `wiliot-api-4.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
-Version 4.1.1:
+Version 4.1.2:
 -----------------
 * Changed additional functions use the metadataFetch API to support larger returned data sets:
     * Get Locations
     * Get zones
     * Get location associations
     * Get zone associations
 * Added the ability to associate pixels to zones
```

### Comparing `wiliot-api-4.1.1/bitbucket-pipelines.yml` & `wiliot-api-4.1.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/setup.py` & `wiliot-api-4.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/__init__.py` & `wiliot-api-4.1.2/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/api_client.py` & `wiliot-api-4.1.2/wiliot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/edge/edge.py` & `wiliot-api-4.1.2/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.1.2/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.1.2/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.1.2/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.1.2/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/platform/platform.py` & `wiliot-api-4.1.2/wiliot_api/platform/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 class ZoneAssociationType(Enum):
     BRIDGE = 'bridge'
     TAG = 'tag'
 
 
 class LocationAssociationType(Enum):
     BRIDGE = 'bridge'
+    GATEWAY = 'gateway'
 
 
 class PlatformClient(Client):
     def __init__(self, api_key, owner_id, env='', log_file=None, logger_=None):
         self.client_path = "traceability/owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
         super().__init__(api_key=api_key, env=env, log_file=log_file, logger_=logger_)
```

### Comparing `wiliot-api-4.1.1/wiliot_api/platform/platform_models.py` & `wiliot-api-4.1.2/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/security/security.py` & `wiliot-api-4.1.2/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api/utils/get_version.py` & `wiliot-api-4.1.2/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.1/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.1.2/wiliot_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.1.1
+Version: 4.1.2
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,15 +57,15 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
-Version 4.1.1:
+Version 4.1.2:
 -----------------
 * Changed additional functions use the metadataFetch API to support larger returned data sets:
     * Get Locations
     * Get zones
     * Get location associations
     * Get zone associations
 * Added the ability to associate pixels to zones
```

### Comparing `wiliot-api-4.1.1/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.1.2/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*


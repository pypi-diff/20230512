# Comparing `tmp/mlflow-watsonml-0.6.2.tar.gz` & `tmp/mlflow-watsonml-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-watsonml-0.6.2.tar", last modified: Wed May  3 12:17:38 2023, max compression
+gzip compressed data, was "mlflow-watsonml-0.6.3.tar", last modified: Fri May 12 13:50:30 2023, max compression
```

## Comparing `mlflow-watsonml-0.6.2.tar` & `mlflow-watsonml-0.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/mlflow_watsonml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/wml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:30.392009 mlflow-watsonml-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 13:50:30.392009 mlflow-watsonml-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:30.388009 mlflow-watsonml-0.6.3/mlflow_watsonml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/mlflow_watsonml/wml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:50:30.388009 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 13:50:30.000000 mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:50:30.392009 mlflow-watsonml-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-12 13:50:18.000000 mlflow-watsonml-0.6.3/setup.py
```

### Comparing `mlflow-watsonml-0.6.2/PKG-INFO` & `mlflow-watsonml-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.2
+Version: 0.6.3
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.6.2/README.md` & `mlflow-watsonml-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.2/mlflow_watsonml/config.py` & `mlflow-watsonml-0.6.3/mlflow_watsonml/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.2/mlflow_watsonml/deploy.py` & `mlflow-watsonml-0.6.3/mlflow_watsonml/deploy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import sys
 from typing import Dict, List, Optional
 
 import mlflow
 import pandas as pd
 from ibm_watson_machine_learning.client import APIClient
 from mlflow.deployments import BaseDeploymentClient
 from mlflow.exceptions import MlflowException
@@ -382,7 +381,26 @@
         raise NotImplementedError()
 
     def list_endpoints(self):
         return list_endpoints(client=self.get_wml_client())
 
     def get_endpoint(self, endpoint):
         return get_endpoint(client=self.get_wml_client(), endpoint=endpoint)
+
+    def create_custom_wml_spec(
+        self,
+        name: str,
+        base_software_spec: str,
+        custom_packages: List[Dict[str, str]],
+        rewrite: bool = False,
+        endpoint: Optional[str] = None,
+    ):
+        client = self.get_wml_client(endpoint=endpoint)
+        software_spec_id = create_custom_software_spec(
+            client=client,
+            name=name,
+            base_sofware_spec=base_software_spec,
+            custom_packages=custom_packages,
+            rewrite=rewrite,
+        )
+
+        return software_spec_id
```

### Comparing `mlflow-watsonml-0.6.2/mlflow_watsonml/utils.py` & `mlflow-watsonml-0.6.3/mlflow_watsonml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import zipfile
 from typing import Dict, List
 
 from ibm_watson_machine_learning.client import APIClient
 from mlflow.exceptions import ENDPOINT_NOT_FOUND, MlflowException
 from tabulate import tabulate
 
 
@@ -278,7 +280,18 @@
 
     return any(item for item in sw_specs if item["metadata"]["name"] == sw_spec)
 
 
 def delete_sw_spec(client, name):
     sw_spec_id = client.software_specifications.get_id_by_name(name)
     client.software_specifications.delete(sw_spec_id)
+
+
+def is_zipfile(file_path: str) -> bool:
+    if not os.path.isfile(file_path):
+        return False
+
+    try:
+        with zipfile.ZipFile(file_path) as zf:
+            return zf.testzip() is None
+    except zipfile.BadZipFile:
+        return False
```

### Comparing `mlflow-watsonml-0.6.2/mlflow_watsonml/wml.py` & `mlflow-watsonml-0.6.3/mlflow_watsonml/wml.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,24 +181,28 @@
 
 def create_custom_software_spec(
     client: APIClient,
     name: str,
     base_sofware_spec: str,
     custom_packages: List[Dict[str, str]],
     rewrite: bool = False,
-):
+) -> str:
     if software_spec_exists(client=client, sw_spec=name):
         if rewrite:
             delete_sw_spec(client=client, name=name)
         else:
-            raise MlflowException(
-                f"""Software spec {name} already exists. 
-                Please delete the software spec or create one with another name."""
+            LOGGER.warn(
+                f"""Software spec {name} already exists."""
+                """skipping software spec creation."""
+                """restart with rewrite=True if software spec needs to be updated."""
             )
 
+            software_spec_id = client.software_specifications.get_id_by_name(name)
+            return software_spec_id
+
     try:
         base_software_spec_id = client.software_specifications.get_id_by_name(
             base_sofware_spec
         )
 
         meta_prop_sw_spec = {
             client.software_specifications.ConfigurationMetaNames.NAME: name,
@@ -209,14 +213,18 @@
 
         sw_spec_details = client.software_specifications.store(
             meta_props=meta_prop_sw_spec
         )
         software_spec_id = client.software_specifications.get_uid(sw_spec_details)
 
         for custom_package in custom_packages:
+            if not is_zipfile(custom_package["file"]):
+                raise MlflowException(
+                    f"{custom_package['file']} is not a valid zip file."
+                )
             meta_prop_pkg_extn = {
                 client.package_extensions.ConfigurationMetaNames.NAME: custom_package[
                     "name"
                 ],
                 client.package_extensions.ConfigurationMetaNames.TYPE: "pip_zip",
             }
 
@@ -227,13 +235,18 @@
             pkg_extn_id = client.package_extensions.get_id(pkg_extn_details)
 
             client.software_specifications.add_package_extension(
                 software_spec_id, pkg_extn_id
             )
 
     except Exception as e:
+        LOGGER.exception(e)
         if software_spec_exists(client=client, sw_spec=name):
             delete_sw_spec(client, name)
 
         raise MlflowException(e)
 
+    LOGGER.info(
+        f"Successfully created {name} software specification with ID {software_spec_id}"
+    )
+
     return software_spec_id
```

### Comparing `mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/PKG-INFO` & `mlflow-watsonml-0.6.3/mlflow_watsonml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.2
+Version: 0.6.3
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.6.2/setup.py` & `mlflow-watsonml-0.6.3/setup.py`

 * *Files identical despite different names*


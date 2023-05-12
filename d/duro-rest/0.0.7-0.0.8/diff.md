# Comparing `tmp/duro_rest-0.0.7.tar.gz` & `tmp/duro_rest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duro_rest-0.0.7.tar", max compression
+gzip compressed data, was "duro_rest-0.0.8.tar", max compression
```

## Comparing `duro_rest-0.0.7.tar` & `duro_rest-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    16726 2022-12-13 18:32:39.878220 duro_rest-0.0.7/LICENSE
--rw-r--r--   0        0        0     1758 2022-12-15 15:51:37.207962 duro_rest-0.0.7/README.md
--rw-r--r--   0        0        0      477 2022-12-19 16:20:02.232066 duro_rest-0.0.7/duro_rest/__init__.py
--rw-r--r--   0        0        0     7679 2023-04-27 18:07:29.757753 duro_rest-0.0.7/duro_rest/bom_client.py
--rw-r--r--   0        0        0     8312 2023-04-27 17:19:54.511297 duro_rest-0.0.7/duro_rest/duro_client.py
--rw-r--r--   0        0        0      641 2022-12-13 22:48:34.469642 duro_rest-0.0.7/duro_rest/error.py
--rw-r--r--   0        0        0      556 2023-04-27 13:40:55.065101 duro_rest-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 duro_rest-0.0.7/setup.py
--rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 duro_rest-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    16726 2022-12-13 18:32:39.878220 duro_rest-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1758 2022-12-15 15:51:37.207962 duro_rest-0.0.8/README.md
+-rw-r--r--   0        0        0      477 2022-12-19 16:20:02.232066 duro_rest-0.0.8/duro_rest/__init__.py
+-rw-r--r--   0        0        0     7667 2023-05-12 15:56:33.186124 duro_rest-0.0.8/duro_rest/bom_client.py
+-rw-r--r--   0        0        0     8362 2023-05-12 15:59:48.062363 duro_rest-0.0.8/duro_rest/duro_client.py
+-rw-r--r--   0        0        0      641 2022-12-13 22:48:34.469642 duro_rest-0.0.8/duro_rest/error.py
+-rw-r--r--   0        0        0      556 2023-05-12 16:01:17.925154 duro_rest-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 duro_rest-0.0.8/setup.py
+-rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 duro_rest-0.0.8/PKG-INFO
```

### Comparing `duro_rest-0.0.7/LICENSE` & `duro_rest-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `duro_rest-0.0.7/README.md` & `duro_rest-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `duro_rest-0.0.7/duro_rest/bom_client.py` & `duro_rest-0.0.8/duro_rest/bom_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,28 +167,28 @@
     # We we request a product or component from Duro the 'children' property only contains a single
     # level of depth. What we need is the full nested BOM. We call expand_child_components on each
     # child to build out that full tree.
     parent['children'] = list(map(lambda child: expand_child_components(child, components), parent['children']))
 
     return NestedBOM(parent)
 
-def expand_child_components(parent, components):
+def expand_child_components(child, components):
   # The components list contains most of the needed data, but we need some of the properties that
-  # are defined by the parent component (specifically the quantity). Therefore we combine the
-  # properties of the parent we are currently expanding with the expanded data available from
+  # are defined by the child component (specifically the quantity). Therefore we combine the
+  # properties of the child we are currently expanding with the expanded data available from
   # fetching all of the components
-  matching_components = list(component for component in components if component['_id'] == parent['component'])
+  matching_components = list(component for component in components if component['_id'] == child['component'])
 
   if len(matching_components) == 0:
-    raise LookupError('Failed to find component in cache ' + parent['component'])
+    raise LookupError('Failed to find component in cache ' + child['component'])
   elif len(matching_components) > 1:
-    raise LookupError('Found multiple components in cache ' + parent['component'])
+    raise LookupError('Found multiple components in cache ' + child['component'])
 
-  expanded_parent = {**parent, **matching_components[0]}
+  expanded_child = {**child, **matching_components[0]}
 
-  # Now that we have expanded the parent component, we need to expand each of the child components
-  expanded_parent['children'] = list(map(lambda child: expand_child_components(child, components), expanded_parent['children']))
+  # Now that we have expanded the child component, we need to expand each of its child components
+  expanded_child['children'] = list(map(lambda child: expand_child_components(child, components), expanded_child['children']))
 
-  return expanded_parent
+  return expanded_child
 
 def flatten(l):
   return [item for sublist in l for item in sublist]
```

### Comparing `duro_rest-0.0.7/duro_rest/duro_client.py` & `duro_rest-0.0.8/duro_rest/duro_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 # Copyright 2022 Oxide Computer Company
 
+import copy
 from datetime import datetime, timedelta
 import json
 from json import JSONDecodeError
 import math
 import requests
 
 from duro_rest.error import AuthenticationError, BadRequestError, ForbiddenError, NotFoundError
@@ -18,15 +19,15 @@
     self.__data = {}
 
   def get(self, key):
     if key in self.__data:
       (value, expiration) = self.__data[key]
 
       if datetime.now().timestamp() < expiration:
-        return value
+        return copy.deepcopy(value)
 
     return None
 
   def insert(self, key, value):
     if self.__delta.seconds > 0:
       self.__data[key] = (value, (datetime.now() + self.__delta).timestamp())
 
@@ -330,8 +331,8 @@
     if resp.status_code == 403:
       raise ForbiddenError(resp.json()["message"])
     if resp.status_code == 404:
       raise NotFoundError(resp.json()["message"])
     else:
       data = resp.json()
       self.__cache.insert(cache_key, data)
-      return data
+      return self.__cache.get(cache_key)
```

### Comparing `duro_rest-0.0.7/duro_rest/error.py` & `duro_rest-0.0.8/duro_rest/error.py`

 * *Files identical despite different names*

### Comparing `duro_rest-0.0.7/pyproject.toml` & `duro_rest-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "duro_rest"
-version = "0.0.7"
+version = "0.0.8"
 description = "An API client for the Duro REST API"
 license = "MPL-2.0"
 authors = [
   "Augustus Mayo <augustus@oxidecomputer.com>"
 ]
 maintainers = [
   "Augustus Mayo <augustus@oxidecomputer.com>"
```

### Comparing `duro_rest-0.0.7/setup.py` & `duro_rest-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2,<3']
 
 setup_kwargs = {
     'name': 'duro-rest',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'An API client for the Duro REST API',
     'long_description': '# duro_rest\n\nAn API client for the [Duro REST API](https://public-api.duro.app/v1/docs/).\n\n## Installation\n\nInstalling from [PyPi]()\n\n```pip install duro_rest```\n\nInstalling from [conda-forge]()\n\nTBD\n\n## Examples\n\nThe Duro client is a very minimal API client for reading data from the [Duro v1 REST API](https://public-api.duro.app/v1/docs/). It does not define classes for each object type and instead returns plain dictionaries\nand lists.\n\n#### Base Client\n\n```python\nfrom duro_rest import Client\n\n# Create a new client, providing your API key. By default clients will make calls to the public REST\n# API, but the endpoint base can be overridden if needed\nclient = Client("your-api-key")\n\n# Fetch a component by its Duro assigned id (as opposed to the CPN)\ncomponent = client.component("component-id")\n\n# Fetch a list of all components in Duro\ncomponents = client.components()\n\n# Fetch a list of all components in Duro filtered by status\ncomponents = client.components(status = "OBSOLETE")\n```\n\n#### BOM Client\n\nThe Duro API does not support pulling BOMs directly. The BOM Client is here to make that experience\na little easier.\n\n```python\nfrom duro_rest import BOMClient\n\n# Create a new bom client for fetching full BOMs (either nested or flattened). It accepts the same\n# arguments as the base client\nclient = Client("your-api-key")\n\n# Get a nested BOM starting from a product\nnested_product_bom = client.product_bom("product-id")\n\n# Get a nested BOM starting from a component\nnested_component_bom = client.component("component-id")\n\n# Convert the nested BOM into flattened BOM\nindented_product_bom = nested_product_bom.idented()\n\n# Flattening will collapse rows for the same components together\nflattened_product_bom = indented_product_bom.flatten()\n```',
     'author': 'Augustus Mayo',
     'author_email': 'augustus@oxidecomputer.com',
     'maintainer': 'Augustus Mayo',
     'maintainer_email': 'augustus@oxidecomputer.com',
     'url': 'https://pypi.org/project/duro-rest/',
```

### Comparing `duro_rest-0.0.7/PKG-INFO` & `duro_rest-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duro-rest
-Version: 0.0.7
+Version: 0.0.8
 Summary: An API client for the Duro REST API
 Home-page: https://pypi.org/project/duro-rest/
 License: MPL-2.0
 Author: Augustus Mayo
 Author-email: augustus@oxidecomputer.com
 Maintainer: Augustus Mayo
 Maintainer-email: augustus@oxidecomputer.com
```


# Comparing `tmp/python-oauth-token-manager-0.1.3.tar.gz` & `tmp/python-oauth-token-manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.1.3.tar", last modified: Thu May 11 15:30:41 2023, max compression
+gzip compressed data, was "python-oauth-token-manager-0.2.0.tar", last modified: Fri Oct 14 16:30:05 2022, max compression
```

## Comparing `python-oauth-token-manager-0.1.3.tar` & `python-oauth-token-manager-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-11 15:30:41.487208 python-oauth-token-manager-0.1.3/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.1.3/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2936 2023-05-11 15:30:41.487208 python-oauth-token-manager-0.1.3/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2344 2022-08-23 16:30:58.000000 python-oauth-token-manager-0.1.3/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-11 15:30:41.479209 python-oauth-token-manager-0.1.3/auth/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2022-07-08 21:29:45.000000 python-oauth-token-manager-0.1.3/auth/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.1.3/auth/abstract_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5774 2022-07-15 21:00:46.000000 python-oauth-token-manager-0.1.3/auth/credentials.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.1.3/auth/credentials_helpers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.1.3/auth/credentials_helpers_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.1.3/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.1.3/auth/decorators_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.1.3/auth/exceptions.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4695 2022-07-11 19:58:17.000000 python-oauth-token-manager-0.1.3/auth/firestore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5977 2022-07-11 19:47:18.000000 python-oauth-token-manager-0.1.3/auth/gcs_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2022-07-11 19:34:13.000000 python-oauth-token-manager-0.1.3/auth/gcs_datastore_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5061 2022-07-11 14:35:08.000000 python-oauth-token-manager-0.1.3/auth/local_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6314 2022-07-11 14:13:42.000000 python-oauth-token-manager-0.1.3/auth/local_datastore_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5994 2023-05-10 20:43:41.000000 python-oauth-token-manager-0.1.3/auth/secret_manager.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       98 2022-08-24 18:15:10.000000 python-oauth-token-manager-0.1.3/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-11 15:30:41.487208 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2936 2023-05-11 15:30:41.000000 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      669 2023-05-11 15:30:41.000000 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-05-11 15:30:41.000000 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-08-24 18:09:16.000000 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/not-zip-safe
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-05-11 15:30:41.000000 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-05-11 15:30:41.000000 python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-05-11 15:30:41.487208 python-oauth-token-manager-0.1.3/setup.cfg
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)     2516 2023-05-10 20:43:47.000000 python-oauth-token-manager-0.1.3/setup.py
+drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)    11357 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/LICENSE
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      670 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/PKG-INFO
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2344 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/README.md
+drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-10-14 16:30:05.190130 python-oauth-token-manager-0.2.0/auth/
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      610 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/__init__.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4035 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/abstract_datastore.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5760 2022-10-14 16:24:52.000000 python-oauth-token-manager-0.2.0/auth/credentials.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1322 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/credentials_helpers.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1057 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/credentials_helpers_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/decorators_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      739 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/exceptions.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4695 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/firestore.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5977 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/gcs_datastore.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     8319 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/gcs_datastore_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5061 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/local_datastore.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6314 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/local_datastore_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5226 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/secret_manager.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       98 2022-08-24 18:15:10.000000 python-oauth-token-manager-0.2.0/pyproject.toml
+drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      670 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      620 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-08-24 18:09:16.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/not-zip-safe
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)       38 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/setup.cfg
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1498 2022-10-14 16:29:59.000000 python-oauth-token-manager-0.2.0/setup.py
```

### Comparing `python-oauth-token-manager-0.1.3/LICENSE` & `python-oauth-token-manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/PKG-INFO` & `python-oauth-token-manager-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: python-oauth-token-manager
-Version: 0.1.3
-Summary: API for managing stored OAuth credentials.
-Home-page: 
-Author: David Harcombe
-Author-email: david.harcombe@gmail.com
-License: Apache 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Library for storing OAuth credentials in many locations
 
 ## What's this for?
 
 By their very nature, OAuth credentials are valuable and dangerous, and have
 to be stored securely. As a result, the same tasks to store these tokens in a
 simple and secure fashion have to be written each time, or copied and pasted
```

### Comparing `python-oauth-token-manager-0.1.3/auth/__init__.py` & `python-oauth-token-manager-0.2.0/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/abstract_datastore.py` & `python-oauth-token-manager-0.2.0/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/credentials.py` & `python-oauth-token-manager-0.2.0/auth/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,15 @@
 
       if creds.expired:
         creds.expiry = expiry
         self._refresh_credentials(creds=creds)
 
     else:
       creds = None
-      raise CredentialsError(
-          message='credentials not found', email=self._email)
+      raise CredentialsError(f'credentials not found for user {self._email}')
 
     return creds
 
   @property
   def auth_headers(self) -> Dict[str, Any]:
     """Returns authorized http headers.
```

### Comparing `python-oauth-token-manager-0.1.3/auth/credentials_helpers.py` & `python-oauth-token-manager-0.2.0/auth/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.2.0/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/decorators.py` & `python-oauth-token-manager-0.2.0/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/decorators_test.py` & `python-oauth-token-manager-0.2.0/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/exceptions.py` & `python-oauth-token-manager-0.2.0/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/firestore.py` & `python-oauth-token-manager-0.2.0/auth/firestore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/gcs_datastore.py` & `python-oauth-token-manager-0.2.0/auth/gcs_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/gcs_datastore_test.py` & `python-oauth-token-manager-0.2.0/auth/gcs_datastore_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/local_datastore.py` & `python-oauth-token-manager-0.2.0/auth/local_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/local_datastore_test.py` & `python-oauth-token-manager-0.2.0/auth/local_datastore_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.1.3/auth/secret_manager.py` & `python-oauth-token-manager-0.2.0/auth/secret_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from __future__ import annotations
 
 import json
 from typing import Any, List, Mapping, Optional, Type
 
 from google.cloud import secretmanager, secretmanager_v1
 from google.cloud.secretmanager_v1.types import resources
-from google.cloud.secretmanager_v1.services.secret_manager_service import pagers
 
 from . import decorators
 from .abstract_datastore import AbstractDatastore
 
 
 class SecretManager(AbstractDatastore):
 
@@ -57,15 +56,15 @@
                                                    secret_id=id)
     response = self.client.create_secret(request=request)
 
     return response
 
   @decorators.implicit_create(creator=create_secret)
   def store_document(self,  id: str, document: Mapping[str, Any],
-                     type: Optional[Type] = None) -> resources.SecretVersion:
+                     type: Optional[Type] = None) -> None:
     """Stores a document.
 
     Store a document in Secret Manager. This will, for credentials, always be
     the OAuth token.
 
     Arguments:
         id (str): The document id.
@@ -73,47 +72,29 @@
         type (Optional[Type]): Unused.
     """
     payload = secretmanager_v1.SecretPayload(
         data=json.dumps(document).encode('utf-8'))
     request = secretmanager_v1.AddSecretVersionRequest(
         parent=self.client.secret_path(self._project, id),
         payload=payload)
-    return self.client.add_secret_version(request=request)
+    self.client.add_secret_version(request=request)
 
   def update_document(self, id: str, new_data: Mapping[str, Any],
                       type: Optional[Type] = None) -> None:
     """Updates a document.
 
     Update a document in Secret Manager. If the document is not already there,
     it will be created as a net-new document. If it is, it will be updated.
 
-    As this is a specific 'update' request, remove any other enabled versions.
-
     Args:
         id (str): the id of the document.
         new_data (Dict[str, Any]): the document content.
         type (Optional[Type]): Unused.
     """
-    new_version = self.store_document(id=id, type=type, document=new_data)
-
-    # Destroy other versions
-    request = secretmanager_v1.ListSecretVersionsRequest(
-        parent=self.client.secret_path(project=self._project, secret=id),
-        filter='state:enabled'
-    )
-    version_list = self.client.list_secret_versions(request=request)
-    for page in version_list.pages:
-      for version in page.versions:
-        if version == new_version:
-          continue
-        else:
-          self.client.destroy_secret_version(
-              secretmanager_v1.DestroySecretVersionRequest(
-                  name=version.name
-              ))
+    self.store_document(id=id, type=type, document=new_data)
 
   def get_document(self, id: str, type: Optional[Type] = None,
                    key: Optional[str] = None) -> Mapping[str, Any]:
     """Fetches a document (could be anything).
 
     Fetch a document
```

### Comparing `python-oauth-token-manager-0.1.3/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 auth/local_datastore.py
 auth/local_datastore_test.py
 auth/secret_manager.py
 python_oauth_token_manager.egg-info/PKG-INFO
 python_oauth_token_manager.egg-info/SOURCES.txt
 python_oauth_token_manager.egg-info/dependency_links.txt
 python_oauth_token_manager.egg-info/not-zip-safe
-python_oauth_token_manager.egg-info/requires.txt
 python_oauth_token_manager.egg-info/top_level.txt
```


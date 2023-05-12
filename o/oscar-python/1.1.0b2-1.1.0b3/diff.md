# Comparing `tmp/oscar_python-1.1.0b2.tar.gz` & `tmp/oscar_python-1.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscar_python-1.1.0b2.tar", last modified: Thu May 11 09:07:42 2023, max compression
+gzip compressed data, was "oscar_python-1.1.0b3.tar", last modified: Fri May 12 07:34:23 2023, max compression
```

## Comparing `oscar_python-1.1.0b2.tar` & `oscar_python-1.1.0b3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/oscar_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/oscar_python/_providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_onedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_providers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/oscar_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:34:23.670017 oscar_python-1.1.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-12 07:34:23.670017 oscar_python-1.1.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:34:23.666017 oscar_python-1.1.0b3/oscar_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:34:23.670017 oscar_python-1.1.0b3/oscar_python/_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/_providers/_minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/_providers/_onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/_providers/_providers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/_providers/_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/_providers/_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/oscar_python/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:34:23.666017 oscar_python-1.1.0b3/oscar_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-12 07:34:23.000000 oscar_python-1.1.0b3/oscar_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-12 07:34:23.000000 oscar_python-1.1.0b3/oscar_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:34:23.000000 oscar_python-1.1.0b3/oscar_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:34:23.000000 oscar_python-1.1.0b3/oscar_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 07:34:23.000000 oscar_python-1.1.0b3/oscar_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 07:34:23.000000 oscar_python-1.1.0b3/oscar_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:34:23.670017 oscar_python-1.1.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-12 07:34:11.000000 oscar_python-1.1.0b3/setup.py
```

### Comparing `oscar_python-1.1.0b2/LICENSE` & `oscar_python-1.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/PKG-INFO` & `oscar_python-1.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscar_python
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oscar_python-1.1.0b2/README.md` & `oscar_python-1.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python/_providers/_minio.py` & `oscar_python-1.1.0b3/oscar_python/_providers/_minio.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python/_providers/_onedata.py` & `oscar_python-1.1.0b3/oscar_python/_providers/_onedata.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python/_providers/_providers_base.py` & `oscar_python-1.1.0b3/oscar_python/_providers/_providers_base.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python/_providers/_s3.py` & `oscar_python-1.1.0b3/oscar_python/_providers/_s3.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python/_providers/_webdav.py` & `oscar_python-1.1.0b3/oscar_python/_providers/_webdav.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python/_utils.py` & `oscar_python-1.1.0b3/oscar_python/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 
 """ Function to generate headers with basic authentication or OIDC """
 def get_headers(c):
     if c._AUTH_TYPE == "basicauth":
         usr_pass_as_bytes = bytes(c.user+":"+c.password,"utf-8")
         usr_pass_base_64 = base64.b64encode(usr_pass_as_bytes).decode("utf-8")
         return {"Authorization": "Basic "+ usr_pass_base_64}
-    if c._AUTH_TYPE == "oidc":
+    if c._AUTH_TYPE == "oidc-agent":
         token = agent.get_access_token(c.shortname)
         return get_headers_with_token(token)
+    if c._AUTH_TYPE == "oidc":
+        return get_headers_with_token(c.oidc_token)
 
 """ Function to generate headers with token auth """
 def get_headers_with_token(token):
     return {"Authorization": "Bearer "+ str(token)}
 
 def write_text_file(content, file_path):
     with open(file_path, 'w') as f:
```

### Comparing `oscar_python-1.1.0b2/oscar_python/client.py` & `oscar_python-1.1.0b3/oscar_python/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 import json
 import yaml
 import liboidcagent as agent
-import oscar_python._utils as utils
+#import oscar_python._utils as utils
+import _utils as utils
 from oscar_python.storage import Storage
 
 _INFO_PATH = "/system/info"
 _CONFIG_PATH = "/system/config"
 _SVC_PATH = "/system/services"
 _LOGS_PATH = "/system/logs"
 _RUN_PATH = "/run"
@@ -34,39 +35,49 @@
 
 class Client:
     #Cluster info 
     def __init__(self, options) -> None:
         self.set_auth_type(options)
         if self._AUTH_TYPE == 'basicauth':
             self.basic_auth_client(options)
+        if self._AUTH_TYPE == 'oidc-agent':
+            self.oidc_agent_client(options)
         if self._AUTH_TYPE == 'oidc':
             self.oidc_client(options)
 
     def basic_auth_client(self, options):
         self.id = options['cluster_id']
         self.endpoint = options['endpoint']
         self.user = options['user']
         self.password = options['password']
         self.ssl = bool(options['ssl'])
 
-    def oidc_client(self, options):
+    def oidc_agent_client(self, options):
         self.id = options['cluster_id']
         self.endpoint = options['endpoint']
         self.shortname = options['shortname']
         self.ssl = bool(options['ssl'])
+    
+    def oidc_client(self, options):
+        self.id = options['cluster_id']
+        self.endpoint = options['endpoint']
+        self.oidc_token = options['oidc_token']
+        self.ssl = bool(options['ssl'])
 
     def set_auth_type(self, options):
         if 'user' in options:
             self._AUTH_TYPE = "basicauth"
         elif 'shortname' in options:
-            self._AUTH_TYPE = "oidc"
+            self._AUTH_TYPE = "oidc-agent"
             try:
                 agent.get_access_token(options['shortname'])
             except agent.OidcAgentError as e:
                 print("ERROR oidc-agent: {}".format(e))
+        elif 'oidc_token' in options:
+            self._AUTH_TYPE == "oidc"
         else:
             raise ValueError("Unrecognized authentication credentials in options")
 
     """ Creates a generic storage client to interact with the storage providers 
     defined on a specific service of the refered OSCAR cluster """
     def create_storage_client(self, svc):
         return Storage(
```

### Comparing `oscar_python-1.1.0b2/oscar_python/storage.py` & `oscar_python-1.1.0b3/oscar_python/storage.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/oscar_python.egg-info/PKG-INFO` & `oscar_python-1.1.0b3/oscar_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscar-python
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oscar_python-1.1.0b2/oscar_python.egg-info/SOURCES.txt` & `oscar_python-1.1.0b3/oscar_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b2/setup.py` & `oscar_python-1.1.0b3/setup.py`

 * *Files identical despite different names*


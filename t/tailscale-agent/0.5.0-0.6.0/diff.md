# Comparing `tmp/tailscale_agent-0.5.0.tar.gz` & `tmp/tailscale_agent-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailscale_agent-0.5.0.tar", max compression
+gzip compressed data, was "tailscale_agent-0.6.0.tar", max compression
```

## Comparing `tailscale_agent-0.5.0.tar` & `tailscale_agent-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1071 2022-07-06 20:22:15.735438 tailscale_agent-0.5.0/LICENSE
--rw-r--r--   0        0        0      148 2022-07-06 20:38:28.861728 tailscale_agent-0.5.0/README.md
--rw-r--r--   0        0        0      512 2022-10-26 17:40:00.109614 tailscale_agent-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-07-06 20:22:56.189715 tailscale_agent-0.5.0/tailscale_agent/__init__.py
--rw-r--r--   0        0        0    13853 2022-10-26 17:35:39.093440 tailscale_agent-0.5.0/tailscale_agent/tailscale_agent.py
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 tailscale_agent-0.5.0/setup.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 tailscale_agent-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-07-06 20:22:15.735438 tailscale_agent-0.6.0/LICENSE
+-rw-r--r--   0        0        0      148 2022-07-06 20:38:28.861728 tailscale_agent-0.6.0/README.md
+-rw-r--r--   0        0        0      512 2023-05-12 14:44:06.148074 tailscale_agent-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-07-06 20:22:56.189715 tailscale_agent-0.6.0/tailscale_agent/__init__.py
+-rw-r--r--   0        0        0    15148 2023-05-12 18:56:18.092910 tailscale_agent-0.6.0/tailscale_agent/tailscale_agent.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 tailscale_agent-0.6.0/PKG-INFO
```

### Comparing `tailscale_agent-0.5.0/LICENSE` & `tailscale_agent-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tailscale_agent-0.5.0/pyproject.toml` & `tailscale_agent-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailscale_agent"
-version = "0.5.0"
+version = "0.6.0"
 description = "Python Bindings for the TailScal API"
 authors = ["Kevin Bringard <kevin.bringard@phreesia.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/kevinbringard/tailscale-python-client/"
 include = [
     "LICENSE",
```

### Comparing `tailscale_agent-0.5.0/tailscale_agent/tailscale_agent.py` & `tailscale_agent-0.6.0/tailscale_agent/tailscale_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -373,16 +373,17 @@
 
         url = f'{self._base_url}/tailnet/{self._tailnet}/dns/searchpaths'
 
         response = requests.get(url, auth=self._auth, headers=self._headers, data=dns_searchpaths_data)
 
         return(response)
 
+
     # Logs related methods
-    def get_logs(self, starttime, endtime):
+    def get_audit_logs(self, starttime, endtime):
         """
         Get Audit logs from the logs/ API endpoint.
 
         You *must* specify a start time and an end time to scope the query, and they
         *must* be in the format "1990-01-01T00:00:00Z" or the API will reject it as
         invalid
 
@@ -395,14 +396,43 @@
 
         url = f'{self._base_url}/tailnet/{self._tailnet}/logs?start={starttime}&end={endtime}'
 
         response = requests.get(url, auth=self._auth, headers=self._headers)
 
         return response
 
+    # Create an alias for backward compatibility
+    # This will be deprecated at some point in the future
+    get_logs = get_audit_logs
+
+
+    def get_network_logs(self, starttime, endtime):
+        """
+
+        Get Network Audit logs from the network-logs/ API endpoint.
+
+        You *must* specify a start time and an end time to scope the query, and they
+        *must* be in the format "1990-01-01T00:00:00Z" or the API will reject it as
+        invalid
+
+        You must also have network flow logs enabled in the logs section of your tailnet's admin console
+
+        :param starttime: Start time in ISO-8601 format. For example: 1990-01-01T00:00:00Z
+        :param endtime: End time in ISO-8601 format. For example: 1991-01-01T00:00:00Z
+
+        :return: requests response object, or None if the date strings are invalid
+
+        """
+
+        url = f'{self._base_url}/tailnet/{self._tailnet}/network-logs?start={starttime}&end={endtime}'
+
+        response = requests.get(url, auth=self._auth, headers=self._headers)
+
+        return response
+
 
     # OAuth token support
     def get_oauth_token(self, client_id, client_secret, client_embed=True):
         """
         Use a static oauth client id and secret to generate scoped API tokens
 
         https://tailscale.com/kb/1215/oauth-clients/
@@ -427,12 +457,17 @@
         url = f'https://api.tailscale.com/api/v2/oauth/token'
 
         response = requests.post(url, headers=self._headers, data=oauth_client_data)
 
         if not client_embed:
             return response
 
-        access_token = response.json()['access_token']
-        self._api_key = access_token
-        self._auth = HTTPBasicAuth(access_token, '')
+        try:
+            access_token = response.json()['access_token']
+            self._api_key = access_token
+            self._auth = HTTPBasicAuth(access_token, '')
+        except:
+            print ('I was not able to set the access token.')
+            print ('Please ensure you have your OAuth client set '
+                  'correctly and it has the necessary permissions.')
 
-        return response
+        return response
```

### Comparing `tailscale_agent-0.5.0/PKG-INFO` & `tailscale_agent-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailscale-agent
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python Bindings for the TailScal API
 Home-page: https://github.com/kevinbringard/tailscale-python-client/
 License: MIT
 Author: Kevin Bringard
 Author-email: kevin.bringard@phreesia.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


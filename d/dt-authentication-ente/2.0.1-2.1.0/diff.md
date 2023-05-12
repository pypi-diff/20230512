# Comparing `tmp/dt-authentication-ente-2.0.1.tar.gz` & `tmp/dt-authentication-ente-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-authentication-ente-2.0.1.tar", last modified: Sun May  7 18:43:22 2023, max compression
+gzip compressed data, was "dt-authentication-ente-2.1.0.tar", last modified: Fri May 12 04:20:00 2023, max compression
```

## Comparing `dt-authentication-ente-2.0.1.tar` & `dt-authentication-ente-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:43:22.246346 dt-authentication-ente-2.0.1/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.0.1/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-07 18:43:22.246346 dt-authentication-ente-2.0.1/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.0.1/README.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-05-07 18:43:22.246346 dt-authentication-ente-2.0.1/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2299 2023-05-07 18:37:07.000000 dt-authentication-ente-2.0.1/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:43:22.246346 dt-authentication-ente-2.0.1/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:43:22.246346 dt-authentication-ente-2.0.1/src/dt_authentication/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      153 2023-05-07 18:43:20.000000 dt-authentication-ente-2.0.1/src/dt_authentication/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2545 2023-05-07 18:36:38.000000 dt-authentication-ente-2.0.1/src/dt_authentication/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2023-05-07 18:35:09.000000 dt-authentication-ente-2.0.1/src/dt_authentication/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.0.1/src/dt_authentication/scope.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8461 2023-05-07 18:42:51.000000 dt-authentication-ente-2.0.1/src/dt_authentication/token.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-07 07:29:27.000000 dt-authentication-ente-2.0.1/src/dt_authentication/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:43:22.246346 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-07 18:43:22.000000 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-05-07 18:43:22.000000 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-05-07 18:43:22.000000 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      127 2023-05-07 18:43:22.000000 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       13 2023-05-07 18:43:22.000000 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-05-07 18:43:22.000000 dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.0/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.0/README.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2299 2023-05-07 18:37:07.000000 dt-authentication-ente-2.1.0/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.485245 dt-authentication-ente-2.1.0/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.485245 dt-authentication-ente-2.1.0/src/dt_authentication/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      153 2023-05-12 04:19:55.000000 dt-authentication-ente-2.1.0/src/dt_authentication/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2545 2023-05-12 03:53:49.000000 dt-authentication-ente-2.1.0/src/dt_authentication/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2023-05-07 18:35:09.000000 dt-authentication-ente-2.1.0/src/dt_authentication/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.0/src/dt_authentication/scope.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10981 2023-05-12 04:00:36.000000 dt-authentication-ente-2.1.0/src/dt_authentication/token.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-07 07:29:27.000000 dt-authentication-ente-2.1.0/src/dt_authentication/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      127 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       13 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/top_level.txt
```

### Comparing `dt-authentication-ente-2.0.1/setup.py` & `dt-authentication-ente-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.0.1/src/dt_authentication/cli.py` & `dt-authentication-ente-2.1.0/src/dt_authentication/cli.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.0.1/src/dt_authentication/scope.py` & `dt-authentication-ente-2.1.0/src/dt_authentication/scope.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.0.1/src/dt_authentication/token.py` & `dt-authentication-ente-2.1.0/src/dt_authentication/token.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     "dt1": "%Y-%m-%d",
     "dt2": "%Y-%m-%d/%H:%M"
 }
 
 PAYLOAD_FIELDS = {"uid", "exp"}
 CURVE = NIST192p
 SUPPORTED_VERSIONS = ["dt1", "dt2"]
+SUPPORTED_FIELDS = {
+    "dt1": [],
+    "dt2": ["scope", "data", "duration"],
+}
 DEFAULT_VERSION = "dt2"
 
 
 ScopeList = List[Union[Scope, str]]
 DEFAULT_SCOPE = [Scope(action="auth")]
 
 
@@ -95,14 +99,35 @@
     def scope(self) -> List[Scope]:
         """
         The scope of this token.
         """
         return self._payload.get("scope", DEFAULT_SCOPE)
 
     @property
+    def data(self) -> Optional[dict]:
+        """
+        The data baked into the token.
+        """
+        return self._payload.get("data", None)
+
+    @property
+    def duration(self) -> Optional[int]:
+        """
+        The duration of the token in minutes.
+        """
+        return self._payload.get("duration", None)
+
+    @property
+    def renewable(self) -> bool:
+        """
+        Whether the token can be renewed.
+        """
+        return self.duration is not None
+
+    @property
     def expiration(self) -> Optional[datetime.datetime]:
         """
         The token's expiration date.
         """
         if self._payload['exp'] is None:
             return None
         return datetime.datetime.strptime(self._payload['exp'], DATETIME_FORMAT[self._version])
@@ -143,14 +168,29 @@
     def grants(self, action: str, resource: Optional[str] = None, identifier: Optional[str] = None,
                service: Optional[str] = None) -> bool:
         for s in self.scope:
             if s.grants(action, resource, identifier, service):
                 return True
         return False
 
+    def renew(self, key: SigningKey):
+        # make sure the token is renewable
+        if not self.renewable:
+            raise ValueError("This token is not renewable")
+        # generate new token
+        return self.generate(
+            key,
+            self.uid,
+            minutes=self.duration,
+            renewable=True,
+            data=self.data,
+            scope=self.scope,
+            version=self.version,
+        )
+
     @staticmethod
     def from_string(s: str, vk: Optional[VerifyingKey] = None, allow_expired: bool = True) \
             -> 'DuckietownToken':
         """
         Decodes a Duckietown Token string into an instance of
         :py:class:`dt_authentication.DuckietownToken`.
 
@@ -200,39 +240,84 @@
         # make sure the token is not expired
         if not allow_expired and token.expired:
             raise ExpiredToken("This token is expired. Obtain a new one.")
         # ---
         return token
 
     @classmethod
-    def generate(cls, key: SigningKey, user_id: int, days: int = 365, hours: int = 0, minutes: int = 0,
-                 scope: ScopeList = None, version: str = DEFAULT_VERSION) -> 'DuckietownToken':
-        if scope is None:
-            scope = DEFAULT_SCOPE
-        # make sure the scope is valid
-        if not isinstance(scope, list):
-            raise ValueError("Argument 'scope' must be a list")
-        scope_parsed: List[Scope] = []
-        scope_encoded: List[Union[str, dict]] = []
-        for s in scope:
-            if not isinstance(s, Scope):
-                s = Scope.parse(s)
-            scope_parsed.append(s)
-            scope_encoded.append(s.compact())
+    def generate(cls, key: SigningKey, user_id: int, *,
+                 # duration
+                 days: int = 0, hours: int = 0, minutes: int = 0,
+                 # payload
+                 renewable: bool = False, data: Optional[dict] = None, scope: ScopeList = None,
+                 # metadata
+                 version: str = DEFAULT_VERSION) -> 'DuckietownToken':
+        # get supported fields for version
+        fields = SUPPORTED_FIELDS[version]
         # compute expiration date
         exp = None
         if (days + hours + minutes) > 0:
             now = datetime.datetime.now()
             delta = datetime.timedelta(days=days, hours=hours, minutes=minutes)
             exp = (now + delta).strftime(DATETIME_FORMAT[version])
-        # form payload
-        payload = {"uid": user_id, "scope": scope_encoded, "exp": exp}
+        # initialize payload
+        payload = {
+            "uid": user_id,
+            "exp": exp
+        }
+        # - scope
+        if "scope" in fields:
+            # sanitize scope
+            if scope is None:
+                scope = DEFAULT_SCOPE
+            else:
+                # a scope list is given, prepend the default scope to it
+                for s in DEFAULT_SCOPE:
+                    if s not in scope:
+                        scope = [s] + scope
+            # make sure the scope is valid
+            if not isinstance(scope, list):
+                raise ValueError("Argument 'scope' must be a list")
+            scope_parsed: List[Scope] = []
+            scope_encoded: List[Union[str, dict]] = []
+            for s in scope:
+                if not isinstance(s, Scope):
+                    s = Scope.parse(s)
+                scope_parsed.append(s)
+                scope_encoded.append(s.compact())
+            # ---
+            # noinspection PyTypedDict
+            payload["scope"] = scope_encoded
+
+        # - data
+        if "data" in fields:
+            # check data
+            if data is not None:
+                if not isinstance(data, dict):
+                    raise ValueError("Argument 'data' must be a dictionary")
+                try:
+                    json.dumps(data)
+                except TypeError:
+                    raise ValueError("The given 'data' is not JSON-serializable")
+                # ---
+                payload["data"] = data
+
+        # - duration
+        if "duration" in fields:
+            # add duration (only if renewable)
+            if renewable:
+                payload["duration"] = days * 1440 + hours * 60 + minutes
 
         def entropy(numbytes):
             e = b"duckietown is a place of relaxed introspection, and hub extends this place a lot"
             return e[:numbytes]
 
+        # compile payload
         payload_bytes = str.encode(json.dumps(payload, sort_keys=True))
         signature = key.sign(payload_bytes, entropy=entropy)
 
-        payload["scope"] = scope_parsed
+        # - scope
+        if "scope" in fields:
+            # noinspection PyUnboundLocalVariable
+            payload["scope"] = scope_parsed
+
         return DuckietownToken(version, payload, signature)
```

### Comparing `dt-authentication-ente-2.0.1/src/dt_authentication/utils.py` & `dt-authentication-ente-2.1.0/src/dt_authentication/utils.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.0.1/src/dt_authentication_ente.egg-info/SOURCES.txt` & `dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/h2o_cloud_discovery-1.0.0rc1.tar.gz` & `tmp/h2o_cloud_discovery-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h2o_cloud_discovery-1.0.0rc1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `h2o_cloud_discovery-1.0.0rc1.tar` & `h2o_cloud_discovery-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-03-08 07:22:30.866139 h2o_cloud_discovery-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1904 2023-03-08 07:22:30.866139 h2o_cloud_discovery-1.0.0rc1/README.md
--rw-r--r--   0        0        0     1093 2023-03-08 07:22:49.470437 h2o_cloud_discovery-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1739 2023-03-08 07:22:30.866139 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/__init__.py
--rw-r--r--   0        0        0       28 2023-03-08 07:22:49.510438 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/_version.py
--rw-r--r--   0        0        0     2522 2023-03-08 07:22:30.870139 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/async_client.py
--rw-r--r--   0        0        0     2800 2023-03-08 07:22:30.870139 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/client.py
--rw-r--r--   0        0        0     2175 2023-03-08 07:22:30.870139 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/discovery.py
--rw-r--r--   0        0        0     1282 2023-03-08 07:22:30.870139 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/lookup.py
--rw-r--r--   0        0        0     3613 2023-03-08 07:22:30.870139 h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/model.py
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 h2o_cloud_discovery-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.flake8
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.release-please-manifest.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/SECURITY.md
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/pydoc-markdown.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/release-please-config.json
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/api-docs-release.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/python-lint.yml
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/src/h2o_discovery/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/src/h2o_discovery/_version.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/src/h2o_discovery/model.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/src/h2o_discovery/_internal/client.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/src/h2o_discovery/_internal/load.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/src/h2o_discovery/_internal/lookup.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/tests/test_model.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/tests/test_version.py
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/tests/_internal/test_client.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/tests/_internal/test_load.py
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/tests/_internal/test_lookup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/README.md
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.0.1/PKG-INFO
```

### Comparing `h2o_cloud_discovery-1.0.0rc1/LICENSE` & `h2o_cloud_discovery-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.0.0rc1/README.md` & `h2o_cloud_discovery-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/__init__.py` & `h2o_cloud_discovery-1.0.1/src/h2o_discovery/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import Optional
 
-from h2o_discovery import async_client
-from h2o_discovery import discovery
-from h2o_discovery import lookup
-from h2o_discovery import client
-
+from h2o_discovery import model
+from h2o_discovery._internal import client
+from h2o_discovery._internal import load
+from h2o_discovery._internal import lookup
 from h2o_discovery._version import __version__  # noqa: F401
 
-
-Discovery = discovery.Discovery
+Discovery = model.Discovery
 
 
 def discover(
     environment: Optional[str] = None, discovery_address: Optional[str] = None
 ) -> Discovery:
     """Obtains and returns a Discovery object from the discovery service.
 
@@ -23,15 +21,15 @@
     Args:
         environment: The H2O Cloud environment URL to use (e.g. https://cloud.h2o.ai).
         discovery_address: The address of the discovery service.
 
     """
     uri = lookup.determine_uri(environment, discovery_address)
     cl = client.Client(uri)
-    return Discovery.load(cl)
+    return load.load_discovery(cl)
 
 
 async def discover_async(
     environment: Optional[str] = None, discovery_address: Optional[str] = None
 ) -> Discovery:
     """Obtains and returns a Discovery object from the discovery service.
 
@@ -41,9 +39,9 @@
 
     Args:
         environment: The H2O Cloud environment URL to use (e.g. https://cloud.h2o.ai).
         discovery_address: The address of the discovery service.
 
     """
     uri = lookup.determine_uri(environment, discovery_address)
-    cl = async_client.AsyncClient(uri)
-    return await Discovery.load_async(cl)
+    cl = client.AsyncClient(uri)
+    return await load.load_discovery_async(cl)
```

### Comparing `h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/discovery.py` & `h2o_cloud_discovery-1.0.1/src/h2o_discovery/_internal/load.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,31 @@
-import dataclasses
 import types
 from typing import Iterable
 from typing import Mapping
 
-from h2o_discovery import async_client
-from h2o_discovery import client
 from h2o_discovery import model
+from h2o_discovery._internal import client
 
 
-@dataclasses.dataclass(frozen=True)
-class Discovery:
-    """Representation of the discovery records."""
-
-    # Environment information.
-    environment: model.Environment
-
-    # Registered services.
-    services: Mapping[str, model.Service]
-
-    # Registered clients.
-    clients: Mapping[str, model.Client]
-
-    @classmethod
-    def load(cls, cl: client.Client) -> "Discovery":
-        """Loads the discovery records from the Discovery Service."""
-        environment = cl.get_environment()
-        services = _get_service_map(cl.list_services())
-        clients = _get_client_map(cl.list_clients())
-
-        return cls(environment=environment, services=services, clients=clients)
-
-    @classmethod
-    async def load_async(cls, cl: async_client.AsyncClient) -> "Discovery":
-        """Loads the discovery records from the Discovery Service."""
-        environment = await cl.get_environment()
-        services = _get_service_map(await cl.list_services())
-        clients = _get_client_map(await cl.list_clients())
+def load_discovery(cl: client.Client) -> model.Discovery:
+    """Loads the discovery records from the Discovery Service."""
+    environment = cl.get_environment()
+    services = _get_service_map(cl.list_services())
+    clients = _get_client_map(cl.list_clients())
 
-        return cls(environment=environment, services=services, clients=clients)
+    return model.Discovery(environment=environment, services=services, clients=clients)
+
+
+async def load_discovery_async(cl: client.AsyncClient) -> model.Discovery:
+    """Loads the discovery records from the Discovery Service."""
+    environment = await cl.get_environment()
+    services = _get_service_map(await cl.list_services())
+    clients = _get_client_map(await cl.list_clients())
+
+    return model.Discovery(environment=environment, services=services, clients=clients)
 
 
 def _get_service_map(services: Iterable[model.Service]) -> Mapping[str, model.Service]:
     out = {}
     for s in services:
         out[_service_key(s.name)] = s
     return types.MappingProxyType(out)
```

### Comparing `h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/lookup.py` & `h2o_cloud_discovery-1.0.1/src/h2o_discovery/_internal/lookup.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.0.0rc1/src/h2o_discovery/model.py` & `h2o_cloud_discovery-1.0.1/src/h2o_discovery/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import dataclasses
 from typing import Mapping
 from typing import Optional
 
 
 @dataclasses.dataclass(frozen=True)
 class Service:
-    """Internal representation of a registered service record."""
+    """Representation of a registered service record."""
 
-    # Name of the Service. For example: "services/my-service-name".
+    #: Name of the Service. For example: "services/my-service-name".
     name: str
 
-    # Name of the Service that can be displayed on the front-end.
+    #: Name of the Service that can be displayed on the front-end
     display_name: str
 
-    # URI for accessing the Service.
+    #: URI for accessing the Service.
+    #: This is usually the string that can be passed connection definition to the
+    #: client for the particular service.
     uri: str
 
-    # Version of the service. Can be the version of the API or the version of
-    # the service. Clients can utilize this information change their behavior
-    # in accessing the service or downloading the correct client version.
+    #: Version of the service.
+    #: Can be the version of the API or the version of
+    #: the service. Clients can utilize this information change their behavior
+    #: in accessing the service or downloading the correct client version.
     version: Optional[str]
 
-    # OAuth 2.0 Scope required to access the service. Clients request the
-    # access token with this scope in order to access the service. If the scope
-    # is not defined, clients should use h2o_cloud_platform_scope.
+    #: OAuth 2.0 Scope required to access the service.
+    #: Clients request the access token with this scope in order to access the service.
+    #: If the scope is not defined (or empty), clients should use
+    #: h2o_cloud_platform_scope.
     oauth2_scope: Optional[str]
 
-    # Requirement Specifier (PEP 508) for the Python client that can be used
-    # for accessing the service.
-    # Any string that can be `pip install`ed.
-    #
-    # Example: my-client==0.1.0
+    #: Requirement Specifier (PEP 508) for the Python client that can be used for
+    #: accessing the service.
+    #: Any string that can be `pip install`ed.
+    #:     Example: my-client==0.1.0
     python_client: Optional[str]
 
     @classmethod
     def from_json_dict(cls, json: Mapping[str, str]) -> "Service":
         """Create a Service from a JSON dict returned by the server."""
         return cls(
             name=json["name"],
@@ -44,59 +47,77 @@
             oauth2_scope=json.get("oauth2Scope"),
             python_client=json.get("pythonClient"),
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class Client:
-    """Internal representation of a registered client record."""
+    """Representation of a registered client record."""
 
-    # Name of the Client. For example: "clients/h2o-public-client".
+    #: Name of the Client. For example: "clients/h2o-public-client".
     name: str
 
-    # Name of the Client that can be displayed on the front-end.
+    #: Name of the Client that can be displayed on the front-end.
     display_name: str
 
-    # Public OAuth 2.0 client ID that the client needs to use to identify
-    # itself with the IDP.
+    #: Public OAuth 2.0 client ID that the client needs to use to identify
+    #: itself with the IDP.
     oauth2_client_id: str
 
     @classmethod
     def from_json_dict(cls, json: Mapping[str, str]) -> "Client":
         """Create a Client from a JSON dict returned by the server."""
         return cls(
             name=json["name"],
             display_name=json["displayName"],
             oauth2_client_id=json["oauth2ClientId"],
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class Environment:
-    """Internal representation of the environment."""
+    """Representation of the information about the H2O Cloud environment."""
 
-    # Identifier of the environment. For example: "https://cloud.h2o.ai".
-    # This is the base URL of the environment. Clients can use this to validate
-    # that they are talking to the correct environment.
+    #: Identifier of the environment. For example: "https://cloud.h2o.ai".
+    #: This is the base URL of the environment. Clients can use this to validate
+    #: that they are talking to the correct environment.
     h2o_cloud_environment: str
 
-    # OpenID Connect issuer_url. This is where clients find the OpenID Connect discovery
-    # on the well-known endpoint.
+    #: OpenID Connect issuer_url.
+    #: This is where clients find the OpenID Connect discovery on the well-known e
+    #: endpoint.
     issuer_url: str
 
-    # OAuth 2.0 scope that clients should use to access the H2O Cloud Platform.
-    # This is the default scope that clients should use if the service does not
-    # define its own scope.
+    #: OAuth 2.0 scope that clients should use to access the H2O Cloud Platform.
+    #: This is the default scope that clients should use if the service does not
+    #: define its own scope.
     h2o_cloud_platform_oauth2_scope: str
 
-    # Version of the H2O Cloud Platform release that is running in the environment.
+    #: Version of the H2O Cloud Platform release that is running in the environment.
+    #: In the XC YY.MM.V format for released versions (e.g. MC 23.04.01 for managed
+    #: cloud or HC 23.01.1 for hybrid cloud). Can be arbitrary string for
+    #: testing or special environments.
     h2o_cloud_version: Optional[str]
 
     @classmethod
     def from_json_dict(cls, json: Mapping[str, str]) -> "Environment":
         """Create an Environment from a JSON dict returned by the server."""
         return cls(
             h2o_cloud_environment=json["h2oCloudEnvironment"],
             issuer_url=json["issuerUrl"],
             h2o_cloud_platform_oauth2_scope=json["h2oCloudPlatformOauth2Scope"],
             h2o_cloud_version=json.get("h2oCloudVersion"),
         )
+
+
+@dataclasses.dataclass(frozen=True)
+class Discovery:
+    """Representation of the discovery records."""
+
+    #: Information about the environment.
+    environment: Environment
+
+    #: Map of registered services in the `{"service-identifier": Service(...)}` format.
+    services: Mapping[str, Service]
+
+    #: Map of registered clients in the `{"client-identifier": Client(...)}` format.
+    clients: Mapping[str, Client]
```

### Comparing `h2o_cloud_discovery-1.0.0rc1/PKG-INFO` & `h2o_cloud_discovery-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: h2o-cloud-discovery
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: H2O Cloud Discovery Python CLient
-License: Apache-2.0
-Author: H2O.ai
-Author-email: support@h2o.ai
-Requires-Python: >=3.7,<4.0
+Project-URL: Documentation, https://github.com/h2oai/cloud-discovery-py#readme
+Project-URL: Issues, https://github.com/h2oai/cloud-discovery-py/issues
+Project-URL: Source, https://github.com/h2oai/cloud-discovery-py
+Author-email: "H2O.ai" <support@h2o.ai>
+License-Expression: Apache-2.0
+License-File: LICENSE
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Dist: httpx (>=0.16)
+Requires-Python: >=3.7
+Requires-Dist: httpx>=0.16
 Description-Content-Type: text/markdown
 
 # `h2o-cloud-discovery`
 
 [![licence](https://img.shields.io/github/license/h2oai/cloud-discovery-py?style=flat-square)](https://github.com/h2oai/cloud-discovery-py/blob/main/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/h2o-cloud-discovery?style=flat-square)](https://pypi.org/project/h2o-cloud-discovery/)
 
@@ -84,8 +80,7 @@
         gateway_url=discovery.services["mlops-api"].uri,
         token_provider=token_provider,
     )
 
     ...
 
 ```
-
```


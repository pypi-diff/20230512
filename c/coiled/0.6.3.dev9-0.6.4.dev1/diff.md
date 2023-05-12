# Comparing `tmp/coiled-0.6.3.dev9.tar.gz` & `tmp/coiled-0.6.4.dev1.tar.gz`

## Comparing `coiled-0.6.3.dev9.tar` & `coiled-0.6.4.dev1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/context.py
--rw-r--r--   0        0        0   112031 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/magic.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/software.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/types.py
--rw-r--r--   0        0        0    47664 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    84970 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    60439 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/README.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/pyproject.toml
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 coiled-0.6.3.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/magic.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/software.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/types.py
+-rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    86022 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    60097 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.4.dev1/PKG-INFO
```

### Comparing `coiled-0.6.3.dev9/coiled/__init__.py` & `coiled-0.6.4.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/analytics.py` & `coiled-0.6.4.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cluster.py` & `coiled-0.6.4.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/coiled.yaml` & `coiled-0.6.4.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/context.py` & `coiled-0.6.4.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/core.py` & `coiled-0.6.4.dev1/coiled/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 When it comes to the Cluster class, this complexity is probably forced on us by distributed supporting sync and async.
 But for our own stuff (e.g. create_software_environment) we could probably simplify to a simpler sync-only API
 if we choose.
 """
 from __future__ import annotations, with_statement
 
 import asyncio
-import copy
 import datetime
 import json
 import logging
 import numbers
 import os
 import pathlib
 import platform
@@ -59,15 +58,14 @@
 
 import aiohttp
 import backoff
 import dask
 import dask.distributed
 import distributed
 import rich
-import yaml
 from distributed.comm import parse_address
 from distributed.utils import LoopRunner, sync
 from importlib_metadata import PackageNotFoundError, version
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from tornado.ioloop import IOLoop
@@ -93,15 +91,14 @@
     from typing_extensions import TypedDict
 
 from .compatibility import COILED_VERSION, DISTRIBUTED_VERSION, PY_VERSION
 from .context import COILED_SESSION_ID, TRACE_CONFIG, track_context
 from .types import (
     ArchitectureTypesEnum,
     CondaEnvSchema,
-    PiplessCondaEnvSchema,
     SoftwareEnvironmentAlias,
     SoftwareEnvSpec,
     event_type_list,
 )
 from .utils import (
     ALLOWED_PROVIDERS,
     COILED_LOGGER_NAME,
@@ -115,15 +112,15 @@
     parse_gcp_region_zone,
     parse_identifier,
     parse_requested_memory,
     rich_console,
     validate_account,
     verify_aws_credentials,
 )
-from .websockets import ConfigureBackendConnector, WebsocketConnector
+from .websockets import ConfigureBackendConnector
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 console = Console()
 SUPPORTED_BACKENDS = {"aws", "gcp"}
 
 
 class AWSSessionCredentials(TypedDict):
@@ -653,23 +650,17 @@
         self: Cloud[Sync],
         name: Optional[str] = None,
         *,
         account: Optional[str] = None,
         conda: Optional[Union[list, CondaEnvSchema, str, pathlib.Path]] = None,
         pip: Optional[Union[list, str, pathlib.Path]] = None,
         container: Optional[str] = None,
-        post_build: Optional[Union[list, str]] = None,
-        conda_env_name: Optional[str] = None,
-        backend_options: Optional[Dict] = None,
         log_output=sys.stdout,
-        private: bool = True,
         force_rebuild: bool = False,
-        environ: Optional[Dict] = None,
         use_entrypoint: bool = True,
-        new_build_backend: bool = True,
         wait_build: bool = True,
         gpu_enabled: bool = False,
         architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
     ) -> Optional[SoftwareEnvironmentAlias]:
         ...
 
     @overload
@@ -677,271 +668,120 @@
         self: Cloud[Async],
         name: Optional[str] = None,
         *,
         account: Optional[str] = None,
         conda: Optional[Union[list, CondaEnvSchema, str, pathlib.Path]] = None,
         pip: Optional[Union[list, str, pathlib.Path]] = None,
         container: Optional[str] = None,
-        post_build: Optional[Union[list, str]] = None,
-        conda_env_name: Optional[str] = None,
-        backend_options: Optional[Dict] = None,
         log_output=sys.stdout,
-        private: bool = True,
         force_rebuild: bool = False,
-        environ: Optional[Dict] = None,
         use_entrypoint: bool = True,
-        new_build_backend: bool = True,
         wait_build: bool = True,
         gpu_enabled: bool = False,
         architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
     ) -> Awaitable[Optional[SoftwareEnvironmentAlias]]:
         ...
 
     def create_software_environment(
         self: CloudSyncAsync,
         name: Optional[str] = None,
         *,
         account: Optional[str] = None,
         conda: Optional[Union[list, CondaEnvSchema, str, pathlib.Path]] = None,
         pip: Optional[Union[list, str, pathlib.Path]] = None,
         container: Optional[str] = None,
-        post_build: Optional[Union[list, str]] = None,
-        conda_env_name: Optional[str] = None,
-        backend_options: Optional[Dict] = None,
         log_output=sys.stdout,
-        private: bool = True,
         force_rebuild: bool = False,
-        environ: Optional[Dict] = None,
         use_entrypoint: bool = True,
-        new_build_backend: bool = True,
         wait_build: bool = True,
         gpu_enabled: bool = False,
         architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
     ) -> Union[Awaitable[Optional[SoftwareEnvironmentAlias]], Optional[SoftwareEnvironmentAlias],]:
         return self._sync(
             self._create_software_environment,
             name=name,
             account=account,
             conda=conda,
             pip=pip,
             container=container,
-            post_build=post_build,
             log_output=log_output,
-            conda_env_name=conda_env_name,
-            backend_options=backend_options,
-            private=private,
             force_rebuild=force_rebuild,
-            environ=environ,
             use_entrypoint=use_entrypoint,
-            new_build_backend=new_build_backend,
             wait_build=wait_build,
             gpu_enabled=gpu_enabled,
             architecture=architecture,
         )
 
     @track_context
     async def _create_software_environment(
         self,
         name: Optional[str] = None,
         *,
         account: Optional[str] = None,
         conda: Union[CondaEnvSchema, str, pathlib.Path, list, None] = None,
         pip: Union[List[str], str, pathlib.Path, None] = None,
         container: Optional[str] = None,
-        post_build=None,
-        conda_env_name: Optional[str] = None,
         log_output=sys.stdout,
-        backend_options: Optional[Dict] = None,
-        private: bool = True,
         force_rebuild: bool = False,
-        environ: Optional[Dict] = None,
         use_entrypoint: bool = True,
-        new_build_backend: bool = True,
         wait_build: bool = True,
         gpu_enabled: bool = False,
         architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
     ) -> Optional[SoftwareEnvironmentAlias]:
-        """
-        :param name:
-        :param conda:
-        :param pip:
-        :param container:
-        :param post_build:
-        :param conda_env_name:
-        :param log_output:
-        :param backend_options: Dict or None
-          backend_options["container_registry"]
-        :param private:
-        :param force_rebuild:
-        :param environ: Dict or None
-        :return:
-        """
-        session = self._ensure_session()
         if name is None and conda is not None and isinstance(conda, dict) and "name" in conda:
             name = conda["name"]
 
         if name is None:
             raise ValueError("Must provide a name when creating a software environment")
 
         account, name = self._normalize_name(str(name), context_account=account, raise_on_account_conflict=True)
 
-        if new_build_backend and post_build:
-            raise TypeError("The build backend does not support post build commands")
-        if new_build_backend and conda_env_name:
-            raise TypeError("The build backend does not support custom conda environment names")
-        if new_build_backend and (pip or conda) and container:
-            raise TypeError("The build backend does not support public software environments")
-
-        if new_build_backend and not private:
-            raise TypeError("The build backend does not support public software environments")
-        if new_build_backend and environ:
-            raise TypeError("The build backend does not support specifying env vars")
-        if new_build_backend:
-            if conda or pip:
-                senv = await create_env_spec(conda=conda, pip=pip)
-            else:
-                senv = None
-            logger.info("Creating software environment")
-            alias = await self._create_software_environment_v2(
-                senv=senv,
-                container=container,
-                name=name,
-                account=account,
-                force_rebuild=force_rebuild,
-                use_entrypoint=use_entrypoint,
-                gpu_enabled=gpu_enabled,
-                architecture=architecture,
-            )
-            if wait_build and alias:
-                # pyright complains unless we nest like this
-                # only tail software environments that have builds
-                if alias.get("latest_spec"):
-                    assert alias["latest_spec"]
-                    spec = alias["latest_spec"]
-                    if spec.get("latest_build"):
-                        assert spec["latest_build"]
-                        build = spec["latest_build"]
-                        if build["state"] == "built":
-                            logger.info("Software environment already built")
-                        else:
-                            log_output.write("--- Logs from remote build follow ---\n")
-                            final_state = await self._tail_software_build_logs(
-                                build["id"], account=account, log_output=log_output
-                            )
-                            info_url = (
-                                self.server + f"/software/alias/{alias['id']}"
-                                f"/build/{build['id']}?account={account}&tab=logs"
-                            )
-                            log_output.write(f"--- Logs end, may be truncated, see {info_url} for full output ---\n")
-                            if final_state == "error":
-                                raise BuildError("The software environment failed to build")
-                logger.info("Software environment created")
-            return alias
-        conda_parsed: Optional[CondaEnvSchema] = None
-        if conda is None and container is None and pip is not None:
-            v = ".".join(map(str, sys.version_info[:2]))
-            conda_parsed = {"dependencies": [f"python={v}", {"pip": []}]}
-        elif isinstance(conda, list):
-            conda_parsed = {"dependencies": conda}
-        elif isinstance(conda, (str, pathlib.Path)):
-            if not os.path.isfile(conda):
-                raise FileNotFoundError(
-                    f"Unable to find file '{conda}', please make sure it exists "
-                    "and the path is correct. If you are trying to create a "
-                    "software environment by specifying dependencies, you can "
-                    "do so by passing a list of dependencies or a dictionary. For example:\n"
-                    "\tcoiled.create_software_environment(\n"
-                    "\t    name='my-env', conda={'channels': ['conda-forge'], 'dependencies': ['coiled']}\n"
-                    "\t)"
-                )
-            else:
-                # Local conda environment YAML file
-                with open(conda, mode="r") as f:
-                    conda_parsed = yaml.safe_load(f)
-        else:
-            conda_parsed = conda
-        pip_parsed: Optional[List[str]] = None
-        if isinstance(pip, (str, pathlib.Path)):
-            if not os.path.isfile(pip):
-                raise FileNotFoundError(
-                    f"Unable to find file '{pip}', please make sure it exists "
-                    "and the path is correct. If you are trying to create a "
-                    "software environment by specifying dependencies, you can "
-                    "do so by passing a list of dependencies. For example:\n"
-                    "\tcoiled.create_software_environment(\n"
-                    "\t    name='my-env', pip=['coiled']\n"
-                    "\t)"
-                )
-            else:
-                # Local pip requirements file
-                with open(pip, mode="r") as f:
-                    pip_parsed = f.read().splitlines()
-        else:
-            pip_parsed = pip
-
-        if isinstance(post_build, (str, pathlib.Path)):
-            # Post-build script
-            with open(post_build, mode="r") as f:
-                post_build = f.read().splitlines()
-
-        # Conda supports specifying pip packages via their CLI, but not when
-        # using conda.api.Solver. So we move any pip packages to the pip portion
-        # of this software environment
-        pip_extracted_conda: Optional[PiplessCondaEnvSchema] = None
-        if conda_parsed is not None and "dependencies" in conda_parsed:
-            for _, dep in enumerate(conda_parsed["dependencies"]):
-                if isinstance(dep, dict) and list(dep.keys()) == ["pip"]:
-                    # Copy conda to avoid mutating input from users
-                    temp = copy.deepcopy(conda_parsed)
-                    temp["dependencies"].remove(dep)
-                    if pip_parsed:
-                        pip_parsed.extend(dep["pip"])
-                    else:
-                        pip_parsed = dep["pip"]
-                    pip_extracted_conda = cast(PiplessCondaEnvSchema, temp)
-            if not pip_extracted_conda:
-                pip_extracted_conda = cast(PiplessCondaEnvSchema, conda_parsed)
-
-        # Remove duplicates and ensure consistent package ordering which helps with
-        # downstream tokenization of package spec
-        if pip_parsed is not None:
-            pip_parsed = sorted(set(pip_parsed))
-        if pip_extracted_conda is not None and "dependencies" in pip_extracted_conda:
-            pip_extracted_conda["dependencies"] = sorted(set(pip_extracted_conda["dependencies"]))
-
-        # Connect to the websocket, send the data and get some logs
-        data = {
-            "type": "build",
-            "container": container,
-            "conda": pip_extracted_conda,
-            "conda_env_name": conda_env_name,
-            "pip": pip_parsed,
-            "post_build": post_build,
-            "options": {**self._default_backend_options, **(backend_options or {})},
-            "private": private,
-            "force_rebuild": force_rebuild,
-            "environ": environ or {},
-            "use_entrypoint": use_entrypoint,
-        }
+        if (pip or conda) and container:
+            raise TypeError("The build backend does not support specifying both packages and a container")
 
-        ws_server = self.server.replace("http", "ws", 1)
-
-        ws = WebsocketConnector(
-            endpoint=f"{ws_server}/ws/api/v1/{account}/software_environments/{name}/",
-            notifications_endpoint=f"{ws_server}/ws/api/v1/{account}/notifications/",
-            session=session,
-            log_output=log_output,
-            connection_error_message=(
-                "Unable to connect to server, do you have permissions to "
-                f'create environments in the "{account}" account?'
-            ),
+        if conda or pip:
+            senv = await create_env_spec(conda=conda, pip=pip)
+        else:
+            senv = None
+        logger.info("Creating software environment")
+        alias = await self._create_software_environment_v2(
+            senv=senv,
+            container=container,
+            name=name,
+            account=account,
+            force_rebuild=force_rebuild,
+            use_entrypoint=use_entrypoint,
+            gpu_enabled=gpu_enabled,
+            architecture=architecture,
         )
-        await ws.connect()
-        await ws.send_json(data)
-        await ws.stream_messages()
+        if wait_build and alias:
+            # pyright complains unless we nest like this
+            # only tail software environments that have builds
+            if alias.get("latest_spec"):
+                assert alias["latest_spec"]
+                spec = alias["latest_spec"]
+                if spec.get("latest_build"):
+                    assert spec["latest_build"]
+                    build = spec["latest_build"]
+                    if build["state"] == "built":
+                        logger.info("Software environment already built")
+                    else:
+                        log_output.write("--- Logs from remote build follow ---\n")
+                        final_state = await self._tail_software_build_logs(
+                            build["id"], account=account, log_output=log_output
+                        )
+                        info_url = (
+                            self.server + f"/software/alias/{alias['id']}"
+                            f"/build/{build['id']}?account={account}&tab=logs"
+                        )
+                        log_output.write(f"--- Logs end, may be truncated, see {info_url} for full output ---\n")
+                        if final_state == "error":
+                            raise BuildError("The software environment failed to build")
+            logger.info("Software environment created")
+        return alias
 
     async def _tail_software_build_logs(
         self,
         senv_build_id: int,
         account: Optional[str] = None,
         log_output: TextIO = sys.stdout,
     ) -> str:
@@ -1144,19 +984,16 @@
             results_all.update(results)
             offset = len(results_all)
             if len(results_all) == count:
                 break
         return results_all
 
     @track_context
-    async def _list_software_environments(self, account: Optional[str] = None, new_build_backend: bool = True) -> dict:
-        if new_build_backend:
-            return await self._depaginate_v2(self._list_software_environments_page_v2, account=account)
-        else:
-            return await self._depaginate(self._list_software_environments_page, account=account)
+    async def _list_software_environments(self, account: Optional[str] = None) -> dict:
+        return await self._depaginate_v2(self._list_software_environments_page_v2, account=account)
 
     @track_context
     async def _list_software_environments_page_v2(self, offset: int, account: Optional[str] = None) -> Tuple[dict, int]:
         account = account or self.default_account
         response = await self._do_request(
             "GET",
             self.server + f"/api/v2/software-environment/account/{account}/alias",
@@ -1360,37 +1197,32 @@
         else:
             msg = (
                 f"Coiled API responded with a {response.status} status code " "while fetching available instance types."
             )
             raise ApiResponseStatusError(msg)
 
     @overload
-    def list_software_environments(
-        self: Cloud[Sync], account: Optional[str] = None, new_build_backend: bool = True
-    ) -> dict:
+    def list_software_environments(self: Cloud[Sync], account: Optional[str] = None) -> dict:
         ...
 
     @overload
     def list_software_environments(
         self: Cloud[Async],
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> Awaitable[dict]:
         ...
 
     @list_docstring
     def list_software_environments(
         self: CloudSyncAsync,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> Union[dict, Awaitable[dict]]:
         return self._sync(
             self._list_software_environments,
             account=account,
-            new_build_backend=new_build_backend,
         )
 
     def _normalize_name(
         self,
         name: str,
         context_account: Optional[str] = None,
         raise_on_account_conflict: bool = False,
@@ -1412,56 +1244,45 @@
         return account, parsed_name
 
     @overload
     def delete_software_environment(
         self: Cloud[Sync],
         name: str,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> None:
         ...
 
     @overload
     def delete_software_environment(
         self: Cloud[Async],
         name: str,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> Awaitable[None]:
         ...
 
     @delete_docstring
     def delete_software_environment(
         self: CloudSyncAsync,
         name: str,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> Optional[Awaitable[None]]:
-        return self._sync(self._delete_software_environment, name, account, new_build_backend)
+        return self._sync(self._delete_software_environment, name, account)
 
     @track_context
-    async def _delete_software_environment(
-        self, name: str, account: Optional[str] = None, new_build_backend: bool = True
-    ) -> None:
+    async def _delete_software_environment(self, name: str, account: Optional[str] = None) -> None:
         context_account = account
         account, name, tag = parse_identifier(name)
         account = account or context_account or self.default_account
 
         if tag:
             name = ":".join([name, tag])
-        if not new_build_backend:
-            response = await self._do_request(
-                "DELETE",
-                f"{self.server}/api/v1/{account}/software_environments/{name}/",
-            )
-        else:
-            response = await self._do_request(
-                "DELETE",
-                f"{self.server}/api/v2/software-environment/account/{account}/alias/name/{name}",
-            )
+        response = await self._do_request(
+            "DELETE",
+            f"{self.server}/api/v2/software-environment/account/{account}/alias/name/{name}",
+        )
         if response.status == 404:
             raise NotFound(
                 f"Unable to find software environment with the name '{name}' " f"in the account '{account}'."
             )
         elif response.status == 403:
             await handle_api_exception(response, exception_cls=PermissionsError)
         elif response.status >= 400:
@@ -1653,80 +1474,59 @@
         return provider_name
 
     @overload
     def get_software_info(
         self: Cloud[Sync],
         name: str,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> dict:
         ...
 
     @overload
     def get_software_info(
         self: Cloud[Async],
         name: str,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> Awaitable[dict]:
         ...
 
     def get_software_info(
         self: CloudSyncAsync,
         name: str,
         account: Optional[str] = None,
-        new_build_backend: bool = True,
     ) -> Union[dict, Awaitable[dict]]:
         return self._sync(
             self._get_software_info,
             name=name,
             account=account,
-            new_build_backend=new_build_backend,
         )
 
     @track_context
-    async def _get_software_info(
-        self, name: str, account: Optional[str] = None, new_build_backend: bool = True
-    ) -> dict:
+    async def _get_software_info(self, name: str, account: Optional[str] = None) -> dict:
         """Retrieve solved spec for a Coiled software environment
 
         Parameters
         ----------
         name
             Software environment name
 
         Returns
         -------
         results
             Coiled software environment information
         """
         account, name = self._normalize_name(name, context_account=account)
-        if new_build_backend:
-            response = await self._do_request(
-                "GET",
-                self.server + f"/api/v2/software-environment/account/{account}/alias/name/{name}",
-            )
-            if response.status >= 400:
-                await handle_api_exception(response)
-            alias = await response.json()
-            return await self._get_software_spec(alias["latest_spec"]["id"], account=account)
-        else:
-            response = await self._do_request(
-                "GET",
-                self.server + f"/api/v1/{account}/software_environments/{name}/",
-            )
+        response = await self._do_request(
+            "GET",
+            self.server + f"/api/v2/software-environment/account/{account}/alias/name/{name}",
+        )
         if response.status >= 400:
-            text = await response.text()
-            if "Not found" in text:
-                raise ValueError(f"Could not find a '{account}/{name}' Coiled software environment")
-            else:
-                await handle_api_exception(response)
-
-        results = await response.json()
-        return results
+            await handle_api_exception(response)
+        alias = await response.json()
+        return await self._get_software_spec(alias["latest_spec"]["id"], account=account)
 
     async def _get_software_spec(self, pk: str, account: Optional[str] = None) -> dict:
         account = account or self.default_account
         response = await self._do_request(
             "GET",
             self.server + f"/api/v2/software-environment/account/{account}/spec/{pk}",
         )
@@ -2332,35 +2132,28 @@
     name: Optional[str] = None,
     *,
     account: Optional[str] = None,
     conda: Optional[Union[list, CondaEnvSchema, str, pathlib.Path]] = None,
     pip: Optional[Union[list, str, pathlib.Path]] = None,
     container: Optional[str] = None,
     log_output=sys.stdout,
-    post_build: Optional[Union[list, str]] = None,
-    conda_env_name: Optional[str] = None,
-    backend_options: Optional[Dict] = None,
-    private: bool = True,
     force_rebuild: bool = False,
-    environ: Optional[Dict] = None,
     use_entrypoint: bool = True,
-    new_build_backend: bool = True,
     gpu_enabled: bool = False,
     architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
 ) -> Optional[SoftwareEnvironmentAlias]:
     """Create a software environment
 
     .. seealso::
 
        By default, your local environment is automatically replicated in your cluster (see :doc:`package_sync`).
 
-    .. deprecated:: 0.4.0
+    .. deprecated:: 0.6.0
 
-      The following parameters for ``create_software_environment`` have been deprecated: ``post_build``,
-      ``conda_env_name``, ``private``, ``backend_options``, ``environ``, ``use_entrypoint``
+      The following parameters for ``create_software_environment`` have been deprecated: ``use_entrypoint``
 
     Parameters
     ----------
     name
         Name of software environment. Name can't contain uppercase letters.
     account
         The account in which to create the software environment, if not given in the name.
@@ -2375,20 +2168,16 @@
         on Docker hub. Defaults to ``coiled/default``.
     log_output
         Stream to output logs to. Defaults to ``sys.stdout``.
     force_rebuild
         By default, if an existing software environment with the same name and dependencies already
         exists, a rebuild is aborted. If this is set to ``True``, those checks are skipped and the
         environment will be rebuilt. Defaults to ``False``
-    environ
-        Dictionary of environment variables.
     use_entrypoint
         Whether to use (or override) entrypoint set on container.
-    new_build_backend
-        Use the new build system
     gpu_enabled
         Set CUDA version for Conda
     architecture
         CPU architecture of the software environment. Defaults to ``x86_64``;
         specify ``aarch64`` for ARM.
     """
     error = False
@@ -2397,23 +2186,17 @@
         try:
             return cloud.create_software_environment(
                 name=name,
                 account=account,
                 conda=conda,
                 pip=pip,
                 container=container,
-                post_build=post_build,
                 log_output=log_output,
-                conda_env_name=conda_env_name,
-                backend_options=backend_options,
-                private=private,
                 force_rebuild=force_rebuild,
-                environ=environ,
                 use_entrypoint=use_entrypoint,
-                new_build_backend=new_build_backend,
                 gpu_enabled=gpu_enabled,
                 architecture=architecture,
             )
         except Exception as e:
             error = e
             raise
         finally:
@@ -2421,18 +2204,14 @@
                 "error_class": error.__class__.__name__,
                 "error_message": str(error),
                 "name": str(name),
                 "conda": bool(conda),
                 "account": account,
                 "pip": bool(pip),
                 "container": container,
-                "post_build": bool(post_build),
-                "conda_env_name": bool(conda_env_name),
-                "private": bool(private),
-                "environ": bool(environ),
                 "use_entrypoint": bool(use_entrypoint),
             }
             if error:
                 cloud.add_interaction(
                     "create-software-environment",
                     success=False,
                     additional_data=data,
@@ -2442,23 +2221,28 @@
                     "create-software-environment",
                     success=True,
                     additional_data=data,
                 )
 
 
 @list_docstring
-def list_software_environments(account=None, new_build_backend: bool = True):
+def list_software_environments(account=None):
     with Cloud() as cloud:
-        return cloud.list_software_environments(account=account, new_build_backend=new_build_backend)
+        return cloud.list_software_environments(
+            account=account,
+        )
 
 
 @delete_docstring
-def delete_software_environment(name, account: Optional[str] = None, new_build_backend: bool = True):
+def delete_software_environment(name, account: Optional[str] = None):
     with Cloud() as cloud:
-        return cloud.delete_software_environment(name=name, account=account, new_build_backend=new_build_backend)
+        return cloud.delete_software_environment(
+            name=name,
+            account=account,
+        )
 
 
 def get_software_info(name: str, account: Optional[str] = None) -> dict:
     """Retrieve solved spec for a Coiled software environment
 
     Parameters
     ----------
```

### Comparing `coiled-0.6.3.dev9/coiled/exceptions.py` & `coiled-0.6.4.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/magic.py` & `coiled-0.6.4.dev1/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/scan.py` & `coiled-0.6.4.dev1/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/software.py` & `coiled-0.6.4.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/types.py` & `coiled-0.6.4.dev1/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/utils.py` & `coiled-0.6.4.dev1/coiled/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import contextlib
 import functools
 import itertools
 import json
 import logging
 import os
+import platform
 import random
 import re
 import ssl
 import string
 import subprocess
 import sys
 import tempfile
@@ -99,14 +100,15 @@
 
     name: str
     cores: int
     gpus: int
     gpu_name: str
     memory: int
     backend_type: str
+    coiled_credits: float
 
 
 # TODO: copied from distributed, introduced in 2021.12.0.
 # We should be able to remove this someday once we can increase
 # the minimum supported version.
 def in_async_call(loop, default=False):
     """Whether this call is currently within an async call"""
@@ -1133,14 +1135,27 @@
             "and use the `scheduler_vm_types=[]` or `worker_vm_types=[]` keyword "
             "argument to specify the specific instance type you want."
         )
         raise InstanceTypeError(error_message)
     return instances
 
 
+def any_gpu_instance_type(type_list: Optional[Union[str, List[str]]]) -> bool:
+    # TODO (future PR) ideally we'd get this from database via endpoint as part of preflight check
+    #   but for now we'll just use regex to match instance types with bundled GPU
+    if not type_list:
+        return False
+    if isinstance(type_list, str):
+        type_list = [type_list]
+    # check supported AWS instance types and GCP type with non-guest GPU (A100)
+    return any(
+        re.search(r"^(((p4|p3|g5|g5g|g4dn|g4ad)\.)|(a2-))", vm_type, flags=re.IGNORECASE) for vm_type in type_list
+    )
+
+
 def validate_type(type_, obj_) -> bool:
     if hasattr(type_, "__forward_arg__"):
         # evaluate ForwardRef types -- this function breaks if we can't
         return validate_type(type_.__forward_arg__, obj_)
     try:
         if hasattr(type_, "__annotations__"):
             # check for type TypedDict
@@ -1378,7 +1393,28 @@
     p = urlparse(file_uri)
     unquoted_path = unquote(p.path)
     if os.name == "nt":
         # handling valid windows URIs of
         # file:///C:/somewhere/something.whl
         unquoted_path = unquoted_path.lstrip("/")
     return Path(unquoted_path)
+
+
+def is_system_python() -> bool:
+    """Determine if the current Python executable is a system Python."""
+    # Check if we are in a virtualenv
+    if (
+        "VIRTUAL_ENV" in os.environ
+        or "PYENV_VERSION" in os.environ
+        or getattr(sys, "base_prefix", sys.prefix) != sys.prefix
+        or getattr(sys, "real_prefix", sys.prefix) != sys.prefix
+        or os.path.exists(os.path.join(sys.prefix, "conda-meta"))
+    ):
+        return False
+    # Check installation directory for each OS
+    system = platform.system()
+    if system == "Linux" and sys.prefix == "/usr":
+        return True
+    if system == "Darwin" and (sys.prefix.startswith("/Library") or sys.prefix.startswith("/System")):
+        return True
+    # Default to False
+    return False
```

### Comparing `coiled-0.6.3.dev9/coiled/websockets.py` & `coiled-0.6.4.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/_beta/cluster.py` & `coiled-0.6.4.dev1/coiled/_beta/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,20 @@
 from coiled.core import IsAsynchronous
 from coiled.errors import ClusterCreationError, DoesNotExist
 from coiled.exceptions import ArgumentCombinationError, InstanceTypeError
 from coiled.types import ArchitectureTypesEnum, PackageLevel, PackageLevelEnum
 from coiled.utils import (
     COILED_LOGGER_NAME,
     GCP_SCHEDULER_GPU,
+    any_gpu_instance_type,
     cluster_firewall,
     get_details_url,
     get_grafana_url,
     get_instance_type_from_cpu_memory,
+    is_system_python,
     parse_identifier,
     parse_wait_for_workers,
     validate_vm_typing,
 )
 
 from ..core import Async, AWSSessionCredentials, Sync
 from .core import (
@@ -133,21 +135,24 @@
         Amount of memory to request for each worker, Coiled will use a +/- 10% buffer
         from the memory that you specify. You may specify a range of memory by using a
         list of two elements, for example: ``worker_memory=["2GiB", "4GiB"]``.
     worker_disk_size
         Non-default size of persistent disk attached to each worker instance, specified
         in GB.
     worker_gpu
-        For instance types that don't come with a fixed number of GPUs, the number of
-        GPUs to attach. This only applies to GCP, and will default to 1 if you specify
-        ``worker_gpu_type``. Coiled currently only supports a single GPU per instance.
+        Number of GPUs to attach to each worker. Default is 0.
+        Note that this is ignored if you're explicitly specifying an instance type which
+        includes a fixed number of GPUs.
     worker_gpu_type
-        For instance types that don't always come with GPU, the type of GPU to attach.
-        This only applied to GCP. Should match the way the cloud provider specifies the
-        GPU, for example: ``worker_gpu_type="nvidia-tesla-t4"``.
+        For GCP, this lets you specify type of guest GPU for instances.
+        Should match the way the cloud provider specifies the GPU, for example:
+        ``worker_gpu_type="nvidia-tesla-t4"``.
+        By default, Coiled will request NVIDIA T4 if GPU type isn't specified.
+        For AWS, if you want GPU other than T4, you'll need to explicitly specify the VM
+        instance type (e.g., ``p3.2xlarge`` for instance with one NVIDIA Tesla V100).
     scheduler_class
         Scheduler class to use. Defaults to :class:`distributed.scheduler.Scheduler`.
     scheduler_options
         Mapping with keyword arguments to pass to ``scheduler_class``. Defaults
         to ``{}``.
     scheduler_vm_types
         List of instance types that you would like the scheduler to use, default instances
@@ -157,17 +162,18 @@
         Number, or range, of CPUs requested for the scheduler. Specify a range by
         using a list of two elements, for example: ``scheduler_cpu=[2, 8]``.
     scheduler_memory
         Amount of memory to request for the scheduler, Coiled will use a +/-10%
         buffer from the memory what you specify. You may specify a range of memory by using a
         list of two elements, for example: ``scheduler_memory=["2GiB", "4GiB"]``.
     scheduler_gpu
-        Whether to attach GPU to scheduler. This will affect instance type (if not specified explicitly).
-        For Google Cloud, it will also add a single "guest" T4 to the scheduler.
-        It's recommended to use GPU on scheduler for GPU clusters.
+        Whether to attach GPU to scheduler; this would be a single NVIDIA T4.
+        The best practice for Dask is to have a GPU on the scheduler if you are using GPUs on your
+        workers, so if you don't explicitly specify, Coiled will follow this best practice and give
+        you a scheduler GPU just in case you have ``worker_gpu`` set.
     asynchronous
         Set to True if using this Cloud within ``async``/``await`` functions or
         within Tornado ``gen.coroutines``. Otherwise this should remain
         ``False`` for normal use. Default is ``False``.
     cloud
         Cloud object to use for interacting with Coiled. This object contains user/authentication/account
         information. If this is None (default), we look for a recently-cached Cloud object, and if none
@@ -259,25 +265,23 @@
         Specify a port other than the default (8786) for communication with Dask scheduler; this is useful
         if your client is on a network that blocks 8786.
     allow_ingress_from
         Control the CIDR from which cluster firewall allows ingress to scheduler; by default this is open
         to any source address (0.0.0.0/0). You can specify CIDR, or "me" for just your IP address.
     allow_ssh
         Allow connections to scheduler over port 22, used for SSH.
-    new_build_backend
-        Use software environment created with the new build system.
     jupyter
         Start a Jupyter server in the same process as Dask scheduler. The Jupyter server will be behind HTTPS
         with authentication (unless you disable ``use_dashboard_https``, which we strongly recommend against).
         Note that ``jupyterlab`` will need to be installed in the software environment used on the cluster
         (or in your local environment if using package sync).
         Once the cluster is running, you can use ``jupyter_link`` to get link to access the Jupyter server.
-    region:
+    region
         The cloud provider region in which to run the cluster.
-    arm:
+    arm
         Use ARM instances for cluster; default is x86 (Intel) instances.
     """
 
     _instances = weakref.WeakSet()
 
     def __init__(
         self: ClusterSyncAsync,
@@ -322,25 +326,23 @@
         private_to_creator: Optional[bool] = None,
         use_best_zone: bool = True,
         compute_purchase_option: Optional[Literal["on-demand", "spot", "spot_with_fallback"]] = None,
         # easier network config
         scheduler_port: Optional[int] = None,
         allow_ingress_from: Optional[str] = None,
         allow_ssh: Optional[bool] = None,
-        new_build_backend: bool = False,
         jupyter: Optional[bool] = None,
         region: Optional[str] = None,
         arm: Optional[bool] = None,
     ):
         # NOTE:
         # this attribute is only updated while we wait for cluster to come up
         self.errored_worker_count: int = 0
         self.init_time = datetime.datetime.now()
         type(self)._instances.add(self)
-        self.new_build_backend = new_build_backend
         if package_sync and software:
             raise ValueError("Both parameters 'software' and 'package_sync'" "were passed. Please only pass one")
         self.package_sync = bool(package_sync)  # TODO: this should be mutually exclusive with passing a software env
         self.package_sync_ignore = package_sync_ignore
         if isinstance(package_sync, list):
             # ensure python is always included
             self.package_sync_only = set(package_sync)
@@ -425,49 +427,62 @@
         self.software_environment = software or dask.config.get("coiled.software")
         if not software and not package_sync:
             self.package_sync = True
         self.worker_class = worker_class or dask.config.get("coiled.worker.class")
         self.worker_cpu = worker_cpu or cast(Union[int, List[int]], dask.config.get("coiled.worker.cpu"))
 
         if isinstance(worker_cpu, int) and worker_cpu <= 1:
-            raise ValueError("`worker_cpu` should be at least 2.")
+            if not arm:
+                raise ValueError("`worker_cpu` should be at least 2 for x86 instance types.")
+            elif worker_cpu < 1:
+                raise ValueError("`worker_cpu` should be at least 1 for arm instance types.")
 
         self.worker_memory = worker_memory or dask.config.get("coiled.worker.memory")
         # FIXME get these from dask config
         self.worker_vm_types = worker_vm_types
         self.worker_disk_size = worker_disk_size
         self.worker_gpu_count = worker_gpu
         self.worker_gpu_type = worker_gpu_type
         self.worker_options = {
             **(cast(dict, dask.config.get("coiled.worker-options", {}))),
             **(worker_options or {}),
         }
 
         self.scheduler_vm_types = scheduler_vm_types
         self.scheduler_class = scheduler_class or cast(str, dask.config.get("coiled.scheduler.class"))
-
-        self.scheduler_class = scheduler_class or cast(str, dask.config.get("coiled.scheduler.class"))
-
-        self.scheduler_class = scheduler_class or cast(str, dask.config.get("coiled.scheduler.class"))
         self.scheduler_cpu = scheduler_cpu or cast(Union[int, List[int]], dask.config.get("coiled.scheduler.cpu"))
         self.scheduler_memory = scheduler_memory or cast(
             Union[int, List[int]], dask.config.get("coiled.scheduler.memory")
         )
-        self.scheduler_gpu = (
-            scheduler_gpu if scheduler_gpu is not None else cast(bool, dask.config.get("coiled.scheduler.gpu"))
-        )
-        self.use_best_zone = use_best_zone
-        self.compute_purchase_option = compute_purchase_option
-
-        self.scheduler_vm_types = scheduler_vm_types
         self.scheduler_options = {
             **(cast(dict, dask.config.get("coiled.scheduler-options", {}))),
             **(scheduler_options or {}),
         }
 
+        # use dask config if kwarg not specified for scheduler gpu
+        scheduler_gpu = scheduler_gpu if scheduler_gpu is not None else dask.config.get("coiled.scheduler.gpu")
+
+        self._is_gpu_cluster = (
+            # explicitly specified GPU (needed for GCP guest GPU)
+            bool(worker_gpu or worker_gpu_type or scheduler_gpu)
+            # or GPU bundled with explicitly specified instance type
+            or any_gpu_instance_type(worker_vm_types)
+            or any_gpu_instance_type(scheduler_vm_types)
+        )
+
+        if scheduler_gpu is None:
+            # when not specified by user (via kwarg or config), default to GPU on scheduler if workers have GPU
+            scheduler_gpu = True if self._is_gpu_cluster else False
+        else:
+            scheduler_gpu = bool(scheduler_gpu)
+        self.scheduler_gpu = scheduler_gpu
+
+        self.use_best_zone = use_best_zone
+        self.compute_purchase_option = compute_purchase_option
+
         self.name = name or cast(Optional[str], dask.config.get("coiled.name"))
         self.account = account
         self._start_n_workers = n_workers
         self._lock = None
         self._asynchronous = asynchronous
         self.shutdown_on_close = shutdown_on_close
         self.environ = {k: str(v) for (k, v) in (environ or {}).items() if v}
@@ -674,34 +689,33 @@
             scheduler_vm_types_to_use = self.scheduler_vm_types
 
         # If we still don't have instance types, use the defaults
         if not scheduler_vm_types_to_use or not worker_vm_types_to_use:
             provider = await self._get_account_cloud_provider_name()
 
             if not self.scheduler_gpu and not self.worker_gpu_count:
-                # When no GPUs, us same default for scheduler and workers
+                # When no GPUs, use same default for scheduler and workers
                 default_vm_types = await cloud._get_default_instance_types(
                     provider=provider,
                     gpu=False,
                     arch=self.arch.vm_arch,
                 )
                 scheduler_vm_types_to_use = scheduler_vm_types_to_use or default_vm_types
                 worker_vm_types_to_use = worker_vm_types_to_use or default_vm_types
             else:
                 # GPUs so there might be different defaults for scheduler/workers
                 if not scheduler_vm_types_to_use:
-                    scheduler_vm_types_to_use = await cloud._get_default_instance_types(
-                        provider=provider,
-                        gpu=self.scheduler_gpu,
+                    scheduler_vm_types_to_use = get_instance_type_from_cpu_memory(
+                        gpus=1 if self.scheduler_gpu else 0,
+                        backend=await self._get_account_cloud_provider_name(),
                         arch=self.arch.vm_arch,
                     )
                 if not worker_vm_types_to_use:
-                    worker_vm_types_to_use = await cloud._get_default_instance_types(
-                        provider=provider,
-                        gpu=bool(self.worker_gpu_count),
+                    worker_vm_types_to_use = get_instance_type_from_cpu_memory(
+                        gpus=self.worker_gpu_count,
                         arch=self.arch.vm_arch,
                     )
 
         return scheduler_vm_types_to_use, worker_vm_types_to_use
 
     @track_context
     async def _get_account_cloud_provider_name(self) -> str:
@@ -727,15 +741,17 @@
         else:
             should_create = True
             self.name = self.name or (self.account or cloud.default_account) + "-" + str(uuid.uuid4())[:10]
         return should_create
 
     @track_context
     async def _determine_senv(
-        self, architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64
+        self,
+        architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
+        gpu_enabled: bool = False,
     ) -> Optional[int]:
         # For package sync, this is where we scrape local environment, determine
         # what to install on cluster, and build/upload wheels as needed.
         if self.package_sync:
             progress = Progress(
                 TextColumn("[progress.description]{task.description}"), BarColumn(), TimeElapsedColumn()
             )
@@ -785,15 +801,19 @@
                         and package_level_lookup.get(pkg["name"], PackageLevelEnum.MEDIUM) > PackageLevelEnum.IGNORE
                     )
                 ]
                 for pkg_with_note in packages_with_notes:
                     logger.info(f"Package - {pkg_with_note['name']}, {pkg_with_note['note']}")
 
                 package_sync_env_alias = await self.cloud._create_package_sync_env(
-                    packages=approximation, account=self.account, progress=progress, architecture=architecture
+                    packages=approximation,
+                    account=self.account,
+                    progress=progress,
+                    gpu_enabled=gpu_enabled,
+                    architecture=architecture,
                 )
                 package_sync_env = package_sync_env_alias["id"]
             if HAS_RICH and self.show_widget:
                 from .widgets.rich import print_rich_package_table
 
                 print_rich_package_table(packages_with_notes, packages_with_errors)
 
@@ -994,20 +1014,24 @@
                 # (It also catches if our code to pick ARM instances types returns an x86 instance type.)
                 if architecture != self.arch:
                     # TODO (future PR) more specific error about which instance type doesn't match
                     raise RuntimeError(
                         f"Requested cluster architecture ({self.arch.vm_arch}) does not match "
                         f"architecture of some instance types ({scheduler_vm_types_to_use}, {worker_vm_types_to_use})."
                     )
-                if platform.machine() == architecture and platform.system() == "Linux":
+                # TODO (future PR) still used strict mode for GPU cluster if local env also has GPU
+                if (
+                    platform.machine() == architecture
+                    and platform.system() == "Linux"
+                    and not is_system_python()
+                    and not self._is_gpu_cluster
+                ):
                     self.package_sync_strict = True
 
-                senv_v2_id = await self._determine_senv(
-                    architecture=architecture,
-                )
+                senv_v2_id = await self._determine_senv(architecture=architecture, gpu_enabled=self._is_gpu_cluster)
                 self.cluster_id = await cloud._create_cluster(
                     account=self.account,
                     name=self.name,
                     workers=self._start_n_workers,
                     software_environment=self.software_environment,
                     worker_class=self.worker_class,
                     worker_options=self.worker_options,
@@ -1022,15 +1046,14 @@
                     scheduler_vm_types=scheduler_vm_types_to_use,
                     worker_vm_types=worker_vm_types_to_use,
                     backend_options=self.backend_options,
                     use_scheduler_public_ip=self.use_scheduler_public_ip,
                     use_dashboard_https=self.use_dashboard_https,
                     senv_v2_id=senv_v2_id,
                     private_to_creator=self.private_to_creator,
-                    new_build_backend=self.new_build_backend,
                 )
 
             if not self.cluster_id:
                 raise RuntimeError(f"Failed to find/create cluster {self.name}")
 
             if should_create:
                 logger.info(
```

### Comparing `coiled-0.6.3.dev9/coiled/_beta/core.py` & `coiled-0.6.4.dev1/coiled/_beta/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,14 +566,15 @@
 
     @track_context
     async def _create_package_sync_env(
         self,
         packages: List[ResolvedPackageInfo],
         progress: Optional[Progress] = None,
         account: Optional[str] = None,
+        gpu_enabled: bool = False,
         architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
     ) -> SoftwareEnvironmentAlias:
         account = account or self.default_account
         prepared_packages: List[PackageSchema] = []
         for pkg in packages:
             if pkg["sdist"] and pkg["md5"]:
                 with simple_progress(f"Uploading {pkg['name']}", progress=progress):
@@ -597,14 +598,15 @@
                 senv={
                     "packages": prepared_packages,
                     "raw_pip": None,
                     "raw_conda": None,
                 },
                 account=account,
                 architecture=architecture,
+                gpu_enabled=gpu_enabled,
             )
         return result
 
     @track_context
     async def _create_senv_package(
         self, package_file: BinaryIO, contents_md5: str, account: Optional[str] = None
     ) -> int:
@@ -672,15 +674,14 @@
         gcp_worker_gpu_count: Optional[int] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[AWSOptions, GCPOptions, dict]] = None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         private_to_creator: Optional[bool] = None,
-        new_build_backend: bool = True,
     ) -> int:
         # TODO (Declarative): support these args, or decide not to
         # https://gitlab.com/coiled/cloud/-/issues/4305
 
         if scheduler_class is not None:
             raise ValueError("scheduler_class is not supported in beta/new Coiled yet")
 
@@ -694,25 +695,24 @@
         self._verify_account(account)
 
         data = {
             "name": name,
             "workers": workers,
             "worker_instance_types": worker_vm_types,
             "scheduler_instance_types": scheduler_vm_types,
-            "software_environment": software_environment if not new_build_backend else None,
             "worker_options": worker_options,
             "worker_class": worker_class,
             "worker_disk_size": worker_disk_size,
             "scheduler_options": scheduler_options,
             "environ": environ,
             "tags": tags,
             "dask_config": dask_config,
             "private_to_creator": private_to_creator,
             "env_id": senv_v2_id,
-            "env_name": software_environment if new_build_backend else None,
+            "env_name": software_environment,
             # "jupyter_on_scheduler": True,
         }
 
         if gcp_worker_gpu_type is not None:
             # for backwards compatibility with v1 options
             backend_options = backend_options if backend_options else {}
             backend_options = {
@@ -821,15 +821,14 @@
         dask_config: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-        new_build_backend: bool = True,
     ) -> int:
         ...
 
     @overload
     def create_cluster(
         self: Cloud[Async],
         name: str,
@@ -846,15 +845,14 @@
         dask_config: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-        new_build_backend: bool = True,
     ) -> Awaitable[int]:
         ...
 
     def create_cluster(
         self,
         name: str,
         *,
@@ -870,15 +868,14 @@
         private_to_creator: Optional[bool] = None,
         dask_config: Optional[Dict] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-        new_build_backend: bool = True,
     ) -> Union[int, Awaitable[int]]:
         return self._sync(
             self._create_cluster,
             name=name,
             software_environment=software,
             worker_class=worker_class,
             worker_options=worker_options,
@@ -891,15 +888,14 @@
             dask_config=dask_config,
             private_to_creator=private_to_creator,
             scheduler_vm_types=scheduler_vm_types,
             worker_vm_types=worker_vm_types,
             gcp_worker_gpu_type=worker_gpu_type,
             worker_disk_size=worker_disk_size,
             backend_options=backend_options,
-            new_build_backend=new_build_backend,
         )
 
     @track_context
     async def _delete_cluster(self, cluster_id: int, account: Optional[str] = None) -> None:
         account = account or self.default_account
 
         route = f"/api/v2/clusters/account/{account}/id/{cluster_id}"
@@ -1660,15 +1656,14 @@
     tags: Optional[Dict] = None,
     dask_config: Optional[Dict] = None,
     private_to_creator: Optional[bool] = None,
     scheduler_vm_types: Optional[list] = None,
     worker_vm_types: Optional[list] = None,
     worker_disk_size: Optional[int] = None,
     backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-    new_build_backend: bool = True,
 ) -> int:
     """Create a cluster
 
     Parameters
     ---------
     name
         Name of cluster.
@@ -1713,15 +1708,14 @@
             tags=tags,
             dask_config=dask_config,
             private_to_creator=private_to_creator,
             backend_options=backend_options,
             worker_vm_types=worker_vm_types,
             worker_disk_size=worker_disk_size,
             scheduler_vm_types=scheduler_vm_types,
-            new_build_backend=new_build_backend,
         )
 
 
 @list_docstring
 def list_clusters(account=None, max_pages: Optional[int] = None):
     with CloudBeta() as cloud:
         return cloud.list_clusters(account=account, max_pages=max_pages)
```

### Comparing `coiled-0.6.3.dev9/coiled/_beta/cwi_log_link.py` & `coiled-0.6.4.dev1/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/_beta/states.py` & `coiled-0.6.4.dev1/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/_beta/widgets/__init__.py` & `coiled-0.6.4.dev1/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/_beta/widgets/rich.py` & `coiled-0.6.4.dev1/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/_beta/widgets/util.py` & `coiled-0.6.4.dev1/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/config.py` & `coiled-0.6.4.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/core.py` & `coiled-0.6.4.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/curl.py` & `coiled-0.6.4.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/env.py` & `coiled-0.6.4.dev1/coiled/cli/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from coiled._beta.core import setup_logging
 from coiled.exceptions import BuildError
 from coiled.types import ArchitectureTypesEnum
 
 from ..core import Cloud, create_software_environment, delete_software_environment
 from ..utils import COILED_SERVER
-from .utils import CONTEXT_SETTINGS, ENVIRON
+from .utils import CONTEXT_SETTINGS
 
 console = Console()
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def env():
     """Commands for managing Coiled software environments"""
@@ -27,62 +27,26 @@
     "--conda",
     default=None,
     help="Conda environment file.",
     type=click.Path(exists=True),
 )
 @click.option("--pip", default=None, help="Pip requirements file.", type=click.Path(exists=True))
 @click.option(
-    "--post-build",
-    default=None,
-    help="Post-build script.",
-    type=click.Path(exists=True),
-)
-@click.option(
-    "--conda-env-name",
-    default=None,
-    help=(
-        "Name of conda environment to install packages into. "
-        "Only use when using `--container`, and the image expects commands to run in "
-        'a conda environment not named "coiled"'
-    ),
-)
-@click.option(
-    "--private/--no-private",
-    default=True,
-    help="Flag to set software environment private.",
-    is_flag=True,
-)
-@click.option(
     "--force-rebuild",
     default=False,
     help="Skip checks for an existing software environment build.",
     is_flag=True,
 )
 @click.option(
-    "-e",
-    "--environ",
-    default=None,
-    type=ENVIRON,
-    multiple=True,
-    help="Custom environment variable(s).",
-)
-@click.option(
     "--account",
     default=None,
     type=str,
     help="Account to use for creating this software environment.",
 )
 @click.option(
-    "--new-build-backend/--no-new-build-backend",
-    is_flag=True,
-    show_default=True,
-    default=True,
-    help="Use the new build system",
-)
-@click.option(
     "--gpu-enabled",
     is_flag=True,
     show_default=True,
     default=False,
     help="Set CUDA virtual package for Conda",
 )
 @click.option(
@@ -93,64 +57,53 @@
     help="CPU architecture to use for the software environment",
 )
 def create(
     name,
     container,
     conda,
     pip,
-    post_build,
-    conda_env_name,
-    private,
     force_rebuild,
-    environ,
     account,
-    new_build_backend,
     gpu_enabled,
     architecture,
 ):
     """Create a Coiled software environment"""
     try:
         create_software_environment(
             name=name,
             container=container,
             conda=conda,
             pip=pip,
-            post_build=post_build,
-            conda_env_name=conda_env_name,
-            private=private,
             force_rebuild=force_rebuild,
-            environ=dict(environ),
             account=account,
-            new_build_backend=new_build_backend,
             gpu_enabled=gpu_enabled,
             architecture=architecture,
         )
     except BuildError as e:
         raise click.ClickException(f"{e}")
 
 
 @env.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("name")
-@click.option("--new-build-backend/--no-new-build-backend", is_flag=True, default=True)
-def delete(name: str, new_build_backend: bool):
+def delete(name: str):
     """Delete a Coiled software environment"""
-    delete_software_environment(name, new_build_backend=new_build_backend)
+    delete_software_environment(
+        name,
+    )
 
 
 @env.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("account", default=None, required=False)
-@click.option("--new-build-backend/--no-new-build-backend", is_flag=True, default=True)
-def list(account: str, new_build_backend: bool):
+def list(account: str):
     """List the Coiled software environments in an account"""
     with Cloud(account=account) as cloud:
-        environments = cloud.list_software_environments(account, new_build_backend=new_build_backend)
+        environments = cloud.list_software_environments(
+            account,
+        )
         account = cloud.default_account
-    if not new_build_backend:
-        console.print(environments)
-    else:
         table = Table(title="Software Environments")
         table.add_column("Name", style="cyan")
         table.add_column("Updated", style="magenta")
         table.add_column("Link", style="magenta")
         table.add_column("Status", style="green")
         server = config.get("coiled.server", COILED_SERVER).replace("8000", "5173")
         account = account or config.get("coiled.account")
```

### Comparing `coiled-0.6.3.dev9/coiled/cli/login.py` & `coiled-0.6.4.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/package_sync.py` & `coiled-0.6.4.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/utils.py` & `coiled-0.6.4.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.6.4.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.6.4.dev1/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/cluster/logs.py` & `coiled-0.6.4.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.6.4.dev1/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.6.4.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.6.4.dev1/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/setup/__init__.py` & `coiled-0.6.4.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/setup/amp.py` & `coiled-0.6.4.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/setup/aws.py` & `coiled-0.6.4.dev1/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/setup/entry.py` & `coiled-0.6.4.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/setup/gcp.py` & `coiled-0.6.4.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.6.4.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/coiled/v2/__init__.py` & `coiled-0.6.4.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/LICENSE` & `coiled-0.6.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/README.md` & `coiled-0.6.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.3.dev9/pyproject.toml` & `coiled-0.6.4.dev1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "ipywidgets",
     "jmespath",
     "jsondiff",
     "pip",
     "pip>=19.3",
     "prometheus_client",
     "rich>=11.2.0",
-    "setuptools",
+    "setuptools>=49.3.0",
     "typing_extensions",
     "wheel",
 ]
 description = ""
 dynamic = ["version"]
 license = ""
 maintainers = [{ name = "Coiled", email = "info@coiled.io" }]
```

### Comparing `coiled-0.6.3.dev9/PKG-INFO` & `coiled-0.6.4.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.3.dev9
+Version: 0.6.4.dev1
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
@@ -16,15 +16,15 @@
 Requires-Dist: ipywidgets
 Requires-Dist: jmespath
 Requires-Dist: jsondiff
 Requires-Dist: pip
 Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client
 Requires-Dist: rich>=11.2.0
-Requires-Dist: setuptools
+Requires-Dist: setuptools>=49.3.0
 Requires-Dist: typing-extensions
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/coiled/logos/master/Coiled-Logo_Horizontal_Black-RGB.png" width="200" style="max-width: 200px;" alt="Coiled">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.3.dev9 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.4.dev1 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
-setuptools Requires-Dist: typing-extensions Requires-Dist: wheel Description-
-Content-Type: text/markdown
+setuptools>=49.3.0 Requires-Dist: typing-extensions Requires-Dist: wheel
+Description-Content-Type: text/markdown
                                    [Coiled]
              Coiled.io â¢ Documentation â¢ Community â¢ Support
 Coiled is a deployment-as-a-service library for scaling Python with Dask, a
 popular open source library for parallel analytics. Coiled manages cloud
 resources, networking, software environments, and everything you need to scale
 Python in the cloud robustly and easily. Go to https://cloud.coiled.io to get
 started with Coiled.
```


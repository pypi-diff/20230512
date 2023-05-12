# Comparing `tmp/vdk-server-0.1.824443273.tar.gz` & `tmp/vdk-server-0.1.865727599.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-server-0.1.824443273.tar", last modified: Fri Mar 31 14:26:05 2023, max compression
+gzip compressed data, was "vdk-server-0.1.865727599.tar", last modified: Fri May 12 14:08:27 2023, max compression
```

## Comparing `vdk-server-0.1.824443273.tar` & `vdk-server-0.1.865727599.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      992 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-03-31 14:25:55.000000 vdk-server-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/src/vdk/plugin/server/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/src/vdk/plugin/server/configmap-local-registry-hosting-template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    20085 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/src/vdk/plugin/server/ingress-nginx-deploy.yaml
--rw-rw-rw-   0 root         (0) root         (0)    33089 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/src/vdk/plugin/server/installer.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/src/vdk/plugin/server/kind-cluster-config-template.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/src/vdk/plugin/server/server_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/src/vdk/plugin/server/server_plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/src/vdk_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      992 2023-03-31 14:26:04.000000 vdk-server-0.1.824443273/src/vdk_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-03-31 14:26:04.000000 vdk-server-0.1.824443273/src/vdk_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:26:04.000000 vdk-server-0.1.824443273/src/vdk_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-03-31 14:26:04.000000 vdk-server-0.1.824443273/src/vdk_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-31 14:26:04.000000 vdk-server-0.1.824443273/src/vdk_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:26:04.000000 vdk-server-0.1.824443273/src/vdk_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.997152 vdk-server-0.1.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-03-31 14:25:52.000000 vdk-server-0.1.824443273/tests/test_plugin_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.208601 vdk-server-0.1.865727599/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      992 2023-05-12 14:08:27.208601 vdk-server-0.1.865727599/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 14:08:27.208601 vdk-server-0.1.865727599/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-05-12 14:08:14.000000 vdk-server-0.1.865727599/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.204601 vdk-server-0.1.865727599/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.204601 vdk-server-0.1.865727599/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.204601 vdk-server-0.1.865727599/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.204601 vdk-server-0.1.865727599/src/vdk/plugin/server/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/src/vdk/plugin/server/configmap-local-registry-hosting-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    20085 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/src/vdk/plugin/server/ingress-nginx-deploy.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    33344 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/src/vdk/plugin/server/installer.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/src/vdk/plugin/server/kind-cluster-config-template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/src/vdk/plugin/server/server_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/src/vdk/plugin/server/server_plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.208601 vdk-server-0.1.865727599/src/vdk_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-05-12 14:08:27.000000 vdk-server-0.1.865727599/src/vdk_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-12 14:08:27.000000 vdk-server-0.1.865727599/src/vdk_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:08:27.000000 vdk-server-0.1.865727599/src/vdk_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 14:08:27.000000 vdk-server-0.1.865727599/src/vdk_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-12 14:08:27.000000 vdk-server-0.1.865727599/src/vdk_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-12 14:08:27.000000 vdk-server-0.1.865727599/src/vdk_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:08:27.208601 vdk-server-0.1.865727599/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-12 14:08:10.000000 vdk-server-0.1.865727599/tests/test_plugin_template.py
```

### Comparing `vdk-server-0.1.824443273/PKG-INFO` & `vdk-server-0.1.865727599/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-server
-Version: 0.1.824443273
+Version: 0.1.865727599
 Summary: Versatile Data Kit SDK plugin that facilitates the installation of a local Control Service.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-server-0.1.824443273/setup.py` & `vdk-server-0.1.865727599/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.865727599"
 
 setuptools.setup(
     name="vdk-server",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin that facilitates the installation of a local Control Service.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-server-0.1.824443273/src/vdk/plugin/server/ingress-nginx-deploy.yaml` & `vdk-server-0.1.865727599/src/vdk/plugin/server/ingress-nginx-deploy.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
-# This is a copy of the ingress-nginx manifest for KinD, available here:
+# This is a copy of the ingress-nginx manifest for Kind, available here:
 # https://github.com/kubernetes/ingress-nginx/blob/main/deploy/static/provider/kind/deploy.yaml
 apiVersion: v1
 kind: Namespace
 metadata:
   name: ingress-nginx
   labels:
     app.kubernetes.io/name: ingress-nginx
```

### Comparing `vdk-server-0.1.824443273/src/vdk/plugin/server/installer.py` & `vdk-server-0.1.865727599/src/vdk/plugin/server/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         self.__connect_container_to_kind_network(self.docker_registry_container_name)
         self.__connect_container_to_kind_network(self.git_server_container_name)
         self.__configure_kind_local_docker_registry()
         self.__install_ingress_prerequisites()
         self.__install_helm_chart()
         self.__finalize_configuration()
         log.info("Versatile Data Kit Control Service installed successfully")
+        log.info("Access the UI at http://localhost:8092")
         log.info(
             "Access the REST API at http://localhost:8092/data-jobs/swagger-ui.html\n"
         )
         log.info(
             "\n"
             "You can now use the other vdk commands to create, run, and deploy jobs. "
             "Run vdk --help to see all commands and examples"
@@ -641,14 +642,16 @@
             self.helm_chart_name,
             "--atomic",
             "--set",
             "service.type=ClusterIP",
             "--set",
             "deploymentBuilderResourcesDefault.limits.cpu=0",
             "--set",
+            "dataJob.executions.logsUrl.urlTemplate=http://localhost:8092/data-jobs/for-team/{{team_name}}/jobs/{{job_name}}/executions/{{execution_id}}/logs?tail_lines=400",
+            "--set",
             "deploymentBuilderResourcesDefault.requests.cpu=0",
             "--set",
             "deploymentBuilderResourcesDefault.limits.memory=0",
             "--set",
             "deploymentBuilderResourcesDefault.requests.memory=0",
             "--set",
             "deploymentDefaultDataJobsResources.limits.cpu=0",
```

### Comparing `vdk-server-0.1.824443273/src/vdk/plugin/server/kind-cluster-config-template.yaml` & `vdk-server-0.1.865727599/src/vdk/plugin/server/kind-cluster-config-template.yaml`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.824443273/src/vdk/plugin/server/server_plugin.py` & `vdk-server-0.1.865727599/src/vdk/plugin/server/server_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.824443273/src/vdk/plugin/server/server_plugin_utils.py` & `vdk-server-0.1.865727599/src/vdk/plugin/server/server_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-server-0.1.824443273/src/vdk_server.egg-info/PKG-INFO` & `vdk-server-0.1.865727599/src/vdk_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-server
-Version: 0.1.824443273
+Version: 0.1.865727599
 Summary: Versatile Data Kit SDK plugin that facilitates the installation of a local Control Service.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-server-0.1.824443273/src/vdk_server.egg-info/SOURCES.txt` & `vdk-server-0.1.865727599/src/vdk_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/cmflib-0.0.2.tar.gz` & `tmp/cmflib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmflib-0.0.2.tar", last modified: Thu Dec  1 21:38:29 2022, max compression
+gzip compressed data, was "cmflib-0.0.3.tar", last modified: Fri May 12 20:03:53 2023, max compression
```

## Comparing `cmflib-0.0.2.tar` & `cmflib-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,67 @@
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2022-12-01 21:38:29.271818 cmflib-0.0.2/
--rw-r--r--   0 royann   (121683555) users      (100)    11356 2022-09-12 18:00:26.000000 cmflib-0.0.2/LICENSE
--rw-r--r--   0 royann   (121683555) users      (100)    10565 2022-12-01 21:38:29.271818 cmflib-0.0.2/PKG-INFO
--rw-r--r--   0 royann   (121683555) users      (100)    10090 2022-11-30 15:00:06.000000 cmflib-0.0.2/README.md
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2022-12-01 21:38:29.267819 cmflib-0.0.2/cmflib/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2022-10-13 15:17:47.000000 cmflib-0.0.2/cmflib/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)    41532 2022-11-30 15:59:56.000000 cmflib-0.0.2/cmflib/cmf.py
--rw-r--r--   0 royann   (121683555) users      (100)    11319 2022-11-28 16:00:09.000000 cmflib-0.0.2/cmflib/cmfquery.py
--rw-r--r--   0 royann   (121683555) users      (100)    21626 2022-10-03 22:44:31.000000 cmflib-0.0.2/cmflib/cmfquery_bk.py
--rw-r--r--   0 royann   (121683555) users      (100)     9027 2022-11-28 16:00:09.000000 cmflib-0.0.2/cmflib/dvc_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)    17079 2022-11-29 19:33:03.000000 cmflib-0.0.2/cmflib/graph_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)    18137 2022-11-29 19:33:03.000000 cmflib-0.0.2/cmflib/metadata_helper.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2022-12-01 21:38:29.271818 cmflib-0.0.2/cmflib.egg-info/
--rw-r--r--   0 royann   (121683555) users      (100)    10565 2022-12-01 21:38:29.000000 cmflib-0.0.2/cmflib.egg-info/PKG-INFO
--rw-r--r--   0 royann   (121683555) users      (100)      346 2022-12-01 21:38:29.000000 cmflib-0.0.2/cmflib.egg-info/SOURCES.txt
--rw-r--r--   0 royann   (121683555) users      (100)        1 2022-12-01 21:38:29.000000 cmflib-0.0.2/cmflib.egg-info/dependency_links.txt
--rw-r--r--   0 royann   (121683555) users      (100)       77 2022-12-01 21:38:29.000000 cmflib-0.0.2/cmflib.egg-info/requires.txt
--rw-r--r--   0 royann   (121683555) users      (100)        7 2022-12-01 21:38:29.000000 cmflib-0.0.2/cmflib.egg-info/top_level.txt
--rw-r--r--   0 royann   (121683555) users      (100)      433 2022-12-01 21:37:57.000000 cmflib-0.0.2/pyproject.toml
--rw-r--r--   0 royann   (121683555) users      (100)      103 2022-12-01 21:38:29.271818 cmflib-0.0.2/setup.cfg
--rw-r--r--   0 royann   (121683555) users      (100)     1039 2022-12-01 21:37:36.000000 cmflib-0.0.2/setup.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/
+-rw-r--r--   0 royann   (121683555) users      (100)    11356 2023-03-01 22:34:14.000000 cmflib-0.0.3/LICENSE
+-rw-r--r--   0 royann   (121683555) users      (100)    10629 2023-05-12 20:03:53.688822 cmflib-0.0.3/PKG-INFO
+-rw-r--r--   0 royann   (121683555) users      (100)    10154 2023-04-25 18:07:06.000000 cmflib-0.0.3/README.md
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-03-01 22:34:14.000000 cmflib-0.0.3/cmflib/__init__.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/bin/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/bin/__init__.py
+-rwxr-xr-x   0 royann   (121683555) users      (100)      214 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/bin/cmf
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/cli/
+-rw-r--r--   0 royann   (121683555) users      (100)     1665 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)      910 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/command.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2912 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/parser.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2148 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/utils.py
+-rw-r--r--   0 royann   (121683555) users      (100)    57153 2023-05-12 17:30:36.000000 cmflib-0.0.3/cmflib/cmf.py
+-rw-r--r--   0 royann   (121683555) users      (100)     6341 2023-05-12 17:24:33.000000 cmflib-0.0.3/cmflib/cmf_merger.py
+-rw-r--r--   0 royann   (121683555) users      (100)    16923 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cmfquery.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/__init__.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/artifact/
+-rw-r--r--   0 royann   (121683555) users      (100)     1450 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/artifact/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     9043 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/artifact/pull.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1612 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/artifact/push.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/init/
+-rw-r--r--   0 royann   (121683555) users      (100)     1543 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/init/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5163 2023-05-12 17:25:32.000000 cmflib-0.0.3/cmflib/commands/init/amazonS3.py
+-rw-r--r--   0 royann   (121683555) users      (100)     4610 2023-05-12 17:25:48.000000 cmflib-0.0.3/cmflib/commands/init/local.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5496 2023-05-12 17:26:14.000000 cmflib-0.0.3/cmflib/commands/init/minioS3.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2094 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/init/show.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5403 2023-05-12 17:25:12.000000 cmflib-0.0.3/cmflib/commands/init/sshremote.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/metadata/
+-rw-r--r--   0 royann   (121683555) users      (100)     1444 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/metadata/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     4131 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/metadata/pull.py
+-rw-r--r--   0 royann   (121683555) users      (100)     4830 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/metadata/push.py
+-rw-r--r--   0 royann   (121683555) users      (100)    15584 2023-04-25 19:37:49.000000 cmflib-0.0.3/cmflib/dvc_wrapper.py
+-rw-r--r--   0 royann   (121683555) users      (100)    20186 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/graph_wrapper.py
+-rw-r--r--   0 royann   (121683555) users      (100)    19118 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/metadata_helper.py
+-rw-r--r--   0 royann   (121683555) users      (100)      179 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/mlmd_objects.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/server_interface/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/server_interface/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)      657 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/server_interface/server_interface.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/cmflib/storage_backends/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1713 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/amazonS3_artifacts.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1793 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/local_artifacts.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1779 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/minio_artifacts.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2166 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/sshremote_artifacts.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/cmflib/utils/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/utils/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1477 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/utils/cmf_config.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1300 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/utils/dvc_config.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib.egg-info/
+-rw-r--r--   0 royann   (121683555) users      (100)    10629 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/PKG-INFO
+-rw-r--r--   0 royann   (121683555) users      (100)     1409 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/SOURCES.txt
+-rw-r--r--   0 royann   (121683555) users      (100)        1 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/dependency_links.txt
+-rw-r--r--   0 royann   (121683555) users      (100)      113 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/requires.txt
+-rw-r--r--   0 royann   (121683555) users      (100)       14 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/top_level.txt
+-rw-r--r--   0 royann   (121683555) users      (100)      433 2023-05-12 19:54:35.000000 cmflib-0.0.3/pyproject.toml
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/server/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/__init__.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/server/app/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/app/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1966 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/app/get_data.py
+-rw-r--r--   0 royann   (121683555) users      (100)     6573 2023-05-12 17:24:33.000000 cmflib-0.0.3/server/app/main.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1413 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/app/query_visualization.py
+-rw-r--r--   0 royann   (121683555) users      (100)      103 2023-05-12 20:03:53.688822 cmflib-0.0.3/setup.cfg
+-rw-r--r--   0 royann   (121683555) users      (100)     1106 2023-04-25 18:07:06.000000 cmflib-0.0.3/setup.py
```

### Comparing `cmflib-0.0.2/LICENSE` & `cmflib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.2/PKG-INFO` & `cmflib-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cmflib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Track metadata for AI pipeline
 Author: Hewlett Packard Enterprise
 Project-URL: Homepage, https://github.com/HewlettPackard/cmf
 Project-URL: Bug Tracker, https://github.com/HewlettPackard/cmf/issues
 Keywords: python,first package
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <=3.9,>=3.7
+Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cmf
 ## Common Metadata Framework
-[Getting Started](docs/index.md)<br><br>
-[Detailed documentation of the API's](docs/API.md) <br> 
+[Getting Started](https://hewlettpackard.github.io/cmf/)<br><br>
+[Detailed documentation of the API's](https://hewlettpackard.github.io/cmf/api/public/cmf) <br> 
 
 Interactions in data pipelines can be complex. The Different stages in the pipeline, (which may not be next to each other) may have to interact to produce or transform artifacts. As the artifacts navigates and undergo transformations through this pipeline, it can take a complicated path, which might also involve bidirectional movement across these stages.  Also there could be dependencies between the multiple stages, where the metrics produced by a stage could influence the metrics at a subsequent stage.  It is important to track the metadata across a pipeline to provide features like, lineage tracking, provenance and reproducibility.  
 
 The tracking of metadata through these complex pipelines have multiple challenges, some of them being,  
 
 - Each stage in the pipeline could be executed in a different datacenter or an edge site having intermittent connection to the core datacenter.
```

### Comparing `cmflib-0.0.2/README.md` & `cmflib-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # cmf
 ## Common Metadata Framework
-[Getting Started](docs/index.md)<br><br>
-[Detailed documentation of the API's](docs/API.md) <br> 
+[Getting Started](https://hewlettpackard.github.io/cmf/)<br><br>
+[Detailed documentation of the API's](https://hewlettpackard.github.io/cmf/api/public/cmf) <br> 
 
 Interactions in data pipelines can be complex. The Different stages in the pipeline, (which may not be next to each other) may have to interact to produce or transform artifacts. As the artifacts navigates and undergo transformations through this pipeline, it can take a complicated path, which might also involve bidirectional movement across these stages.  Also there could be dependencies between the multiple stages, where the metrics produced by a stage could influence the metrics at a subsequent stage.  It is important to track the metadata across a pipeline to provide features like, lineage tracking, provenance and reproducibility.  
 
 The tracking of metadata through these complex pipelines have multiple challenges, some of them being,  
 
 - Each stage in the pipeline could be executed in a different datacenter or an edge site having intermittent connection to the core datacenter.
```

### Comparing `cmflib-0.0.2/cmflib/cmf.py` & `cmflib-0.0.3/cmflib/cmf.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,437 +19,636 @@
 import uuid
 import re
 import os
 import sys
 import pandas as pd
 import typing as t
 
+# This import is needed for jupyterlab environment
+import dvc
 from ml_metadata.proto import metadata_store_pb2 as mlpb
 from ml_metadata.metadata_store import metadata_store
-from cmflib.dvc_wrapper import dvc_get_url, dvc_get_hash, git_get_commit, \
-    commit_output, git_get_repo, commit_dvc_lock_file,  \
-    git_checkout_new_branch, \
-    check_git_repo, check_default_remote, check_git_remote
+from cmflib.dvc_wrapper import (
+    dvc_get_url,
+    dvc_get_hash,
+    git_get_commit,
+    commit_output,
+    git_get_repo,
+    commit_dvc_lock_file,
+    git_checkout_new_branch,
+    check_git_repo,
+    check_default_remote,
+    check_git_remote,
+    git_commit,
+)
 from cmflib import graph_wrapper
-from cmflib.metadata_helper import get_or_create_parent_context,   \
-    get_or_create_run_context, associate_child_to_parent_context,  \
-    create_new_execution_in_existing_run_context, link_execution_to_artifact, \
-    create_new_artifact_event_and_attribution, get_artifacts_by_id,  \
-    put_artifact, link_execution_to_input_artifact
+from cmflib.metadata_helper import (
+    get_or_create_parent_context,
+    get_or_create_run_context,
+    associate_child_to_parent_context,
+    create_new_execution_in_existing_run_context,
+    link_execution_to_artifact,
+    create_new_artifact_event_and_attribution,
+    get_artifacts_by_id,
+    put_artifact,
+    link_execution_to_input_artifact,
+)
+from cmflib.utils.cmf_config import CmfConfig
 
 
 class Cmf:
     """This class provides methods to log metadata for distributed AI pipelines.
-
-    The class instance creates an ML metadata store to store the metadata. It creates a driver to store nodes and its
-    relationships to neo4j. The user has to provide the name of the pipeline, that needs to be recorded with it.
-
+    The class instance creates an ML metadata store to store the metadata.
+    It creates a driver to store nodes and its relationships to neo4j.
+    The user has to provide the name of the pipeline, that needs to be recorded with CMF.
     ```python
     cmflib.cmf.Cmf(
         filename="mlmd",
         pipeline_name="test_pipeline",
         custom_properties={"owner": "user_a"},
         graph=False
     )
     ```
-
     Args:
         filename: Path  to the sqlite file to store the metadata
-        pipeline_name: Name to uniquely identify the pipeline. Note that name is the unique identification for a
-            pipeline.  If a pipeline already exist with the same name, the existing pipeline object is reused.
+        pipeline_name: Name to uniquely identify the pipeline.
+        Note that name is the unique identifier for a pipeline.
+        If a pipeline already exist with the same name, the existing pipeline object is reused.
         custom_properties: Additional properties of the pipeline that needs to be stored.
-        graph: If set to true, the libray also stores the relationships in the provided graph database. The following
-            environment variables should be set: `NEO4J_URI` (graph server URI), `NEO4J_USER_NAME` (user name) and
-            `NEO4J_PASSWD` (user password), e.g.:
-            ```bash
-            export NEO4J_URI="bolt://ip:port"
-            export NEO4J_USER_NAME=neo4j
-            export NEO4J_PASSWD=neo4j
-            ```
+        graph: If set to true, the libray also stores the relationships in the provided graph database.
+        The following
+        variables should be set: `neo4j_uri` (graph server URI), `neo4j_user` (user name) and
+        `neo4j_password` (user password), e.g.:
+        ```
+        cmf init local --path /home/user/local-storage --git-remote-url https://github.com/XXX/exprepo.git --neo4j-user neo4j --neo4j-password neo4j
+                              --neo4j-uri bolt://localhost:7687
+        ```
     """
 
     # pylint: disable=too-many-instance-attributes
-
-    __neo4j_uri = os.getenv('NEO4J_URI', "")
-    __neo4j_user = os.getenv('NEO4J_USER_NAME', "")
-    __neo4j_password = os.getenv('NEO4J_PASSWD', "")
-
-    def __init__(self, filename: str = "mlmd",
-                 pipeline_name: str = "", custom_properties: t.Optional[t.Dict] = None,
-                 graph: bool = False):
-        Cmf.__prechecks()
+    # Reading CONFIG_FILE variable
+    cmf_config = os.environ.get("CONFIG_FILE", ".cmfconfig")
+    if os.path.exists(cmf_config):
+        attr_dict = CmfConfig.read_config(cmf_config)
+        __neo4j_uri = attr_dict.get("neo4j-uri", "")
+        __neo4j_password = attr_dict.get("neo4j-password", "")
+        __neo4j_user = attr_dict.get("neo4j-user", "")
+
+    def __init__(
+        self,
+        filename: str = "mlmd",
+        pipeline_name: str = "",
+        custom_properties: t.Optional[t.Dict] = None,
+        graph: bool = False,
+        is_server: bool = False,
+    ):
+        if is_server is False:
+            Cmf.__prechecks()
         if custom_properties is None:
             custom_properties = {}
         config = mlpb.ConnectionConfig()
         config.sqlite.filename_uri = filename
         self.store = metadata_store.MetadataStore(config)
         self.filename = filename
         self.child_context = None
         self.execution = None
         self.execution_name = ""
         self.execution_command = ""
         self.metrics = {}
         self.input_artifacts = []
         self.execution_label_props = {}
         self.graph = graph
-        self.branch_name = filename.rsplit('/',1)[-1]
+        self.branch_name = filename.rsplit("/", 1)[-1]
 
-        git_checkout_new_branch(self.branch_name)
+        if is_server is False:
+            git_checkout_new_branch(self.branch_name)
         self.parent_context = get_or_create_parent_context(
-            store=self.store, pipeline=pipeline_name, custom_properties=custom_properties)
+            store=self.store,
+            pipeline=pipeline_name,
+            custom_properties=custom_properties,
+        )
+        if is_server:
+            Cmf.__get_neo4j_server_config()
         if graph is True:
             self.driver = graph_wrapper.GraphDriver(
-                Cmf.__neo4j_uri, Cmf.__neo4j_user, Cmf.__neo4j_password)
+                Cmf.__neo4j_uri, Cmf.__neo4j_user, Cmf.__neo4j_password
+            )
             self.driver.create_pipeline_node(
-                pipeline_name, self.parent_context.id, custom_properties)
+                pipeline_name, self.parent_context.id, custom_properties
+            )
+
+    @staticmethod
+    def __get_neo4j_server_config():
+        Cmf.__neo4j_uri = os.getenv('NEO4J_URI', "")
+        Cmf.__neo4j_user = os.getenv('NEO4J_USER_NAME', "")
+        Cmf.__neo4j_password = os.getenv('NEO4J_PASSWD', "")
+
 
     @staticmethod
     def __prechecks():
         """Pre checks for cmf
-
         1. Needs to be a git repository and
            git remote should be set
         2. Needs to be a dvc repository and
            default dvc remote should be set
         """
         Cmf.__check_git_init()
         Cmf.__check_default_remote()
         Cmf.__check_git_remote()
 
     @staticmethod
     def __check_git_remote():
         """Executes precheck for git remote"""
         if not check_git_remote():
-            print("*** Error git remote not set ***\n"
-                  "*** Run the command "
-                  "`git remote add origin <GIT_REMOTE_URL>` ***\n"
-                  " or \n"
-                  " After Updating the sample_env file,"
-                  " run `source sample_env`\n"
-                  " Then run 'sh initialize.sh'")
+            print(
+                "*** Error git remote not set ***\n"
+                "*** Run cmf init ***"
+            )
             sys.exit(1)
 
     @staticmethod
     def __check_default_remote():
         """Executes precheck for default dvc remote"""
         if not check_default_remote():
-            print("*** DVC not configured correctly***\n"
-                  "Initialize dvc and add a default dvc remote\n"
-                  "Run commands\n"
-                  "dvc init\n"
-                  "dvc remote add -d <remotename> <remotelocation>\n")
+            print(
+                "*** DVC not configured correctly ***\n"
+                "*** Run command cmf init ***" 
+            )
             sys.exit(1)
 
     @staticmethod
     def __check_git_init():
         """Verifies that the directory is a git repo"""
         if not check_git_repo():
-            print("*** Not a git repo, Please do the following ***\n"
-                  " Initialize git\n"
-                  " Initialize dvc and add a default dvc remote\n"
-                  " or \n"
-                  " After Updating the sample_env file,"
-                  " run `source sample_env`\n"
-                  " Then run 'sh initialize.sh'")
+            print(
+                "*** Not a git repo, Please do the following ***\n"
+                "*** Run Command cmf init ***"
+            )
             sys.exit(1)
 
     def __del__(self):
-        """Destructor - Cleans up the connection to neo4j"""
-        # if self.execution is not None:
-        #    commit_output(self.filename, self.execution.id)
-        if hasattr(self, 'driver'):
+        git_commit(self.execution.id)
+        if self.graph:
             self.driver.close()
 
-    def create_context(self, pipeline_stage: str,
-                       custom_properties: t.Optional[t.Dict] = None) -> mlpb.Context:
-        """Creates a stage in the pipeline.
-
-        If it already exists, it is reused and not created again.
-
+    def create_context(
+        self, pipeline_stage: str, custom_properties: t.Optional[t.Dict] = None
+    ) -> mlpb.Context:
+        """Create's a  context(stage).
+        Every call creates a unique pipeline stage.
         Example:
             ```python
+            #Create context
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
-
             # Create CMF logger
             cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
-
-            # Create or reuse context for this stage
+            # Create context
             context: mlmd.proto.Context = cmf.create_context(
                 pipeline_stage="prepare",
                 custom_properties ={"user-metadata1": "metadata_value"}
             )
+
             ```
+            Args:
+                Pipeline_stage: Name of the Stage.
+                custom_properties: Developers can provide key value pairs with additional properties of the execution that
+                    need to be stored.
+            Returns:
+                Context object from ML Metadata library associated with the new context for this stage.
+        """
+        custom_props = {} if custom_properties is None else custom_properties
+        pipeline_stage = self.parent_context.name + "/" + pipeline_stage
+        ctx = get_or_create_run_context(
+            self.store, pipeline_stage, custom_props)
+        self.child_context = ctx
+        associate_child_to_parent_context(
+            store=self.store, parent_context=self.parent_context, child_context=ctx
+        )
+        if self.graph:
+            self.driver.create_stage_node(
+                pipeline_stage, self.parent_context, ctx.id, custom_props
+            )
+        return ctx
 
-        Args:
-            pipeline_stage: Name of the pipeline stage.
-            custom_properties: Developers can provide key value pairs with additional properties of the stage that
-                need to be stored.
-        Returns:
-            Context object from ML Metadata library associated with the new stage.
+    def merge_created_context(
+        self, pipeline_stage: str, custom_properties: t.Optional[t.Dict] = None
+    ) -> mlpb.Context:
+        """Create context.
+        Every call creates a unique pipeline stage.
+        Example:
+
+            ```python
+            #Create context
+            # Import CMF
+            from cmflib.cmf import Cmf
+            from ml_metadata.proto import metadata_store_pb2 as mlpb
+            # Create CMF logger
+            cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
+            # Create context
+            context: mlmd.proto.Context = cmf.create_context(
+                pipeline_stage="prepare",
+                custom_properties ={"user-metadata1": "metadata_value"}
+            ```
+            Args:
+                Pipeline_stage: Name of the Stage.
+                custom_properties: Developers can provide key value pairs with additional properties of the execution that
+                    need to be stored.
+            Returns:
+                Context object from ML Metadata library associated with the new context for this stage.
         """
+
         custom_props = {} if custom_properties is None else custom_properties
         ctx = get_or_create_run_context(
             self.store, pipeline_stage, custom_props)
         self.child_context = ctx
         associate_child_to_parent_context(
-            store=self.store,
-            parent_context=self.parent_context,
-            child_context=ctx)
+            store=self.store, parent_context=self.parent_context, child_context=ctx
+        )
         if self.graph:
             self.driver.create_stage_node(
-                pipeline_stage, self.parent_context, ctx.id, custom_props)
+                pipeline_stage, self.parent_context, ctx.id, custom_props
+            )
         return ctx
 
-    def create_execution(self, execution_type: str,
-                         custom_properties: t.Optional[t.Dict] = None) -> mlpb.Execution:
+    def create_execution(
+        self,
+        execution_type: str,
+        custom_properties: t.Optional[t.Dict] = None,
+        cmd: str = None,
+        create_new_execution: bool = True,
+    ) -> mlpb.Execution:
         """Create execution.
-
         Every call creates a unique execution. Execution can only be created within a context, so
         [create_context][cmflib.cmf.Cmf.create_context] must be called first.
-
         Example:
             ```python
             # Import CMF
             from cmflib.cmf import Cmf
             from ml_metadata.proto import metadata_store_pb2 as mlpb
-
             # Create CMF logger
             cmf = Cmf(filename="mlmd", pipeline_name="test_pipeline")
-
             # Create or reuse context for this stage
             context: mlmd.proto.Context = cmf.create_context(
                 pipeline_stage="prepare",
                 custom_properties ={"user-metadata1": "metadata_value"}
             )
-
             # Create a new execution for this stage run
             execution: mlmd.proto.Execution = cmf.create_execution(
                 execution_type="Prepare",
                 custom_properties = {"split": split, "seed": seed}
             )
             ```
-
         Args:
-            execution_type: Name of the execution.
+            execution_type: Type of the execution.(when create_new_execution is False, this is the name of execution)
             custom_properties: Developers can provide key value pairs with additional properties of the execution that
                 need to be stored.
 
+            cmd: command used to run this execution.
+
+            create_new_execution:bool = True, This can be used by advanced users to re-use executions
+                This is applicable, when working with framework code like mmdet, pytorch lightning etc, where the
+                custom call-backs are used to log metrics.
+                if create_new_execution is True(Default), execution_type parameter will be used as the name of the execution type.
+                if create_new_execution is False, if existing execution exist with the same name as execution_type.
+                it will be reused.
+                Only executions created with  create_new_execution as False will have "name" as a property.
+
+
         Returns:
             Execution object from ML Metadata library associated with the new execution for this stage.
         """
         # Initializing the execution related fields
         self.metrics = {}
         self.input_artifacts = []
         self.execution_label_props = {}
         custom_props = {} if custom_properties is None else custom_properties
         git_repo = git_get_repo()
         git_start_commit = git_get_commit()
+        cmd = str(sys.argv) if cmd is None else cmd
         self.execution = create_new_execution_in_existing_run_context(
             store=self.store,
-            execution_type_name=execution_type,
+            # Type field when re-using executions
+            execution_type_name=self.child_context.name+'_'+str(uuid.uuid1()),
+            execution_name=execution_type, 
+            #Name field if we are re-using executions
+            #Type field , if creating new executions always 
             context_id=self.child_context.id,
-            execution=str(sys.argv),
+            execution=cmd,
             pipeline_id=self.parent_context.id,
             pipeline_type=self.parent_context.name,
             git_repo=git_repo,
             git_start_commit=git_start_commit,
-            custom_properties=custom_props
+            custom_properties=custom_props,
+            create_new_execution=create_new_execution,
         )
         self.execution_name = str(self.execution.id) + "," + execution_type
-        self.execution_command = str(sys.argv)
+        self.execution_command = cmd
         for k, v in custom_props.items():
-            k = re.sub('-', '_', k)
+            k = re.sub("-", "_", k)
             self.execution_label_props[k] = v
-        self.execution_label_props["Execution_Name"] = execution_type + \
-            ":" + str(self.execution.id)
+        self.execution_label_props["Execution_Name"] = (
+            execution_type + ":" + str(self.execution.id)
+        )
         self.execution_label_props["execution_command"] = str(sys.argv)
         if self.graph:
             self.driver.create_execution_node(
-                self.execution_name, self.child_context.id, self.parent_context, str(
-                    sys.argv), self.execution.id, custom_props)
+                self.execution_name,
+                self.child_context.id,
+                self.parent_context,
+                str(sys.argv),
+                self.execution.id,
+                custom_props,
+            )
         return self.execution
 
-    def update_execution(self, execution_id: int, custom_properties: t.Optional[t.Dict] = None):
+    def update_execution(
+        self, execution_id: int, custom_properties: t.Optional[t.Dict] = None
+    ):
         """Updates an existing execution.
-
         The custom properties can be updated after creation of the execution.
         The new custom properties is merged with earlier custom properties.
         """
         self.execution = self.store.get_executions_by_id([execution_id])[0]
         if self.execution is None:
             print("Error - no execution id")
             sys.exit(1)
-        execution_type = self.store.get_execution_types_by_id(
-            [self.execution.type_id])[0]
+        execution_type = self.store.get_execution_types_by_id([self.execution.type_id])[
+            0
+        ]
 
         if custom_properties:
             for key, value in custom_properties.items():
                 if isinstance(value, int):
                     self.execution.custom_properties[key].int_value = value
                 else:
                     self.execution.custom_properties[key].string_value = str(
                         value)
         self.store.put_executions([self.execution])
         c_props = {}
         for k, v in self.execution.custom_properties.items():
-            key = re.sub('-', '_', k)
-            val_type = str(v).split(':', maxsplit=1)[0]
+            key = re.sub("-", "_", k)
+            val_type = str(v).split(":", maxsplit=1)[0]
             if val_type == "string_value":
                 val = self.execution.custom_properties[k].string_value
             else:
-                val = str(v).split(':')[1]
+                val = str(v).split(":")[1]
             # The properties value are stored in the format type:value hence,
             # taking only value
             self.execution_label_props[key] = val
             c_props[key] = val
-        self.execution_name = str(
-            self.execution.id) + "," + execution_type.name
+        self.execution_name = str(self.execution.id) + \
+            "," + execution_type.name
         self.execution_command = self.execution.properties["Execution"]
-        self.execution_label_props["Execution_Name"] = execution_type.name + \
-            ":" + str(self.execution.id)
-        self.execution_label_props["execution_command"] = self.execution.properties["Execution"].string_value
+        self.execution_label_props["Execution_Name"] = (
+            execution_type.name + ":" + str(self.execution.id)
+        )
+        self.execution_label_props["execution_command"] = self.execution.properties[
+            "Execution"
+        ].string_value
         if self.graph:
             self.driver.create_execution_node(
                 self.execution_name,
                 self.child_context.id,
                 self.parent_context,
                 self.execution.properties["Execution"].string_value,
                 self.execution.id,
-                c_props)
+                c_props,
+            )
+        return self.execution
+
+    def merge_created_execution(
+        self,
+        execution_type: str,
+        execution_cmd: str,
+        properties: t.Optional[t.Dict] = None,
+        custom_properties: t.Optional[t.Dict] = None,
+    ) -> mlpb.Execution:
+        # Initializing the execution related fields
+        properties = {} if properties is None else properties
+        self.metrics = {}
+        self.input_artifacts = []
+        self.execution_label_props = {}
+        custom_props = {} if custom_properties is None else custom_properties
+        # print(custom_props)
+        git_repo = properties.get("Git_Repo", "")
+        git_start_commit = properties.get("Git_Start_Commit", "")
+        name = properties.get("Name", "")
+        create_new_execution = True
+        execution_name = execution_type
+        if name != "":
+            create_new_execution = False
+            execution_name = name
+
+        self.execution = create_new_execution_in_existing_run_context(
+            store=self.store,
+            execution_type_name=execution_type,
+            execution_name=execution_name,
+            context_id=self.child_context.id,
+            execution=execution_cmd,
+            pipeline_id=self.parent_context.id,
+            pipeline_type=self.parent_context.name,
+            git_repo=git_repo,
+            git_start_commit=git_start_commit,
+            custom_properties=custom_props,
+            create_new_execution=create_new_execution
+        )
+        self.execution_name = str(self.execution.id) + "," + execution_type
+        self.execution_command = execution_cmd
+        for k, v in custom_props.items():
+            k = re.sub("-", "_", k)
+            self.execution_label_props[k] = v
+        self.execution_label_props["Execution_Name"] = (
+            execution_type + ":" + str(self.execution.id)
+        )
+        self.execution_label_props["execution_command"] = execution_cmd
+        if self.graph:
+            self.driver.create_execution_node(
+                self.execution_name,
+                self.child_context.id,
+                self.parent_context,
+                execution_cmd,
+                self.execution.id,
+                custom_props,
+            )
         return self.execution
 
     def log_dvc_lock(self, file_path: str):
         """Used to update the dvc lock file created with dvc run command."""
+        print("Entered dvc lock file commit")
         return commit_dvc_lock_file(file_path, self.execution.id)
 
-    def log_dataset(self, url: str, event: str, custom_properties: t.Optional[t.Dict] = None) -> mlpb.Artifact:
+    def log_dataset(
+        self,
+        url: str,
+        event: str,
+        custom_properties: t.Optional[t.Dict] = None,
+        external: bool = False,
+    ) -> mlpb.Artifact:
         """Logs a dataset as artifact.
-
         This call adds the dataset to dvc. The dvc metadata file created (.dvc) will be added to git and committed. The
         version of the  dataset is automatically obtained from the versioning software(DVC) and tracked as a metadata.
-
         Example:
             ```python
             artifact: mlmd.proto.Artifact = cmf.log_dataset(
                 url="/repo/data.xml",
                 event="input",
                 custom_properties={"source":"kaggle"}
             )
             ```
-
         Args:
              url: The path to the dataset.
              event: Takes arguments `INPUT` OR `OUTPUT`.
              custom_properties: Dataset properties (key/value pairs).
-
         Returns:
             Artifact object from ML Metadata library associated with the new dataset artifact.
         """
         custom_props = {} if custom_properties is None else custom_properties
         git_repo = git_get_repo()
-        name = re.split('/', url)[-1]
+        name = re.split("/", url)[-1]
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
         if event.lower() == "input":
             event_type = mlpb.Event.Type.INPUT
 
-        dataset_commit = commit_output(url, self.execution.id)
+        commit_output(url, self.execution.id)
         c_hash = dvc_get_hash(url)
-
+        dataset_commit = c_hash
+        dvc_url = dvc_get_url(url)
+        dvc_url_with_pipeline = f"{self.parent_context.name}:{dvc_url}"
         url = url + ":" + c_hash
         if c_hash and c_hash.strip:
             existing_artifact.extend(self.store.get_artifacts_by_uri(c_hash))
 
         # To Do - What happens when uri is the same but names are different
         if existing_artifact and len(existing_artifact) != 0:
             existing_artifact = existing_artifact[0]
 
             # Quick fix- Updating only the name
             if custom_properties is not None:
                 self.update_existing_artifact(
                     existing_artifact, custom_properties)
             uri = c_hash
+            # update url for existing artifact
+            self.update_dataset_url(existing_artifact, dvc_url_with_pipeline)
             artifact = link_execution_to_artifact(
                 store=self.store,
                 execution_id=self.execution.id,
                 uri=uri,
                 input_name=url,
-                event_type=event_type)
+                event_type=event_type,
+            )
         else:
             # if((existing_artifact and len(existing_artifact )!= 0) and c_hash != ""):
             #   url = url + ":" + str(self.execution.id)
             uri = c_hash if c_hash and c_hash.strip() else str(uuid.uuid1())
             artifact = create_new_artifact_event_and_attribution(
                 store=self.store,
                 execution_id=self.execution.id,
                 context_id=self.child_context.id,
                 uri=uri,
                 name=url,
                 type_name="Dataset",
                 event_type=event_type,
                 properties={
                     "git_repo": str(git_repo),
-                    "Commit": str(dataset_commit)},
+                    # passing c_hash value to commit
+                    "Commit": str(dataset_commit),
+                    "url": str(dvc_url_with_pipeline),
+                },
                 artifact_type_properties={
                     "git_repo": mlpb.STRING,
-                    "Commit": mlpb.STRING},
+                    "Commit": mlpb.STRING,
+                    "url": mlpb.STRING,
+                },
                 custom_properties=custom_props,
-                milliseconds_since_epoch=int(
-                    time.time() * 1000),
+                milliseconds_since_epoch=int(time.time() * 1000),
             )
         custom_props["git_repo"] = git_repo
         custom_props["Commit"] = dataset_commit
         self.execution_label_props["git_repo"] = git_repo
         self.execution_label_props["Commit"] = dataset_commit
 
         if self.graph:
             self.driver.create_dataset_node(
                 name,
                 url,
                 uri,
                 event,
                 self.execution.id,
                 self.parent_context,
-                custom_props)
+                custom_props,
+            )
             if event.lower() == "input":
-                self.input_artifacts.append({"Name": name,
-                                             "Path": url,
-                                             "URI": uri,
-                                             "Event": event.lower(),
-                                             "Execution_Name": self.execution_name,
-                                             "Type": "Dataset",
-                                             "Execution_Command": self.execution_command,
-                                             "Pipeline_Id": self.parent_context.id,
-                                             "Pipeline_Name": self.parent_context.name})
+                self.input_artifacts.append(
+                    {
+                        "Name": name,
+                        "Path": url,
+                        "URI": uri,
+                        "Event": event.lower(),
+                        "Execution_Name": self.execution_name,
+                        "Type": "Dataset",
+                        "Execution_Command": self.execution_command,
+                        "Pipeline_Id": self.parent_context.id,
+                        "Pipeline_Name": self.parent_context.name,
+                    }
+                )
                 self.driver.create_execution_links(uri, name, "Dataset")
             else:
                 child_artifact = {
                     "Name": name,
                     "Path": url,
                     "URI": uri,
                     "Event": event.lower(),
                     "Execution_Name": self.execution_name,
                     "Type": "Dataset",
                     "Execution_Command": self.execution_command,
                     "Pipeline_Id": self.parent_context.id,
-                    "Pipeline_Name": self.parent_context.name}
+                    "Pipeline_Name": self.parent_context.name,
+                }
                 self.driver.create_artifact_relationships(
-                    self.input_artifacts, child_artifact, self.execution_label_props)
+                    self.input_artifacts, child_artifact, self.execution_label_props
+                )
         return artifact
 
+    def update_dataset_url(self, artifact: mlpb.Artifact, updated_url: str):
+        for key, value in artifact.properties.items():
+            if key == "url":
+                old_url = value.string_value
+                if updated_url not in old_url:
+                    new_url = f"{old_url},{updated_url}"
+                    artifact.properties[key].string_value = new_url
+        put_artifact(self.store, artifact)
 
-    def log_dataset_with_version(self, url: str, version: str, event: str,
-                                 custom_properties: t.Optional[t.Dict] = None) -> mlpb.Artifact:
+    def update_model_url(self, dup_artifact: list, updated_url: str):
+        for art in dup_artifact:
+            dup_art = art
+            for key, value in dup_art.properties.items():
+                if key == "url":
+                    old_url = value.string_value
+                    if updated_url not in old_url:
+                        new_url = f"{old_url},{updated_url}"
+                        dup_art.properties[key].string_value = new_url
+            put_artifact(self.store, dup_art)
+        return dup_artifact
+
+    def log_dataset_with_version(
+        self,
+        url: str,
+        version: str,
+        event: str,
+        props: t.Optional[t.Dict] = None,
+        custom_properties: t.Optional[t.Dict] = None,
+    ) -> mlpb.Artifact:
         """Logs a dataset when the version(hash) is known"""
-
+        props = {} if props is None else props
         custom_props = {} if custom_properties is None else custom_properties
-        git_repo = git_get_repo()
-        name = re.split('/', url)[-1]
+        git_repo = props.get("git_repo", "")
+        name = url
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
         c_hash = version
         if event.lower() == "input":
             event_type = mlpb.Event.Type.INPUT
 
         # dataset_commit = commit_output(url, self.execution.id)
@@ -464,312 +663,498 @@
             existing_artifact = existing_artifact[0]
 
             # Quick fix- Updating only the name
             if custom_properties is not None:
                 self.update_existing_artifact(
                     existing_artifact, custom_properties)
             uri = c_hash
+            # update url for existing artifact
+            self.update_dataset_url(existing_artifact, props.get("url", ""))
             artifact = link_execution_to_artifact(
                 store=self.store,
                 execution_id=self.execution.id,
                 uri=uri,
                 input_name=url,
-                event_type=event_type)
+                event_type=event_type,
+            )
         else:
             # if((existing_artifact and len(existing_artifact )!= 0) and c_hash != ""):
             #   url = url + ":" + str(self.execution.id)
             uri = c_hash if c_hash and c_hash.strip() else str(uuid.uuid1())
             artifact = create_new_artifact_event_and_attribution(
                 store=self.store,
                 execution_id=self.execution.id,
                 context_id=self.child_context.id,
                 uri=uri,
                 name=url,
                 type_name="Dataset",
                 event_type=event_type,
                 properties={
                     "git_repo": str(git_repo),
-                    "Commit": str(dataset_commit)},
+                    "Commit": str(dataset_commit),
+                    "url": props.get("url", " "),
+                },
                 artifact_type_properties={
                     "git_repo": mlpb.STRING,
-                    "Commit": mlpb.STRING},
+                    "Commit": mlpb.STRING,
+                    "url": mlpb.STRING,
+                },
                 custom_properties=custom_props,
-                milliseconds_since_epoch=int(
-                    time.time() * 1000),
+                milliseconds_since_epoch=int(time.time() * 1000),
             )
         custom_props["git_repo"] = git_repo
         custom_props["Commit"] = dataset_commit
         self.execution_label_props["git_repo"] = git_repo
         self.execution_label_props["Commit"] = dataset_commit
 
         if self.graph:
             self.driver.create_dataset_node(
                 name,
                 url,
                 uri,
                 event,
                 self.execution.id,
                 self.parent_context,
-                custom_props)
+                custom_props,
+            )
             if event.lower() == "input":
-                self.input_artifacts.append({"Name": name,
-                                             "Path": url,
-                                             "URI": uri,
-                                             "Event": event.lower(),
-                                             "Execution_Name": self.execution_name,
-                                             "Type": "Dataset",
-                                             "Execution_Command": self.execution_command,
-                                             "Pipeline_Id": self.parent_context.id,
-                                             "Pipeline_Name": self.parent_context.name})
+                self.input_artifacts.append(
+                    {
+                        "Name": name,
+                        "Path": url,
+                        "URI": uri,
+                        "Event": event.lower(),
+                        "Execution_Name": self.execution_name,
+                        "Type": "Dataset",
+                        "Execution_Command": self.execution_command,
+                        "Pipeline_Id": self.parent_context.id,
+                        "Pipeline_Name": self.parent_context.name,
+                    }
+                )
                 self.driver.create_execution_links(uri, name, "Dataset")
             else:
                 child_artifact = {
                     "Name": name,
                     "Path": url,
                     "URI": uri,
                     "Event": event.lower(),
                     "Execution_Name": self.execution_name,
                     "Type": "Dataset",
                     "Execution_Command": self.execution_command,
                     "Pipeline_Id": self.parent_context.id,
-                    "Pipeline_Name": self.parent_context.name}
+                    "Pipeline_Name": self.parent_context.name,
+                }
                 self.driver.create_artifact_relationships(
-                    self.input_artifacts, child_artifact,
-                    self.execution_label_props)
+                    self.input_artifacts, child_artifact, self.execution_label_props
+                )
         return artifact
 
     # Add the model to dvc do a git commit and store the commit id in MLMD
-    def log_model(self, path: str, event: str, model_framework: str = "Default",
-                  model_type: str = "Default", model_name: str = "Default",
-                  custom_properties: t.Optional[t.Dict] = None) -> mlpb.Artifact:
+    def log_model(
+        self,
+        path: str,
+        event: str,
+        model_framework: str = "Default",
+        model_type: str = "Default",
+        model_name: str = "Default",
+        custom_properties: t.Optional[t.Dict] = None,
+    ) -> mlpb.Artifact:
         """Logs a model.
-
         The model is added to dvc and the metadata file (.dvc) gets committed to git.
-
         Example:
             ```python
             artifact: mlmd.proto.Artifact= cmf.log_model(
                 path="path/to/model.pkl",
                 event="output",
                 model_framework="SKlearn",
                 model_type="RandomForestClassifier",
                 model_name="RandomForestClassifier:default"
             )
             ```
-
         Args:
             path: Path to the model file.
             event: Takes arguments `INPUT` OR `OUTPUT`.
             model_framework: Framework used to create the model.
             model_type: Type of model algorithm used.
             model_name: Name of the algorithm used.
             custom_properties: The model properties.
-
         Returns:
             Artifact object from ML Metadata library associated with the new model artifact.
         """
 
         if custom_properties is None:
             custom_properties = {}
         custom_props = {} if custom_properties is None else custom_properties
         # name = re.split('/', path)[-1]
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
         if event.lower() == "input":
             event_type = mlpb.Event.Type.INPUT
 
-        model_commit = commit_output(path, self.execution.id)
+        commit_output(path, self.execution.id)
         c_hash = dvc_get_hash(path)
+        model_commit = c_hash
 
         # If connecting to an existing artifact - The name of the artifact is
         # used as path/steps/key
         model_uri = path + ":" + c_hash
-        # uri = ""
+        dvc_url = dvc_get_url(path, False)
+        url = dvc_url
+        url_with_pipeline = f"{self.parent_context.name}:{url}"
+        uri = ""
         if c_hash and c_hash.strip():
             uri = c_hash.strip()
             existing_artifact.extend(self.store.get_artifacts_by_uri(uri))
         else:
             raise RuntimeError("Model commit failed, Model uri empty")
 
-        if existing_artifact and len(
-                existing_artifact) != 0 and event_type == mlpb.Event.Type.INPUT:
+        if (
+            existing_artifact
+            and len(existing_artifact) != 0
+            and event_type == mlpb.Event.Type.INPUT
+        ):
+            # update url for existing artifact
+            existing_artifact = self.update_model_url(
+                existing_artifact, url_with_pipeline
+            )
             artifact = link_execution_to_artifact(
                 store=self.store,
                 execution_id=self.execution.id,
                 uri=c_hash,
                 input_name=model_uri,
-                event_type=event_type)
+                event_type=event_type,
+            )
             model_uri = artifact.name
         else:
-
             uri = c_hash if c_hash and c_hash.strip() else str(uuid.uuid1())
             model_uri = model_uri + ":" + str(self.execution.id)
             artifact = create_new_artifact_event_and_attribution(
                 store=self.store,
                 execution_id=self.execution.id,
                 context_id=self.child_context.id,
                 uri=uri,
                 name=model_uri,
                 type_name="Model",
                 event_type=event_type,
                 properties={
                     "model_framework": str(model_framework),
                     "model_type": str(model_type),
                     "model_name": str(model_name),
-                    "Commit": str(model_commit)},
+                    # passing c_hash value to commit
+                    "Commit": str(model_commit),
+                    "url": str(url_with_pipeline),
+                },
                 artifact_type_properties={
                     "model_framework": mlpb.STRING,
                     "model_type": mlpb.STRING,
                     "model_name": mlpb.STRING,
                     "Commit": mlpb.STRING,
+                    "url": mlpb.STRING,
                 },
                 custom_properties=custom_props,
-                milliseconds_since_epoch=int(
-                    time.time() * 1000),
+                milliseconds_since_epoch=int(time.time() * 1000),
             )
         # custom_properties["Commit"] = model_commit
         self.execution_label_props["Commit"] = model_commit
         if self.graph:
             self.driver.create_model_node(
                 model_uri,
                 uri,
                 event,
                 self.execution.id,
                 self.parent_context,
-                custom_props)
+                custom_props,
+            )
             if event.lower() == "input":
-
                 self.input_artifacts.append(
-                    {"Name": model_uri, "URI": uri, "Event": event.lower(),
+                    {
+                        "Name": model_uri,
+                        "URI": uri,
+                        "Event": event.lower(),
                         "Execution_Name": self.execution_name,
-                     "Type": "Model", "Execution_Command": self.execution_command,
-                     "Pipeline_Id": self.parent_context.id,
-                     "Pipeline_Name": self.parent_context.name})
+                        "Type": "Model",
+                        "Execution_Command": self.execution_command,
+                        "Pipeline_Id": self.parent_context.id,
+                        "Pipeline_Name": self.parent_context.name,
+                    }
+                )
                 self.driver.create_execution_links(uri, model_uri, "Model")
             else:
+                child_artifact = {
+                    "Name": model_uri,
+                    "URI": uri,
+                    "Event": event.lower(),
+                    "Execution_Name": self.execution_name,
+                    "Type": "Model",
+                    "Execution_Command": self.execution_command,
+                    "Pipeline_Id": self.parent_context.id,
+                    "Pipeline_Name": self.parent_context.name,
+                }
+
+                self.driver.create_artifact_relationships(
+                    self.input_artifacts, child_artifact, self.execution_label_props
+                )
+
+        return artifact
+
+    # Add the model to dvc do a git commit and store the commit id in MLMD
+    def log_model_with_version(
+        self,
+        path: str,
+        event: str,
+        props=None,
+        custom_properties: t.Optional[t.Dict] = None,
+    ) -> object:
+        """Logs a model when the version(hash) is known
+         The model is added to dvc and the metadata file (.dvc) gets committed to git.
+        Example:
+            ```python
+            artifact: mlmd.proto.Artifact= cmf.log_model_with_version(
+                path="path/to/model.pkl",
+                event="output",
+                props={
+                        "url": "/home/user/local-storage/bf/629ccd5cd008066b72c04f9a918737",
+                        "model_type": "RandomForestClassifier",
+                        "model_name": "RandomForestClassifier:default",
+                        "Commit": "commit 1146dad8b74cae205db6a3132ea403db1e4032e5",
+                        "model_framework": "SKlearn",
+                       },
+                custom_properties={
+                        "uri": "bf629ccd5cd008066b72c04f9a918737",
+                },
+
+            )
+            ```
+        Args:
+            path: Path to the model file.
+            event: Takes arguments `INPUT` OR `OUTPUT`.
+            model_framework: Framework used to create the model.
+            model_type: Type of model algorithm used.
+            model_name: Name of the algorithm used.
+            custom_properties: The model properties.
+        Returns:
+            Artifact object from ML Metadata library associated with the new model artifact.
+        """
+
+        if custom_properties is None:
+            custom_properties = {}
+        custom_props = {} if custom_properties is None else custom_properties
+        name = re.split("/", path)[-1]
+        event_type = mlpb.Event.Type.OUTPUT
+        existing_artifact = []
+        if event.lower() == "input":
+            event_type = mlpb.Event.Type.INPUT
 
+        # props["commit"] = "" # To do get from incoming data
+        c_hash = props.get("uri", " ")
+        # If connecting to an existing artifact - The name of the artifact is used as path/steps/key
+        model_uri = path + ":" + c_hash
+        # dvc_url = dvc_get_url(path, False)
+        url = props.get("url", "")
+        # uri = ""
+        if c_hash and c_hash.strip():
+            uri = c_hash.strip()
+            existing_artifact.extend(self.store.get_artifacts_by_uri(uri))
+        else:
+            raise RuntimeError("Model commit failed, Model uri empty")
+
+        if (
+            existing_artifact
+            and len(existing_artifact) != 0
+            and event_type == mlpb.Event.Type.INPUT
+        ):
+            # update url for existing artifact
+            existing_artifact = self.update_model_url(existing_artifact, url)
+            artifact = link_execution_to_artifact(
+                store=self.store,
+                execution_id=self.execution.id,
+                uri=c_hash,
+                input_name=model_uri,
+                event_type=event_type,
+            )
+            model_uri = artifact.name
+        else:
+            uri = c_hash if c_hash and c_hash.strip() else str(uuid.uuid1())
+            model_uri = model_uri + ":" + str(self.execution.id)
+            artifact = create_new_artifact_event_and_attribution(
+                store=self.store,
+                execution_id=self.execution.id,
+                context_id=self.child_context.id,
+                uri=uri,
+                name=model_uri,
+                type_name="Model",
+                event_type=event_type,
+                properties={
+                    "model_framework": props.get("model_framework", ""),
+                    "model_type": props.get("model_type", ""),
+                    "model_name": props.get("model_name", ""),
+                    "Commit": props.get("Commit", ""),
+                    "url": str(url),
+                },
+                artifact_type_properties={
+                    "model_framework": mlpb.STRING,
+                    "model_type": mlpb.STRING,
+                    "model_name": mlpb.STRING,
+                    "Commit": mlpb.STRING,
+                    "url": mlpb.STRING,
+                },
+                custom_properties=custom_props,
+                milliseconds_since_epoch=int(time.time() * 1000),
+            )
+        # custom_properties["Commit"] = model_commit
+        # custom_props["url"] = url
+        self.execution_label_props["Commit"] = props.get("Commit", "")
+        if self.graph:
+            self.driver.create_model_node(
+                model_uri,
+                uri,
+                event,
+                self.execution.id,
+                self.parent_context,
+                custom_props,
+            )
+            if event.lower() == "input":
+                self.input_artifacts.append(
+                    {
+                        "Name": model_uri,
+                        "URI": uri,
+                        "Event": event.lower(),
+                        "Execution_Name": self.execution_name,
+                        "Type": "Model",
+                        "Execution_Command": self.execution_command,
+                        "Pipeline_Id": self.parent_context.id,
+                        "Pipeline_Name": self.parent_context.name,
+                    }
+                )
+                self.driver.create_execution_links(uri, model_uri, "Model")
+            else:
                 child_artifact = {
                     "Name": model_uri,
                     "URI": uri,
                     "Event": event.lower(),
                     "Execution_Name": self.execution_name,
                     "Type": "Model",
                     "Execution_Command": self.execution_command,
                     "Pipeline_Id": self.parent_context.id,
-                    "Pipeline_Name": self.parent_context.name}
+                    "Pipeline_Name": self.parent_context.name,
+                }
                 self.driver.create_artifact_relationships(
-                    self.input_artifacts, child_artifact, self.execution_label_props)
+                    self.input_artifacts, child_artifact, self.execution_label_props
+                )
 
         return artifact
 
-    def log_execution_metrics(self, metrics_name: str, custom_properties: t.Optional[t.Dict] = None) -> mlpb.Artifact:
+    def log_execution_metrics(
+        self, metrics_name: str, custom_properties: t.Optional[t.Dict] = None
+    ) -> mlpb.Artifact:
         """Log the metadata associated with the execution (coarse-grained tracking).
-
         It is stored as a metrics artifact. This does not have a backing physical file, unlike other artifacts that we
         have.
-
         Example:
             ```python
             exec_metrics: mlpb.Artifact = cmf.log_execution_metrics(
                 metrics_name="Training_Metrics",
                 {"auc": auc, "loss": loss}
             )
             ```
-
         Args:
             metrics_name: Name to identify the metrics.
             custom_properties: Dictionary with metric values.
-
         Returns:
               Artifact object from ML Metadata library associated with the new coarse-grained metrics artifact.
         """
         custom_props = {} if custom_properties is None else custom_properties
         uri = str(uuid.uuid1())
         metrics_name = metrics_name + ":" + uri + ":" + str(self.execution.id)
         metrics = create_new_artifact_event_and_attribution(
             store=self.store,
             execution_id=self.execution.id,
             context_id=self.child_context.id,
             uri=uri,
             name=metrics_name,
             type_name="Metrics",
             event_type=mlpb.Event.Type.OUTPUT,
-            properties={
-                "metrics_name": metrics_name},
-            artifact_type_properties={
-                "metrics_name": mlpb.STRING},
+            properties={"metrics_name": metrics_name},
+            artifact_type_properties={"metrics_name": mlpb.STRING},
             custom_properties=custom_props,
-            milliseconds_since_epoch=int(
-                time.time() * 1000),
+            milliseconds_since_epoch=int(time.time() * 1000),
         )
         if self.graph:
             # To do create execution_links
             self.driver.create_metrics_node(
                 metrics_name,
                 uri,
                 "output",
                 self.execution.id,
                 self.parent_context,
-                custom_props)
+                custom_props,
+            )
             child_artifact = {
                 "Name": metrics_name,
                 "URI": uri,
                 "Event": "output",
                 "Execution_Name": self.execution_name,
                 "Type": "Metrics",
                 "Execution_Command": self.execution_command,
                 "Pipeline_Id": self.parent_context.id,
-                "Pipeline_Name": self.parent_context.name}
+                "Pipeline_Name": self.parent_context.name,
+            }
             self.driver.create_artifact_relationships(
-                self.input_artifacts, child_artifact, self.execution_label_props)
+                self.input_artifacts, child_artifact, self.execution_label_props
+            )
         return metrics
 
-    def log_metric(self, metrics_name: str, custom_properties: t.Optional[t.Dict] = None) -> None:
+    def log_metric(
+        self, metrics_name: str, custom_properties: t.Optional[t.Dict] = None
+    ) -> None:
         """Stores the fine-grained (per step or per epoch) metrics to memory.
-
         The metrics provided are stored in a parquet file. The `commit_metrics` call add the parquet file in the version
         control framework. The metrics written in the parquet file can be retrieved using the `read_metrics` call.
-
         Example:
             ```python
             # Can be called at every epoch or every step in the training. This is logged to a parquet file and committed
             # at the commit stage.
-
             # Inside training loop
             while True:
                  cmf.log_metric("training_metrics", {"train_loss": train_loss})
             cmf.commit_metrics("training_metrics")
             ```
-
         Args:
             metrics_name: Name to identify the metrics.
             custom_properties: Dictionary with metrics.
         """
         if metrics_name in self.metrics:
             key = max((self.metrics[metrics_name]).keys()) + 1
             self.metrics[metrics_name][key] = custom_properties
         else:
             self.metrics[metrics_name] = {}
             self.metrics[metrics_name][1] = custom_properties
 
-
     def commit_metrics(self, metrics_name: str):
         """Writes the inmemory metrics to parquet file
-
         Commit the metrics file associated with the metrics id to dvc and git and
         store the artifact in mlmd
         """
         metrics_df = pd.DataFrame.from_dict(
-            self.metrics[metrics_name], orient='index')
-        metrics_df.index.names = ['SequenceNumber']
+            self.metrics[metrics_name], orient="index")
+        metrics_df.index.names = ["SequenceNumber"]
         metrics_df.to_parquet(metrics_name)
-        metrics_commit = commit_output(metrics_name, self.execution.id)
+        commit_output(metrics_name, self.execution.id)
         uri = dvc_get_hash(metrics_name)
-        name = metrics_name + ":" + uri + ":" + \
-            str(self.execution.id) + ":" + str(uuid.uuid1())
+        metrics_commit = uri
+        name = (
+            metrics_name
+            + ":"
+            + uri
+            + ":"
+            + str(self.execution.id)
+            + ":"
+            + str(uuid.uuid1())
+        )
+        # passing uri value to commit
         custom_props = {"Name": metrics_name, "Commit": metrics_commit}
         metrics = create_new_artifact_event_and_attribution(
             store=self.store,
             execution_id=self.execution.id,
             context_id=self.child_context.id,
             uri=uri,
             name=name,
@@ -781,197 +1166,212 @@
         if self.graph:
             self.driver.create_metrics_node(
                 name,
                 uri,
                 "output",
                 self.execution.id,
                 self.parent_context,
-                custom_props)
+                custom_props,
+            )
             child_artifact = {
                 "Name": name,
                 "URI": uri,
                 "Event": "output",
                 "Execution_Name": self.execution_name,
                 "Type": "Metrics",
                 "Execution_Command": self.execution_command,
-                "Pipeline_Id": self.parent_context.id}
+                "Pipeline_Id": self.parent_context.id,
+            }
             self.driver.create_artifact_relationships(
-                self.input_artifacts, child_artifact, self.execution_label_props)
+                self.input_artifacts, child_artifact, self.execution_label_props
+            )
         return metrics
 
-
-    def log_validation_output(self, version: str, custom_properties: t.Optional[t.Dict] = None) -> object:
+    def log_validation_output(
+        self, version: str, custom_properties: t.Optional[t.Dict] = None
+    ) -> object:
         uri = str(uuid.uuid1())
         return create_new_artifact_event_and_attribution(
             store=self.store,
             execution_id=self.execution.id,
             context_id=self.child_context.id,
             uri=uri,
             name=uri,
             type_name="Validation_output",
             event_type=mlpb.Event.Type.INTERNAL_OUTPUT,
             properties={"version": version},
-
             artifact_type_properties={"version": mlpb.STRING},
             custom_properties=custom_properties,
             milliseconds_since_epoch=int(time.time() * 1000),
         )
 
-
-    def update_existing_artifact(self, artifact: mlpb.Artifact, custom_props: t.Dict):
+    def update_existing_artifact(
+        self, artifact: mlpb.Artifact, custom_properties: t.Dict
+    ):
         """Updates an existing artifact and stores it back to mlmd"""
-        for key, value in custom_props.items():
+        for key, value in custom_properties.items():
             if isinstance(value, int):
                 artifact.custom_properties[key].int_value = value
             else:
                 artifact.custom_properties[key].string_value = str(value)
         put_artifact(self.store, artifact)
 
-
     def get_artifact(self, artifact_id: int) -> mlpb.Artifact:
         """Gets the artifact object from mlmd"""
         return get_artifacts_by_id(self.store, [artifact_id])[0]
 
+    # To Do - The interface should be simplified.
+    # To Do - Links should be created in mlmd also.
+    # Todo - assumes source as Dataset and target as slice - should be generic and accomodate any types
+    def link_artifacts(
+        self, artifact_source: mlpb.Artifact, artifact_target: mlpb.Artifact
+    ):
+        self.driver.create_links(artifact_source.name,
+                                 artifact_target.name, "derived")
 
     def update_model_output(self, artifact: mlpb.Artifact):
         """updates an artifact"""
         put_artifact(self.store, artifact)
 
     def create_dataslice(self, name: str) -> "Cmf.DataSlice":
         """Creates a dataslice object.
-
         Once created, users can add data instances to this data slice with [add_data][cmflib.cmf.Cmf.DataSlice.add_data]
         method. Users are also responsible for committing data slices by calling the
         [commit][cmflib.cmf.Cmf.DataSlice.commit] method.
-
         Example:
             ```python
             dataslice = cmf.create_dataslice("slice-a")
             ```
-
         Args:
             name: Name to identify the dataslice.
 
         Returns:
             Instance of a newly created [DataSlice][cmflib.cmf.Cmf.DataSlice].
         """
         return Cmf.DataSlice(name, self)
 
-
     def read_dataslice(self, name: str) -> pd.DataFrame:
         """Reads the dataslice"""
         # To do checkout if not there
         df = pd.read_parquet(name)
         return df
 
     # To do - Once update the hash and the new version should be updated in
     # the mlmd
-    def update_dataslice(self, name: str, record: str, custom_props: t.Dict):
+    def update_dataslice(self, name: str, record: str, custom_properties: t.Dict):
         df = pd.read_parquet(name)
-        temp_dict = df.to_dict('index')
-        temp_dict[record].update(custom_props)
-        dataslice_df = pd.DataFrame.from_dict(temp_dict, orient='index')
-        dataslice_df.index.names = ['Path']
+        temp_dict = df.to_dict("index")
+        temp_dict[record].update(custom_properties)
+        dataslice_df = pd.DataFrame.from_dict(temp_dict, orient="index")
+        dataslice_df.index.names = ["Path"]
         dataslice_df.to_parquet(name)
 
     class DataSlice:
         """A data slice represents a named subset of data.
-
         It can be used to track performance of an ML model on different slices of the training or testing dataset
         splits. This can be useful from different perspectives, for instance, to mitigate model bias.
-
         > Instances of data slices are not meant to be created manually by users. Instead, use
         [Cmf.create_dataslice][cmflib.cmf.Cmf.create_dataslice] method.
-
         """
-        def __init__(self, name: str, writer, props: t.Optional[t.Dict] = None):
-            self.props = {} if props is None else props
+
+        def __init__(self, name: str, writer):
+            self.props = {}
             self.name = name
             self.writer = writer
 
-        def add_data(self, path: str, custom_props: t.Optional[t.Dict] = None) -> None:
-            """Add data to create the dataslice.
+        # def add_files(self, list_of_files:np.array ):
+        #    for i in list_of_files:
 
+        def add_data(
+            self, path: str, custom_properties: t.Optional[t.Dict] = None
+        ) -> None:
+            """Add data to create the dataslice.
             Currently supported only for file abstractions. Pre-condition - the parent folder, containing the file
                 should already be versioned.
-
             Example:
                 ```python
                 dataslice.add_data(f"data/raw_data/{j}.xml)
                 ```
             Args:
                 path: Name to identify the file to be added to the dataslice.
-                custom_props: Properties associated with this datum.
+                custom_properties: Properties associated with this datum.
             """
 
             self.props[path] = {}
-            self.props[path]['hash'] = dvc_get_hash(path)
-            if custom_props:
-                for k, v in custom_props.items():
+            # self.props[path]['hash'] = dvc_get_hash(path)
+            parent_path = path.rsplit("/", 1)[0]
+            self.data_parent = parent_path.rsplit("/", 1)[1]
+            if custom_properties:
+                for k, v in custom_properties.items():
                     self.props[path][k] = v
 
-#        """
-#        Place holder for updating back to mlmd
+        #        """
+        #        Place holder for updating back to mlmd
 
-#        def update_data(self, path, custom_props:{}):
-#            for k ,v in custom_props.items():
-#                self.props[path][k] = v
-#        """
+        #        def update_data(self, path, custom_props:{}):
+        #            for k ,v in custom_props.items():
+        #                self.props[path][k] = v
+        #        """
 
-        def commit(self, custom_props: t.Optional[t.Dict] = None) -> None:
+        def commit(self, custom_properties: t.Optional[t.Dict] = None) -> None:
             """Commit the dataslice.
-
             The created dataslice is versioned and added to underneath data versioning software.
-
             Example:
-                ```python
+
                 dataslice.commit()
                 ```
-
             Args:
-                custom_props: Properties associated with this data slice.
+                custom_properties: Dictionary to store key value pairs associated with Dataslice
+                Example{"mean":2.5, "median":2.6}
             """
+            custom_props = {} if custom_properties is None else custom_properties
             git_repo = git_get_repo()
-            dataslice_df = pd.DataFrame.from_dict(self.props, orient='index')
-            dataslice_df.index.names = ['Path']
+            dataslice_df = pd.DataFrame.from_dict(self.props, orient="index")
+            dataslice_df.index.names = ["Path"]
             dataslice_df.to_parquet(self.name)
             existing_artifact = []
 
-            dataslice_commit = commit_output(
-                self.name, self.writer.execution.id)
+            commit_output(self.name, self.writer.execution.id)
             c_hash = dvc_get_hash(self.name)
+            dataslice_commit = c_hash
             remote = dvc_get_url(self.name)
             if c_hash and c_hash.strip():
                 existing_artifact.extend(
                     self.writer.store.get_artifacts_by_uri(c_hash))
             if existing_artifact and len(existing_artifact) != 0:
                 print("Adding to existing data slice")
-                _ = link_execution_to_input_artifact(
+                slice = link_execution_to_input_artifact(
                     store=self.writer.store,
                     execution_id=self.writer.execution.id,
                     uri=c_hash,
-                    input_name=self.name + ":" + c_hash)
+                    input_name=self.name + ":" + c_hash,
+                )
             else:
                 props = {
-                    "Commit": dataslice_commit,
+                    "Commit": dataslice_commit,  # passing c_hash value to commit
                     "git_repo": git_repo,
-                    "Remote": remote}
-                custom_properties = props.update(
-                    custom_props) if custom_props else props
-                create_new_artifact_event_and_attribution(
+                    "Remote": remote,
+                }
+                props.update(custom_props)
+                slice = create_new_artifact_event_and_attribution(
                     store=self.writer.store,
                     execution_id=self.writer.execution.id,
                     context_id=self.writer.child_context.id,
                     uri=c_hash,
                     name=self.name + ":" + c_hash,
                     type_name="Dataslice",
                     event_type=mlpb.Event.Type.OUTPUT,
-                    custom_properties=custom_properties,
+                    custom_properties=props,
                     milliseconds_since_epoch=int(time.time() * 1000),
                 )
+            if self.writer.graph:
+                self.writer.driver.create_dataslice_node(
+                    self.name, self.name + ":" + c_hash, c_hash, self.data_parent, props
+                )
+            return slice
 
 
 #        """Temporary code"""
 #
 #        def materialize(self, name):
 #            slicedir = name + "-" + "dir"
 #            os.mkdir(slicedir)
```

### Comparing `cmflib-0.0.2/cmflib/cmfquery.py` & `cmflib-0.0.3/cmflib/cmfquery.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###
 
 import pandas as pd
 from ml_metadata.metadata_store import metadata_store
 from ml_metadata.proto import metadata_store_pb2 as mlpb
+from cmflib.mlmd_objects import CONTEXT_LIST
+import json
 
 
 class CmfQuery(object):
     def __init__(self, filepath: str = "mlmd"):
         config = mlpb.ConnectionConfig()
         config.sqlite.filename_uri = filepath
         self.store = metadata_store.MetadataStore(config)
@@ -112,32 +114,34 @@
         artifacts = self.store.get_artifacts()
         for art in artifacts:
             if art.name == name:
                 artifact = art
                 break
         return self.get_artifact_df(artifact)
 
-    def get_all_artifacts_for_execution(self, execution_id: int) -> pd.DataFrame:
+    def get_all_artifacts_for_execution(self, execution_id: int) -> pd.DataFrame: # change here
         df = pd.DataFrame()
         input_artifacts = []
         output_artifacts = []
         events = self.store.get_events_by_execution_ids([execution_id])
         for event in events:
             if event.type == mlpb.Event.Type.INPUT:  # 3 - INPUT #4 - Output
                 input_artifacts.extend(self.store.get_artifacts_by_id([event.artifact_id]))
             else:
                 output_artifacts.extend(self.store.get_artifacts_by_id([event.artifact_id]))
         for art in input_artifacts:
             d1 = self.get_artifact_df(art)
             d1["event"] = "INPUT"
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
         for art in output_artifacts:
             d1 = self.get_artifact_df(art)
             d1["event"] = "OUTPUT"
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
         return df
 
     def get_all_executions_for_artifact(self, artifact_name: str) -> pd.DataFrame:
         selected_artifact = None
         linked_execution = {}
         events = []
         df = pd.DataFrame()
@@ -154,15 +158,16 @@
             linked_execution["execution_id"] = evt.execution_id
             linked_execution["execution_name"] = self.store.get_executions_by_id([evt.execution_id])[0].name
             ctx = self.store.get_contexts_by_execution(evt.execution_id)[0]
             linked_execution["stage"] = self.store.get_contexts_by_execution(evt.execution_id)[0].name
 
             linked_execution["pipeline"] = self.store.get_parent_contexts_by_context(ctx.id)[0].name
             d1 = pd.DataFrame(linked_execution, index=[0, ])
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
 
         return df
 
     def get_one_hop_child_artifacts(self, artifact_name: str) -> pd.DataFrame:
         df = pd.DataFrame()
 
         artifact = None
@@ -180,24 +185,27 @@
         artifacts_ids = set(
             event.artifact_id
             for event in self.store.get_events_by_execution_ids(executions_ids)
             if event.type == mlpb.Event.OUTPUT)
         artifacts = self.store.get_artifacts_by_id(artifacts_ids)
         for art in artifacts:
             d1 = self.get_artifact_df(art)
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
         return df
 
     def get_all_child_artifacts(self, artifact_name: str) -> pd.DataFrame:
         df = pd.DataFrame()
         d1 = self.get_one_hop_child_artifacts(artifact_name)
-        df = df.append(d1, sort=True, ignore_index=True)
+        #df = df.append(d1, sort=True, ignore_index=True)
+        df = pd.concat([df, d1], sort=True, ignore_index=True)
         for row in d1.itertuples():
             d1 = self.get_all_child_artifacts(row.name)
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
         df = df.drop_duplicates(subset=None, keep='first', inplace=False)
         return df
 
     def get_one_hop_parent_artifacts(self, artifact_name: str) -> pd.DataFrame:
         df = pd.DataFrame()
 
         artifact = None
@@ -215,24 +223,27 @@
         artifacts_ids = set(
             event.artifact_id
             for event in self.store.get_events_by_execution_ids(executions_ids)
             if event.type == mlpb.Event.INPUT)
         artifacts = self.store.get_artifacts_by_id(artifacts_ids)
         for art in artifacts:
             d1 = self.get_artifact_df(art)
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
         return df
 
     def get_all_parent_artifacts(self, artifact_name: str) -> pd.DataFrame:
         df = pd.DataFrame()
         d1 = self.get_one_hop_parent_artifacts(artifact_name)
-        df = df.append(d1, sort=True, ignore_index=True)
+        #df = df.append(d1, sort=True, ignore_index=True)
+        df = pd.concat([df, d1], sort=True, ignore_index=True)
         for row in d1.itertuples():
             d1 = self.get_all_parent_artifacts(row.name)
-            df = df.append(d1, sort=True, ignore_index=True)
+            #df = df.append(d1, sort=True, ignore_index=True)
+            df = pd.concat([df, d1], sort=True, ignore_index=True)
         df = df.drop_duplicates(subset=None, keep='first', inplace=False)
         return df
 
     def get_all_parent_executions(self, artifact_name:str)-> pd.DataFrame:
         df = self.get_all_parent_artifacts(artifact_name)
         artifact_ids = df.id.values.tolist()
 
@@ -244,29 +255,147 @@
 
         df = pd.DataFrame()
         for exe in executions:
             d1 = self._transform_to_dataframe(exe)
             # df = df.append(d1, sort=True, ignore_index=True)
             df = pd.concat([df, d1], sort=True, ignore_index=True)
         return df
-        
 
     def find_producer_execution(self, artifact_name: str) -> object:
         artifact = None
         artifacts = self.store.get_artifacts()
         for art in artifacts:
             if art.name == artifact_name:
                 artifact = art
                 break
 
         executions_ids = set(
             event.execution_id
             for event in self.store.get_events_by_artifact_ids([artifact.id])
             if event.type == mlpb.Event.OUTPUT)
         return self.store.get_executions_by_id(executions_ids)[0]
+    
+    def get_metrics(self, metrics_name:str) ->pd.DataFrame:
+        metric = None
+        metrics = self.store.get_artifacts_by_type("Step_Metrics")
+        for m in metrics:
+            if m.name == metrics_name:
+                metric = m
+                break
+        if metric is None:
+            print("Error : The given metrics does not exist")
+            return None
+        name = ""
+        for k, v in metric.custom_properties.items():
+            if k == "Name":
+                name = v
+                break
+        df = pd.read_parquet(name)
+        return df
+    
+    def read_dataslice(self, name: str) -> pd.DataFrame:
+        """Reads the dataslice"""
+        # To do checkout if not there
+        df = pd.read_parquet(name)
+        return df
+        
+
+
+
+    @staticmethod
+    def __get_node_properties(node) -> dict:
+        # print(node)
+        node_dict = {}
+        for attr in dir(node):
+            if attr in CONTEXT_LIST:
+                if attr == "properties":
+                    node_dict["properties"] = CmfQuery.__get_properties(node)
+                elif attr == "custom_properties":
+                    node_dict["custom_properties"] = CmfQuery.__get_customproperties(
+                        node
+                    )
+                else:
+                    node_dict[attr] = node.__getattribute__(attr)
+
+        # print(node_dict)
+        return node_dict
+
+    @staticmethod
+    def __get_properties(node) -> dict:
+        prop_dict = {}
+        for k, v in node.properties.items():
+            if v.HasField("string_value"):
+                prop_dict[k] = v.string_value
+            elif v.HasField("int_value"):
+                prop_dict[k] = v.int_value
+            else:
+                prop_dict[k] = v.double_value
+        return prop_dict
+
+    @staticmethod
+    def __get_customproperties(node) -> dict:
+        prop_dict = {}
+        for k, v in node.custom_properties.items():
+            if v.HasField("string_value"):
+                prop_dict[k] = v.string_value
+            elif v.HasField("int_value"):
+                prop_dict[k] = v.int_value
+            else:
+                prop_dict[k] = v.double_value
+        return prop_dict
+
+    def dumptojson(self, pipeline_name: str, exec_id):
+        mlmd_json = {}
+        mlmd_json["Pipeline"] = []
+        contexts = self.store.get_contexts_by_type("Parent_Context")
+        for ctx in contexts:
+            if ctx.name == pipeline_name:
+                ctx_dict = CmfQuery.__get_node_properties(ctx)
+                ctx_dict["stages"] = []
+                stages = self.store.get_children_contexts_by_context(ctx.id)
+                for stage in stages:
+                    stage_dict = CmfQuery.__get_node_properties(stage)
+                    # ctx["stages"].append(stage_dict)
+                    stage_dict["executions"] = []
+                    executions = self.store.get_executions_by_context(stage.id)
+                    if exec_id is None:
+                        list_executions = [exe for exe in executions]
+                    elif exec_id is not None:
+                        list_executions = [
+                            exe for exe in executions if exe.id == int(exec_id)
+                        ]
+                    else:
+                        return "Invalid execution id given."
+                    for exe in list_executions:
+                        exe_dict = CmfQuery.__get_node_properties(exe)
+                        exe_type = self.store.get_execution_types_by_id([exe.type_id])
+                        exe_dict["type"] = exe_type[0].name
+                        exe_dict["events"] = []
+                        if exe.name != "":
+                            exe_dict["Name"] = exe.name
+                        events = self.store.get_events_by_execution_ids([exe.id])
+                        for evt in events:
+                            evt_dict = CmfQuery.__get_node_properties(evt)
+                            artifact = self.store.get_artifacts_by_id([evt.artifact_id])
+                            if artifact is not None:
+                                artifact_type = self.store.get_artifact_types_by_id(
+                                    [artifact[0].type_id]
+                                )
+                                artifact_dict = CmfQuery.__get_node_properties(
+                                    artifact[0]
+                                )
+                                artifact_dict["type"] = artifact_type[0].name
+                                evt_dict["artifact"] = artifact_dict
+                            exe_dict["events"].append(evt_dict)
+                        stage_dict["executions"].append(exe_dict)
+                    ctx_dict["stages"].append(stage_dict)
+                mlmd_json["Pipeline"].append(ctx_dict)
+                json_str = json.dumps(mlmd_json)
+                # json_str = jsonpickle.encode(ctx_dict)
+                return json_str
 
     '''def materialize(self, artifact_name:str):
        artifacts = self.store.get_artifacts()
        for art in artifacts:
            if art.name == artifact_name:
                selected_artifact = art
                break
```

### Comparing `cmflib-0.0.2/cmflib/dvc_wrapper.py` & `cmflib-0.0.3/cmflib/dvc_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     commit = ""
     is_git_repo = False
     try:
         process = subprocess.Popen(['git',
                                     'rev-parse',
                                     '--is-inside-work-tree'],
                                    stdout=subprocess.PIPE,
+                                   stderr=subprocess.PIPE,
                                    universal_newlines=True)
         # output = process.stdout.readline()
         output, error = process.communicate(timeout=60)
 
         is_git_repo = output.strip()
     except Exception as err:
         process.kill()
@@ -194,14 +195,40 @@
         process.kill()
         outs, errs = process.communicate()
         print(f"Unexpected {err}, {type(err)}")
         print(f"Unexpected {outs}")
         print(f"Unexpected {errs}")
     return commit
 
+def git_commit(execution_id: str) -> str:
+    commit = ""
+    process = None
+    try:
+        # To-Do : Parse the output and report if error
+        process = subprocess.Popen(['git', 'commit', '-m ' + 'commiting ' + str(execution_id)],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+        process = subprocess.Popen(['git', 'log'],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        # To-Do : Parse the output and report if error
+        output, errs = process.communicate(timeout=60)
+        commit = output.splitlines()[0].strip()
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
 
 def commit_output(folder: str, execution_id: str) -> str:
     commit = ""
     process = ""
     try:
         process = subprocess.Popen(['dvc', 'add', folder],
                                    stdout=subprocess.PIPE,
@@ -210,36 +237,36 @@
         # To-Do : Parse the output and report if error
         output, errs = process.communicate(timeout=60)
         commit = output.strip()
         process = subprocess.Popen(['git', 'add', folder + '.dvc'],
                                    stdout=subprocess.PIPE,
                                    universal_newlines=True)
         # To-Do : Parse the output and report if error
-        _, _ = process.communicate(timeout=60)
-        process = subprocess.Popen(
-            [
-                'git',
-                'commit',
-                '-m ' +
-                'commiting dvc metadata file for ' +
-                str(folder) +
-                "-" +
-                str(execution_id)],
-            stdout=subprocess.PIPE,
-            universal_newlines=True)
-
-        output, errs = process.communicate(timeout=60)
-        commit = output.strip()
-
-        process = subprocess.Popen(['git', 'log', folder + '.dvc'],
-                                   stdout=subprocess.PIPE,
-                                   universal_newlines=True)
+        # _, _ = process.communicate(timeout=60)
+        # process = subprocess.Popen(
+        #     [
+        #         'git',
+        #         'commit',
+        #         '-m ' +
+        #         'commiting dvc metadata file for ' +
+        #         str(folder) +
+        #         "-" +
+        #         str(execution_id)],
+        #     stdout=subprocess.PIPE,
+        #     universal_newlines=True)
+        # 
+        # output, errs = process.communicate(timeout=60)
+        # commit = output.strip()
+        # 
+        # process = subprocess.Popen(['git', 'log', folder + '.dvc'],
+        #                            stdout=subprocess.PIPE,
+        #                            universal_newlines=True)
         # To-Do : Parse the output and report if error
-        output, errs = process.communicate(timeout=60)
-        commit = output.splitlines()[0].strip()
+        # output, errs = process.communicate(timeout=60)
+        # commit = output.splitlines()[0].strip()
     except Exception as err:
         process.kill()
         outs, errs = process.communicate()
         print(f"Unexpected {err}, {type(err)}")
         print(f"Unexpected {outs}")
         print(f"Unexpected {errs}")
     return commit
@@ -260,7 +287,162 @@
 
     except Exception as err:
         process.kill()
         print(f"Unexpected {err}, {type(err)}")
         print(f"Unexpected {output}")
         print(f"Unexpected {errs}")
     return commit.split()[1]
+
+#Initialise git with quiet option
+def git_quiet_init() -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['git', 'init', '-q'],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+
+# Initial git commit
+def git_initial_commit() -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['git', 'commit', '-q', '--allow-empty', '-n', '-m', "Initial code commit"],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+# Add a remote repo url
+def git_add_remote(git_url) -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['git', 'remote', 'add', 'cmf_origin', f"{git_url}"],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+# dvc init with quiet option
+def dvc_quiet_init() -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['dvc', 'init', '-q'],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+# add repo in dvc
+def dvc_add_remote_repo(repo_type, repo_path) -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['dvc', 'remote', 'add', '-d', '-f', f"{repo_type}", f"{repo_path}"],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+# add repo related attributes in dvc
+def dvc_add_attribute(repo_type, attribute_type, attribute_value) -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['dvc', 'remote', 'modify', f"{repo_type}", f"{attribute_type}", f"{attribute_value}"],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+
+# get dvc config
+def dvc_get_config() -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['dvc','config', '-l'],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
+
+
+# dvc push
+def dvc_push() -> str:
+    commit = ""
+    try:
+        process = subprocess.Popen(['dvc', 'push'],
+                                   stdout=subprocess.PIPE,
+                                   universal_newlines=True)
+        output, errs = process.communicate(timeout=60)
+        commit = output.strip()
+
+    except Exception as err:
+        print(f"Unexpected {err}, {type(err)}")
+        if isinstance(object, subprocess.Popen):
+           process.kill()
+           outs, errs = process.communicate()
+           print(f"Unexpected {outs}")
+           print(f"Unexpected {errs}")
+    return commit
```

### Comparing `cmflib-0.0.2/cmflib/graph_wrapper.py` & `cmflib-0.0.3/cmflib/graph_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,14 +84,38 @@
             node = session.write_transaction(
                 self._run_transaction, dataset_syntax)
             node_id = node[0]["node_id"]
             pc_syntax = self._create_execution_artifacts_link_syntax(
                 "Execution", "Dataset", self.execution_id, node_id, event)
             _ = session.write_transaction(self._run_transaction, pc_syntax)
 
+    def create_dataslice_node(self, name: str, path: str, uri: str, parent_name:str,
+                            custom_properties=None):
+        if custom_properties is None:
+            custom_properties = {}
+        dataslice_syntax = self._create_dataslice_syntax(
+            name, path, uri, custom_properties)
+        with self.driver.session() as session:
+            node = session.write_transaction(
+                self._run_transaction, dataslice_syntax)
+            node_id = node[0]["node_id"]
+        p_nid = self._get_node("Dataset", parent_name )
+        with self.driver.session() as session:
+            pc_syntax = self._create_parent_child_syntax(
+                "Dataset", "Dataslice", p_nid, node_id, "contains")
+            _ = session.write_transaction(self._run_transaction, pc_syntax)
+
+    def create_links(self, source_path:str, target_path:str, relation:str ):
+        source_node_id = self._get_node_with_path("Dataset", source_path)
+        target_node_id = self._get_node_with_path("Dataslice", target_path)
+        with self.driver.session() as session:
+            pc_syntax = self._create_parent_child_syntax("Dataset", "Dataslice", source_node_id, target_node_id, relation)
+            _ = session.write_transaction(self._run_transaction, pc_syntax)
+
+
     def create_model_node(self, name: str, uri: str, event: str, execution_id: str, pipeline_context: mlpb.Context,
                           custom_properties=None):
         if custom_properties is None:
             custom_properties = {}
         pipeline_id = pipeline_context.id
         pipeline_name = pipeline_context.name
         model_syntax = self._create_model_syntax(
@@ -188,14 +212,40 @@
             execution_id_to_link = unlinked_executions[0]
             execution_uri = executions[execution_id_to_link]
             pc_syntax = self._create_execution_link_syntax(
                 "Execution", "Execution", execution_uri, execution_id_to_link, self.execution_id, "linked", {
                     "Artifact_Name": parent_artifact_name, "uri": parent_artifact_uri})
             _ = session.write_transaction(self._run_transaction, pc_syntax)
 
+    def _get_node(self, node_label: str, node_name: str)->int:
+        #Match(n:Metrics) where n.Name contains 'metrics_1' return n
+        search_syntax = "MATCH (n:{}) where '{}' in n.Name  \
+                              return ID(n) as node_id".format(node_label, node_name)
+        print(search_syntax)
+        node_id = None
+        with self.driver.session() as session:
+            nodes = session.read_transaction(
+                self._run_transaction, search_syntax)
+
+            node_id = nodes[0]["node_id"]
+        return node_id
+
+    def _get_node_with_path(self, node_label: str, node_path: str)->int:
+        #Match(n:Metrics) where n.Path contains 'metrics_1' return n
+        search_syntax = "MATCH (n:{}) where '{}' in n.Path  \
+                              return ID(n) as node_id".format(node_label, node_path)
+        print(search_syntax)
+        node_id = None
+        with self.driver.session() as session:
+            nodes = session.read_transaction(
+                self._run_transaction, search_syntax)
+
+            node_id = nodes[0]["node_id"]
+        return node_id
+
     @staticmethod
     def _run_transaction(tx, message):
         result = tx.run(message)
         values = []
         for record in result:
             values.append(record)
         return values
@@ -232,14 +282,30 @@
                 " = coalesce([x in a." + k + " where x <>\"" + str(v) + "\"], []) + \"" + str(v) + "\","
             syntax_str = syntax_str + props_str
         syntax_str = syntax_str.rstrip(",")
         syntax_str = syntax_str + " RETURN ID(a) as node_id"
         return syntax_str
 
     @staticmethod
+    def _create_dataslice_syntax(name: str, path: str, uri: str,
+                               custom_properties):
+        custom_properties["Name"] = name
+        custom_properties["Path"] = path
+        syntax_str = "MERGE (a:Dataslice {uri:\"" + uri + "\"}) SET "
+        # props_str = ""
+        for k, v in custom_properties.items():
+            k = re.sub('\W+', '', k)
+            props_str = "a." + k + \
+                " = coalesce([x in a." + k + " where x <>\"" + str(v) + "\"], []) + \"" + str(v) + "\","
+            syntax_str = syntax_str + props_str
+        syntax_str = syntax_str.rstrip(",")
+        syntax_str = syntax_str + " RETURN ID(a) as node_id"
+        return syntax_str
+
+    @staticmethod
     def _create_model_syntax(name: str, uri: str, pipeline_id: int, pipeline_name: str, custom_properties):
         custom_properties["Name"] = name
         custom_properties["uri"] = uri
         custom_properties["pipeline_id"] = str(pipeline_id)
         custom_properties["pipeline_name"] = pipeline_name
         syntax_str = "MERGE (a:Model {"  # + str(props) + ")"
         for k, v in custom_properties.items():
@@ -278,14 +344,15 @@
             k = re.sub('\W+', '', k)
             syntax_str = syntax_str + k + ":" + "\"" + str(v) + "\"" + ","
 
         syntax_str = syntax_str.rstrip(syntax_str[-1])
         syntax_str = syntax_str + "}) RETURN ID(a) as node_id"
         return syntax_str
 
+
     @staticmethod
     def _create_parent_child_syntax(parent_label: str, child_label: str, parent_id: int, child_id: int, relation: str):
         parent_child_syntax = "MATCH (a:{}), (b:{}) where ID(a) = {} AND ID(b) = {} MERGE (a)-[r:{}]->(b) \
                               return type(r)".format(parent_label, child_label, parent_id, child_id, relation)
         return parent_child_syntax
 
     @staticmethod
```

### Comparing `cmflib-0.0.2/cmflib/metadata_helper.py` & `cmflib-0.0.3/cmflib/metadata_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,29 +147,48 @@
     artifact.id = store.put_artifacts([artifact])[0]
     return artifact
 
 
 def create_execution_with_type(
         store,
         type_name: str,
+        name:str,
         properties: dict = None,
         type_properties: dict = None,
-        custom_properties: dict = None,
+        custom_properties: t.Optional[t.Dict] = None,
+        create_new_execution:bool = True
 ) -> metadata_store_pb2.Execution:
-    execution_type = get_or_create_execution_type(
+    if create_new_execution:
+        execution_type = get_or_create_execution_type(
+        store=store,
+        type_name=name,
+        properties=type_properties,
+        )
+        execution = metadata_store_pb2.Execution(
+            type_id=execution_type.id,
+            properties=properties,
+            custom_properties=custom_properties,
+        )
+        execution.id = store.put_executions([execution])[0]
+    else:
+        execution_type = get_or_create_execution_type(
         store=store,
         type_name=type_name,
         properties=type_properties,
-    )
-    execution = metadata_store_pb2.Execution(
-        type_id=execution_type.id,
-        properties=properties,
-        custom_properties=custom_properties,
-    )
-    execution.id = store.put_executions([execution])[0]
+        )
+        execution = store.get_execution_by_type_and_name(type_name, name)
+        if not execution:
+
+            execution = metadata_store_pb2.Execution(
+                type_id=execution_type.id,
+                name=name,
+                properties=properties,
+                custom_properties=custom_properties,
+             )
+            execution.id = store.put_executions([execution])[0]
     return execution
 
 
 def create_context_with_type(
         store,
         context_name: str,
         type_name: str,
@@ -222,40 +241,44 @@
             store=store,
             context_name=context_name,
             type_name=type_name,
             properties=properties,
             type_properties=type_properties,
             custom_properties=custom_properties,
         )
-        return context
+    return context
 
     # Verifying that the context has the expected type name
     context_types = store.get_context_types_by_id([context.type_id])
     assert len(context_types) == 1
     if context_types[0].name != type_name:
         raise RuntimeError(
             'Context "{}" was found, but it has type "{}" instead of "{}"'.format(
                 context_name, context_types[0].name, type_name))
     return context
 
 
 def create_new_execution_in_existing_context(
         store,
         execution_type_name: str,
+        execution_name:str,
         context_id: int,
         properties: dict = None,
         execution_type_properties: dict = None,
         custom_properties: dict = None,
+        create_new_execution:bool = True
 ) -> metadata_store_pb2.Execution:
     execution = create_execution_with_type(
         store=store,
         properties=properties,
         custom_properties=custom_properties,
         type_name=execution_type_name,
+        name=execution_name,
         type_properties=execution_type_properties,
+        create_new_execution=create_new_execution
     )
     association = metadata_store_pb2.Association(
         execution_id=execution.id,
         context_id=context_id,
     )
 
     store.put_attributions_and_associations([], [association])
@@ -349,31 +372,34 @@
         # print('Warning: Exception:{}'.format(str(e)), file=sys.stderr)
         sys.stderr.flush()
 
 
 def create_new_execution_in_existing_run_context(
         store,
         execution_type_name: str = None,  # TRAINING EXECUTION
+        execution_name:str = None,
         context_id: int = 0,  # TRAINING CONTEXT ASSOCIATED WITH THIS EXECUTION
         execution: str = None,
         pipeline_id: int = 0,  # THE PARENT CONTEXT
         pipeline_type: str = None,
         git_repo: str = None,
         git_start_commit: str = None,
         git_end_commit: str = "",
-        custom_properties: t.Optional[t.Dict] = None,
+        custom_properties: {} = None,
+        create_new_execution:bool = True
 ) -> metadata_store_pb2.Execution:
     mlmd_custom_properties = {}
     for property_name, property_value in (custom_properties or {}).items():
         mlmd_custom_properties[property_name] = value_to_mlmd_value(
             property_value)
 
     return create_new_execution_in_existing_context(
         store=store,
         execution_type_name=execution_type_name,
+        execution_name = execution_name,
         context_id=context_id,
         execution_type_properties={
             EXECUTION_CONTEXT_NAME_PROPERTY_NAME: metadata_store_pb2.STRING,
             EXECUTION_CONTEXT_ID: metadata_store_pb2.INT,
             EXECUTION_EXECUTION: metadata_store_pb2.STRING,
             EXECUTION_PIPELINE_TYPE: metadata_store_pb2.STRING,
             EXECUTION_PIPELINE_ID: metadata_store_pb2.INT,
@@ -391,14 +417,15 @@
             EXECUTION_PIPELINE_ID: metadata_store_pb2.Value(int_value=pipeline_id),
             EXECUTION_REPO: metadata_store_pb2.Value(string_value=git_repo),
             EXECUTION_START_COMMIT: metadata_store_pb2.Value(string_value=git_start_commit),
             EXECUTION_END_COMMIT: metadata_store_pb2.Value(string_value=git_end_commit)
             # should set to task ID, not component ID
         },
         custom_properties=mlmd_custom_properties,
+        create_new_execution=create_new_execution
     )
 
 
 def create_new_artifact_event_and_attribution(
         store,
         execution_id: int,
         context_id: int,
```

### Comparing `cmflib-0.0.2/cmflib.egg-info/PKG-INFO` & `cmflib-0.0.3/cmflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cmflib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Track metadata for AI pipeline
 Author: Hewlett Packard Enterprise
 Project-URL: Homepage, https://github.com/HewlettPackard/cmf
 Project-URL: Bug Tracker, https://github.com/HewlettPackard/cmf/issues
 Keywords: python,first package
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <=3.9,>=3.7
+Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cmf
 ## Common Metadata Framework
-[Getting Started](docs/index.md)<br><br>
-[Detailed documentation of the API's](docs/API.md) <br> 
+[Getting Started](https://hewlettpackard.github.io/cmf/)<br><br>
+[Detailed documentation of the API's](https://hewlettpackard.github.io/cmf/api/public/cmf) <br> 
 
 Interactions in data pipelines can be complex. The Different stages in the pipeline, (which may not be next to each other) may have to interact to produce or transform artifacts. As the artifacts navigates and undergo transformations through this pipeline, it can take a complicated path, which might also involve bidirectional movement across these stages.  Also there could be dependencies between the multiple stages, where the metrics produced by a stage could influence the metrics at a subsequent stage.  It is important to track the metadata across a pipeline to provide features like, lineage tracking, provenance and reproducibility.  
 
 The tracking of metadata through these complex pipelines have multiple challenges, some of them being,  
 
 - Each stage in the pipeline could be executed in a different datacenter or an edge site having intermittent connection to the core datacenter.
```

### Comparing `cmflib-0.0.2/setup.py` & `cmflib-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3'
 DESCRIPTION = 'Metadata Python Package'
 LONG_DESCRIPTION = 'Metadata framework storing AI metadata into MLMD'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
-        name="cmflib", 
+        name="cmflib",
         version=VERSION,
         author="Hewlett Packard Enterprise",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=["ml-metadata==1.11.0",
-                          "dvc", "pandas", "retrying", "pyarrow", "neo4j", \
-                            "sklearn", "tabulate", "click"],  # add any additional packages that 
+                          "dvc[ssh,s3]==2.27.0", "pandas", "retrying", "pyarrow", "neo4j", \
+                            "scikit-learn", "tabulate", "click", "minio", "paramiko"],  # add any additional packages that
         # needs to be installed along with your package. Eg: 'caer'
-        
+
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 3",
             "Operating System :: POSIX :: Linux",
-        ]
+        ],
+        scripts=['cmflib/bin/cmf']
 )
```


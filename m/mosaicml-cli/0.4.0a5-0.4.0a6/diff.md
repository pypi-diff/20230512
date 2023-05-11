# Comparing `tmp/mosaicml-cli-0.4.0a5.tar.gz` & `tmp/mosaicml-cli-0.4.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a5.tar", last modified: Wed May  3 00:12:03 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a6.tar", last modified: Tue May  9 23:14:27 2023, max compression
```

## Comparing `mosaicml-cli-0.4.0a5.tar` & `mosaicml-cli-0.4.0a6.tar`

### file list

```diff
@@ -1,195 +1,193 @@
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.859705 mosaicml-cli-0.4.0a5/
--rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-05-03 00:12:03.859367 mosaicml-cli-0.4.0a5/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     7199 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/README.md
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.811890 mosaicml-cli-0.4.0a5/mcli/
--rw-r--r--   0 tylerlee   (502) staff       (20)       54 2022-03-04 18:07:55.000000 mosaicml-cli-0.4.0a5/mcli/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.814143 mosaicml-cli-0.4.0a5/mcli/api/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/api/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.814981 mosaicml-cli-0.4.0a5/mcli/api/cluster/
--rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.0a5/mcli/api/cluster/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4216 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.815445 mosaicml-cli-0.4.0a5/mcli/api/engine/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/api/engine/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    25914 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/engine/engine.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10685 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/exceptions.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.817896 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1023 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3427 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3311 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3586 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6117 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1294 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1596 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.818625 mosaicml-cli-0.4.0a5/mcli/api/mint/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/api/mint/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7005 2023-05-03 00:02:41.000000 mosaicml-cli-0.4.0a5/mcli/api/mint/shell.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2489 2023-05-03 00:02:41.000000 mosaicml-cli-0.4.0a5/mcli/api/mint/tty.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.819597 mosaicml-cli-0.4.0a5/mcli/api/model/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/model/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6290 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/model/cluster_details.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2992 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/model/inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10439 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/model/run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.822357 mosaicml-cli-0.4.0a5/mcli/api/runs/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-04-25 23:51:33.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2750 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_create_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4143 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8371 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10912 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5141 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_start_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5329 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3937 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.822976 mosaicml-cli-0.4.0a5/mcli/api/schema/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/api/schema/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.0a5/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.824437 mosaicml-cli-0.4.0a5/mcli/api/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2365 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2998 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3697 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.0a5/mcli/api/typing_future.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.825075 mosaicml-cli-0.4.0a5/mcli/api/users/
--rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/api/users/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2694 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.825570 mosaicml-cli-0.4.0a5/mcli/cli/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a5/mcli/cli/__init__.py
--rwxr-xr-x   0 tylerlee   (502) staff       (20)     6436 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/cli.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.826347 mosaicml-cli-0.4.0a5/mcli/cli/common/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/cli/common/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2670 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7331 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.826925 mosaicml-cli-0.4.0a5/mcli/cli/m_connect/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1541 2023-04-21 23:37:59.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.828039 mosaicml-cli-0.4.0a5/mcli/cli/m_create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_create/m_create.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    16874 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.828886 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6098 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/delete.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5380 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.829268 mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3896 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.830275 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4367 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9702 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1860 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.832541 mosaicml-cli-0.4.0a5/mcli/cli/m_get/
--rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6226 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/clusters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6452 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/display.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5467 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4796 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/m_get.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9517 2023-04-26 01:33:20.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/users.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.833224 mosaicml-cli-0.4.0a5/mcli/cli/m_init/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_init/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4115 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    13963 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.833972 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9005 2023-05-03 00:02:41.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9321 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.834313 mosaicml-cli-0.4.0a5/mcli/cli/m_log/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_log/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10260 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.834747 mosaicml-cli-0.4.0a5/mcli/cli/m_ping/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2343 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.835087 mosaicml-cli-0.4.0a5/mcli/cli/m_predict/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2684 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.835551 mosaicml-cli-0.4.0a5/mcli/cli/m_root/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_root/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.836120 mosaicml-cli-0.4.0a5/mcli/cli/m_run/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_run/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8099 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.837627 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2973 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1802 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      881 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.838038 mosaicml-cli-0.4.0a5/mcli/cli/m_stop/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3847 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.838582 mosaicml-cli-0.4.0a5/mcli/cli/m_util/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_util/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_util/m_util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_util/util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    12743 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.840315 mosaicml-cli-0.4.0a5/mcli/models/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/gpu_type.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    11816 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/models/inference_deployment_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/mcli_cluster.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      563 2022-09-13 15:17:57.000000 mosaicml-cli-0.4.0a5/mcli/models/mcli_envvar.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6156 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/mcli_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    19547 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/models/run_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.840611 mosaicml-cli-0.4.0a5/mcli/objects/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/objects/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.842490 mosaicml-cli-0.4.0a5/mcli/objects/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.844126 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/base.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/env_var.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/mounted.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.844424 mosaicml-cli-0.4.0a5/mcli/proto/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/proto/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.844668 mosaicml-cli-0.4.0a5/mcli/sdk/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1099 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/sdk/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.850357 mosaicml-cli-0.4.0a5/mcli/utils/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a5/mcli/utils/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5306 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_cli.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_date.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10453 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_docker.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_epilog.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4527 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_logging.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6614 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_pypi.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_rich.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4307 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_run_status.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_spinner.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_string_functions.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_types.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_yaml.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3887 2023-05-03 00:08:44.000000 mosaicml-cli-0.4.0a5/mcli/version.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.854904 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/
--rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     4744 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)     1565 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/pyproject.toml
--rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-05-03 00:12:03.859925 mosaicml-cli-0.4.0a5/setup.cfg
--rw-r--r--   0 tylerlee   (502) staff       (20)     2991 2023-05-03 00:11:27.000000 mosaicml-cli-0.4.0a5/setup.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.858363 mosaicml-cli-0.4.0a5/tests/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a5/tests/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/tests/conftest.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5991 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/tests/test_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.0a5/tests/test_simple.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/tests/test_upgrade.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.854441 mosaicml-cli-0.4.0a6/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-05-09 23:14:27.854286 mosaicml-cli-0.4.0a6/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     7199 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/README.md
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.818394 mosaicml-cli-0.4.0a6/mcli/
+-rw-r--r--   0 anna       (501) staff       (20)     1794 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.818966 mosaicml-cli-0.4.0a6/mcli/api/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.819743 mosaicml-cli-0.4.0a6/mcli/api/cluster/
+-rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/cluster/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4237 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.820226 mosaicml-cli-0.4.0a6/mcli/api/engine/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/engine/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    25914 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/engine/engine.py
+-rw-r--r--   0 anna       (501) staff       (20)    10685 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/exceptions.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.822790 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/
+-rw-r--r--   0 anna       (501) staff       (20)     1023 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3301 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     3179 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     3582 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)     6138 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     1301 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     1603 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.823737 mosaicml-cli-0.4.0a6/mcli/api/mint/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/mint/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     7759 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/api/mint/shell.py
+-rw-r--r--   0 anna       (501) staff       (20)     2676 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/api/mint/tty.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.825154 mosaicml-cli-0.4.0a6/mcli/api/model/
+-rw-r--r--   0 anna       (501) staff       (20)     1114 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/model/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6290 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/model/cluster_details.py
+-rw-r--r--   0 anna       (501) staff       (20)     2992 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.0a6/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)    10439 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/model/run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.827931 mosaicml-cli-0.4.0a6/mcli/api/runs/
+-rw-r--r--   0 anna       (501) staff       (20)     1199 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2804 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     4211 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     8405 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)    11069 2023-05-09 23:13:21.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     5213 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     5405 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 anna       (501) staff       (20)    10609 2023-05-09 23:10:42.000000 mosaicml-cli-0.4.0a6/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.828365 mosaicml-cli-0.4.0a6/mcli/api/schema/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/schema/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.829352 mosaicml-cli-0.4.0a6/mcli/api/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/secrets/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2386 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)     3128 2023-05-09 23:09:39.000000 mosaicml-cli-0.4.0a6/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     3828 2023-05-09 23:09:29.000000 mosaicml-cli-0.4.0a6/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/typing_future.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.829811 mosaicml-cli-0.4.0a6/mcli/api/users/
+-rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/api/users/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2715 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.830107 mosaicml-cli-0.4.0a6/mcli/cli/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/__init__.py
+-rwxr-xr-x   0 anna       (501) staff       (20)     6436 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/cli.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.830669 mosaicml-cli-0.4.0a6/mcli/cli/common/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/common/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2461 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 anna       (501) staff       (20)     7489 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.831007 mosaicml-cli-0.4.0a6/mcli/cli/m_connect/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1694 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.831665 mosaicml-cli-0.4.0a6/mcli/cli/m_create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2385 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 anna       (501) staff       (20)    16874 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.832416 mosaicml-cli-0.4.0a6/mcli/cli/m_delete/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6056 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 anna       (501) staff       (20)     5380 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.832874 mosaicml-cli-0.4.0a6/mcli/cli/m_deploy/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.833897 mosaicml-cli-0.4.0a6/mcli/cli/m_describe/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4274 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     9999 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     2002 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.835497 mosaicml-cli-0.4.0a6/mcli/cli/m_get/
+-rw-r--r--   0 anna       (501) staff       (20)      467 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6226 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/display.py
+-rw-r--r--   0 anna       (501) staff       (20)     5409 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     4803 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-26 20:19:58.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     2189 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_get/users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.835985 mosaicml-cli-0.4.0a6/mcli/cli/m_init/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4115 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 anna       (501) staff       (20)    13963 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.837280 mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     9325 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)    44284 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 anna       (501) staff       (20)     9321 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.837689 mosaicml-cli-0.4.0a6/mcli/cli/m_log/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    10180 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.838073 mosaicml-cli-0.4.0a6/mcli/cli/m_ping/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2115 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.838549 mosaicml-cli-0.4.0a6/mcli/cli/m_predict/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2610 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.839005 mosaicml-cli-0.4.0a6/mcli/cli/m_root/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      536 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.839368 mosaicml-cli-0.4.0a6/mcli/cli/m_run/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     8099 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.840955 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 anna       (501) staff       (20)     1802 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 anna       (501) staff       (20)     1940 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 anna       (501) staff       (20)     1421 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.841573 mosaicml-cli-0.4.0a6/mcli/cli/m_stop/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.842511 mosaicml-cli-0.4.0a6/mcli/cli/m_util/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      797 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 anna       (501) staff       (20)     6837 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/cli/m_util/util.py
+-rw-r--r--   0 anna       (501) staff       (20)    12743 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.844469 mosaicml-cli-0.4.0a6/mcli/models/
+-rw-r--r--   0 anna       (501) staff       (20)     1047 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/models/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2103 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/models/gpu_type.py
+-rw-r--r--   0 anna       (501) staff       (20)    10321 2023-05-09 21:40:25.000000 mosaicml-cli-0.4.0a6/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      427 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/models/mcli_cluster.py
+-rw-r--r--   0 anna       (501) staff       (20)      456 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/models/mcli_envvar.py
+-rw-r--r--   0 anna       (501) staff       (20)     6156 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/models/mcli_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)    19547 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/models/run_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.844739 mosaicml-cli-0.4.0a6/mcli/objects/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/objects/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.846315 mosaicml-cli-0.4.0a6/mcli/objects/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.847881 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1646 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 anna       (501) staff       (20)     2244 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     2408 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     6377 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 anna       (501) staff       (20)     3858 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)     3001 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     5342 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 anna       (501) staff       (20)      783 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     1017 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 anna       (501) staff       (20)      556 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     1267 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 anna       (501) staff       (20)      967 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)      961 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     1718 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.848219 mosaicml-cli-0.4.0a6/mcli/proto/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a6/mcli/proto/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a6/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.848652 mosaicml-cli-0.4.0a6/mcli/sdk/
+-rw-r--r--   0 anna       (501) staff       (20)     1786 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/sdk/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.852508 mosaicml-cli-0.4.0a6/mcli/utils/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_cli.py
+-rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_date.py
+-rw-r--r--   0 anna       (501) staff       (20)    10749 2023-05-09 23:05:12.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_docker.py
+-rw-r--r--   0 anna       (501) staff       (20)     2225 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_epilog.py
+-rw-r--r--   0 anna       (501) staff       (20)    10774 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)     4527 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_logging.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 anna       (501) staff       (20)     6614 2023-05-06 11:02:40.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_pypi.py
+-rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_rich.py
+-rw-r--r--   0 anna       (501) staff       (20)     4332 2023-05-09 23:11:38.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_run_status.py
+-rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_spinner.py
+-rw-r--r--   0 anna       (501) staff       (20)    10751 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 anna       (501) staff       (20)     1677 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_types.py
+-rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/mcli/utils/utils_yaml.py
+-rw-r--r--   0 anna       (501) staff       (20)     3887 2023-05-09 21:40:36.000000 mosaicml-cli-0.4.0a6/mcli/version.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.853357 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-05-09 23:14:27.000000 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     4708 2023-05-09 23:14:27.000000 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anna       (501) staff       (20)        1 2023-05-09 23:14:27.000000 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anna       (501) staff       (20)       75 2023-05-09 23:14:27.000000 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anna       (501) staff       (20)     1567 2023-05-09 23:14:27.000000 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 anna       (501) staff       (20)        5 2023-05-09 23:14:27.000000 mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 anna       (501) staff       (20)    31087 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/pyproject.toml
+-rw-r--r--   0 anna       (501) staff       (20)       38 2023-05-09 23:14:27.854484 mosaicml-cli-0.4.0a6/setup.cfg
+-rw-r--r--   0 anna       (501) staff       (20)     2992 2023-05-09 21:40:25.000000 mosaicml-cli-0.4.0a6/setup.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-09 23:14:27.854003 mosaicml-cli-0.4.0a6/tests/
+-rw-r--r--   0 anna       (501) staff       (20)     5991 2023-05-09 21:40:23.000000 mosaicml-cli-0.4.0a6/tests/test_config.py
+-rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/tests/test_simple.py
+-rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a6/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a5/PKG-INFO` & `mosaicml-cli-0.4.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a5/README.md` & `mosaicml-cli-0.4.0a6/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a6/mcli/api/cluster/api_get_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,33 +78,36 @@
   }}
 }}"""
 
 
 @overload
 def get_clusters(
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
+    *,
     include_utilization: bool = False,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
 ) -> List[ClusterDetails]:
     ...
 
 
 @overload
 def get_clusters(
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
+    *,
     include_utilization: bool = False,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[List[ClusterDetails]]:
     ...
 
 
 def get_clusters(
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
+    *,
     include_utilization: bool = False,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """Get clusters available in the MosaicML platform
 
     Arguments:
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a6/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a6/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,39 @@
     publicDNS
     createdByEmail
   }}
 }}"""
 
 
 @overload
-def create_inference_deployment(deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
-                                timeout: Optional[float] = 10,
-                                future: Literal[False] = False) -> InferenceDeployment:
+def create_inference_deployment(
+    deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> InferenceDeployment:
     ...
 
 
 @overload
-def create_inference_deployment(deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
-                                timeout: Optional[float] = None,
-                                future: Literal[True] = True) -> Future[InferenceDeployment]:
+def create_inference_deployment(
+    deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[InferenceDeployment]:
     ...
 
 
-def create_inference_deployment(deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
-                                timeout: Optional[float] = 10,
-                                future: bool = False) -> Union[InferenceDeployment, Future[InferenceDeployment]]:
+def create_inference_deployment(
+    deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+) -> Union[InferenceDeployment, Future[InferenceDeployment]]:
     """Launch a inference deployment in the MosaicML platform
 
     The provided :class:`deploy <mcli.models.inference_deployment_config.InferenceDeploymentConfig>` must contain
     enough information to fully detail the inference deployment
     
     Args:
         deployment: A fully-configured inference deployment to launch. The deployment will be queued and persisted
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,39 @@
   }}
 }}"""
 
 __all__ = ['delete_inference_deployments']
 
 
 @overload
-def delete_inference_deployments(deployments: Union[List[str], List[InferenceDeployment]],
-                                 timeout: Optional[float] = 10,
-                                 future: Literal[False] = False) -> List[InferenceDeployment]:
+def delete_inference_deployments(
+    deployments: Union[List[str], List[InferenceDeployment]],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> List[InferenceDeployment]:
     ...
 
 
 @overload
-def delete_inference_deployments(deployments: Union[List[str], List[InferenceDeployment]],
-                                 timeout: Optional[float] = None,
-                                 future: Literal[True] = True) -> Future[List[InferenceDeployment]]:
+def delete_inference_deployments(
+    deployments: Union[List[str], List[InferenceDeployment]],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[List[InferenceDeployment]]:
     ...
 
 
-def delete_inference_deployments(deployments: Union[List[str], List[InferenceDeployment]],
-                                 timeout: Optional[float] = 10,
-                                 future: bool = False):
+def delete_inference_deployments(
+    deployments: Union[List[str], List[InferenceDeployment]],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Delete a list of inference deployments in the MosaicML Cloud
     Any deployments that are currently running will first be stopped.
     Args:
         deploymnets: A list of inference deployments or inference deployment names to delete
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     Get the current logs for an active or completed inference deployment in the MosaicML platform.
     This returns the full logs as a ``str``, as they exist at the time the request is
     made.
 
     Args:
         deployment (:obj:`str` | :class:`~mcli.api.model.inference_deployment.InferenceDeployment`): The
             inference deployment to get logs for. If a name is provided, the remaining required deployment details
-            will be queried with :func:`~mcli.sdk.get_inference_deployments`.
+            will be queried with :func:`~mcli.get_inference_deployments`.
         restart (``Optional[int]``): Which restart of a inference deployment to get logs for. Defaults to the most
             recent deployment restart.
         timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
             If the the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored.
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
             call to :func:`get_inference_deployment_logs` will return immediately and the request will be
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
   }}
 }}"""
 
 
 @overload
 def get_inference_deployments(
     deployments: Optional[Union[List[str], List[InferenceDeployment]]] = None,
+    *,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[List[str]] = None,
     timeout: Optional[float] = 10,
@@ -48,28 +49,30 @@
 ) -> List[InferenceDeployment]:
     ...
 
 
 @overload
 def get_inference_deployments(
     deployments: Optional[Union[List[str], List[InferenceDeployment]]] = None,
+    *,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[List[str]] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[List[InferenceDeployment]]:
     ...
 
 
 def get_inference_deployments(
     deployments: Optional[Union[List[str], List[InferenceDeployment]]] = None,
+    *,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[List[str]] = None,
     timeout: Optional[float] = 10,
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from mcli.api.model.inference_deployment import InferenceDeployment
 
 __all__ = ['ping_inference_deployment']
 
 
 def ping_inference_deployment(
     deployment: Union[InferenceDeployment, str],
+    *,
     timeout: Optional[float] = 10,
 ) -> dict:
     """Pings an inference deployment that has been launched in the MosaicML platform
     and returns the status of the deployment. The deployment must have a '/ping' endpoint
     defined.
     Arguments:
         deployment:(InferenceDeployment | str): The deployment to check the status of. Can be
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a6/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 __all__ = ['predict']
 
 
 def predict(
     deployment: Union[InferenceDeployment, str],
     inputs: Dict[str, Any],
+    *,
     timeout: Optional[float] = 20,
 ) -> dict:
     """Sends input to \'/predict\' endpoint of an inference deployment on the MosaicML
     platform. Runs prediction on input and returns output produced by the model.
     Arguments:
         deployment (InferenceDeployment | str): The deployment to make a prediction with.
             Can be either an InferenceDeployment object to send or a string which is of
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a6/mcli/api/mint/shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 connection engine to MINT
 """
 
 from __future__ import annotations
 
 import asyncio
+import io
+import json
 import logging
 import shutil
 import ssl
 import sys
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional, TextIO, Union, cast
 
 import backoff
 from websockets.client import WebSocketClientProtocol
 from websockets.client import connect as ws_connect
 
-from mcli.api.exceptions import MintConnectionException, MintException, MintServerException, handle_mint_errors
+from mcli.api.exceptions import MintConnectionException, MintServerException, handle_mint_errors
 from mcli.api.mint import tty
+from mcli.api.model.run import Run
 from mcli.proto.mint_pb2 import MINTMessage, TerminalSize, UserInput
-from mcli.utils.utils_logging import FAIL, WARN
+from mcli.utils.utils_logging import WARN
 from mcli.utils.utils_message_decoding import MessageDecoder
 
 logger = logging.getLogger(__name__)
 
 
 class MintShell:
     """Interactive shell into MINT (Mosaic Interactive service)
@@ -36,19 +39,27 @@
             exist, the default setting will be used.
     """
     api_key: str
     endpoint: str
 
     def __init__(
         self,
+        run: Union[Run, str],
+        *,
+        rank: int = 0,
         api_key: Optional[str] = None,
         endpoint: Optional[str] = None,
     ):
+        self.run_name = run.name if isinstance(run, Run) else run
+        self.rank = rank
+
+        # Load the API key and endpoint from the environment if not specified
         self._load_from_environment(api_key, endpoint)
 
+        # Start the async event loop
         self._loop = asyncio.get_event_loop_policy().get_event_loop()
 
     def _load_from_environment(self, api_key: Optional[str] = None, endpoint: Optional[str] = None) -> None:
         # pylint: disable-next=import-outside-toplevel
         from mcli import config
         conf = config.MCLIConfig.load_config(safe=True)
         if api_key is None:
@@ -60,45 +71,62 @@
         self.api_key = api_key
 
         if endpoint is None:
             endpoint = conf.mint_endpoint
         self.endpoint = endpoint
 
     @property
-    def header(self) -> Dict[str, str]:
-        return {"Authorization": self.api_key}
+    def _uri(self) -> str:
+        return f"{self.endpoint}/{self.run_name}/{self.rank}"
+
+    def _make_header(self, command: Optional[str] = None) -> Dict[str, Any]:
+        header = {"Authorization": self.api_key}
+        if command:
+            header['Commands'] = json.dumps([command])
+        return header
 
-    async def _connect(self, uri: str):
+    async def _connect(
+        self,
+        uri: str,
+        command: Optional[str] = None,
+        stdin: TextIO = sys.stdin,
+        stdout: TextIO = sys.stdout,
+    ) -> None:
         """
         Connection helper
 
         Given a uri, connects to a websocket and streams data in the terminal shell
         """
 
+        if stdin is None:
+            stdin = sys.stdin
+        if stdout is None:
+            stdout = sys.stdout
+
         async def read_stdin(ws: WebSocketClientProtocol):
             """Reads the stdin and write to the websocket
             """
             while True:
-                char = sys.stdin.read()
+                char = stdin.read()
                 if char:
                     message = MINTMessage(user_input=UserInput(input=char))
                     await ws.send(message.SerializeToString())
                 else:
                     # This can be very short, since its main purpose is to not block the event loop
                     await asyncio.sleep(0.01)
 
         async def write_stdout(ws: WebSocketClientProtocol):
             """Reads from the websocket and writes to stdout
             """
             decoder = MessageDecoder()
             async for msg in ws:
                 if msg:
                     decoded = decoder.decode(cast(bytes, msg))
-                    sys.stdout.write(decoded)
-                    sys.stdout.flush()
+                    stdout.write(decoded)
+                    stdout.flush()
 
         async def monitor_terminal_size(ws: WebSocketClientProtocol):
             """Monitors terminal size and sends it to the server when it changes
 
             This sends the width x height tuple as a byte string so MINT can parse it
             """
             size = None
@@ -106,27 +134,27 @@
                 new_size = shutil.get_terminal_size()
                 if new_size != size:
                     message = MINTMessage(terminal_size=TerminalSize(width=new_size.columns, height=new_size.lines))
                     await ws.send(message.SerializeToString())
                     size = new_size
                 await asyncio.sleep(0.1)
 
+        header = self._make_header(command)
+
         use_logger = logger if logger.isEnabledFor(logging.DEBUG) else None
         connect_params = {
             "uri": uri,
-            "extra_headers": self.header,
+            "extra_headers": header,
             # Useful for debugging. If logging is set to DEBUG level, this will log debug statements
             "logger": use_logger,
             # Set the close timeout to a small value. When the server closes connection, it often
             # does not respond to the client's close request. This keeps the waiting to a minimum.
             # If we start having reasons for the client to initiate the close, we may need to modify
             # this value.
             "close_timeout": 0.25,
-            # Give enough time for MINT to get a connection from the agent
-            # "open_timeout": 10,
         }
         if uri.startswith("wss:"):
             connect_params["ssl"] = ssl.SSLContext(ssl.PROTOCOL_TLS)
 
         # Maintain a list of tasks so that we can cancel them on retries
         tasks: List[asyncio.Task] = []
 
@@ -160,26 +188,25 @@
                     await asyncio.gather(*done)
                     # Cancel any remaining tasks
                     for task in pending:
                         task.cancel()
 
         await connect_and_handle_errors(connect_params)
 
-    def connect(self, run_name: str, rank: int = 0) -> int:
+    def execute(self, command: str) -> str:
+        """ Execute a command in the run's shell
         """
-        Connect to a run using the MINT Shell
+        with io.StringIO() as output:
+            self._loop.run_until_complete(self._connect(self._uri, command, stdout=output))
+            output.seek(0)
+            response = output.read()
+
+        return response
 
-        args:
-            run_name (str): Name of run to connect to
-            rank (int): Integer of node rank. By default, selects the first.
+    def connect(self, command: Optional[str] = None) -> None:
+        """
+        Connect to a run using the MINT Shell
         """
         if not tty.TTY_SUPPORTED:
             logger.warning(f'{WARN} MCLI Connect does not currently support TTY for your OS')
 
-        uri = f"{self.endpoint}/{run_name}/{rank}"
-
-        try:
-            self._loop.run_until_complete(self._connect(uri))
-        except MintException as e:
-            logger.error(f'{FAIL} {e}')
-            return 1
-        return 0
+        return self._loop.run_until_complete(self._connect(self._uri, command=command))
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a6/mcli/api/mint/tty.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """tty for mint shell, defined by OS
 """
 
 import os
 import sys
+from typing import TextIO
 
 TTY_SUPPORTED = False
 
 
 class TTY:  # pyright: ignore
     """TTY to be used in the mint shell
     """
 
     fd: int = 0
 
-    def __init__(self):
-        self.fd = sys.stdin.fileno()
+    def __init__(self, stdin: TextIO = sys.stdin):
+        self.fd = stdin.fileno()
 
     def setup(self):
         """Setup the TTY
         """
         pass
 
     def reset(self):
@@ -45,19 +46,23 @@
     class TTY:  # pylint: disable=function-redefined
         """Unix TTY to be used in the mint shell
         """
 
         fd: int = 0
         old_settings = None
 
-        def __init__(self):
-            self.fd = sys.stdin.fileno()
+        def __init__(self, stdin: TextIO = sys.stdin):
+            self.fd = stdin.fileno()
             self.old_settings = termios.tcgetattr(self.fd)
 
         def setup(self, when=termios.TCSAFLUSH):
+            # Only setup the TTY if we are in a TTY
+            if not os.isatty(self.fd):
+                return
+
             mode = termios.tcgetattr(self.fd)
 
             # See: https://man7.org/linux/man-pages/man3/termios.3.html
             mode[tty.LFLAG] &= ~(
                 # Disable signals so they are sent through to MINT
                 termios.ISIG |
                 # Turn off "echo" so we don't see the characters we type
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.0a6/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a6/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a6/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a6/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_create_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,27 +34,30 @@
     }}
   }}
 }}"""
 
 
 @overload
 def create_run(run: Union[RunConfig, FinalRunConfig],
+               *,
                timeout: Optional[float] = 10,
                future: Literal[False] = False) -> Run:
     ...
 
 
 @overload
 def create_run(run: Union[RunConfig, FinalRunConfig],
+               *,
                timeout: Optional[float] = None,
                future: Literal[True] = True) -> Future[Run]:
     ...
 
 
 def create_run(run: Union[RunConfig, FinalRunConfig],
+               *,
                timeout: Optional[float] = 10,
                future: bool = False) -> Union[Run, Future[Run]]:
     """Launch a run in the MosaicML platform
 
     The provided :class:`run <mcli.models.run_config.RunConfig>` must contain
     enough information to fully detail the run
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_delete_runs.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,24 +28,39 @@
     updatedAt
     reason
   }}
 }}"""
 
 
 @overload
-def delete_run(run: Union[str, Run], timeout: Optional[float] = 10, future: Literal[False] = False) -> Run:
+def delete_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> Run:
     ...
 
 
 @overload
-def delete_run(run: Union[str, Run], timeout: Optional[float] = None, future: Literal[True] = True) -> Future[Run]:
+def delete_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[Run]:
     ...
 
 
-def delete_run(run: Union[str, Run], timeout: Optional[float] = 10, future: bool = False):
+def delete_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Delete a run in the MosaicML platform
 
     If a run is currently running, it will first be stopped.
 
     Args:
         run: A run to delete
         timeout: Time, in seconds, in which the call should complete. If the call
@@ -66,28 +81,39 @@
         res = delete_runs(runs=runs, timeout=None, future=True)
         return convert_plural_future_to_singleton(res)
 
     return delete_runs(runs=runs, timeout=timeout, future=False)[0]
 
 
 @overload
-def delete_runs(runs: Union[List[str], List[Run]],
-                timeout: Optional[float] = 10,
-                future: Literal[False] = False) -> List[Run]:
+def delete_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> List[Run]:
     ...
 
 
 @overload
-def delete_runs(runs: Union[List[str], List[Run]],
-                timeout: Optional[float] = None,
-                future: Literal[True] = True) -> Future[List[Run]]:
+def delete_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[List[Run]]:
     ...
 
 
-def delete_runs(runs: Union[List[str], List[Run]], timeout: Optional[float] = 10, future: bool = False):
+def delete_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Delete a list of runs in the MosaicML platform
 
     Any runs that are currently running will first be stopped.
 
     Args:
         runs: A list of runs or run names to delete
         timeout: Time, in seconds, in which the call should complete. If the call
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_get_run_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,49 +21,52 @@
 }}"""
 
 
 @overload
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
+    *,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
     failed: Optional[bool] = False,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
+    *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     failed: Optional[bool] = False,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
+    *,
     timeout: Optional[float] = None,
     future: bool = False,
     failed: Optional[bool] = False,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Get the current logs for an active or completed run
 
     Get the current logs for an active or completed run in the MosaicML platform.
     This returns the full logs as a ``str``, as they exist at the time the request is
     made. If you want to follow the logs for an active run line-by-line, use
     :func:`follow_run_logs`.
 
     Args:
         run (:obj:`str` | :class:`~mcli.api.model.run.Run`): The run to get logs for. If a
-            name is provided, the remaining required run details will be queried with :func:`~mcli.sdk.get_runs`.
+            name is provided, the remaining required run details will be queried with :func:`~mcli.get_runs`.
         rank (``Optional[int]``): Node rank of a run to get logs for. Defaults to the lowest
             available rank. This will usually be rank 0 unless something has gone wrong.
         timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
             If the the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored.
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
             call to :func:`get_run_logs` will return immediately and the request will be
@@ -102,45 +105,48 @@
             yield message
 
 
 @overload
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
+    *,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
+    *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
+    *,
     timeout: Optional[float] = None,
     future: bool = False,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Follow the logs for an active or completed run in the MosaicML platform
 
     This returns a :obj:`generator` of individual log lines, line-by-line, and will wait until
     new lines are produced if the run is still active.
 
     Args:
         run (:obj:`str` | :class:`~mcli.api.model.run.Run`): The run to get logs for. If a
             name is provided, the remaining required run details will be queried with
-            :func:`~mcli.sdk.get_runs`.
+            :func:`~mcli.get_runs`.
         rank (``Optional[int]``): Node rank of a run to get logs for. Defaults to the lowest
             available rank. This will usually be rank 0 unless something has gone wrong.
         timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
             If the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored. A run may
             take some time to generate logs, so you likely do not want to set a timeout.
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_get_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         raise MAPIException(HTTPStatus.NOT_FOUND, error_message)
     return res[0]
 
 
 @overload
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
+    *,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
@@ -170,14 +171,15 @@
 ) -> List[Run]:
     ...
 
 
 @overload
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
+    *,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = None,
@@ -188,14 +190,15 @@
     limit: Optional[int] = None,
 ) -> Future[List[Run]]:
     ...
 
 
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
+    *,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
@@ -252,15 +255,22 @@
         date_filters = {}
         if before:
             date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
         if after:
             date_filters['gte'] = after.astimezone().isoformat() if isinstance(after, datetime) else after
         filters['createdAt'] = date_filters
     if statuses:
-        filters['status'] = {'in': [s.value.upper() if isinstance(s, RunStatus) else s.upper() for s in statuses]}
+        statuses = []
+        for s in statuses:
+            if isinstance(s, RunStatus):
+                statuses.append(str(s.value).upper())
+            else:
+                statuses.append(s.upper())
+
+        filters['status'] = {'in': statuses}
 
     cluster_names = cluster_names or clusters  # for backwards compatibility, clusters is supported as cluster_names
     if cluster_names:
         filters['clusterName'] = {'in': [c.name if isinstance(c, Cluster) else c for c in cluster_names]}
     if gpu_types:
         filters['gpuType'] = {'in': [gt.value if isinstance(gt, GPUType) else gt for gt in gpu_types]}
     if gpu_nums:
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_start_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,39 @@
     updatedAt
     reason
   }}
 }}"""
 
 
 @overload
-def start_run(run: Union[str, Run], timeout: Optional[float] = 10, future: Literal[False] = False) -> Run:
+def start_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> Run:
     ...
 
 
 @overload
-def start_run(run: Union[str, Run], timeout: Optional[float] = None, future: Literal[True] = True) -> Future[Run]:
+def start_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[Run]:
     ...
 
 
-def start_run(run: Union[str, Run], timeout: Optional[float] = 10, future: bool = False):
+def start_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Start a run
 
     Start a run currently stopped in the MosaicML platform.
 
     Args:
         run (``Optional[str | ``:class:`~mcli.api.model.run.Run` ``]``): A run or run name to start
         timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
@@ -73,28 +88,39 @@
         res = start_runs(runs=runs, timeout=None, future=True)
         return convert_plural_future_to_singleton(res)
 
     return start_runs(runs=runs, timeout=timeout, future=False)[0]
 
 
 @overload
-def start_runs(runs: Union[List[str], List[Run]],
-               timeout: Optional[float] = 10,
-               future: Literal[False] = False) -> List[Run]:
+def start_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> List[Run]:
     ...
 
 
 @overload
-def start_runs(runs: Union[List[str], List[Run]],
-               timeout: Optional[float] = None,
-               future: Literal[True] = True) -> Future[List[Run]]:
+def start_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[List[Run]]:
     ...
 
 
-def start_runs(runs: Union[List[str], List[Run]], timeout: Optional[float] = 10, future: bool = False):
+def start_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Start a list of runs
 
     Start a list of runs currently stopped in the MosaicML platform.
 
     Args:
         runs (``Optional[List[str] | List[``:class:`~mcli.api.model.run.Run` ``]]``):
             A list of runs or run names to start
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_stop_runs.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,39 @@
     updatedAt
     reason
   }}
 }}"""
 
 
 @overload
-def stop_run(run: Union[str, Run], timeout: Optional[float] = 10, future: Literal[False] = False) -> Run:
+def stop_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> Run:
     ...
 
 
 @overload
-def stop_run(run: Union[str, Run], timeout: Optional[float] = None, future: Literal[True] = True) -> Future[Run]:
+def stop_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[Run]:
     ...
 
 
-def stop_run(run: Union[str, Run], timeout: Optional[float] = 10, future: bool = False):
+def stop_run(
+    run: Union[str, Run],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Stop a run
 
     Stop a run currently running in the MosaicML platform.
 
     Args:
         run (``Optional[str | ``:class:`~mcli.api.model.run.Run` ``]``):
             A run or run name to stop. Using :class:`~mcli.api.model.run.Run` objects is most
@@ -75,28 +90,39 @@
         res = stop_runs(runs=runs, timeout=None, future=True)
         return convert_plural_future_to_singleton(res)
 
     return stop_runs(runs=runs, timeout=timeout, future=False)[0]
 
 
 @overload
-def stop_runs(runs: Union[List[str], List[Run]],
-              timeout: Optional[float] = 10,
-              future: Literal[False] = False) -> List[Run]:
+def stop_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = 10,
+    future: Literal[False] = False,
+) -> List[Run]:
     ...
 
 
 @overload
-def stop_runs(runs: Union[List[str], List[Run]],
-              timeout: Optional[float] = None,
-              future: Literal[True] = True) -> Future[List[Run]]:
+def stop_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = None,
+    future: Literal[True] = True,
+) -> Future[List[Run]]:
     ...
 
 
-def stop_runs(runs: Union[List[str], List[Run]], timeout: Optional[float] = 10, future: bool = False):
+def stop_runs(
+    runs: Union[List[str], List[Run]],
+    *,
+    timeout: Optional[float] = 10,
+    future: bool = False,
+):
     """Stop a list of runs
 
     Stop a list of runs currently running in the MosaicML platform.
 
     Args:
         runs (``Optional[List[str] | List[``:class:`~mcli.api.model.run.Run` ``]]``):
             A list of runs or run names to stop. Using :class:`~mcli.api.model.run.Run`
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a6/mcli/api/runs/api_watch_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
          If future is False:
             A :class:`~mcli.api.model.run.Run` object once it has reached the requested status
         Otherwise:
             A :class:`~concurrent.futures.Future` for the run. This will not resolve until
             the run reaches the requested status
     """
 
-    if not isinstance(status, RunStatus):
+    if isinstance(status, str):
         status = RunStatus.from_string(status)
 
     response = run_in_threadpool(_threaded_wait_for_run_status, run=run, status=status)
     return get_return_response(response, future=future, timeout=timeout)
 
 
 def _threaded_wait_for_run_status(run: Union[Run, str], status: RunStatus):
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a6/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a6/mcli/api/secrets/api_create_secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,34 @@
     }}
 }}"""
 
 
 @overload
 def create_secret(
     secret: Secret,
+    *,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
 ) -> Secret:
     ...
 
 
 @overload
 def create_secret(
     secret: Secret,
+    *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[Secret]:
     ...
 
 
 def create_secret(
     secret: Secret,
+    *,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """Create a secret in the MosaicML platform
 
     Arguments:
         secret (:class:`~mcli.models.mcli_secret.Secret`): A
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a6/mcli/api/secrets/api_delete_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,34 @@
   }}
 }}"""
 
 
 @overload
 def delete_secrets(
     secrets: Optional[Union[List[str], List[Secret]]] = None,
+    *,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
 ) -> List[Secret]:
     ...
 
 
 @overload
 def delete_secrets(
     secrets: Optional[Union[List[str], List[Secret]]] = None,
+    *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[List[Secret]]:
     ...
 
 
 def delete_secrets(
     secrets: Optional[Union[List[str], List[Secret]]] = None,
+    *,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """Deletes secrets from the MosaicML platform
 
     Arguments:
         secrets (:class:`~mcli.models.mcli_secret.Secret`): List of
@@ -66,16 +69,20 @@
     Raises:
         ``MAPIException``: If connecting to MAPI, raised when a MAPI communication error occurs
     """
 
     # Convert to strings
     secret_names = []
     if secrets:
-        secret_names = [s.name if isinstance(s, Secret) else s for s in secrets]
-
+        secret_names = []
+        for s in secrets:
+            if isinstance(s, Secret):
+                secret_names.append(s.name)
+            else:
+                secret_names.append(s)
     filters = {}
     if secret_names:
         filters['name'] = {'in': secret_names}
 
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a6/mcli/api/secrets/api_get_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,33 +25,36 @@
   }}
 }}"""
 
 
 @overload
 def get_secrets(
     secrets: Optional[Union[List[str], List[Secret]]] = None,
+    *,
     secret_types: Optional[Union[List[str], List[SecretType]]] = None,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
 ) -> List[Secret]:
     ...
 
 
 @overload
 def get_secrets(
     secrets: Optional[Union[List[str], List[Secret]]] = None,
+    *,
     secret_types: Optional[Union[List[str], List[SecretType]]] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[List[Secret]]:
     ...
 
 
 def get_secrets(
     secrets: Optional[Union[List[str], List[Secret]]] = None,
+    *,
     secret_types: Optional[Union[List[str], List[SecretType]]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """Get secrets available in the MosaicML platform
 
     Arguments:
@@ -73,15 +76,20 @@
     Raises:
         ``MAPIException``: If connecting to MAPI, raised when a MAPI communication error occurs
     """
     filters = {}
 
     if secrets:
         # Convert to strings
-        secret_names = [s.name if isinstance(s, Secret) else s for s in secrets]
+        secret_names = []
+        for s in secrets:
+            if isinstance(s, Secret):
+                secret_names.append(s.name)
+            else:
+                secret_names.append(s)
         filters['name'] = {'in': secret_names}
 
     if secret_types:
         mapi_secret_types = []
         for st in secret_types:
             mcli_st = SecretType.ensure_enum(st.value if isinstance(st, SecretType) else st)
             mapi_secret_types.append(get_mapi_secret_type(mcli_st))
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a6/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a6/mcli/api/users/api_get_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,29 +53,32 @@
             email=response['email'],
             organizations=organizations,
         )
 
 
 @overload
 def get_users(
+    *,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
 ) -> List[User]:
     ...
 
 
 @overload
 def get_users(
+    *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[List[User]]:
     ...
 
 
 def get_users(
+    *,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """List users in the MosaicML platform
 
     Arguments:
         timeout: Time, in seconds, in which the call should complete. If the call
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a6/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a6/mcli/cli/common/deployment_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,25 @@
     name_filter: Optional[List[str]] = None,
     cluster_filter: Optional[List[str]] = None,
     before_filter: Optional[str] = None,
     after_filter: Optional[str] = None,
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[str]] = None,
-    latest: bool = False,
     action_all: Optional[bool] = None,
 ) -> List[InferenceDeployment]:
 
     filter_used = any([
         name_filter,
         before_filter,
         after_filter,
         cluster_filter,
         gpu_type_filter,
         gpu_num_filter,
         status_filter,
-        latest,
     ])
     if not filter_used:
         if action_all is False:
             raise MCLIException('Must specify at least one filter or --all')
 
     if not name_filter:
         # Accept all that pass other filters
@@ -68,12 +66,8 @@
         expected_names = set(deployment_names)
         for deploy_name in found_deployments:
             if deploy_name in expected_names:
                 filtered.add(deploy_name)
 
         deployments = list(found_deployments[d] for d in filtered)
 
-    if latest and deployments:
-        latest_deployment = sorted(deployments, key=lambda x: x.created_at, reverse=True)[0]
-        deployments = [latest_deployment]
-
     return deployments
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a6/mcli/cli/common/run_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,22 +108,23 @@
         metavar='STATUS',
         type=status,
         help=f'{action.capitalize()} {submission_type.value}s with the specified statuses (choices: '
         f'{", ".join(submission_type.get_status_options())}). Multiple statuses should be specified '
         'using a comma-separated list, e.g. "failed,pending"',
     )
 
-    parser.add_argument(
-        '-l',
-        '--latest',
-        action='store_true',
-        dest='latest',
-        default=False,
-        help=f'Connect to the latest {submission_type.value}',
-    )
+    if submission_type == SubmissionType.RUN:
+        parser.add_argument(
+            '-l',
+            '--latest',
+            action='store_true',
+            dest='latest',
+            default=False,
+            help=f'Connect to the latest {submission_type.value}',
+        )
 
     if include_all:
         parser.add_argument(
             '-a',
             '--all',
             dest=f'{action}_all',
             action='store_true',
@@ -154,14 +155,15 @@
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[RunStatus]] = None,
     latest: bool = False,
     action_all: Optional[bool] = None,
     user_filter: Optional[List[str]] = None,
     limit: Optional[int] = None,
+    include_details: bool = False,
 ) -> List[Run]:
 
     filter_used = any([
         name_filter,
         before_filter,
         after_filter,
         cluster_filter,
@@ -190,14 +192,15 @@
             before=before_filter,
             after=after_filter,
             gpu_types=gpu_type_filter,
             gpu_nums=gpu_num_filter,
             statuses=status_filter,
             timeout=None,
             limit=limit,
+            include_details=include_details,
         )
 
     if glob_filters:
         found_runs: Dict[str, Run] = {r.name: r for r in runs}
 
         # Any globs will be handled by additional client-side filtering
         filtered = set()
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_connect/m_connect.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,14 +23,18 @@
         '-l',
         '--latest',
         action='store_true',
         dest='latest',
         default=False,
         help='Connect to the latest run',
     )
+    parser.add_argument(
+        '--command',
+        help='The command to execute in the run. By default you will be dropped into a bash shell',
+    )
 
     parser.set_defaults(func=connect_entrypoint)
     return parser
 
 
 def add_connect_argparser(subparser: argparse._SubParsersAction,) -> argparse.ArgumentParser:
     """Adds the get parser to a subparser
@@ -51,9 +55,10 @@
 
     connect_parser: argparse.ArgumentParser = subparser.add_parser(
         'connect',
         help='Create an interactive session that\'s connected to a run',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog=examples,
     )
+
     get_parser = configure_argparser(parser=connect_parser)
     return get_parser
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_delete/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,30 +141,28 @@
     name_filter: Optional[List[str]] = None,
     cluster_filter: Optional[List[str]] = None,
     before_filter: Optional[str] = None,
     after_filter: Optional[str] = None,
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[str]] = None,
-    latest: bool = False,
     delete_all: bool = False,
     force: bool = False,
     **kwargs,
 ):
     del kwargs
 
     deployments = get_deployments_with_filters(
         name_filter,
         cluster_filter,
         before_filter,
         after_filter,
         gpu_type_filter,
         gpu_num_filter,
         status_filter,
-        latest,
         delete_all,
     )
 
     if not deployments:
         extra = '' if delete_all else ' matching the specified criteria'
         logger.error(f'{WARN} No deployments found{extra}.')
         return 1
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,24 +83,23 @@
 
     def __iter__(self) -> Generator[DescribeDeployMetadataDisplayItem, None, None]:
         for model in self.models:
             item = DescribeDeployMetadataDisplayItem.from_deployment(model)
             yield item
 
 
-def describe_deploy(deployment_name: Optional[str] = None, output: OutputDisplay = OutputDisplay.TABLE, **kwargs):
+def describe_deploy(deployment_name: str, output: OutputDisplay = OutputDisplay.TABLE, **kwargs):
     """
     Fetches more details of a Inference Deployment
     """
     del kwargs
 
     deployments: List[InferenceDeployment] = []
     try:
-        name_filter = [deployment_name] if deployment_name else None
-        deployments = get_deployments_with_filters(name_filter=name_filter, latest=True)
+        deployments = get_deployments_with_filters(name_filter=[deployment_name])
     except (MAPIException, RuntimeError) as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except MCLIConfigError:
         logger.error(MESSAGE.MCLI_NOT_INITIALIZED)
 
     if len(deployments) == 0:
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_describe/describe_runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from enum import Enum
 from typing import Any, Dict, Generator, List, Optional, Tuple, TypeVar
 
 from rich.table import Table
 
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.run import Node, Run, RunLifecycle
+from mcli.cli.common.run_filters import get_runs_with_filters
 from mcli.cli.m_get.display import (MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table,
                                     format_timestamp)
 from mcli.models.run_config import DEFAULT_PRIORITY_NAME, ComputeConfig
-from mcli.sdk import get_run
 from mcli.utils.utils_logging import FormatString, console, format_string, print_timedelta, seconds_to_str
 
 logger = logging.getLogger(__name__)
 
 DISPLAY_RUN_STATUSES = ['PENDING', 'RUNNING', 'COMPLETED']
 
 
@@ -241,21 +241,29 @@
         data = {self.display_names.get(k, k.capitalize()): str(v) for k, v in asdict(self).items() if v is not None}
         columns = list(data.keys())
         values = [tuple(data.values())]
         return create_vertical_display_table(data=values, columns=columns)
 
 
 @cli_error_handler("mcli describe run")
-def describe_run(run_name: str, output: OutputDisplay = OutputDisplay.TABLE, **kwargs):
+def describe_run(run_name: Optional[str], output: OutputDisplay = OutputDisplay.TABLE, **kwargs):
     """
     Fetches more details of a Run
     """
     del kwargs
 
-    run = get_run(run_name)
+    latest = not run_name
+    name_filter = [run_name] if run_name else []
+
+    runs = get_runs_with_filters(name_filter=name_filter, latest=latest, include_details=True)
+
+    if len(runs) == 0:
+        print(f'No runs found with name: {run_name}')
+        return
+    run = runs[0]
 
     # Run details section
     print(format_string('Run Details', FormatString.BOLD))
     metadata_display = MCLIDescribeRunDetailsDisplay([run])
     metadata_display.print(output)
     print()
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_describe/m_describe.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 def describe_entrypoint(parser, **kwargs):
     del kwargs
     parser.print_help()
 
 
 def describe_runs_argparser(subparser: argparse._SubParsersAction) -> None:
     run_parser = subparser.add_parser('run', help='List metadata about a specific run')
-    run_parser.add_argument('run_name', type=str, help='Run name')
+    run_parser.add_argument('run_name',
+                            type=str,
+                            nargs='?',
+                            help='The name of the run. If not provided, will describe the latest run')
     run_parser.set_defaults(func=describe_run)
 
 
 def describe_deployments_argparser(subparser: argparse._SubParsersAction) -> None:
     deploy_parser = subparser.add_parser('deployment', help='List metadata about a specific inference deployment')
-    deploy_parser.add_argument('deployment_name', type=str, nargs='?', help='Inference Deployment name')
+    deploy_parser.add_argument('deployment_name', type=str, help='Inference Deployment name')
     deploy_parser.set_defaults(func=describe_deploy)
 
 
 def add_describe_parser(subparser: argparse._SubParsersAction) -> argparse.ArgumentParser:
     describe_parser: argparse.ArgumentParser = subparser.add_parser(
         'describe',
         help='Get detailed information on an object',
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,31 +89,22 @@
     before_filter: Optional[str] = None,
     after_filter: Optional[str] = None,
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[str]] = None,
     output: OutputDisplay = OutputDisplay.TABLE,
     include_ids: bool = False,
-    latest: bool = False,
     **kwargs,
 ) -> int:
     """Get a table of ongoing and completed inference deployments
     """
     del kwargs
 
-    deployments = get_deployments_with_filters(
-        name_filter,
-        cluster_filter,
-        before_filter,
-        after_filter,
-        gpu_type_filter,
-        gpu_num_filter,
-        status_filter,
-        latest,
-    )
+    deployments = get_deployments_with_filters(name_filter, cluster_filter, before_filter, after_filter,
+                                               gpu_type_filter, gpu_num_filter, status_filter)
 
     display = InferenceDeploymentDisplay(deployments, include_ids=include_ids)
     display.print(output)
 
     return 0
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/m_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                                 help='Include the secret ids in the output')
     runs_parser = get_runs_argparser(subparsers)
     add_common_arguments(runs_parser)
     deployments_parser = get_deployments_argparser(subparsers)
     add_common_arguments(deployments_parser)
     deployment_details_parsers = deployments_parser.add_subparsers(title='Deployment Details')
 
-    # mcli get run logs
+    # mcli get deployment logs
     add_log_parser(deployment_details_parsers, SubmissionType.DEPLOYMENT)
 
     return parser
 
 
 def add_get_argparser(subparser: argparse._SubParsersAction,
                       is_admin: bool = False,
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import argparse
 import logging
 from typing import Optional
 
 from mcli.api.cluster import get_clusters
+from mcli.api.exceptions import MintException
 from mcli.api.mint import shell
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
 from mcli.cli.m_get.display import format_timestamp
 from mcli.sdk import Run, RunConfig, RunStatus, create_run, get_runs
 from mcli.utils.utils_epilog import CommonLog
 from mcli.utils.utils_interactive import choose_one
 from mcli.utils.utils_logging import FAIL
@@ -85,22 +86,28 @@
     ready = wait_for_run(run)
     if not ready:
         return 1
 
     if not connect:
         return 0
 
-    mint_shell = shell.MintShell()
-    return mint_shell.connect(run.name, rank)
+    try:
+        mint_shell = shell.MintShell(run.name, rank=rank)
+        mint_shell.connect()
+    except MintException as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
+    return 0
 
 
 def connect_entrypoint(
     name: Optional[str] = None,
     rank: int = 0,
     latest: bool = False,
+    command: Optional[str] = None,
     **kwargs,
 ):
     del kwargs
 
     if name:
         runs = get_runs([name])
         if not runs:
@@ -138,16 +145,21 @@
                     formatter=get_name,
                 )
 
     ready = wait_for_run(run)
     if not ready:
         return 1
 
-    mint_shell = shell.MintShell()
-    return mint_shell.connect(run.name, rank)
+    try:
+        mint_shell = shell.MintShell(run.name, rank=rank)
+        mint_shell.connect(command=command)
+    except MintException as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
+    return 0
 
 
 def interactive_entrypoint(
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     gpu_type: Optional[str] = None,
     gpus: Optional[int] = None,
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_log/m_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 def get_with_filters(submission_type: SubmissionType,
                      name: Optional[str] = None,
                      latest: bool = False) -> Union[List[Run], List[InferenceDeployment]]:
     name_filter = [name] if name else None
     if submission_type == SubmissionType.RUN:
         return get_runs_with_filters(name_filter=name_filter, latest=latest)
     else:
-        return get_deployments_with_filters(name_filter=name_filter, latest=latest)
+        return get_deployments_with_filters(name_filter=name_filter)
 
 
 # pylint: disable-next=too-many-statements
 def get_logs(
     submission_type: SubmissionType,
     submission_name: Optional[str] = None,
     rank: Optional[int] = None,
@@ -192,21 +192,17 @@
 
     return 0
 
 
 def configure_deployments_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.set_defaults(func=partial(get_logs, SubmissionType.DEPLOYMENT))
 
-    parser.add_argument(
-        'submission_name',
-        metavar='DEPLOYMENT',
-        nargs='?',
-        help=
-        'The name of the inference deployment. If not provided, will return the logs of the latest inference deployment'
-    )
+    parser.add_argument('submission_name',
+                        metavar='DEPLOYMENT',
+                        help='The name of the inference deployment to fetch logs for.')
     parser.add_argument('--restart',
                         type=int,
                         default=None,
                         help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
 
     return parser
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_ping/m_ping.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """ mcli ping entrypoint """
 import argparse
 import logging
 from pprint import pprint
-from typing import Optional, Union
+from typing import Callable, Union, cast
 
 import validators
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.sdk import ping_inference_deployment
 from mcli.utils.utils_logging import FAIL, err_console
 
 logger = logging.getLogger(__name__)
 
 
 def ping(
-    deployment: Optional[str] = None,
+    deployment: str,
     **kwargs,
 ) -> int:
     del kwargs
     try:
-        deployment_obj_or_url: Union[InferenceDeployment, Optional[str]] = deployment
-        if not deployment_obj_or_url or not validators.url(deployment):
+        deployment_obj_or_url: Union[InferenceDeployment, str] = deployment
+        validate_url = cast(Callable[[str], bool], validators.url)
+        if not deployment_obj_or_url or not validate_url(deployment):
             # if a url is not passed in then lookup the deployment and get the name
-            name_filter = [deployment] if deployment else None
-            deployment_objs = get_deployments_with_filters(name_filter=name_filter, latest=True)
+            deployment_objs = get_deployments_with_filters(name_filter=[deployment])
             if len(deployment_objs) == 0:
+
                 if not deployment:
                     err_console.print("No inference deployments found.")
                 else:
                     err_console.log(f'No inference deployment found with name {deployment}.')
                 return 1
 
             deployment_obj_or_url = deployment_objs[0]
@@ -49,14 +50,10 @@
 
 
 def add_ping_parser(subparser: argparse._SubParsersAction):
     ping_parser: argparse.ArgumentParser = subparser.add_parser(
         'ping',
         help='Ping a inference deployment in the MosaicML platform for health metrics',
     )
-    ping_parser.add_argument('deployment',
-                             metavar='DEPLOYMENT',
-                             nargs='?',
-                             help='The name or url of the inference deployment. ' +
-                             'If not provided, will return the metrics of the latest deployment')
+    ping_parser.add_argument('deployment', metavar='DEPLOYMENT', help='The name or url of the inference deployment.')
 
     ping_parser.set_defaults(func=ping)
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_predict/m_predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """mcli predict entrypoint"""
 import argparse
 import logging
 from pprint import pprint
-from typing import Any, Dict, Optional, Union
+from typing import Any, Callable, Dict, Union, cast
 
 import validators
 import yaml
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
@@ -14,24 +14,24 @@
 from mcli.utils.utils_logging import FAIL, err_console
 
 logger = logging.getLogger(__name__)
 
 
 def predict_cli(
     inputs: Dict[str, Any],
-    deployment: Optional[str] = None,
+    deployment: str,
     **kwargs,
 ) -> int:
     del kwargs
     try:
-        deployment_obj_or_url: Union[InferenceDeployment, Optional[str]] = deployment
-        if not deployment_obj_or_url or not validators.url(deployment):
+        deployment_obj_or_url: Union[InferenceDeployment, str] = deployment
+        validate_url = cast(Callable[[str], bool], validators.url)
+        if not deployment_obj_or_url or not validate_url(deployment):
             # if a url is not passed in then lookup the deployment and get the name
-            name_filter = [deployment] if deployment else None
-            deployment_objs = get_deployments_with_filters(name_filter=name_filter, latest=True)
+            deployment_objs = get_deployments_with_filters(name_filter=[deployment])
             if len(deployment_objs) == 0:
                 if not deployment:
                     err_console.print("No inference deployments found.")
                 else:
                     err_console.print(f'No inference deployment found with name {deployment}.')
                 return 1
 
@@ -53,15 +53,14 @@
 def add_predict_parser(subparser: argparse._SubParsersAction):
     predict_parser: argparse.ArgumentParser = subparser.add_parser(
         'predict',
         help='Run prediction on a model in the MosaicML Cloud with given inputs. Returns forward pass result',
     )
     predict_parser.add_argument('deployment',
                                 metavar='DEPLOYMENT',
-                                nargs='?',
                                 help='The name or url of the deployment to run inference on')
 
     predict_parser.add_argument(
         '--input',
         '--inputs',
         '-i',
         dest='inputs',
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a6/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/config.py` & `mosaicml-cli-0.4.0a6/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a6/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.0a6/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a6/mcli/models/inference_deployment_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,38 +10,27 @@
 from typing_extensions import TypedDict
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.run_config import _clean_run_name
 from mcli.utils.utils_config import (BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, Translation,
                                      uuid_generator)
-from mcli.utils.utils_string_functions import camel_case_to_snake_case, snake_case_to_camel_case, validate_image
+from mcli.utils.utils_string_functions import validate_image
 
 logger = logging.getLogger(__name__)
 
 DEPLOYMENT_CONFIG_UID_LENGTH = 6
 
 
-class HFModelConfig(TypedDict, total=False):
-    """Typed dictionary for nested hugging face model configs"""
-    task: str
-    model_dtype: Optional[str]
-    autocast_dtype: Optional[str]
-
-
-class CustomModelConfig(TypedDict, total=False):
-    """Typed dictionary for nested custom model configs"""
-    model_handler: str
-
-
 class ModelConfig(TypedDict, total=False):
     """Typed dictionary for model configs"""
-    checkpoint_path: str
-    hf_model: Optional[HFModelConfig]
-    custom_mdoel: Optional[CustomModelConfig]
+    downloader: str
+    download_parameters: Dict[str, str]
+    model_handler: str
+    model_parameters: Dict[str, str]
 
 
 @dataclass
 class FinalInferenceDeploymentConfig(DeserializableModel):
     """A finalized deployment configuration
     This configuration must be complete, with enough details to submit a new deployment to the
     MosaicML Cloud.
@@ -258,51 +247,30 @@
 
         return cls(**data)
 
 
 class InferenceModelTranslation(Translation[ModelConfig, Dict[str, Any]]):
     """Translate model configs to and from MAPI"""
 
-    CHECKPOINT_PATH = 'checkpoint_path'
-    HF_MODEL = 'hf_model'
-    CUSTOM_MODEL = 'custom_model'
+    _property_translations = {
+        'downloader': 'downloader',
+        'download_parameters': 'downloadParameters',
+        'model_handler': 'modelHandler',
+        'model_parameters': 'modelParameters',
+    }
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> ModelConfig:
-        checkpoint_path = value.pop(snake_case_to_camel_case(cls.CHECKPOINT_PATH))
-
         translated_config = {}
-        for model_type, nested_model_config in value.items():
-            translated_model_type = camel_case_to_snake_case(model_type)
-            translated_config[translated_model_type] = {}
-
-            for key, val in nested_model_config.items():
-                # Translate keys to camel case for MAPI parameters
-                translated_key = camel_case_to_snake_case(key)
-                translated_config[translated_model_type][translated_key] = val
+        for mcli_key, mapi_key in cls._property_translations.items():
+            translated_config[mcli_key] = value.get(mapi_key)
 
-        translated_config[cls.CHECKPOINT_PATH] = checkpoint_path
         return ModelConfig(**translated_config)
 
     @classmethod
     def to_mapi(cls, value: ModelConfig) -> Dict[str, Any]:
-        checkpoint_path = value.pop(cls.CHECKPOINT_PATH)
-
         translated_config = {}
-        for model_type, nested_model_config in value.items():
-            translated_model_type = snake_case_to_camel_case(model_type)
-            translated_config[translated_model_type] = {}
-
-            nested_model_config = None
-            if model_type == cls.HF_MODEL:
-                nested_model_config = value.get(cls.HF_MODEL)
-            elif model_type == cls.CUSTOM_MODEL:
-                nested_model_config = value.get(cls.CUSTOM_MODEL)
-
-            if nested_model_config:
-                for key, val in nested_model_config.items():
-                    # Translate keys to camel case for MAPI parameters
-                    translated_key = snake_case_to_camel_case(key)
-                    translated_config[translated_model_type][translated_key] = val
+        for mcli_key, val in value.items():
+            mapi_key = cls._property_translations.get(mcli_key)
+            translated_config[mapi_key] = val
 
-        translated_config[snake_case_to_camel_case(cls.CHECKPOINT_PATH)] = checkpoint_path
         return translated_config
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a6/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a6/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.0a6/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a6/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_docker.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Dict, Generator, List, Optional, Set
 
 import docker
-from docker.errors import APIError
+from docker.errors import APIError, NotFound
 from rich.progress import Progress, SpinnerColumn
 from rich.spinner import Spinner
 
 from mcli.utils.utils_logging import console
 from mcli.utils.utils_spinner import get_spinner_style
 from mcli.utils.utils_string_functions import docker_image_to_repo_tag
 
@@ -34,26 +34,26 @@
     for f in ('username', 'password', 'email', 'registry'):
         if f in data:
             config[f] = data[f]
 
     return config
 
 
-def get_docker_client() -> docker.APIClient:
+def get_docker_client() -> docker.DockerClient:
     """Get the docker client
     """
     return docker.from_env(assert_hostname=True)
 
 
-def get_image_tags(client: docker.APIClient) -> Set[str]:
+def get_image_tags(client: docker.DockerClient) -> Set[str]:
     """Gets all unique image tags available
     """
     tags = set()
     for image in client.images.list():
-        for tag in image.tags:
+        for tag in image.tags:  # type: ignore - typing in library is missing tags
             tags.add(tag)
     return tags
 
 
 def _get_common_path(path1: Path, path2: Path) -> Optional[Path]:
     """Returns a common path of two paths if there is one
     """
@@ -85,16 +85,21 @@
     # Stop existing live display
     live = console._live  # pylint: disable=protected-access
     if live is not None:
         live.stop()
 
     # Yield a progress bar, but don't show it if the console isn't rendering
     spinner = SpinnerColumn(spinner_name=get_spinner_style())
-    with Progress(spinner, *Progress.get_default_columns(), console=console, transient=True, disable=live
-                  is None) as progress:
+    with Progress(
+            spinner,
+            *Progress.get_default_columns(),
+            console=console,
+            transient=True,
+            disable=live is None,
+    ) as progress:
         yield progress
 
     # Restart the existing live display
     if live is not None:
         live.start()
 
 
@@ -171,34 +176,34 @@
 
     auth_config = None
 
     def __init__(
         self,
         base_image: str,
         dest_image: str,
-        client: Optional[docker.APIClient] = None,
+        client: Optional[docker.DockerClient] = None,
         config_file: Optional[str] = None,
     ):
         self.image = dest_image
         self.repo, self.tag = docker_image_to_repo_tag(dest_image)
         self.base_image = base_image
 
         if client is None:
             client = get_docker_client()
-        self.client: docker.APIClient = client
+        self.client = client
 
         if config_file is not None:
             self.auth_config = load_docker_config(config_file)
 
     def pull(self, image: str):
         """Pull a docker image
         """
         # If we are in a rendered environment, pull with progress
         if not is_rendering():
-            self.client.images.pull(image)
+            self.client.images.pull(image)  # type: ignore - typing in library is missing tags
         else:
             client = docker.APIClient()  # use low level to get streaming pull logs
             total, progress_by_layer = 0, {}
             with show_progress() as progress:
                 download = progress.add_task('Pulling base image locally ', total=0)
                 for line in client.pull(image, stream=True, decode=True):
                     if 'progress' in line:
@@ -258,15 +263,15 @@
                 # stream the push to catch any errors (not all raise an APIError)
                 'stream': True,
                 'decode': True,
             }
             with show_progress() as progress:
                 upload = progress.add_task(f'Pushing image {self.repo}:{self.tag} ', total=0)
                 total, progress_by_layer = 0, {}
-                for line in self.client.images.push(**args):
+                for line in self.client.images.push(**args):  # type: ignore - typing in library is missing tags
                     if 'errorDetail' in line:
                         raise RuntimeError(f'Failed to push to docker image: {line["errorDetail"]}')
                     if 'progress' in line:
                         if line['id'] not in progress_by_layer:
                             total += line['progressDetail']['total']
                         progress_by_layer[line['id']] = line['progressDetail']['current']
                         completed = sum(progress_by_layer.values())
@@ -284,17 +289,17 @@
 
     def _will_overwrite_important_tag(self) -> bool:
         # allow overwrites to latest (default) tag
         if self.tag == 'latest':
             return False
 
         try:
-            self.client.images.get_registry_data(self.image)
+            self.client.images.get_registry_data(self.image)  # type: ignore - typing in library is missing tags
             return True
-        except docker.errors.NotFound:
+        except NotFound:
             return False
 
     def delete(self):
         """Delete the image locally
         """
         spinner_update(f'Cleaning up local image {self.image}...')
-        self.client.images.remove(self.image)
+        self.client.images.remove(self.image)  # type: ignore - typing in library is missing tags
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_run_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for interpreting pod status"""
 from __future__ import annotations
 
 import functools
 from enum import Enum, EnumMeta
-from typing import List
+from typing import List, Union
 
 from mcli.utils.utils_string_functions import camel_case_to_snake_case, snake_case_to_camel_case
 
 __all__ = ['RunStatus']
 
 
 class StatusMeta(EnumMeta):
@@ -116,15 +116,15 @@
             True
             >>> RunStatus.PENDING.before(RunStatus.RUNNING)
             True
         """
         return (self > other) or (inclusive and self == other)
 
     @classmethod
-    def from_string(cls, run_status: str) -> RunStatus:
+    def from_string(cls, run_status: Union[str, RunStatus]) -> RunStatus:
         """Convert a string to a valid RunStatus Enum
 
         If the run status string is not recognized, will return RunStatus.UNKNOWN
         instead of raising a KeyError
         """
         if isinstance(run_status, RunStatus):
             return run_status
```

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a6/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/mcli/version.py` & `mosaicml-cli-0.4.0a6/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.0a5"
+__version__ = "0.4.0a6"
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -143,12 +143,10 @@
 mcli/utils/utils_yaml.py
 mosaicml_cli.egg-info/PKG-INFO
 mosaicml_cli.egg-info/SOURCES.txt
 mosaicml_cli.egg-info/dependency_links.txt
 mosaicml_cli.egg-info/entry_points.txt
 mosaicml_cli.egg-info/requires.txt
 mosaicml_cli.egg-info/top_level.txt
-tests/__init__.py
-tests/conftest.py
 tests/test_config.py
 tests/test_simple.py
 tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a6/mosaicml_cli.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,71 +9,71 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
+sphinxcontrib-qthelp>=1.0.3
+sphinx_external_toc==0.3.0
+pylint>=2.12.2
+sphinxcontrib-images>=0.9.4
+sphinx-copybutton==0.5.2
+sphinxcontrib-htmlhelp>=2.0.0
+sphinxcontrib-devhelp>=1.0.2
+sphinxext-opengraph==0.8.2
+pytest>=6.2.5
+sphinx-panels==0.6.0
+sphinx-argparse==0.4.0
+pre-commit>=2.17.0
+furo==2022.9.29
+radon>=5.1.0
+myst-parser>=0.16.1
 sphinx-design
 pytest-cov>=4.0.0
-sphinxemoji>=0.2.0
-sphinx-markdown-tables>=0.0.15
-sphinxcontrib-applehelp>=1.0.2
-sphinx_external_toc>=0.3.0
-radon>=5.1.0
+sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-katex==0.9.4
+sphinx-rtd-theme==1.0.0
 sphinxcontrib-jsmath>=1.0.1
+pyright==1.1.256
 yapf>=0.33.0
-furo>=2022.3.4
-sphinxcontrib-serializinghtml>=1.1.5
-sphinx-panels>=0.6.0
-sphinx-argparse>=0.3.1
-sphinxcontrib-katex>=0.8.6
-pylint>=2.12.2
-pytest-mock>=3.7.0
-sphinx>=4.4.0
-sphinxcontrib-qthelp>=1.0.3
+sphinxcontrib-applehelp>=1.0.2
+sphinx-markdown-tables==0.0.17
+sphinxemoji==0.2.0
 isort>=5.9.3
-pytest>=6.2.5
-sphinx-copybutton>=0.5.0
-sphinxcontrib-devhelp>=1.0.2
-pre-commit>=2.17.0
-sphinxcontrib-images>=0.9.4
-sphinxext-opengraph>=0.6.1
-pyright>=1.1.256
-myst-parser>=0.16.1
-sphinx-rtd-theme>=1.0.0
+pytest-mock>=3.7.0
+sphinx==4.4.0
 toml>=0.10.2
-sphinxcontrib-htmlhelp>=2.0.0
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
-pyright>=1.1.256
+pyright==1.1.256
 pytest-cov>=4.0.0
 pytest-mock>=3.7.0
 pytest>=6.2.5
 radon>=5.1.0
 toml>=0.10.2
 yapf>=0.33.0
 
 [sphinx]
-furo>=2022.3.4
-sphinx>=4.4.0
-sphinx-argparse>=0.3.1
-sphinx-copybutton>=0.5.0
-sphinx-markdown-tables>=0.0.15
-sphinx-panels>=0.6.0
-sphinx-rtd-theme>=1.0.0
-sphinx_external_toc>=0.3.0
+furo==2022.9.29
+sphinx==4.4.0
+sphinx-argparse==0.4.0
+sphinx-copybutton==0.5.2
+sphinx-markdown-tables==0.0.17
+sphinx-panels==0.6.0
+sphinx-rtd-theme==1.0.0
+sphinx_external_toc==0.3.0
 sphinxcontrib-applehelp>=1.0.2
 sphinxcontrib-devhelp>=1.0.2
 sphinxcontrib-htmlhelp>=2.0.0
 sphinxcontrib-images>=0.9.4
 sphinxcontrib-jsmath>=1.0.1
-sphinxcontrib-katex>=0.8.6
+sphinxcontrib-katex==0.9.4
 sphinxcontrib-qthelp>=1.0.3
-sphinxcontrib-serializinghtml>=1.1.5
-sphinxemoji>=0.2.0
-sphinxext-opengraph>=0.6.1
+sphinxcontrib-serializinghtml==1.1.5
+sphinxemoji==0.2.0
+sphinxext-opengraph==0.8.2
 myst-parser>=0.16.1
 sphinx-design
```

### Comparing `mosaicml-cli-0.4.0a5/pyproject.toml` & `mosaicml-cli-0.4.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/setup.py` & `mosaicml-cli-0.4.0a6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,42 +34,42 @@
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'isort>=5.9.3',
     'pre-commit>=2.17.0',
     'pylint>=2.12.2',
-    'pyright>=1.1.256',
+    'pyright==1.1.256',
     'pytest-cov>=4.0.0',
     'pytest-mock>=3.7.0',
     'pytest>=6.2.5',
     'radon>=5.1.0',
     'toml>=0.10.2',
     'yapf>=0.33.0',
 ]
 
 extra_deps['sphinx'] = [
-    'furo>=2022.3.4',
-    'sphinx>=4.4.0',
-    'sphinx-argparse>=0.3.1',
-    'sphinx-copybutton>=0.5.0',
-    'sphinx-markdown-tables>=0.0.15',
-    'sphinx-panels>=0.6.0',
-    'sphinx-rtd-theme>=1.0.0',
-    'sphinx_external_toc>=0.3.0',
+    'furo==2022.9.29',
+    'sphinx==4.4.0',
+    'sphinx-argparse==0.4.0',
+    'sphinx-copybutton==0.5.2',
+    'sphinx-markdown-tables==0.0.17',
+    'sphinx-panels==0.6.0',
+    'sphinx-rtd-theme==1.0.0',
+    'sphinx_external_toc==0.3.0',
     'sphinxcontrib-applehelp>=1.0.2',
     'sphinxcontrib-devhelp>=1.0.2',
     'sphinxcontrib-htmlhelp>=2.0.0',
     'sphinxcontrib-images>=0.9.4',
     'sphinxcontrib-jsmath>=1.0.1',
-    'sphinxcontrib-katex>=0.8.6',
+    'sphinxcontrib-katex==0.9.4',
     'sphinxcontrib-qthelp>=1.0.3',
-    'sphinxcontrib-serializinghtml>=1.1.5',
-    'sphinxemoji>=0.2.0',
-    'sphinxext-opengraph>=0.6.1',
+    'sphinxcontrib-serializinghtml==1.1.5',
+    'sphinxemoji==0.2.0',
+    'sphinxext-opengraph==0.8.2',
     'myst-parser>=0.16.1',
     'sphinx-design',
 ]
 
 
 def package_files(directory: str):
     # from https://stackoverflow.com/a/36693250
```

### Comparing `mosaicml-cli-0.4.0a5/tests/test_config.py` & `mosaicml-cli-0.4.0a6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a5/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a6/tests/test_upgrade.py`

 * *Files identical despite different names*


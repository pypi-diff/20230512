# Comparing `tmp/dagworks-sdk-0.0.1.tar.gz` & `tmp/dagworks-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks-sdk-0.0.1.tar", last modified: Mon May  8 22:05:44 2023, max compression
+gzip compressed data, was "dagworks-sdk-0.0.2.tar", last modified: Fri May 12 05:33:49 2023, max compression
```

## Comparing `dagworks-sdk-0.0.1.tar` & `dagworks-sdk-0.0.2.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.913637 dagworks-sdk-0.0.1/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-05-06 22:02:15.000000 dagworks-sdk-0.0.1/LICENSE
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4727 2023-05-08 22:05:44.913154 dagworks-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3675 2023-05-08 22:04:35.000000 dagworks-sdk-0.0.1/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1910 2023-05-08 21:02:08.000000 dagworks-sdk-0.0.1/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        7 2023-05-06 23:25:38.000000 dagworks-sdk-0.0.1/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      117 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-05-08 22:05:44.913766 dagworks-sdk-0.0.1/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-05-06 22:26:36.000000 dagworks-sdk-0.0.1/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.842249 dagworks-sdk-0.0.1/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.846120 dagworks-sdk-0.0.1/src/dagworks/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.848664 dagworks-sdk-0.0.1/src/dagworks/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.851308 dagworks-sdk-0.0.1/src/dagworks/api/api_client/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.851993 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.855081 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3357 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2884 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5093 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4089 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3467 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.859125 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5253 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4689 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5031 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4526 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4972 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7040 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5671 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5489 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5753 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5625 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.861105 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4399 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5065 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6036 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6264 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5345 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2673 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/client.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/errors.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.878685 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3578 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/dependency.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_function.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_node.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_node_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1616 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/organization_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/paged_api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/paged_project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/paged_run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/phone_home_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3483 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_in_git.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_in_git_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_in_git_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5076 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5585 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_with_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/python_type.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_data.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4299 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in_run_log.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5431 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5908 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_with_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/task_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/task_run_result_summary.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/task_run_status.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2101 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2101 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/user_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/visibility_full.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2570 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/visibility_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/who_am_i_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      974 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/api/api_client/types.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9242 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1168 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.879903 dagworks-sdk-0.0.1/src/dagworks/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1995 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6318 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.880459 dagworks-sdk-0.0.1/src/dagworks/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.882850 dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-05-08 21:41:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-05-08 21:39:25.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      117 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.883344 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.885152 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-05-06 23:33:53.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2423 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.885626 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.887038 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      647 2023-05-08 21:42:04.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.887421 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.888016 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1551 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.888775 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.889153 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.892639 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-05-04 05:23:39.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3844 2023-05-06 23:39:58.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      606 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.893179 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.896680 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.897074 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    13976 2023-05-08 21:07:23.000000 dagworks-sdk-0.0.1/src/dagworks/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.903809 dagworks-sdk-0.0.1/src/dagworks/parsing/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/parsing/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/parsing/dagtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/parsing/parse.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.905181 dagworks-sdk-0.0.1/src/dagworks/telemetry/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.907918 dagworks-sdk-0.0.1/src/dagworks/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9709 2023-05-08 17:27:34.000000 dagworks-sdk-0.0.1/src/dagworks/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.1/src/dagworks/tracking/trackingtypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.909966 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4727 2023-05-08 22:05:44.000000 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8007 2023-05-08 22:05:44.000000 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-05-08 22:05:44.000000 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-05-08 22:05:44.000000 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      132 2023-05-08 22:05:44.000000 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-05-08 22:05:44.000000 dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 22:05:44.912348 dagworks-sdk-0.0.1/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-05-06 23:49:00.000000 dagworks-sdk-0.0.1/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5497 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.1/tests/test_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-02-13 05:18:55.000000 dagworks-sdk-0.0.1/tests/test_telemetry.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5924 2023-05-06 23:33:52.000000 dagworks-sdk-0.0.1/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.670145 dagworks-sdk-0.0.2/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-05-06 22:02:15.000000 dagworks-sdk-0.0.2/LICENSE
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-12 05:33:49.669782 dagworks-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-05-11 21:36:24.000000 dagworks-sdk-0.0.2/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-09 05:21:02.000000 dagworks-sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        7 2023-05-06 23:25:38.000000 dagworks-sdk-0.0.2/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      159 2023-05-12 05:33:31.000000 dagworks-sdk-0.0.2/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-05-12 05:33:49.670212 dagworks-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-05-06 22:26:36.000000 dagworks-sdk-0.0.2/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.619007 dagworks-sdk-0.0.2/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.621050 dagworks-sdk-0.0.2/src/dagworks/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-05-12 05:13:53.000000 dagworks-sdk-0.0.2/src/dagworks/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.621982 dagworks-sdk-0.0.2/src/dagworks/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.622910 dagworks-sdk-0.0.2/src/dagworks/api/api_client/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.623144 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.624794 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3357 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2884 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5093 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4089 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3467 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.627962 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5253 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4689 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5031 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4526 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4972 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7040 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5671 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5489 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5753 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5625 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.629413 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4399 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5065 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6036 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6264 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5345 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2673 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/client.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/errors.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.643862 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3578 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/dependency.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_function.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1616 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/organization_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/phone_home_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3483 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5076 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5585 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/python_type.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_data.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4299 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_run_log.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5431 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5908 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run_result_summary.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run_status.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2101 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2101 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/user_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_full.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2570 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/who_am_i_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      974 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/api/api_client/types.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9242 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1168 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.645138 dagworks-sdk-0.0.2/src/dagworks/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1995 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6512 2023-05-12 05:28:39.000000 dagworks-sdk-0.0.2/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.645454 dagworks-sdk-0.0.2/src/dagworks/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.647412 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-05-08 21:41:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-05-08 21:39:25.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-05-12 05:13:34.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.647745 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.648939 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-05-06 23:33:53.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-05-12 05:09:58.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.649302 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.650672 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-05-12 05:13:41.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.651168 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.651992 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1551 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.652830 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.653229 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.656057 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-05-04 05:23:39.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-05-12 05:09:11.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.656615 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.659340 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.659788 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    13968 2023-05-11 21:36:24.000000 dagworks-sdk-0.0.2/src/dagworks/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.662927 dagworks-sdk-0.0.2/src/dagworks/parsing/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/parsing/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/parsing/dagtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/parsing/parse.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.663693 dagworks-sdk-0.0.2/src/dagworks/telemetry/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.665477 dagworks-sdk-0.0.2/src/dagworks/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9709 2023-05-08 17:27:34.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.2/src/dagworks/tracking/trackingtypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.667885 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8007 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      177 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-05-12 05:33:49.000000 dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-12 05:33:49.669395 dagworks-sdk-0.0.2/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-05-06 23:49:00.000000 dagworks-sdk-0.0.2/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5497 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.2/tests/test_runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-02-13 05:18:55.000000 dagworks-sdk-0.0.2/tests/test_telemetry.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5924 2023-05-06 23:33:52.000000 dagworks-sdk-0.0.2/tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.1/LICENSE` & `dagworks-sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/PKG-INFO` & `dagworks-sdk-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
-Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/dagworks-sdk
+Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -64,29 +64,29 @@
     project_id=1, # The ID of your project. Create one in the UI first if you don't have one.
     api_key="safely_load_your_api_key", # e.g. os.environ["DAGWORKS_API_KEY"]
     username="your_email_address",
     dag_name="name_of_your_dag",
     tags={"tag1": "value1", "tag2": "value2"}, # Optional
 )
 ```
-*Project ID*: You'll need a project ID. Grab one from https://www.app.dagworks.io/dashboard/projects.
+*Project ID*: You'll need a project ID. Grab one from https://app.dagworks.io/dashboard/projects.
 Create a project if you don't have one, and take the ID from that.
 
-*API Key*: You'll need an API key. Create one here https://www.app.dagworks.io/dashboard/settings.
+*API Key*: You'll need an API key. Create one here https://app.dagworks.io/dashboard/settings.
 
 *username*: This is the email address you used to sign up for the DAGWorks Platform.
 
 *dag_name*: for a project, the DAG name is the top level way to group DAGs.
 E.g. ltv_model, us_sales, etc.
 
 *tags*: these are optional are string key value paris. They allow you to filter and curate
 various DAG runs.
 
 Then run Hamilton as normal! Each DAG run will be tracked, and you'll have access to it in the
-DAGWorks Platform. Visit https://www.app.dagworks.io/dashboard/projects to see your projects & DAGs.
+DAGWorks Platform. Visit https://app.dagworks.io/dashboard/projects to see your projects & DAGs.
 
 ## Starter Projects
 There are several starter projects that you can use to get started with the DAGWorks Platform.
 
 Starter Projects:
 
 * hello_world: a simple hello world DAG.
@@ -103,18 +103,18 @@
       --project-id PROJECT_ID_FROM_DAGWORKS_PLATFORM \
       --template STARTER_PROJECT_NAME \
       --location LOCATION
 ```
 Where:
 
 * *API_KEY_HERE*: is your DAGWorks Platform API Key. Create one here
-https://www.app.dagworks.io/dashboard/settings.
+https://app.dagworks.io/dashboard/settings.
 * *EMAIL_HERE*: is the email address you signed up for the DAGWorks Platform with.
 * *PROJECT_ID_FROM_DAGWORKS_PLATFORM*: is the project ID you want to use. Create one here
-https://www.app.dagworks.io/dashboard/projects.
+https://app.dagworks.io/dashboard/projects.
 * *STARTER_PROJECT_NAME*: is the name of the starter project you want to use. Your options
 are hello_world, data_processing, machine_learning, time_series_feature_engineering.
 * *LOCATION*: is the location you want to create the project in. This is a local directory.
 
 # License
 The use of this software is governed by the "The DAGWorks Enterprise license".
 Email support@dagworks.io for more information.
```

### Comparing `dagworks-sdk-0.0.1/README.md` & `dagworks-sdk-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,29 +40,29 @@
     project_id=1, # The ID of your project. Create one in the UI first if you don't have one.
     api_key="safely_load_your_api_key", # e.g. os.environ["DAGWORKS_API_KEY"]
     username="your_email_address",
     dag_name="name_of_your_dag",
     tags={"tag1": "value1", "tag2": "value2"}, # Optional
 )
 ```
-*Project ID*: You'll need a project ID. Grab one from https://www.app.dagworks.io/dashboard/projects.
+*Project ID*: You'll need a project ID. Grab one from https://app.dagworks.io/dashboard/projects.
 Create a project if you don't have one, and take the ID from that.
 
-*API Key*: You'll need an API key. Create one here https://www.app.dagworks.io/dashboard/settings.
+*API Key*: You'll need an API key. Create one here https://app.dagworks.io/dashboard/settings.
 
 *username*: This is the email address you used to sign up for the DAGWorks Platform.
 
 *dag_name*: for a project, the DAG name is the top level way to group DAGs.
 E.g. ltv_model, us_sales, etc.
 
 *tags*: these are optional are string key value paris. They allow you to filter and curate
 various DAG runs.
 
 Then run Hamilton as normal! Each DAG run will be tracked, and you'll have access to it in the
-DAGWorks Platform. Visit https://www.app.dagworks.io/dashboard/projects to see your projects & DAGs.
+DAGWorks Platform. Visit https://app.dagworks.io/dashboard/projects to see your projects & DAGs.
 
 ## Starter Projects
 There are several starter projects that you can use to get started with the DAGWorks Platform.
 
 Starter Projects:
 
 * hello_world: a simple hello world DAG.
@@ -79,18 +79,18 @@
       --project-id PROJECT_ID_FROM_DAGWORKS_PLATFORM \
       --template STARTER_PROJECT_NAME \
       --location LOCATION
 ```
 Where:
 
 * *API_KEY_HERE*: is your DAGWorks Platform API Key. Create one here
-https://www.app.dagworks.io/dashboard/settings.
+https://app.dagworks.io/dashboard/settings.
 * *EMAIL_HERE*: is the email address you signed up for the DAGWorks Platform with.
 * *PROJECT_ID_FROM_DAGWORKS_PLATFORM*: is the project ID you want to use. Create one here
-https://www.app.dagworks.io/dashboard/projects.
+https://app.dagworks.io/dashboard/projects.
 * *STARTER_PROJECT_NAME*: is the name of the starter project you want to use. Your options
 are hello_world, data_processing, machine_learning, time_series_feature_engineering.
 * *LOCATION*: is the location you want to create the project in. This is a local directory.
 
 # License
 The use of this software is governed by the "The DAGWorks Enterprise license".
 Email support@dagworks.io for more information.
```

### Comparing `dagworks-sdk-0.0.1/pyproject.toml` & `dagworks-sdk-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 requires-python = ">=3.7, <4"
 dynamic = ["dependencies", "optional-dependencies", "version"]
 
 [project.urls]
 "Homepage" = "https://www.dagworks.io"
 "Bug Reports" = "https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform"
-"Source" = "https://github.com/dagworks-inc/dagworks-sdk/dagworks-sdk"
+"Source" = "https://github.com/dagworks-inc/dagworks-sdk/"
 "Documenation" = "https://docs.dagworks.io/"
 
 [project.scripts]
 dagworks = "dagworks.cli.cli:cli"
 
 # [project.optional-dependencies]
 # Add optional dependencies here, one per line
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/client.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/client.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/api_key_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/dependency.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/dependency.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_dag.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_function.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_function.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_node.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_node_dependencies.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_dependencies.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/hamilton_node_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/hamilton_node_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/organization_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/organization_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/paged_api_key_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/paged_project_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/paged_run_log_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/paged_run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/phone_home_result.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/phone_home_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_in.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_in_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_out_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_in_git.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_in_git_dag.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_in_git_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_in_git_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_version_info.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_with_dag.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/python_type.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/python_type.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_data.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_data.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in_config.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in_run_log.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_run_log.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_in_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_config.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_with_run.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_with_run_config.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/task_run.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/task_run_result_summary.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/task_run_result_summary.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/user_out.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/user_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/visibility_full.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_full.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/visibility_in.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/visibility_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/models/who_am_i_result.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/models/who_am_i_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/api_client/types.py` & `dagworks-sdk-0.0.2/src/dagworks/api/api_client/types.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/clients.py` & `dagworks-sdk-0.0.2/src/dagworks/api/clients.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/constants.py` & `dagworks-sdk-0.0.2/src/dagworks/api/constants.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/api/projecttypes.py` & `dagworks-sdk-0.0.2/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/cli.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/initialize.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/initialize.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,21 @@
 import os
 import shutil
 from typing import Any, Dict
 
 import jinja2
 import loguru
 
-BASE_TEMPLATES_DIRECTORY = importlib.resources.files("dagworks.cli.templates")
+try:
+    # for python 3.9+
+    BASE_TEMPLATES_DIRECTORY = importlib.resources.files("dagworks.cli.templates")
+except AttributeError:
+    # for python <3.9
+    import pkg_resources
+    BASE_TEMPLATES_DIRECTORY = pkg_resources.resource_filename("dagworks.cli.templates", "")
 
 logger = loguru.logger
 
 HAMILTON_DIR_LOCATION = "components"
 CONFIG_DIR_LOCATION = "config"
 DATA_DIR_LOCATION = "data"
 
@@ -171,13 +177,13 @@
         template_name=template,
         template_data_file=template_data_file,
     )
     print_out_next_steps(copy_to_location, template)
     logger.info("Done!")
     logger.info(
         "Your next steps are:\n"
-        "(1) [Optional] commit this code to a git repository and push it to origin.\n"
-        "(2) create your python virtual environment and install the dependencies "
+        "(1) [Optional] Commit this code to a git repository and push it to origin.\n"
+        "(2) Create your python virtual environment and install the dependencies "
         "you need to run the code.\n"
         "For example if using pip, do `pip install -r requirements.txt`.\n"
-        "(3) execute `./run.sh` to run the example."
+        "(3) Execute `./run.sh` to run the example."
     )
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,25 @@
     {
         "order_id": pa.Column(int, checks=[pa.Check.ge(0)], nullable=False),
         "product_name": pa.Column(
             str,
             checks=[pa.Check.isin(PRODUCT_SET)],
             nullable=False,
         ),
-        "price": pa.Column(
+        "unit_price": pa.Column(
             float,
             checks=[pa.Check.ge(0.0), pa.Check.less_than_or_equal_to(10000.0)],
             nullable=False,
         ),
     },
     strict=True,
 )
 
 
+@check_output(schema=order_details_schema, importance="fail")
 @load_from.csv(path=source("order_details_path"), sep=",")
 def order_details(df: pd.DataFrame) -> pd.DataFrame:
     return df
 
 
 orders_schema = pa.DataFrameSchema(
     {
@@ -41,16 +42,16 @@
             int, checks=[pa.Check.ge(0), pa.Check.less_than_or_equal_to(1000)], nullable=False
         ),
     },
     strict=True,
 )
 
 
-@check_output(schema=orders_schema)
 @config.when(schema_version="old")
+@check_output(schema=orders_schema, importance="fail")
 @load_from.csv(path=source("orders_path"), sep=",")
 def orders__old(df: pd.DataFrame) -> pd.DataFrame:
     df["order_date"] = pd.to_datetime(df["order_date"])
     df["order_list"] = df.apply(
         lambda x: [
             f"{x.product1}-{x.quantity1}",
             f"{x.product2}-{x.quantity2}",
@@ -63,13 +64,13 @@
     df = df.explode("order_list")
     df["product_name"] = df["order_list"].apply(lambda x: x.split("-")[0])
     df["quantity"] = df["order_list"].apply(lambda x: int(x.split("-")[1]))
     del df["order_list"]
     return df
 
 
-@check_output(schema=orders_schema)
 @config.when(schema_version="new")
+@check_output(schema=orders_schema, importance="fail")
 @load_from.csv(path=source("orders_path"), sep=",")
 def orders__new(df: pd.DataFrame) -> pd.DataFrame:
     df["order_date"] = pd.to_datetime(df["order_date"])
     return df
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'template_description'": '"Shows a basic data processing example. This is a contrived example '*

 * *                           "that requires some 'normalization' of data input and then a merging of "*

 * *                           'two tables and subsequent processing. It is basic, but shows a '*

 * *                           'configuration based way to swap out a function, along with how one '*

 * *                           'might approach data quality checks."'}*

```diff
@@ -15,10 +15,10 @@
     ],
     "requirements": [
         "pandas",
         "sf-hamilton",
         "pandera"
     ],
     "return_df": true,
-    "template_description": "Shows a basic data processing example. This is a contrived example that requires some 'normalization' of data input and then a merging of two tables and subsequent processing. It is basic, but shows a configuration based way to swap out a function and data quality checks.",
+    "template_description": "Shows a basic data processing example. This is a contrived example that requires some 'normalization' of data input and then a merging of two tables and subsequent processing. It is basic, but shows a configuration based way to swap out a function, along with how one might approach data quality checks.",
     "use_tags_for_output": null
 }
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
 Module to transform iris data into features.
 """
 import numpy as np
 import pandas as pd
 from hamilton.function_modifiers import parameterize_sources
 
-RAW_FEATURES = ["sepal_length__cm_", "sepal_width__cm_", "petal_length__cm_", "petal_width__cm_"]
+RAW_FEATURES = ["sepal_length_cm", "sepal_width_cm", "petal_length_cm", "petal_width_cm"]
 
 # Here is more terse code that does the same thing as the below *_log functions.
 # Any `@parameterize*` decorator is just a less verbose way of defining functions that differ
 # slightly. We don't see anything wrong with verbose code - so we recommend err'ing on the side of
 # verbosity, but otherwise for this example show the terser code.
 # @parameterize_sources(**{f"{col}_log": {"col": col} for col in RAW_FEATURES})
 # def log_value(col: pd.Series) -> pd.Series:
 #     """Log value of {col}."""
 #     return np.log(col)
 
 
-def sepal_length__cm__log(sepal_length__cm_: pd.Series) -> pd.Series:
-    """Log value of sepal_length__cm_."""
-    return np.log(sepal_length__cm_)
+def sepal_length_cm_log(sepal_length_cm: pd.Series) -> pd.Series:
+    """Log value of sepal_length_cm_."""
+    return np.log(sepal_length_cm)
 
 
-def sepal_width__cm__log(sepal_width__cm_: pd.Series) -> pd.Series:
-    """Log value of sepal_width__cm_."""
-    return np.log(sepal_width__cm_)
+def sepal_width_cm_log(sepal_width_cm: pd.Series) -> pd.Series:
+    """Log value of sepal_width_cm_."""
+    return np.log(sepal_width_cm)
 
 
-def petal_length__cm__log(petal_length__cm_: pd.Series) -> pd.Series:
-    """Log value of petal_length__cm_."""
-    return np.log(petal_length__cm_)
+def petal_length_cm_log(petal_length_cm: pd.Series) -> pd.Series:
+    """Log value of petal_length_cm_."""
+    return np.log(petal_length_cm)
 
 
-def petal_width__cm__log(petal_width__cm_: pd.Series) -> pd.Series:
-    """Log value of petal_width__cm_."""
-    return np.log(petal_width__cm_)
+def petal_width_cm_log(petal_width_cm: pd.Series) -> pd.Series:
+    """Log value of petal_width_cm_."""
+    return np.log(petal_width_cm)
 
 
 @parameterize_sources(**{f"{col}_mean": {"col": col} for col in RAW_FEATURES})
 def mean_value(col: pd.Series) -> float:
     """Mean of {col}."""
     return col.mean()
 
@@ -57,50 +57,50 @@
 )
 def normalized_value(col: pd.Series, col_mean: float, col_std: float) -> pd.Series:
     """Normalized column of {col}."""
     return (col - col_mean) / col_std
 
 
 def data_set_v1(
-    sepal_length__cm__normalized: pd.Series,
-    sepal_width__cm__normalized: pd.Series,
-    petal_length__cm__normalized: pd.Series,
-    petal_width__cm__normalized: pd.Series,
+    sepal_length_cm_normalized: pd.Series,
+    sepal_width_cm_normalized: pd.Series,
+    petal_length_cm_normalized: pd.Series,
+    petal_width_cm_normalized: pd.Series,
     target_class: pd.Series,
 ) -> pd.DataFrame:
     """Explicitly define the feature set we want to use."""
     return pd.DataFrame(
         {
-            "sepal_length__cm__normalized": sepal_length__cm__normalized,
-            "sepal_width__cm__normalized": sepal_width__cm__normalized,
-            "petal_length__cm__normalized": petal_length__cm__normalized,
-            "petal_width__cm__normalized": petal_width__cm__normalized,
+            "sepal_length_cm_normalized": sepal_length_cm_normalized,
+            "sepal_width_cm_normalized": sepal_width_cm_normalized,
+            "petal_length_cm_normalized": petal_length_cm_normalized,
+            "petal_width_cm_normalized": petal_width_cm_normalized,
             "target_class": target_class,
         }
     )
 
 
 def data_set_v2(
-    sepal_length__cm__normalized: pd.Series,
-    sepal_width__cm__normalized: pd.Series,
-    petal_length__cm__normalized: pd.Series,
-    petal_width__cm__normalized: pd.Series,
-    sepal_length__cm__log: pd.Series,
-    sepal_width__cm__log: pd.Series,
-    petal_length__cm__log: pd.Series,
-    petal_width__cm__log: pd.Series,
+    sepal_length_cm_normalized: pd.Series,
+    sepal_width_cm_normalized: pd.Series,
+    petal_length_cm_normalized: pd.Series,
+    petal_width_cm_normalized: pd.Series,
+    sepal_length_cm_log: pd.Series,
+    sepal_width_cm_log: pd.Series,
+    petal_length_cm_log: pd.Series,
+    petal_width_cm_log: pd.Series,
     target_class: pd.Series,
 ) -> pd.DataFrame:
     """Explicitly define the feature set we want to use. This one adds `log` features."""
     return pd.DataFrame(
         {
-            "sepal_length__cm__normalized": sepal_length__cm__normalized,
-            "sepal_width__cm__normalized": sepal_width__cm__normalized,
-            "petal_length__cm__normalized": petal_length__cm__normalized,
-            "petal_width__cm__normalized": petal_width__cm__normalized,
-            "sepal_length__cm__log": sepal_length__cm__log,
-            "sepal_width__cm__log": sepal_width__cm__log,
-            "petal_length__cm__log": petal_length__cm__log,
-            "petal_width__cm__log": petal_width__cm__log,
+            "sepal_length_cm_normalized": sepal_length_cm_normalized,
+            "sepal_width_cm_normalized": sepal_width_cm_normalized,
+            "petal_length_cm_normalized": petal_length_cm_normalized,
+            "petal_width_cm_normalized": petal_width_cm_normalized,
+            "sepal_length_cm_log": sepal_length_cm_log,
+            "sepal_width_cm_log": sepal_width_cm_log,
+            "petal_length_cm_log": petal_length_cm_log,
+            "petal_width_cm_log": petal_width_cm_log,
             "target_class": target_class,
         }
     )
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks-sdk-0.0.2/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/driver.py` & `dagworks-sdk-0.0.2/src/dagworks/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         client_factory: Callable[
             [str, str, str], clients.DAGWorksClient
         ] = clients.BasicDAGWorksClient,
         adapter: base.HamiltonGraphAdapter = None,
         dagworks_api_url=os.environ.get("DAGWORKS_API_URL", constants.DAGWORKS_API_URL),
     ):
         """Instantiates a DAGWorks driver. This:
-        1. Requires a project to exist. Create one via https://www.app.dagworks.io/dashboard/projects.
+        1. Requires a project to exist. Create one via https://app.dagworks.io/dashboard/projects.
         2. Sends over the shape of the DAG.
         3. Sets up execute() run-tracking.
 
         :param config: Configuration to use, same as standard Hamilton driver.
         :param modules: Modules to use, same as standard Hamilton driver.
         :param project_id: Identifier for the project to use to store this DAG under.
         :param api_key: API key to use for authentication. Remember not to save this in plaintext!
@@ -288,15 +288,15 @@
         final_vars: List[Union[str, Callable]],
         overrides: Dict[str, Any] = None,
         display_graph: bool = False,
         inputs: Dict[str, Any] = None,
     ) -> Any:
         logger.warning(
             f"\nCapturing execution run. Results can be found at "
-            f"https://www.app.dagworks.io/dashboard/project/{self.project}/runs\n"
+            f"https://app.dagworks.io/dashboard/project/{self.project}/runs\n"
         )
         return super(Driver, self).execute(final_vars, overrides, display_graph, inputs)
 
     @global_tracker.track_calls(
         tracking_generators={
             "final_vars": [("num_vars", safe_len)],
             "overrides": [("num_overrides", safe_len)],
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks/parsing/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/parsing/dagtypes.py` & `dagworks-sdk-0.0.2/src/dagworks/parsing/dagtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/parsing/parse.py` & `dagworks-sdk-0.0.2/src/dagworks/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/telemetry/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/telemetry/telemetry.py` & `dagworks-sdk-0.0.2/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/tracking/__init__.py` & `dagworks-sdk-0.0.2/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/tracking/example_tracking.py` & `dagworks-sdk-0.0.2/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/tracking/runs.py` & `dagworks-sdk-0.0.2/src/dagworks/tracking/runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks/tracking/trackingtypes.py` & `dagworks-sdk-0.0.2/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
-Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/dagworks-sdk
+Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -64,29 +64,29 @@
     project_id=1, # The ID of your project. Create one in the UI first if you don't have one.
     api_key="safely_load_your_api_key", # e.g. os.environ["DAGWORKS_API_KEY"]
     username="your_email_address",
     dag_name="name_of_your_dag",
     tags={"tag1": "value1", "tag2": "value2"}, # Optional
 )
 ```
-*Project ID*: You'll need a project ID. Grab one from https://www.app.dagworks.io/dashboard/projects.
+*Project ID*: You'll need a project ID. Grab one from https://app.dagworks.io/dashboard/projects.
 Create a project if you don't have one, and take the ID from that.
 
-*API Key*: You'll need an API key. Create one here https://www.app.dagworks.io/dashboard/settings.
+*API Key*: You'll need an API key. Create one here https://app.dagworks.io/dashboard/settings.
 
 *username*: This is the email address you used to sign up for the DAGWorks Platform.
 
 *dag_name*: for a project, the DAG name is the top level way to group DAGs.
 E.g. ltv_model, us_sales, etc.
 
 *tags*: these are optional are string key value paris. They allow you to filter and curate
 various DAG runs.
 
 Then run Hamilton as normal! Each DAG run will be tracked, and you'll have access to it in the
-DAGWorks Platform. Visit https://www.app.dagworks.io/dashboard/projects to see your projects & DAGs.
+DAGWorks Platform. Visit https://app.dagworks.io/dashboard/projects to see your projects & DAGs.
 
 ## Starter Projects
 There are several starter projects that you can use to get started with the DAGWorks Platform.
 
 Starter Projects:
 
 * hello_world: a simple hello world DAG.
@@ -103,18 +103,18 @@
       --project-id PROJECT_ID_FROM_DAGWORKS_PLATFORM \
       --template STARTER_PROJECT_NAME \
       --location LOCATION
 ```
 Where:
 
 * *API_KEY_HERE*: is your DAGWorks Platform API Key. Create one here
-https://www.app.dagworks.io/dashboard/settings.
+https://app.dagworks.io/dashboard/settings.
 * *EMAIL_HERE*: is the email address you signed up for the DAGWorks Platform with.
 * *PROJECT_ID_FROM_DAGWORKS_PLATFORM*: is the project ID you want to use. Create one here
-https://www.app.dagworks.io/dashboard/projects.
+https://app.dagworks.io/dashboard/projects.
 * *STARTER_PROJECT_NAME*: is the name of the starter project you want to use. Your options
 are hello_world, data_processing, machine_learning, time_series_feature_engineering.
 * *LOCATION*: is the location you want to create the project in. This is a local directory.
 
 # License
 The use of this software is governed by the "The DAGWorks Enterprise license".
 Email support@dagworks.io for more information.
```

### Comparing `dagworks-sdk-0.0.1/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks-sdk-0.0.2/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/tests/test_driver.py` & `dagworks-sdk-0.0.2/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/tests/test_runs.py` & `dagworks-sdk-0.0.2/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/tests/test_telemetry.py` & `dagworks-sdk-0.0.2/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.1/tests/test_tracking.py` & `dagworks-sdk-0.0.2/tests/test_tracking.py`

 * *Files identical despite different names*


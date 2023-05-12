# Comparing `tmp/odp_sdk_python_ingest-0.3.1.tar.gz` & `tmp/odp_sdk_python_ingest-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_sdk_python_ingest-0.3.1.tar", max compression
+gzip compressed data, was "odp_sdk_python_ingest-0.4.0.tar", max compression
```

## Comparing `odp_sdk_python_ingest-0.3.1.tar` & `odp_sdk_python_ingest-0.4.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0      842 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/__init__.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/cdf/__init__.py
--rw-r--r--   0        0        0     3258 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/cdf/cdf_token_handler.py
--rw-r--r--   0        0        0     1764 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/cdf/federated_cognite_client.py
--rw-r--r--   0        0        0      163 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/odp/__init__.py
--rw-r--r--   0        0        0     3065 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/odp/interactive_login_token_handler.py
--rw-r--r--   0        0        0     1814 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/odp/ropc_token_handler.py
--rw-r--r--   0        0        0     1358 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/odp/token_handler.py
--rw-r--r--   0        0        0       49 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/prefect/__init__.py
--rw-r--r--   0        0        0     3878 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/auth/prefect/prefect_b2c_client.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/__init__.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/blocks/__init__.py
--rw-r--r--   0        0        0     6043 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/blocks/azure_storage.py
--rw-r--r--   0        0        0     2879 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/blocks/cdf_storage.py
--rw-r--r--   0        0        0      579 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/blocks/db_engine.py
--rw-r--r--   0        0        0     2378 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/blocks/postgres.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/__init__.py
--rw-r--r--   0        0        0      479 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/__main__.py
--rw-r--r--   0        0        0      435 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/authenticate.py
--rw-r--r--   0        0        0     2611 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/block.py
--rw-r--r--   0        0        0     5041 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/context.py
--rw-r--r--   0        0        0     7296 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/deploy.py
--rw-r--r--   0        0        0     2742 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/parameters.py
--rw-r--r--   0        0        0       43 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/params/__init__.py
--rw-r--r--   0        0        0      515 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/params/type_param_type.py
--rw-r--r--   0        0        0     3422 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/run.py
--rw-r--r--   0        0        0     1021 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/cli/schema.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/config/__init__.py
--rw-r--r--   0        0        0      708 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/config/cdf_config.py
--rw-r--r--   0        0        0      816 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/config/dask_config.py
--rw-r--r--   0        0        0      125 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/__init__.py
--rw-r--r--   0        0        0      216 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/abstract_deployment_block.py
--rw-r--r--   0        0        0       40 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/block/__init__.py
--rw-r--r--   0        0        0      502 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/block/generic_block.py
--rw-r--r--   0        0        0     1591 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/deployment_block_factory.py
--rw-r--r--   0        0        0      190 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/__init__.py
--rw-r--r--   0        0        0      481 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/abstract_runtime.py
--rw-r--r--   0        0        0     3465 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/kubernetes.py
--rw-r--r--   0        0        0     4569 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/kubernetes_dask.py
--rw-r--r--   0        0        0     1719 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
--rw-r--r--   0        0        0       88 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/schedule/__init__.py
--rw-r--r--   0        0        0      417 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/schedule/abstract_schedule.py
--rw-r--r--   0        0        0      471 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/schedule/cron_schedule.py
--rw-r--r--   0        0        0     1030 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/schedule/interval_schedule.py
--rw-r--r--   0        0        0       73 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/storage/__init__.py
--rw-r--r--   0        0        0      938 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/storage/abstract_storage.py
--rw-r--r--   0        0        0    10910 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/storage/docker.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/deploy/storage/prefect_healthcheck.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/__init__.py
--rw-r--r--   0        0        0     4679 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/stateful_value_impl.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/__init__.py
--rw-r--r--   0        0        0     1060 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/watermark_file_store.py
--rw-r--r--   0        0        0      639 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/watermark_inmemory_store.py
--rw-r--r--   0        0        0      728 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/watermark_redis_store.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/__init__.py
--rw-r--r--   0        0        0      970 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/abstract_metric.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/client/__init__.py
--rw-r--r--   0        0        0     2369 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/client/metric_mock_client.py
--rw-r--r--   0        0        0     7489 2023-01-04 19:08:10.052197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/client/metric_prometheus_client.py
--rw-r--r--   0        0        0     1669 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/metric_client.py
--rw-r--r--   0        0        0     5223 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/metrics.py
--rw-r--r--   0        0        0      591 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/metrics/prefect.py
--rw-r--r--   0        0        0     5492 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/secrets.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/state_handlers/__init__.py
--rw-r--r--   0        0        0     2007 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/state_handlers/metrics_pusher.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/tasks/cdf/__init__.py
--rw-r--r--   0        0        0     3218 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/tasks/cdf/cdf_credentials.py
--rw-r--r--   0        0        0     1440 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/tasks/concurrency_limit.py
--rw-r--r--   0        0        0      707 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/tasks/measured_task.py
--rw-r--r--   0        0        0     1580 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/compute/tasks/tasks.py
--rw-r--r--   0        0        0        0 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/types/__init__.py
--rw-r--r--   0        0        0      361 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/types/file_info.py
--rw-r--r--   0        0        0      248 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/__init__.py
--rw-r--r--   0        0        0     2887 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/args.py
--rw-r--r--   0        0        0     1128 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/deploy_helpers.py
--rw-r--r--   0        0        0     1591 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/import_helpers.py
--rw-r--r--   0        0        0      608 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/naming.py
--rw-r--r--   0        0        0     5715 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/retry.py
--rw-r--r--   0        0        0      318 2023-01-04 19:08:10.056197 odp_sdk_python_ingest-0.3.1/odp/utils/timers.py
--rw-r--r--   0        0        0     1906 2023-01-04 19:09:01.661230 odp_sdk_python_ingest-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.3.1/setup.py
--rw-r--r--   0        0        0     2543 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/auth/cdf/__init__.py
+-rw-r--r--   0        0        0     3258 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/auth/cdf/cdf_token_handler.py
+-rw-r--r--   0        0        0     1764 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/auth/cdf/federated_cognite_client.py
+-rw-r--r--   0        0        0      163 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/auth/odp/__init__.py
+-rw-r--r--   0        0        0     3064 2023-05-12 07:00:01.589745 odp_sdk_python_ingest-0.4.0/odp/auth/odp/interactive_login_token_handler.py
+-rw-r--r--   0        0        0     1813 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/auth/odp/ropc_token_handler.py
+-rw-r--r--   0        0        0     1358 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/auth/odp/token_handler.py
+-rw-r--r--   0        0        0       49 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/auth/prefect/__init__.py
+-rw-r--r--   0        0        0     3877 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/auth/prefect/prefect_b2c_client.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/blocks/__init__.py
+-rw-r--r--   0        0        0     6042 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/blocks/azure_storage.py
+-rw-r--r--   0        0        0     2879 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/blocks/cdf_storage.py
+-rw-r--r--   0        0        0      579 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/blocks/db_engine.py
+-rw-r--r--   0        0        0     2378 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/blocks/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/__main__.py
+-rw-r--r--   0        0        0      435 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/authenticate.py
+-rw-r--r--   0        0        0     2610 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/block.py
+-rw-r--r--   0        0        0     5041 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/context.py
+-rw-r--r--   0        0        0     7296 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/deploy.py
+-rw-r--r--   0        0        0     2741 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/parameters.py
+-rw-r--r--   0        0        0       43 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/params/__init__.py
+-rw-r--r--   0        0        0      515 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/params/type_param_type.py
+-rw-r--r--   0        0        0     3421 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/run.py
+-rw-r--r--   0        0        0     1019 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/cli/schema.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/config/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/config/cdf_config.py
+-rw-r--r--   0        0        0      816 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/config/dask_config.py
+-rw-r--r--   0        0        0      125 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/abstract_deployment_block.py
+-rw-r--r--   0        0        0       40 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/block/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/block/generic_block.py
+-rw-r--r--   0        0        0     1591 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/deployment_block_factory.py
+-rw-r--r--   0        0        0      190 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/abstract_runtime.py
+-rw-r--r--   0        0        0     3463 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/kubernetes.py
+-rw-r--r--   0        0        0     4567 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/kubernetes_dask.py
+-rw-r--r--   0        0        0     1718 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
+-rw-r--r--   0        0        0       88 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/schedule/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/schedule/abstract_schedule.py
+-rw-r--r--   0        0        0      471 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/schedule/cron_schedule.py
+-rw-r--r--   0        0        0     1030 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/schedule/interval_schedule.py
+-rw-r--r--   0        0        0       73 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/storage/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/storage/abstract_storage.py
+-rw-r--r--   0        0        0    10906 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/storage/docker.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/deploy/storage/prefect_healthcheck.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/__init__.py
+-rw-r--r--   0        0        0     4679 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/stateful_value_impl.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/__init__.py
+-rw-r--r--   0        0        0     1060 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/watermark_file_store.py
+-rw-r--r--   0        0        0      639 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/watermark_inmemory_store.py
+-rw-r--r--   0        0        0      728 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/watermark_redis_store.py
+-rw-r--r--   0        0        0     5488 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/secrets.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/state_handlers/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/state_handlers/metrics_pusher.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/tasks/cdf/__init__.py
+-rw-r--r--   0        0        0     3217 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/tasks/cdf/cdf_credentials.py
+-rw-r--r--   0        0        0     1438 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/tasks/concurrency_limit.py
+-rw-r--r--   0        0        0      705 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/tasks/measured_task.py
+-rw-r--r--   0        0        0     1580 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/compute/tasks/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/__init__.py
+-rw-r--r--   0        0        0     4749 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/abstract_metrics.py
+-rw-r--r--   0        0        0     1038 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/metric_client.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/mock/__init__.py
+-rw-r--r--   0        0        0     2431 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/mock/metric_client.py
+-rw-r--r--   0        0        0     3293 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/mock/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/prometheus/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/prometheus/metric_client.py
+-rw-r--r--   0        0        0     3721 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/metrics/prometheus/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/types/__init__.py
+-rw-r--r--   0        0        0      361 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/types/file_info.py
+-rw-r--r--   0        0        0      248 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/__init__.py
+-rw-r--r--   0        0        0     2887 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/args.py
+-rw-r--r--   0        0        0     1128 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/deploy_helpers.py
+-rw-r--r--   0        0        0     4913 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/import_helpers.py
+-rw-r--r--   0        0        0      607 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/naming.py
+-rw-r--r--   0        0        0     5715 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/retry.py
+-rw-r--r--   0        0        0      317 2023-05-12 07:00:01.593746 odp_sdk_python_ingest-0.4.0/odp/utils/timers.py
+-rw-r--r--   0        0        0     1945 2023-05-12 07:01:02.722517 odp_sdk_python_ingest-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.0/PKG-INFO
```

### Comparing `odp_sdk_python_ingest-0.3.1/README.md` & `odp_sdk_python_ingest-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/auth/cdf/cdf_token_handler.py` & `odp_sdk_python_ingest-0.4.0/odp/auth/cdf/cdf_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/auth/cdf/federated_cognite_client.py` & `odp_sdk_python_ingest-0.4.0/odp/auth/cdf/federated_cognite_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/auth/odp/interactive_login_token_handler.py` & `odp_sdk_python_ingest-0.4.0/odp/auth/odp/interactive_login_token_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 __all__ = ["InteractiveLoginTokenHandler"]
 
 LOG = logging.getLogger(__name__)
 
 
 class InteractiveLoginTokenHandler(TokenHandler):
-
     DEFAULT_CLIENT_ID = "2a18c352-e7ab-4437-96df-6036d815b3fc"
     DEFAULT_AUTHORITY = (
         "https://oceandataplatform.b2clogin.com/oceandataplatform.onmicrosoft.com/B2C_1A_signup_signin_custom"
     )
     DEFAULT_SCOPES = ["https://oceandataplatform.onmicrosoft.com/odp-backend/ODP_ACCESS"]
 
     def __init__(
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/auth/odp/ropc_token_handler.py` & `odp_sdk_python_ingest-0.4.0/odp/auth/odp/ropc_token_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import requests
 
 from .token_handler import TokenHandler
 
 
 class RopcTokenHandler(TokenHandler):
-
     DEFAULT_CLIENT_ID = "33b5d769-787b-466b-bc94-a10125f4c1ee"
     DEFAULT_LOGIN_URL = (
         "https://oceandataplatform.b2clogin.com/oceandataplatform.onmicrosoft.com/B2C_1A_ROPC_Auth/oauth2/v2.0/token"
     )
     DEFAULT_SCOPES = [
         "openid",
         "https://oceandataplatform.onmicrosoft.com/odp-backend/ODP_ACCESS",
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/auth/odp/token_handler.py` & `odp_sdk_python_ingest-0.4.0/odp/auth/odp/token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/auth/prefect/prefect_b2c_client.py` & `odp_sdk_python_ingest-0.4.0/odp/auth/prefect/prefect_b2c_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         schedule: Optional[AbstractSchedule] = None,
         api_server: Optional[str] = None,
         work_queue: Optional[str] = None,
         build: bool = True,
         dry_run: bool = False,
         **kwargs,
     ) -> Optional[str]:
-
         api_server = api_server or self._api_server or os.getenv("ODP_PREFECT_API")
         if not api_server:
             raise ValueError(
                 "Prefect API server not set. Please set using the"
                 "'api_server' argument or 'ODP_PREFECT_API' environment variable"
             )
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/blocks/azure_storage.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/blocks/azure_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
         if blob:
             container_client = self.container_client()
             return container_client.get_blob_client(blob)
 
         raise ValueError("Not enough arguments set for the blob client")
 
     def _get_credential(self) -> Optional[str]:
-
         if self.sas_token:
             return self.sas_token.get_secret_value()
         elif self.acces_key:
             return self.acces_key.get_secret_value()
 
         return None
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/blocks/cdf_storage.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/blocks/cdf_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/blocks/db_engine.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/blocks/db_engine.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/blocks/postgres.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/blocks/postgres.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/block.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                 block.__name__, Block.__module__, Block.__name__
             )
         )
 
     block_parameters = block.__fields__
 
     for p, value in param.items():
-
         if p not in block_parameters:
             raise ValueError(f"The parameter '{p}' is not an input argument of '{block.__name__}'")
 
         try:
             param[p] = literal_eval(value)
         except (ValueError, SyntaxError):
             param[p] = value
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/context.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/context.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/deploy.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/parameters.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         raise ImportError(f"Failed to import flow from module spec '{spec.name}'")
 
     spec.loader.exec_module(flow_module)
 
     flow: Flow = getattr(flow_module, fn)
 
     for pname, param in dict(inspect.signature(flow.fn).parameters).items():
-
         param = cast(inspect.Parameter, param)
         has_default = param.default is not inspect._empty
 
         cols = [f"name='{pname}'", f"required={not has_default}"]
 
         if has_default:
             cols.append(
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/params/type_param_type.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/params/type_param_type.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/run.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     flow: Flow = getattr(flow_module, fn)
 
     # Parse input parameters
 
     flow_parameters = set(inspect.signature(flow.fn).parameters)
 
     for param, value in parameters.items():
-
         if param not in flow_parameters:
             raise ValueError(f"The parameter '{param}' is not defined in the flow '{flow.name}'")
 
         try:
             parameters[param] = literal_eval(value)
         except ValueError:
             parameters[param] = value
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/cli/schema.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/cli/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import inspect
 from dataclasses import dataclass
 from typing import Type
 
 
 def arguments_to_dataclass(cls: Type) -> Type:
-
     signature = inspect.signature(cls.__init__)
 
     annotations = {}
     annotations_with_defaults = {}
     properties = {}
 
     for param in signature.parameters.values():
         if param.name in ("self", "kwargs", "args"):
             continue
 
         if param.annotation is not param.empty:
-
             if param.default is not param.empty:
                 annotations_with_defaults[param.name] = param.annotation
             else:
                 annotations[param.name] = param.annotation
 
         if param.default is not param.empty:
             properties[param.name] = param.default
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/config/cdf_config.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/config/cdf_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/config/dask_config.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/config/dask_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/deployment_block_factory.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/deployment_block_factory.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/kubernetes.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from ..storage import AbstractStorage, Docker
 from .abstract_runtime import AbstractRuntime
 
 __all__ = ["Kubernetes"]
 
 
 class Kubernetes(AbstractRuntime):
-
     ENV_KUBERNETES_NAMESPACE = "PREFECT_RUNTIME_NAMESPACE"
     ENV_ODP_WATERMARK_STORE_CLS = "ODP_WATERMARK_STORE_CLS"
     ENV_ODP_WATERMARK_STORE_ARGS = "ODP_WATERMARK_STORE_ARGS"
     ENV_ODP_METRIC_CLIENT_CLS = "ODP_METRIC_CLIENT_CLS"
     ENV_ODP_METRIC_CLIENT_ARGS = "ODP_METRIC_CLIENT_ARGS"
 
     JOB_TTL_SECONDS = 10
@@ -24,15 +23,14 @@
     def __init__(
         self,
         flow: Flow,
         namespace: Optional[str] = None,
         env: Optional[Dict[str, Union[None, str]]] = None,
         service_account_name: Optional[str] = None,
     ) -> None:
-
         super().__init__(flow)
 
         self._namespace: str = namespace or os.environ.get(self.ENV_KUBERNETES_NAMESPACE, "prefect")
         self._env = env
         self._service_account_name = service_account_name
         self._storage: Optional[Docker] = None
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/kubernetes_dask.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/kubernetes_dask.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         try:
             self._client = distributed.get_client()
         except ValueError:
             self._client = None
 
 
 class KubernetesDask(KubernetesTieredResource):
-
     ENV_DASK_GATEWAY_ADDRESS = "DASK_GATEWAY_ADDRESS"
     ENV_K8S_SERVICE_ACCOUNT = "K8S_SERVICE_ACCOUNT"
 
     def __init__(
         self,
         flow: Flow,
         tier: Optional[str] = None,
@@ -58,15 +57,14 @@
 
         # Cluster nodes defaults to the same tier as the flow
         self._cluster_tier = cluster_tier or self._tier
         self._min_workers = min_workers
         self._max_workers = max_workers
 
     def apply_flow_options(self, flow: Flow):
-
         flow_version = flow.version or "DIRTY"
 
         resources = self.TIERS[self._cluster_tier]
 
         # extra_labels = {"prefect.io/flow": self._flow.name, "hubocean.io/clusterTier": self._cluster_tier}
         # extra_annotations = {"prefect.io/flow": self._flow.name, "hubocean.io/clusterTier": self._cluster_tier}
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/runtime/kubernetes_tiered_resource.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/runtime/kubernetes_tiered_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from .kubernetes import Kubernetes
 
 K8sPodresourceSpec = namedtuple("K8sPodresourceSpec", ("cpu", "mem"))
 
 
 class KubernetesTieredResource(Kubernetes):
-
     TIERS = {
         "default": K8sPodresourceSpec("1", "2Gi"),
         "minimal": K8sPodresourceSpec("1", "2Gi"),
         "small": K8sPodresourceSpec("2", "7Gi"),
         "medium": K8sPodresourceSpec("4", "14Gi"),
         "large": K8sPodresourceSpec("8", "28Gi"),
         "huge": K8sPodresourceSpec("14", "50Gi"),
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/schedule/interval_schedule.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/schedule/interval_schedule.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/storage/abstract_storage.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/deploy/storage/docker.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/deploy/storage/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 def _get_default_base_image() -> str:
     return "prefecthq/prefect:{}-python{}.{}".format(
         prefect.__version__, sys.version_info.major, sys.version_info.minor
     )
 
 
 class Docker(AbstractStorage):
-
     ENV_DOCKER_HOST = "DOCKER_HOST"
     ENV_CONTAINER_REGISTRY = "CONTAINER_REGISTRY"
 
     DEFAULT_BASE_IMAGE = _get_default_base_image()
 
     def __init__(
         self,
@@ -93,15 +92,14 @@
             default_url = "unix://var/run/docker.sock"
 
         base_url = registry_url or os.environ.get(self.ENV_DOCKER_HOST, default_url)
 
         return docker.APIClient(base_url=base_url, version="auto", tls=tls)
 
     def _create_dockerfile_object(self, dir: str) -> str:
-
         if self._dockerfile:
             with open(self._dockerfile, "r") as fd:
                 base_commands = fd.read()
         else:
             base_commands = f"FROM {self._base_image}"
 
         env_vars = ""
@@ -132,15 +130,14 @@
                 else:
                     shutil.copy2(src=src, dst=full_fname)
 
                 copy_files += f"COPY {fname} {dest}\n"
 
         copy_flows = ""
         for flow_name, flow in self._flows.items():
-
             qualified_flow_name = self.flow_qualified_name(flow)
 
             open(os.path.join(dir, f"{qualified_flow_name}.pickle"), "wb+").write(cloudpickle.dumps(flow))
             open(os.path.join(dir, f"{qualified_flow_name}.py"), "w+").write(
                 textwrap.dedent(
                     f"""
                         import cloudpickle
@@ -243,15 +240,14 @@
             self._image_name = self._image_name or slugify(list(self._flows.keys())[0])
 
         self._image_tag = self._image_tag or slugify(datetime.now().isoformat())
 
         return self._build_image(push)
 
     def _build_image(self, push: bool = False) -> Tuple[str, str]:
-
         assert isinstance(self._image_name, str)
         assert isinstance(self._image_tag, str)
 
         full_image_name = f"{self._image_name}:{self._image_tag}"
 
         if self._base_image and not self._dockerfile:
             self.pull_image()
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/stateful_value_impl.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/stateful_value_impl.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/watermark_file_store.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/watermark_file_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/watermark_inmemory_store.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/watermark_inmemory_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/flow_state/store/watermark_redis_store.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/flow_state/store/watermark_redis_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/secrets.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,17 +77,15 @@
     def _getenv(self, key, default=None):
         if self.allow_platform_compensation:
             key = self._platform_compatible_key(key)
 
         return getenv(key, default)
 
     def _get(self):
-
         if self.secret_name:
-
             if self.secret_key:
                 value = self._getenv(f"{self.secret_name}_{self.secret_key}")
                 return self._maybe_raise(self.secret_key, value)
             else:
                 if self.allow_platform_compensation:
                     sn = self._platform_compatible_key(self.secret_name)
                 else:
@@ -103,15 +101,14 @@
             raise ValueError("At least one of secret_name or secret_key must be set")
         else:
             value = self._getenv(self.secret_key)
             return self._maybe_raise(self.secret_key, value)
 
 
 class KubernetesRuntimeSecret(RuntimeSecretBackend):
-
     SERVICE_ACCOUNT_MOUNT_PATH = "/var/run/secrets/kubernetes.io/serviceaccount"
 
     def __init__(
         self,
         secret_name: str,
         secret_key: Optional[str] = None,
         namespace: Optional[str] = None,
@@ -121,15 +118,14 @@
     ):
         super().__init__(secret_name, secret_key, raise_if_missing)
         self.namespace = namespace
         self.exclude_sa_credential = exclude_sa_credential
         self.k8s_api = k8s_api
 
     def _get(self):
-
         if self.k8s_api is None:
             self.k8s_api = pykube.HTTPClient(pykube.KubeConfig.from_service_account())
 
         namespace = self.namespace
         if not namespace and not self.exclude_sa_credential:
             LOG.debug("Namespace not set. Attempting to read from service account")
             namespace = open(path.join(self.SERVICE_ACCOUNT_MOUNT_PATH, "namespace")).read()
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/state_handlers/metrics_pusher.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/state_handlers/metrics_pusher.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,17 @@
     def stop(self, wait: bool = True, timeout: Optional[float] = None):
         self.keep_alive = False
 
         if wait:
             self.join(timeout=timeout)
 
     def run(self) -> None:
-
         last_cycle = 0
 
         while self.keep_alive:
-
             t = time.time()
             dt = t - last_cycle
             if dt < self.push_interval:
                 time.sleep(self.push_interval - dt)
             elif dt >= (1.1 * self.push_interval) and last_cycle > 0:
                 LOG.warning(
                     f"{self.__class__.__name__} cycle time exceeded expected interval: {dt} > {self.push_interval}"
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/tasks/cdf/cdf_credentials.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/tasks/cdf/cdf_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         client = CogniteClient(**{key: val for key, val in asdict(self).items() if val is not None})
         client.geospatial._log_request = self._nop
         return client
 
 
 @dataclass
 class CdfFederatedCredentials(CdfCredentials):
-
     project: str = None
     client_name: str = None
     token_client_id: Optional[str] = None
     token_username: Optional[str] = None
     token_password: Optional[str] = None
     token_scopes: Optional[List[str]] = None
     server: Optional[str] = None
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/tasks/concurrency_limit.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/tasks/concurrency_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from prefect.orion.schemas.filters import TaskRunFilter
 from prefect.orion.schemas.states import TERMINAL_STATES
 
 LOG = logging.getLogger(__name__)
 
 
 async def wait_for_concurrency_limit(client: OrionClient, tag: str, check_interval: float = 1.0, timeout: float = 0.0):
-
     start_time = time.time()
 
     while True:
         if 0 < timeout < (time.time() - start_time):
             LOG.warning("Concurrency wait timeout")
             break
 
@@ -28,15 +27,14 @@
             await anyio.sleep(check_interval)
         else:
             break
 
 
 @asynccontextmanager
 async def concurrency_limit(task: Task, limit: int = 10) -> Task:
-
     context = get_run_context()
 
     tag = f"{context.flow_run.id}-{task.name}"
 
     client = get_client()
 
     await client.create_concurrency_limit(tag, limit)
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/tasks/measured_task.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/tasks/measured_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 
 from odp.compute.metrics import Metrics
 
 __all__ = ["MeasuredTask"]
 
 
 class MeasuredTask(Task):
-
     DEFAULT_METRIC_NAMESPACE = "prefect"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.run = partial(self._run_wrapper, self.run)
         self._run_time_metric = Metrics.distribution(
             MeasuredTask.DEFAULT_METRIC_NAMESPACE,
             "run_time",
             ["flow", "flow_id", "task", "task_id", "flow_run_id", "task_run_id"],
         )
 
     @staticmethod
     def _run_wrapper(fn: Callable, **kwargs):
-
         ret = fn(**kwargs)
         Metrics.push()
 
         return ret
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/compute/tasks/tasks.py` & `odp_sdk_python_ingest-0.4.0/odp/compute/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/utils/args.py` & `odp_sdk_python_ingest-0.4.0/odp/utils/args.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/utils/deploy_helpers.py` & `odp_sdk_python_ingest-0.4.0/odp/utils/deploy_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/odp/utils/naming.py` & `odp_sdk_python_ingest-0.4.0/odp/utils/naming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
 import inflection
 
 
 def __get_formatter_cb(convention: str):
-
     convention = convention or os.getenv("USE_NAMING_CONVENTION") or "snake_case"
 
     if convention == "camelCase":
         return lambda x: inflection.camelize(x, False)
     elif convention == "CamelCase":
         return lambda x: inflection.camelize(x, True)
     elif convention == "snake_case":
```

### Comparing `odp_sdk_python_ingest-0.3.1/odp/utils/retry.py` & `odp_sdk_python_ingest-0.4.0/odp/utils/retry.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.3.1/pyproject.toml` & `odp_sdk_python_ingest-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "odp-sdk-python-ingest"
-version = "0.3.1"
+version = "0.4.0"
 description = "ODP ingest SDK"
 authors = ["Thomas Li Fredriksen <thomas.fredriksen@oceandata.earth>"]
 readme = "README.md"
 packages = [
     {include="odp"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-prefect = "^2.7.2"
+python = "^3.10"
+prefect = "^2.10.6"
 click = "^8.1.3"
-python-dotenv = "^0.21.0"
+python-dotenv = "^1.0.0"
 msal = "^1.19.0"
 msal-extensions = "^1.0.0"
 pykube-ng = "^22.9.0"
 azure-common = "^1.1.28"
 azure-identity = "^1.11.0"
 azure-keyvault = "^4.2.0"
 azure-keyvault-secrets = "^4.6.0"
@@ -28,28 +28,29 @@
 decorator = "^5.1.1"
 prefect-dask = "^0.2.0"
 azure-storage-blob = "^12.13.1"
 psycopg2-binary = "^2.9.3"
 jinja2 = "3.0.3"
 prefect-azure = {extras = ["blob"], version = "^0.2.2"}
 prefect-kv = "^0.1.0"
-cognite-sdk = "^4.11.0"
-fsspec = "^2022.10.0"
+cognite-sdk = "^5.10.1"
+fsspec = "^2023.4.0"
 dask-kubernetes = "~2022.10.1"
 dask = "~2022.11.0"
 requests = "^2.28.1"
-cognite-cdffs = "^0.1.0"
+cognite-cdffs = "^0.2.1"
+prometheus-client = "^0.16.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
-poethepoet = "^0.16.2"
+poethepoet = "^0.19.0"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.4.1"
-mkdocs-material = "^8.5.7"
+mkdocs-material = ">=8.5.7,<10.0.0"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 mkdocs-gen-files = "^0.4.0"
 flake8-pyproject = "^1.1.0.post0"
 types-requests = "^2.28.11.2"
 mypy = "^0.982"
 coverage = "^6.5.0"
```

### Comparing `odp_sdk_python_ingest-0.3.1/PKG-INFO` & `odp_sdk_python_ingest-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: odp-sdk-python-ingest
-Version: 0.3.1
+Version: 0.4.0
 Summary: ODP ingest SDK
 Author: Thomas Li Fredriksen
 Author-email: thomas.fredriksen@oceandata.earth
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-common (>=1.1.28,<2.0.0)
 Requires-Dist: azure-identity (>=1.11.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.6.0,<5.0.0)
 Requires-Dist: azure-storage-blob (>=12.13.1,<13.0.0)
 Requires-Dist: azure-storage-common (>=2.1.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cognite-cdffs (>=0.1.0,<0.2.0)
-Requires-Dist: cognite-sdk (>=4.11.0,<5.0.0)
+Requires-Dist: cognite-cdffs (>=0.2.1,<0.3.0)
+Requires-Dist: cognite-sdk (>=5.10.1,<6.0.0)
 Requires-Dist: dask (>=2022.11.0,<2022.12.0)
 Requires-Dist: dask-kubernetes (>=2022.10.1,<2022.11.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
-Requires-Dist: fsspec (>=2022.10.0,<2023.0.0)
+Requires-Dist: fsspec (>=2023.4.0,<2024.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: msal (>=1.19.0,<2.0.0)
 Requires-Dist: msal-extensions (>=1.0.0,<2.0.0)
-Requires-Dist: prefect (>=2.7.2,<3.0.0)
+Requires-Dist: prefect (>=2.10.6,<3.0.0)
 Requires-Dist: prefect-azure[blob] (>=0.2.2,<0.3.0)
 Requires-Dist: prefect-dask (>=0.2.0,<0.3.0)
 Requires-Dist: prefect-kv (>=0.1.0,<0.2.0)
+Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pykube-ng (>=22.9.0,<23.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: slugify (>=0.0.1,<0.0.2)
 Description-Content-Type: text/markdown
 
 # ODP Ingest SDK
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,31 +1,30 @@
-Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.3.1 Summary: ODP
+Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.0 Summary: ODP
 ingest SDK Author: Thomas Li Fredriksen Author-email:
-thomas.fredriksen@oceandata.earth Requires-Python: >=3.9,<4.0 Classifier:
+thomas.fredriksen@oceandata.earth Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: azure-common
-(>=1.1.28,<2.0.0) Requires-Dist: azure-identity (>=1.11.0,<2.0.0) Requires-
-Dist: azure-keyvault (>=4.2.0,<5.0.0) Requires-Dist: azure-keyvault-secrets
-(>=4.6.0,<5.0.0) Requires-Dist: azure-storage-blob (>=12.13.1,<13.0.0)
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
+azure-common (>=1.1.28,<2.0.0) Requires-Dist: azure-identity (>=1.11.0,<2.0.0)
+Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0) Requires-Dist: azure-keyvault-
+secrets (>=4.6.0,<5.0.0) Requires-Dist: azure-storage-blob (>=12.13.1,<13.0.0)
 Requires-Dist: azure-storage-common (>=2.1.0,<3.0.0) Requires-Dist: click
-(>=8.1.3,<9.0.0) Requires-Dist: cognite-cdffs (>=0.1.0,<0.2.0) Requires-Dist:
-cognite-sdk (>=4.11.0,<5.0.0) Requires-Dist: dask (>=2022.11.0,<2022.12.0)
+(>=8.1.3,<9.0.0) Requires-Dist: cognite-cdffs (>=0.2.1,<0.3.0) Requires-Dist:
+cognite-sdk (>=5.10.1,<6.0.0) Requires-Dist: dask (>=2022.11.0,<2022.12.0)
 Requires-Dist: dask-kubernetes (>=2022.10.1,<2022.11.0) Requires-Dist:
 decorator (>=5.1.1,<6.0.0) Requires-Dist: docker (>=6.0.0,<7.0.0) Requires-
-Dist: fsspec (>=2022.10.0,<2023.0.0) Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Dist: fsspec (>=2023.4.0,<2024.0.0) Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jinja2 (==3.0.3) Requires-Dist: msal (>=1.19.0,<2.0.0) Requires-
-Dist: msal-extensions (>=1.0.0,<2.0.0) Requires-Dist: prefect (>=2.7.2,<3.0.0)
+Dist: msal-extensions (>=1.0.0,<2.0.0) Requires-Dist: prefect (>=2.10.6,<3.0.0)
 Requires-Dist: prefect-azure[blob] (>=0.2.2,<0.3.0) Requires-Dist: prefect-dask
 (>=0.2.0,<0.3.0) Requires-Dist: prefect-kv (>=0.1.0,<0.2.0) Requires-Dist:
-psycopg2-binary (>=2.9.3,<3.0.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: pykube-ng (>=22.9.0,<23.0.0) Requires-Dist: python-dotenv
-(>=0.21.0,<0.22.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist:
-slugify (>=0.0.1,<0.0.2) Description-Content-Type: text/markdown # ODP Ingest
-SDK
+prometheus-client (>=0.16.0,<0.17.0) Requires-Dist: psycopg2-binary
+(>=2.9.3,<3.0.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist:
+pykube-ng (>=22.9.0,<23.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: slugify
+(>=0.0.1,<0.0.2) Description-Content-Type: text/markdown # ODP Ingest SDK
               [https://img.shields.io/badge/slack-join_community-
               red.svg?color=0052FF&labelColor=090422&logo=slack]
 ## Welcome! INTRO ## Setting up developer environment This project uses the
 [Poetry](https://python-poetry.org/) package manager. Please follow the
 [official](https://python-poetry.org/docs/#installation) documentation for
 installation details In addition to Poetry, this project also uses the package
 [Poe the Poet](https://github.com/nat-n/poethepoet) for running simple tasks
```


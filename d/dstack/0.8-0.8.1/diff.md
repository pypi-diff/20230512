# Comparing `tmp/dstack-0.8.tar.gz` & `tmp/dstack-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstack-0.8.tar", last modified: Thu May  4 07:20:45 2023, max compression
+gzip compressed data, was "dstack-0.8.1.tar", last modified: Fri May 12 16:49:00 2023, max compression
```

## Comparing `dstack-0.8.tar` & `dstack-0.8.1.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.419316 dstack-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-04 07:19:59.000000 dstack-0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-04 07:20:45.419316 dstack-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-04 07:19:59.000000 dstack-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.395315 dstack-0.8/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.395315 dstack-0.8/cli/dstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/api/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/internal/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/backend/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/backend/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/backend/local/
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/cp/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/init/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/prune/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/prune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/ps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/rm/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/rm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/run/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/start/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/start/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/stop/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/stop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/tags/
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/dependents.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/log_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/core/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/userconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/background/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/background/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/background/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/background/tasks/resubmit_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/migration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/migration/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/versions/3b900659c822_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/repository/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/repository/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/security/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/security/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/services/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    18554 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/_torchrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/_torchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/_torchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/bash/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/code/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/docker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/lab/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/dstack/providers/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/notebook/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/dstack/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/dstack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/random_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 07:20:44.000000 dstack-0.8/cli/dstack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.395315 dstack-0.8/cli/dstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/backend/base/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/test_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/docker/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/test_local_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.419316 dstack-0.8/cli/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/test_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/test_merge_workflow_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/test_tarignore.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:20:45.419316 dstack-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-04 07:19:59.000000 dstack-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-12 16:47:49.000000 dstack-0.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-12 16:49:00.777871 dstack-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-12 16:47:49.000000 dstack-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.753870 dstack-0.8.1/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/internal/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/prune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/ps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/rm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/rm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/run/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/start/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/start/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/stop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/dependents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/log_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/core/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/userconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/background/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/background/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/background/tasks/resubmit_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/migration/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/versions/3b900659c822_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/repository/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/repository/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/security/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/security/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/services/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/_torchrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/_torchrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/_torchrun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/bash/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/code/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/docker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/lab/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/notebook/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/dstack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/random_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/backend/base/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/docker/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/test_local_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/test_merge_workflow_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/test_tarignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:49:00.777871 dstack-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-12 16:47:49.000000 dstack-0.8.1/setup.py
```

### Comparing `dstack-0.8/LICENSE.md` & `dstack-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dstack-0.8/PKG-INFO` & `dstack-0.8.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,23 @@
-Metadata-Version: 2.1
-Name: dstack
-Version: 0.8
-Summary: The easiest way to define ML workflows and run them on any cloud platform
-Home-page: https://dstack.ai
-Author: Andrey Cheptsov
-Author-email: andrey@dstack.ai
-License: UNKNOWN
-Project-URL: Source, https://github.com/dstackai/dstack
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 <div align="center">
 <h1 align="center">
   <a target="_blank" href="https://dstack.ai">
-    <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo.svg" width="400px"/>
+    <picture>
+      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/images/dstack-logo-dark.svg"/>
+      <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/images/dstack-logo.svg" width="400px"/>
+    </picture>
   </a>
 </h1>
 
 <h4 align="center">
 ML workflows as code
 </h4>
 
 <p align="center">
-The easiest way to define ML workflows and run them on any cloud platform 
+The easiest way to run ML workflows on any cloud platform 
 </p>
 
 [![Slack](https://img.shields.io/badge/slack-join%20chat-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
 
 <p align="center">
 <a href="https://dstack.ai/docs/quick-start" target="_blank"><b>Quick start</b></a> • 
 <a href="https://dstack.ai/docs" target="_blank"><b>Docs</b></a> • 
@@ -49,129 +34,151 @@
 
 `dstack` makes it very easy to define ML workflows
 and run them on any cloud platform. It provisions infrastructure,
 manages data, and monitors usage for you.
 
 Ideal for processing data, training models, running apps, and any other ML development tasks.
 
-## Install the CLI
+## Installation and setup
 
-Use `pip` to install `dstack`:
+To use `dstack`, install it with `pip` and start the Hub application.
 
 ```shell
 pip install dstack
+dstack start
 ```
 
-## Define workflows
+The `dstack start` command starts the Hub application, and creates the default project to run workflows locally.
+
+If you'll want to run workflows in the cloud (e.g. AWS, or GCP), simply log into the Hub application, and 
+create a new project.
 
-Define ML workflows, their output artifacts, hardware requirements, and dependencies via YAML.
+## Run your first  workflows
+
+Let's define our first ML workflow in `.dstack/workflows/hello.yaml`:
 
 ```yaml
 workflows:
   - name: train-mnist
     provider: bash
     commands:
       - pip install torchvision pytorch-lightning tensorboard
       - python examples/mnist/train_mnist.py
     artifacts:
       - path: ./lightning_logs
 ```
 
-## Run locally
+The YAML file allows you to request hardware [resources](https://dstack.ai/docs/usage/resources), run [Python](https://dstack.ai/docs/usage/python),
+save [artifacts](https://dstack.ai/docs/usage/artifacts), use [cache](https://dstack.ai/docs/usage/cache) and  
+[dependencies](https://dstack.ai/docs/usage/deps), create [dev environments](https://dstack.ai/docs/usage/dev-environments),
+run [apps](https://dstack.ai/docs/usage/apps), and many more.
+
+## Run it
 
-By default, workflows run locally on your machine.
+Go ahead and run it:
 
 ```shell
 dstack run train-mnist
 
 RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
 penguin-1  train-mnist  now        Submitted       local
 
 Provisioning... It may take up to a minute. ✓
 
 To interrupt, press Ctrl+C.
 
-GPU available: True, used: True
+GPU available: False, used: False
 
 Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-## Run remotely
+The `dstack run` command runs the workflow using the settings specified for the project configured with the
+Hub application.
+
+## Create a Hub project
+
+As mentioned above, the default project runs workflows locally.
+However, you can log into the application and create other projects that allow you to run workflows in the cloud.
+
+<img src="https://dstack.ai/assets/dstack-hub-create-project.png" width="800px" />
 
-To run workflows remotely in a configured cloud, you will need the Hub application, which can be installed either on a
-dedicated server for team work or directly on your local machine.
+If you want the project to use the cloud, you'll need to provide cloud credentials and specify settings such as the
+artifact storage bucket and the region where the workflows will run.
 
-### Start the Hub application
+<img src="https://dstack.ai/assets/dstack-hub-view-project.png" width="800px" />
 
-To start the Hub application, use this command:
+Once a project is created, copy the CLI command from the project settings and execute it in your terminal.
 
 <div class="termy">
 
 ```shell
-$ dstack hub start
-
-The hub is available at http://127.0.0.1:3000?token=b934d226-e24a-4eab-a284-eb92b353b10f
+dstack config --url http://127.0.0.1:3000 \
+  --project gcp \
+  --token b934d226-e24a-4eab-a284-eb92b353b10f
 ```
 
 </div>
 
-To login as an administrator, visit the URL in the output.
+The `dstack config` command configures `dstack` to run workflows using the settings from
+the corresponding project.
 
-### Create a project
+You can configure multiple projects and use them interchangeably (by passing the `--project` argument to the `dstack 
+run` command. Any project can be set as the default by passing `--default` to the `dstack config` command.
 
-Go ahead and create a new project.
+Configuring multiple projects can be convenient if you want to run workflows both locally and in the cloud or if 
+you would like to use multiple clouds.
 
-<img src="https://dstack.ai/assets/dstack_hub_create_project.png" width="800px"/>
 
-Choose a backend type (such as AWS or GCP), provide cloud credentials, and specify settings like
-artifact storage bucket and the region where to run workflows.
+## Manage resources
 
-<img src="https://dstack.ai/assets/dstack_hub_view_project.png" width="800px"/>
+Consider that you have configured a project that allows you to use a GPU (e.g., a local backend if you have a GPU
+locally, or an AWS or GCP backend).
 
-### Configure the CLI
+Let's update our workflow and add `resources`.
 
-Copy the CLI command from the project settings and execute it in your terminal to configure the project as a remote.
-
-<div class="termy">
-
-```shell
-$ dstack config hub --url http://127.0.0.1:3000 \
-  --project my-awesome-project \
-  --token b934d226-e24a-4eab-a284-eb92b353b10f
+```yaml
+workflows:
+  - name: train-mnist
+    provider: bash
+    commands:
+      - pip install torchvision pytorch-lightning tensorboard
+      - python examples/mnist/train_mnist.py
+    artifacts:
+      - path: ./lightning_logs
+    resources:
+      gpu:
+        name: V100
+        count: 1
 ```
 
-</div>
-
-Now, you can run workflows remotely in the created project by adding the `--remote` flag to the `dstack run` command
-and request hardware [`resources`](usage/resources.md) (like GPU, memory, interruptible instances, etc.) that you need.
+Let's run the workflow:
 
 ```shell
-dstack run train-mnist --remote --gpu 1
+dstack run train-mnist --project gcp
 
-RUN       WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
-turtle-1  train-mnist  now        Submitted       aws
+RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+penguin-1  train-mnist  now        Submitted       local
 
 Provisioning... It may take up to a minute. ✓
 
 To interrupt, press Ctrl+C.
 
 GPU available: True, used: True
 
 Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-The command will automatically provision the required cloud resources in the corresponding cloud upon workflow 
-startup and tear them down upon completion.
+If your project is configured to use the cloud, the Hub application will automatically create the necessary cloud
+resources to execute the workflow and tear them down once it is finished.
 
 ## More information
 
 For additional information and examples, see the following links:
 
 * [Quick start](https://dstack.ai/docs/quick-start)
 * [Docs](https://dstack.ai/docs)
 * [Tutorials](https://dstack.ai/tutorials/dolly)
 * [Blog](https://dstack.ai/blog)
  
 ##  Licence
 
-[Mozilla Public License 2.0](LICENSE.md)
-
+[Mozilla Public License 2.0](LICENSE.md)
```

#### html2text {}

```diff
@@ -1,62 +1,69 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.8 Summary: The easiest way to
-define ML workflows and run them on any cloud platform Home-page: https://
-dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
-UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
-UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
-Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE.md
-                            ****** [dstack] ******
+                           ****** __[dstack]_ ******
                          *** ML workflows as code ***
-   The easiest way to define ML workflows and run them on any cloud platform
+           The easiest way to run ML workflows on any cloud platform
            [![Slack](https://img.shields.io/badge/slack-join%20chat-
 blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/
                shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
                   Quick_start â¢ Docs â¢ Tutorials â¢ Blog
   [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)]
    (https://github.com/dstackai/dstack/commits/) [![PyPI - License](https://
    img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/
                     dstackai/dstack/blob/master/LICENSE.md)
 ## What is dstack? `dstack` makes it very easy to define ML workflows and run
 them on any cloud platform. It provisions infrastructure, manages data, and
 monitors usage for you. Ideal for processing data, training models, running
-apps, and any other ML development tasks. ## Install the CLI Use `pip` to
-install `dstack`: ```shell pip install dstack ``` ## Define workflows Define ML
-workflows, their output artifacts, hardware requirements, and dependencies via
-YAML. ```yaml workflows: - name: train-mnist provider: bash commands: - pip
-install torchvision pytorch-lightning tensorboard - python examples/mnist/
-train_mnist.py artifacts: - path: ./lightning_logs ``` ## Run locally By
-default, workflows run locally on your machine. ```shell dstack run train-mnist
-RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-mnist now Submitted
-local Provisioning... It may take up to a minute. â To interrupt, press
-Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00, 280.17it/s,
-loss=1.35, v_num=0] ``` ## Run remotely To run workflows remotely in a
-configured cloud, you will need the Hub application, which can be installed
-either on a dedicated server for team work or directly on your local machine.
-### Start the Hub application To start the Hub application, use this command:
-```shell $ dstack hub start The hub is available at http://127.0.0.1:
-3000?token=b934d226-e24a-4eab-a284-eb92b353b10f ```
-To login as an administrator, visit the URL in the output. ### Create a project
-Go ahead and create a new project. [https://dstack.ai/assets/
-dstack_hub_create_project.png] Choose a backend type (such as AWS or GCP),
-provide cloud credentials, and specify settings like artifact storage bucket
-and the region where to run workflows. [https://dstack.ai/assets/
-dstack_hub_view_project.png] ### Configure the CLI Copy the CLI command from
-the project settings and execute it in your terminal to configure the project
-as a remote.
-```shell $ dstack config hub --url http://127.0.0.1:3000 \ --project my-
-awesome-project \ --token b934d226-e24a-4eab-a284-eb92b353b10f ```
-Now, you can run workflows remotely in the created project by adding the `--
-remote` flag to the `dstack run` command and request hardware [`resources`]
-(usage/resources.md) (like GPU, memory, interruptible instances, etc.) that you
-need. ```shell dstack run train-mnist --remote --gpu 1 RUN WORKFLOW SUBMITTED
-STATUS TAG BACKENDS turtle-1 train-mnist now Submitted aws Provisioning... It
-may take up to a minute. â To interrupt, press Ctrl+C. GPU available: True,
-used: True Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0] ``` The
-command will automatically provision the required cloud resources in the
-corresponding cloud upon workflow startup and tear them down upon completion.
-## More information For additional information and examples, see the following
+apps, and any other ML development tasks. ## Installation and setup To use
+`dstack`, install it with `pip` and start the Hub application. ```shell pip
+install dstack dstack start ``` The `dstack start` command starts the Hub
+application, and creates the default project to run workflows locally. If
+you'll want to run workflows in the cloud (e.g. AWS, or GCP), simply log into
+the Hub application, and create a new project. ## Run your first workflows
+Let's define our first ML workflow in `.dstack/workflows/hello.yaml`: ```yaml
+workflows: - name: train-mnist provider: bash commands: - pip install
+torchvision pytorch-lightning tensorboard - python examples/mnist/
+train_mnist.py artifacts: - path: ./lightning_logs ``` The YAML file allows you
+to request hardware [resources](https://dstack.ai/docs/usage/resources), run
+[Python](https://dstack.ai/docs/usage/python), save [artifacts](https://
+dstack.ai/docs/usage/artifacts), use [cache](https://dstack.ai/docs/usage/
+cache) and [dependencies](https://dstack.ai/docs/usage/deps), create [dev
+environments](https://dstack.ai/docs/usage/dev-environments), run [apps](https:
+//dstack.ai/docs/usage/apps), and many more. ## Run it Go ahead and run it:
+```shell dstack run train-mnist RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS
+penguin-1 train-mnist now Submitted local Provisioning... It may take up to a
+minute. â To interrupt, press Ctrl+C. GPU available: False, used: False Epoch
+1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0] ``` The `dstack run` command
+runs the workflow using the settings specified for the project configured with
+the Hub application. ## Create a Hub project As mentioned above, the default
+project runs workflows locally. However, you can log into the application and
+create other projects that allow you to run workflows in the cloud. [https://
+dstack.ai/assets/dstack-hub-create-project.png] If you want the project to use
+the cloud, you'll need to provide cloud credentials and specify settings such
+as the artifact storage bucket and the region where the workflows will run.
+[https://dstack.ai/assets/dstack-hub-view-project.png] Once a project is
+created, copy the CLI command from the project settings and execute it in your
+terminal.
+```shell dstack config --url http://127.0.0.1:3000 \ --project gcp \ --token
+b934d226-e24a-4eab-a284-eb92b353b10f ```
+The `dstack config` command configures `dstack` to run workflows using the
+settings from the corresponding project. You can configure multiple projects
+and use them interchangeably (by passing the `--project` argument to the
+`dstack run` command. Any project can be set as the default by passing `--
+default` to the `dstack config` command. Configuring multiple projects can be
+convenient if you want to run workflows both locally and in the cloud or if you
+would like to use multiple clouds. ## Manage resources Consider that you have
+configured a project that allows you to use a GPU (e.g., a local backend if you
+have a GPU locally, or an AWS or GCP backend). Let's update our workflow and
+add `resources`. ```yaml workflows: - name: train-mnist provider: bash
+commands: - pip install torchvision pytorch-lightning tensorboard - python
+examples/mnist/train_mnist.py artifacts: - path: ./lightning_logs resources:
+gpu: name: V100 count: 1 ``` Let's run the workflow: ```shell dstack run train-
+mnist --project gcp RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-
+mnist now Submitted local Provisioning... It may take up to a minute. â To
+interrupt, press Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00,
+280.17it/s, loss=1.35, v_num=0] ``` If your project is configured to use the
+cloud, the Hub application will automatically create the necessary cloud
+resources to execute the workflow and tear them down once it is finished. ##
+More information For additional information and examples, see the following
 links: * [Quick start](https://dstack.ai/docs/quick-start) * [Docs](https://
 dstack.ai/docs) * [Tutorials](https://dstack.ai/tutorials/dolly) * [Blog]
 (https://dstack.ai/blog) ## Licence [Mozilla Public License 2.0](LICENSE.md)
```

### Comparing `dstack-0.8/README.md` & `dstack-0.8.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,38 @@
+Metadata-Version: 2.1
+Name: dstack
+Version: 0.8.1
+Summary: The easiest way to define ML workflows and run them on any cloud platform
+Home-page: https://dstack.ai
+Author: Andrey Cheptsov
+Author-email: andrey@dstack.ai
+License: UNKNOWN
+Project-URL: Source, https://github.com/dstackai/dstack
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 <div align="center">
 <h1 align="center">
   <a target="_blank" href="https://dstack.ai">
-    <picture>
-      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo-dark.svg"/>
-      <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo.svg" width="400px"/>
-    </picture>
+    <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/images/dstack-logo.svg" width="400px"/>
   </a>
 </h1>
 
 <h4 align="center">
 ML workflows as code
 </h4>
 
 <p align="center">
-The easiest way to define ML workflows and run them on any cloud platform 
+The easiest way to run ML workflows on any cloud platform 
 </p>
 
 [![Slack](https://img.shields.io/badge/slack-join%20chat-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
 
 <p align="center">
 <a href="https://dstack.ai/docs/quick-start" target="_blank"><b>Quick start</b></a> • 
 <a href="https://dstack.ai/docs" target="_blank"><b>Docs</b></a> • 
@@ -34,128 +49,152 @@
 
 `dstack` makes it very easy to define ML workflows
 and run them on any cloud platform. It provisions infrastructure,
 manages data, and monitors usage for you.
 
 Ideal for processing data, training models, running apps, and any other ML development tasks.
 
-## Install the CLI
+## Installation and setup
 
-Use `pip` to install `dstack`:
+To use `dstack`, install it with `pip` and start the Hub application.
 
 ```shell
 pip install dstack
+dstack start
 ```
 
-## Define workflows
+The `dstack start` command starts the Hub application, and creates the default project to run workflows locally.
+
+If you'll want to run workflows in the cloud (e.g. AWS, or GCP), simply log into the Hub application, and 
+create a new project.
 
-Define ML workflows, their output artifacts, hardware requirements, and dependencies via YAML.
+## Run your first  workflows
+
+Let's define our first ML workflow in `.dstack/workflows/hello.yaml`:
 
 ```yaml
 workflows:
   - name: train-mnist
     provider: bash
     commands:
       - pip install torchvision pytorch-lightning tensorboard
       - python examples/mnist/train_mnist.py
     artifacts:
       - path: ./lightning_logs
 ```
 
-## Run locally
+The YAML file allows you to request hardware [resources](https://dstack.ai/docs/usage/resources), run [Python](https://dstack.ai/docs/usage/python),
+save [artifacts](https://dstack.ai/docs/usage/artifacts), use [cache](https://dstack.ai/docs/usage/cache) and  
+[dependencies](https://dstack.ai/docs/usage/deps), create [dev environments](https://dstack.ai/docs/usage/dev-environments),
+run [apps](https://dstack.ai/docs/usage/apps), and many more.
+
+## Run it
 
-By default, workflows run locally on your machine.
+Go ahead and run it:
 
 ```shell
 dstack run train-mnist
 
 RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
 penguin-1  train-mnist  now        Submitted       local
 
 Provisioning... It may take up to a minute. ✓
 
 To interrupt, press Ctrl+C.
 
-GPU available: True, used: True
+GPU available: False, used: False
 
 Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-## Run remotely
+The `dstack run` command runs the workflow using the settings specified for the project configured with the
+Hub application.
+
+## Create a Hub project
+
+As mentioned above, the default project runs workflows locally.
+However, you can log into the application and create other projects that allow you to run workflows in the cloud.
+
+<img src="https://dstack.ai/assets/dstack-hub-create-project.png" width="800px" />
 
-To run workflows remotely in a configured cloud, you will need the Hub application, which can be installed either on a
-dedicated server for team work or directly on your local machine.
+If you want the project to use the cloud, you'll need to provide cloud credentials and specify settings such as the
+artifact storage bucket and the region where the workflows will run.
 
-### Start the Hub application
+<img src="https://dstack.ai/assets/dstack-hub-view-project.png" width="800px" />
 
-To start the Hub application, use this command:
+Once a project is created, copy the CLI command from the project settings and execute it in your terminal.
 
 <div class="termy">
 
 ```shell
-$ dstack hub start
-
-The hub is available at http://127.0.0.1:3000?token=b934d226-e24a-4eab-a284-eb92b353b10f
+dstack config --url http://127.0.0.1:3000 \
+  --project gcp \
+  --token b934d226-e24a-4eab-a284-eb92b353b10f
 ```
 
 </div>
 
-To login as an administrator, visit the URL in the output.
+The `dstack config` command configures `dstack` to run workflows using the settings from
+the corresponding project.
 
-### Create a project
+You can configure multiple projects and use them interchangeably (by passing the `--project` argument to the `dstack 
+run` command. Any project can be set as the default by passing `--default` to the `dstack config` command.
 
-Go ahead and create a new project.
+Configuring multiple projects can be convenient if you want to run workflows both locally and in the cloud or if 
+you would like to use multiple clouds.
 
-<img src="https://dstack.ai/assets/dstack_hub_create_project.png" width="800px"/>
 
-Choose a backend type (such as AWS or GCP), provide cloud credentials, and specify settings like
-artifact storage bucket and the region where to run workflows.
+## Manage resources
 
-<img src="https://dstack.ai/assets/dstack_hub_view_project.png" width="800px"/>
+Consider that you have configured a project that allows you to use a GPU (e.g., a local backend if you have a GPU
+locally, or an AWS or GCP backend).
 
-### Configure the CLI
+Let's update our workflow and add `resources`.
 
-Copy the CLI command from the project settings and execute it in your terminal to configure the project as a remote.
-
-<div class="termy">
-
-```shell
-$ dstack config hub --url http://127.0.0.1:3000 \
-  --project my-awesome-project \
-  --token b934d226-e24a-4eab-a284-eb92b353b10f
+```yaml
+workflows:
+  - name: train-mnist
+    provider: bash
+    commands:
+      - pip install torchvision pytorch-lightning tensorboard
+      - python examples/mnist/train_mnist.py
+    artifacts:
+      - path: ./lightning_logs
+    resources:
+      gpu:
+        name: V100
+        count: 1
 ```
 
-</div>
-
-Now, you can run workflows remotely in the created project by adding the `--remote` flag to the `dstack run` command
-and request hardware [`resources`](usage/resources.md) (like GPU, memory, interruptible instances, etc.) that you need.
+Let's run the workflow:
 
 ```shell
-dstack run train-mnist --remote --gpu 1
+dstack run train-mnist --project gcp
 
-RUN       WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
-turtle-1  train-mnist  now        Submitted       aws
+RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+penguin-1  train-mnist  now        Submitted       local
 
 Provisioning... It may take up to a minute. ✓
 
 To interrupt, press Ctrl+C.
 
 GPU available: True, used: True
 
 Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-The command will automatically provision the required cloud resources in the corresponding cloud upon workflow 
-startup and tear them down upon completion.
+If your project is configured to use the cloud, the Hub application will automatically create the necessary cloud
+resources to execute the workflow and tear them down once it is finished.
 
 ## More information
 
 For additional information and examples, see the following links:
 
 * [Quick start](https://dstack.ai/docs/quick-start)
 * [Docs](https://dstack.ai/docs)
 * [Tutorials](https://dstack.ai/tutorials/dolly)
 * [Blog](https://dstack.ai/blog)
  
 ##  Licence
 
-[Mozilla Public License 2.0](LICENSE.md)
+[Mozilla Public License 2.0](LICENSE.md)
+
```

#### html2text {}

```diff
@@ -1,53 +1,78 @@
-                           ****** __[dstack]_ ******
+Metadata-Version: 2.1 Name: dstack Version: 0.8.1 Summary: The easiest way to
+define ML workflows and run them on any cloud platform Home-page: https://
+dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
+UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
+UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
+Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE.md
+                            ****** [dstack] ******
                          *** ML workflows as code ***
-   The easiest way to define ML workflows and run them on any cloud platform
+           The easiest way to run ML workflows on any cloud platform
            [![Slack](https://img.shields.io/badge/slack-join%20chat-
 blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/
                shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
                   Quick_start â¢ Docs â¢ Tutorials â¢ Blog
   [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)]
    (https://github.com/dstackai/dstack/commits/) [![PyPI - License](https://
    img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/
                     dstackai/dstack/blob/master/LICENSE.md)
 ## What is dstack? `dstack` makes it very easy to define ML workflows and run
 them on any cloud platform. It provisions infrastructure, manages data, and
 monitors usage for you. Ideal for processing data, training models, running
-apps, and any other ML development tasks. ## Install the CLI Use `pip` to
-install `dstack`: ```shell pip install dstack ``` ## Define workflows Define ML
-workflows, their output artifacts, hardware requirements, and dependencies via
-YAML. ```yaml workflows: - name: train-mnist provider: bash commands: - pip
-install torchvision pytorch-lightning tensorboard - python examples/mnist/
-train_mnist.py artifacts: - path: ./lightning_logs ``` ## Run locally By
-default, workflows run locally on your machine. ```shell dstack run train-mnist
-RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-mnist now Submitted
-local Provisioning... It may take up to a minute. â To interrupt, press
-Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00, 280.17it/s,
-loss=1.35, v_num=0] ``` ## Run remotely To run workflows remotely in a
-configured cloud, you will need the Hub application, which can be installed
-either on a dedicated server for team work or directly on your local machine.
-### Start the Hub application To start the Hub application, use this command:
-```shell $ dstack hub start The hub is available at http://127.0.0.1:
-3000?token=b934d226-e24a-4eab-a284-eb92b353b10f ```
-To login as an administrator, visit the URL in the output. ### Create a project
-Go ahead and create a new project. [https://dstack.ai/assets/
-dstack_hub_create_project.png] Choose a backend type (such as AWS or GCP),
-provide cloud credentials, and specify settings like artifact storage bucket
-and the region where to run workflows. [https://dstack.ai/assets/
-dstack_hub_view_project.png] ### Configure the CLI Copy the CLI command from
-the project settings and execute it in your terminal to configure the project
-as a remote.
-```shell $ dstack config hub --url http://127.0.0.1:3000 \ --project my-
-awesome-project \ --token b934d226-e24a-4eab-a284-eb92b353b10f ```
-Now, you can run workflows remotely in the created project by adding the `--
-remote` flag to the `dstack run` command and request hardware [`resources`]
-(usage/resources.md) (like GPU, memory, interruptible instances, etc.) that you
-need. ```shell dstack run train-mnist --remote --gpu 1 RUN WORKFLOW SUBMITTED
-STATUS TAG BACKENDS turtle-1 train-mnist now Submitted aws Provisioning... It
-may take up to a minute. â To interrupt, press Ctrl+C. GPU available: True,
-used: True Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0] ``` The
-command will automatically provision the required cloud resources in the
-corresponding cloud upon workflow startup and tear them down upon completion.
-## More information For additional information and examples, see the following
+apps, and any other ML development tasks. ## Installation and setup To use
+`dstack`, install it with `pip` and start the Hub application. ```shell pip
+install dstack dstack start ``` The `dstack start` command starts the Hub
+application, and creates the default project to run workflows locally. If
+you'll want to run workflows in the cloud (e.g. AWS, or GCP), simply log into
+the Hub application, and create a new project. ## Run your first workflows
+Let's define our first ML workflow in `.dstack/workflows/hello.yaml`: ```yaml
+workflows: - name: train-mnist provider: bash commands: - pip install
+torchvision pytorch-lightning tensorboard - python examples/mnist/
+train_mnist.py artifacts: - path: ./lightning_logs ``` The YAML file allows you
+to request hardware [resources](https://dstack.ai/docs/usage/resources), run
+[Python](https://dstack.ai/docs/usage/python), save [artifacts](https://
+dstack.ai/docs/usage/artifacts), use [cache](https://dstack.ai/docs/usage/
+cache) and [dependencies](https://dstack.ai/docs/usage/deps), create [dev
+environments](https://dstack.ai/docs/usage/dev-environments), run [apps](https:
+//dstack.ai/docs/usage/apps), and many more. ## Run it Go ahead and run it:
+```shell dstack run train-mnist RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS
+penguin-1 train-mnist now Submitted local Provisioning... It may take up to a
+minute. â To interrupt, press Ctrl+C. GPU available: False, used: False Epoch
+1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0] ``` The `dstack run` command
+runs the workflow using the settings specified for the project configured with
+the Hub application. ## Create a Hub project As mentioned above, the default
+project runs workflows locally. However, you can log into the application and
+create other projects that allow you to run workflows in the cloud. [https://
+dstack.ai/assets/dstack-hub-create-project.png] If you want the project to use
+the cloud, you'll need to provide cloud credentials and specify settings such
+as the artifact storage bucket and the region where the workflows will run.
+[https://dstack.ai/assets/dstack-hub-view-project.png] Once a project is
+created, copy the CLI command from the project settings and execute it in your
+terminal.
+```shell dstack config --url http://127.0.0.1:3000 \ --project gcp \ --token
+b934d226-e24a-4eab-a284-eb92b353b10f ```
+The `dstack config` command configures `dstack` to run workflows using the
+settings from the corresponding project. You can configure multiple projects
+and use them interchangeably (by passing the `--project` argument to the
+`dstack run` command. Any project can be set as the default by passing `--
+default` to the `dstack config` command. Configuring multiple projects can be
+convenient if you want to run workflows both locally and in the cloud or if you
+would like to use multiple clouds. ## Manage resources Consider that you have
+configured a project that allows you to use a GPU (e.g., a local backend if you
+have a GPU locally, or an AWS or GCP backend). Let's update our workflow and
+add `resources`. ```yaml workflows: - name: train-mnist provider: bash
+commands: - pip install torchvision pytorch-lightning tensorboard - python
+examples/mnist/train_mnist.py artifacts: - path: ./lightning_logs resources:
+gpu: name: V100 count: 1 ``` Let's run the workflow: ```shell dstack run train-
+mnist --project gcp RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-
+mnist now Submitted local Provisioning... It may take up to a minute. â To
+interrupt, press Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00,
+280.17it/s, loss=1.35, v_num=0] ``` If your project is configured to use the
+cloud, the Hub application will automatically create the necessary cloud
+resources to execute the workflow and tear them down once it is finished. ##
+More information For additional information and examples, see the following
 links: * [Quick start](https://dstack.ai/docs/quick-start) * [Docs](https://
 dstack.ai/docs) * [Tutorials](https://dstack.ai/tutorials/dolly) * [Blog]
 (https://dstack.ai/blog) ## Licence [Mozilla Public License 2.0](LICENSE.md)
```

### Comparing `dstack-0.8/cli/dstack/api/hub/_api_client.py` & `dstack-0.8.1/cli/dstack/api/hub/_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from dstack.core.repo import RemoteRepoCredentials, Repo, RepoHead, RepoSpec
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 from dstack.hub.models import (
     AddTagPath,
     AddTagRun,
+    ArtifactsList,
     JobHeadList,
     JobsGet,
     JobsList,
     PollLogs,
     ProjectInfo,
     ReposUpdate,
     RunsList,
@@ -496,26 +497,30 @@
             headers=self._headers(),
             data=self.repo.repo_ref.json(),
         )
         if resp.ok:
             return
         resp.raise_for_status()
 
-    def list_run_artifact_files(self, run_name: str) -> List[Artifact]:
+    def list_run_artifact_files(
+        self, run_name: str, prefix: str, recursive: bool
+    ) -> List[Artifact]:
         url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/artifacts/list",
         )
         resp = _make_hub_request(
             requests.post,
             host=self.url,
             url=url,
             headers=self._headers(),
-            data=JobsList(repo_id=self.repo.repo_id, run_name=run_name).json(),
+            data=ArtifactsList(
+                repo_id=self.repo.repo_id, run_name=run_name, prefix=prefix, recursive=recursive
+            ).json(),
         )
         if resp.ok:
             artifact_data = resp.json()
             return [Artifact.parse_obj(artifact) for artifact in artifact_data]
         resp.raise_for_status()
 
     def poll_logs(
@@ -600,15 +605,15 @@
             additional_path=f"/workflows/{workflow_name}/cache/delete",
         )
         resp = _make_hub_request(
             requests.post,
             host=self.url,
             url=url,
             headers=self._headers(),
-            data=RepoSpec.from_repo(self.repo).json(),
+            data=self.repo.repo_ref.json(),
         )
         if resp.ok:
             return
         resp.raise_for_status()
 
 
 def _project_url(url: str, project: str, additional_path: str, query: Optional[dict] = None):
```

### Comparing `dstack-0.8/cli/dstack/api/hub/_client.py` & `dstack-0.8.1/cli/dstack/api/hub/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,18 +139,24 @@
             run_name=run_name,
             start_time=start_time,
             end_time=end_time,
             descending=descending,
         )
 
     def list_run_artifact_files(
-        self, run_name: str, repo_id: Optional[str] = None
+        self,
+        run_name: str,
+        prefix: str = "",
+        recursive: bool = False,
+        repo_id: Optional[str] = None,
     ) -> List[Artifact]:
         # /{hub_name}/artifacts/list
-        return self._api_client.list_run_artifact_files(run_name=run_name)
+        return self._api_client.list_run_artifact_files(
+            run_name=run_name, prefix=prefix, recursive=recursive
+        )
 
     def download_run_artifact_files(
         self,
         run_name: str,
         output_dir: Optional[str],
         files_path: Optional[str] = None,
     ):
```

### Comparing `dstack-0.8/cli/dstack/api/hub/_storage.py` & `dstack-0.8.1/cli/dstack/api/hub/_storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/api/repos.py` & `dstack-0.8.1/cli/dstack/api/repos.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import os
 from typing import Optional
 
 import git
+import requests
 import yaml
 from git.exc import GitCommandError
 
+from dstack.core.error import DstackError
 from dstack.core.repo import (
     LocalRepo,
     RemoteRepo,
     RemoteRepoCredentials,
     RemoteRepoData,
     Repo,
     RepoProtocol,
 )
 from dstack.core.userconfig import RepoUserConfig
 from dstack.utils.common import PathLike
-from dstack.utils.ssh import get_host_config, make_ssh_command_for_git
+from dstack.utils.ssh import get_host_config, make_ssh_command_for_git, try_ssh_key_passphrase
 
 gh_config_path = os.path.expanduser("~/.config/gh/hosts.yml")
 default_ssh_key = os.path.expanduser("~/.ssh/id_rsa")
 
 
+class InvalidRepoCredentialsError(DstackError):
+    pass
+
+
 def get_local_repo_credentials(
     repo_data: RemoteRepoData,
     identity_file: Optional[PathLike] = None,
     oauth_token: Optional[str] = None,
     original_hostname: Optional[str] = None,
 ) -> RemoteRepoCredentials:
-    try:  # no auth
-        return test_remote_repo_credentials(repo_data, RepoProtocol.HTTPS)
-    except GitCommandError:
-        pass
+    url = repo_data.make_url(RepoProtocol.HTTPS)  # no auth
+    r = requests.get(f"{url}/info/refs?service=git-upload-pack")
+    if r.status_code == 200:
+        return RemoteRepoCredentials(
+            protocol=RepoProtocol.HTTPS, private_key=None, oauth_token=None
+        )
 
     if identity_file is not None:  # must fail if key is invalid
         try:  # user provided ssh key
             return test_remote_repo_credentials(
                 repo_data, RepoProtocol.SSH, identity_file=identity_file
             )
         except GitCommandError:
@@ -86,20 +94,23 @@
     oauth_token: Optional[str] = None,
 ) -> RemoteRepoCredentials:
     url = repo_data.make_url(protocol, oauth_token)
     if protocol == RepoProtocol.HTTPS:
         git.cmd.Git().ls_remote(url, env=dict(GIT_TERMINAL_PROMPT="0"))
         return RemoteRepoCredentials(protocol=protocol, oauth_token=oauth_token, private_key=None)
     elif protocol == RepoProtocol.SSH:
+        if not try_ssh_key_passphrase(identity_file):
+            raise InvalidRepoCredentialsError(
+                f"Repo SSH key must be passphrase-less: {identity_file}"
+            )
         with open(identity_file, "r") as f:
             private_key = f.read()
         git.cmd.Git().ls_remote(
             url, env=dict(GIT_SSH_COMMAND=make_ssh_command_for_git(identity_file))
         )
-        # todo: detect if key requires passphrase
         return RemoteRepoCredentials(protocol=protocol, private_key=private_key, oauth_token=None)
 
 
 def load_repo(user_config: RepoUserConfig) -> Repo:
     if user_config.repo_type == "remote":
         return RemoteRepo(repo_ref=user_config.repo_ref, local_repo_dir=os.getcwd())
     elif user_config.repo_type == "local":
```

### Comparing `dstack-0.8/cli/dstack/api/runs.py` & `dstack-0.8.1/cli/dstack/api/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/aws/__init__.py` & `dstack-0.8.1/cli/dstack/backend/aws/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,20 @@
             repo_id,
             run_name,
             start_time,
             end_time,
             descending,
         )
 
-    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
-        return base_artifacts.list_run_artifact_files(self._storage, repo_id, run_name)
+    def list_run_artifact_files(
+        self, repo_id: str, run_name: str, prefix: str, recursive: bool = False
+    ) -> List[Artifact]:
+        return base_artifacts.list_run_artifact_files(
+            self._storage, repo_id, run_name, prefix, recursive
+        )
 
     def download_run_artifact_files(
         self,
         repo_id: str,
         run_name: str,
         output_dir: Optional[PathLike],
         files_path: Optional[PathLike] = None,
```

### Comparing `dstack-0.8/cli/dstack/backend/aws/compute.py` & `dstack-0.8.1/cli/dstack/backend/aws/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/aws/config.py` & `dstack-0.8.1/cli/dstack/backend/aws/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/aws/logs.py` & `dstack-0.8.1/cli/dstack/backend/aws/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/aws/runners.py` & `dstack-0.8.1/cli/dstack/backend/aws/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/aws/secrets.py` & `dstack-0.8.1/cli/dstack/backend/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/aws/storage.py` & `dstack-0.8.1/cli/dstack/backend/aws/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,29 +39,40 @@
         if response["KeyCount"] == 0:
             return []
         object_keys = []
         for obj_metadata in response["Contents"]:
             object_keys.append(obj_metadata["Key"])
         return object_keys
 
-    def list_files(self, dirpath: str) -> List[StorageFile]:
-        prefix = dirpath
+    def list_files(self, prefix: str, recursive: bool) -> List[StorageFile]:
         paginator = self.s3_client.get_paginator("list_objects")
-        page_iterator = paginator.paginate(Bucket=self.bucket_name, Prefix=prefix)
+        delimiter = "/"
+        if recursive:
+            delimiter = ""
+        page_iterator = paginator.paginate(
+            Bucket=self.bucket_name, Prefix=prefix, Delimiter=delimiter
+        )
         files = []
         for page in page_iterator:
             for obj in page.get("Contents") or []:
                 if obj["Size"] > 0:
                     filepath = obj["Key"]
                     files.append(
                         StorageFile(
-                            filepath=removeprefix(filepath, prefix),
+                            filepath=filepath,
                             filesize_in_bytes=obj["Size"],
                         )
                     )
+            for obj in page.get("CommonPrefixes") or []:
+                filepath = obj["Prefix"]
+                files.append(
+                    StorageFile(
+                        filepath=filepath,
+                    )
+                )
         return files
 
     def download_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         downloader = transfer.S3Transfer(
             self.s3_client, transfer.TransferConfig(), transfer.OSUtils()
         )
         downloader.download_file(self.bucket_name, source_path, dest_path, callback=callback)
```

### Comparing `dstack-0.8/cli/dstack/backend/aws/utils.py` & `dstack-0.8.1/cli/dstack/backend/aws/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/__init__.py` & `dstack-0.8.1/cli/dstack/backend/base/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,29 +80,46 @@
         repo_id: str,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
         interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         pass
 
+    def get_run_head(
+        self,
+        repo_id: str,
+        run_name: str,
+        include_request_heads: bool = True,
+        interrupted_job_new_status: JobStatus = JobStatus.FAILED,
+    ) -> Optional[RunHead]:
+        run_heads_list = self.list_run_heads(
+            repo_id=repo_id,
+            run_name=run_name,
+            include_request_heads=include_request_heads,
+            interrupted_job_new_status=interrupted_job_new_status,
+        )
+        if len(run_heads_list) == 0:
+            return None
+        return run_heads_list[0]
+
     @abstractmethod
     def poll_logs(
         self,
         repo_id: str,
         run_name: str,
         start_time: datetime,
         end_time: Optional[datetime] = None,
         descending: bool = False,
     ) -> Generator[LogEvent, None, None]:
         pass
 
     @abstractmethod
-    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
-        # TODO: add a flag for non-recursive listing.
-        # Backends may implement this via list_run_artifact_files_and_folders()
+    def list_run_artifact_files(
+        self, repo_id: str, run_name: str, prefix: str, recursive: bool = False
+    ) -> List[Artifact]:
         pass
 
     @abstractmethod
     def download_run_artifact_files(
         self,
         repo_id: str,
         run_name: str,
```

### Comparing `dstack-0.8/cli/dstack/backend/base/artifacts.py` & `dstack-0.8.1/cli/dstack/backend/base/artifacts.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,29 +3,42 @@
 from typing import List, Optional
 
 from tqdm import tqdm
 
 from dstack.backend.base import jobs
 from dstack.backend.base.storage import Storage
 from dstack.core.artifact import Artifact
-from dstack.utils.common import PathLike
+from dstack.utils.common import PathLike, removeprefix
 
 
-def list_run_artifact_files(storage: Storage, repo_id: str, run_name: str) -> List[Artifact]:
+def list_run_artifact_files(
+    storage: Storage, repo_id: str, run_name: str, prefix: str, recursive: bool
+) -> List[Artifact]:
+    normalized_prefix = _normalize_path_prefix(prefix)
     jobs_list = jobs.list_jobs(storage, repo_id, run_name)
     artifacts = []
     for job in jobs_list:
-        job_artifacts_dir = _get_job_artifacts_dir(repo_id, job.job_id)
         if job.artifact_paths is None:
             continue
+        job_artifacts_dir = _get_job_artifacts_dir(repo_id, job.job_id)
         for artifact_path in job.artifact_paths:
             artifact_name = os.path.join(artifact_path, "")
-            artifact_path = artifact_name.lstrip(os.sep)
-            job_artifact_files_path = os.path.join(job_artifacts_dir, artifact_path)
-            artifact_files = storage.list_files(job_artifact_files_path)
+            artifact_path = os.path.join(_normalize_path_prefix(artifact_path), "")
+            artifact_full_path = os.path.join(job_artifacts_dir, artifact_path)
+            if artifact_path.startswith(normalized_prefix):
+                files_path = artifact_full_path
+            elif normalized_prefix.startswith(artifact_path):
+                files_path = os.path.join(job_artifacts_dir, normalized_prefix)
+            else:
+                continue
+            artifact_files = storage.list_files(files_path, recursive=recursive)
+            if len(artifact_files) == 0:
+                continue
+            for file in artifact_files:
+                file.filepath = removeprefix(file.filepath, artifact_full_path)
             artifact = Artifact(
                 job_id=job.job_id,
                 name=artifact_name,
                 path=artifact_path,
                 files=artifact_files,
             )
             artifacts.append(artifact)
@@ -105,13 +118,20 @@
                 source_path = filepath
                 dest_path = os.path.join(
                     artifacts_dir, artifact_path, Path(filepath).relative_to(local_path)
                 )
                 storage.upload_file(source_path, dest_path, callback)
 
 
+def _normalize_path_prefix(path: str) -> str:
+    normalized_path = str(Path(path)).lstrip(".").lstrip(os.sep)
+    if path.endswith("/"):
+        normalized_path += "/"
+    return normalized_path
+
+
 def _get_artifacts_dir(repo_id: str) -> str:
     return f"artifacts/{repo_id}/"
 
 
 def _get_job_artifacts_dir(repo_id: str, job_id: str) -> str:
     return f"{_get_artifacts_dir(repo_id)}{job_id}/"
```

### Comparing `dstack-0.8/cli/dstack/backend/base/compute.py` & `dstack-0.8.1/cli/dstack/backend/base/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/config.py` & `dstack-0.8.1/cli/dstack/backend/base/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/jobs.py` & `dstack-0.8.1/cli/dstack/backend/base/jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dstack.backend.base.storage import Storage
 from dstack.core.error import NoMatchingInstanceError
 from dstack.core.job import Job, JobErrorCode, JobHead, JobStatus
 from dstack.core.repo import RepoRef
 from dstack.core.request import RequestStatus
 from dstack.core.runners import Runner
 from dstack.utils.common import get_milliseconds_since_epoch
+from dstack.utils.escape import escape_head, unescape_head
 
 
 def create_job(
     storage: Storage,
     job: Job,
     create_head: bool = True,
 ):
@@ -57,84 +58,28 @@
     return jobs
 
 
 def list_job_head(storage: Storage, repo_id: str, job_id: str) -> Optional[JobHead]:
     job_head_key_prefix = _get_job_head_filename_prefix(repo_id, job_id)
     job_head_keys = storage.list_objects(job_head_key_prefix)
     for job_head_key in job_head_keys:
-        t = job_head_key[len(job_head_key_prefix) :].split(";")
-        (
-            provider_name,
-            hub_user_name,
-            submitted_at,
-            status_info,
-            artifacts,
-            app_names,
-            tag_name,
-        ) = tuple(t)
-        run_name, workflow_name, job_index = tuple(job_id.split(","))
-        status, error_code, container_exit_code = _parse_job_status_info(status_info)
-        return JobHead(
-            job_id=job_id,
-            repo_ref=RepoRef(repo_id=repo_id),
-            hub_user_name=hub_user_name,
-            run_name=run_name,
-            workflow_name=workflow_name or None,
-            provider_name=provider_name,
-            status=JobStatus(status),
-            error_code=JobErrorCode(error_code) if error_code else None,
-            container_exit_code=int(container_exit_code) if container_exit_code else None,
-            submitted_at=int(submitted_at),
-            artifact_paths=artifacts.split(",") if artifacts else None,
-            tag_name=tag_name or None,
-            app_names=app_names.split(",") or None,
-        )
+        return _parse_job_head_key(repo_id, job_head_key)
     return None
 
 
 def list_job_heads(
     storage: Storage,
     repo_id: str,
     run_name: Optional[str] = None,
 ) -> List[JobHead]:
     job_heads_keys_prefix = _get_job_heads_filenames_prefix(repo_id, run_name)
     job_heads_keys = storage.list_objects(job_heads_keys_prefix)
     job_heads = []
     for job_head_key in job_heads_keys:
-        t = job_head_key[len(_get_jobs_dir(repo_id)) :].split(";")
-        (
-            _,
-            job_id,
-            provider_name,
-            hub_user_name,
-            submitted_at,
-            status_info,
-            artifacts,
-            app_names,
-            tag_name,
-        ) = tuple(t)
-        run_name, workflow_name, job_index = tuple(job_id.split(","))
-        status, error_code, container_exit_code = _parse_job_status_info(status_info)
-        job_heads.append(
-            JobHead(
-                job_id=job_id,
-                repo_ref=RepoRef(repo_id=repo_id),
-                hub_user_name=hub_user_name,
-                run_name=run_name,
-                workflow_name=workflow_name or None,
-                provider_name=provider_name,
-                status=JobStatus(status),
-                error_code=JobErrorCode(error_code) if error_code else None,
-                container_exit_code=int(container_exit_code) if container_exit_code else None,
-                submitted_at=int(submitted_at),
-                artifact_paths=artifacts.split(",") if artifacts else None,
-                tag_name=tag_name or None,
-                app_names=app_names.split(",") or None,
-            )
-        )
+        job_heads.append(_parse_job_head_key(repo_id, job_head_key))
     return job_heads
 
 
 def delete_job_head(storage: Storage, repo_id: str, job_id: str):
     job_head_key_prefix = _get_job_head_filename_prefix(repo_id, job_id)
     job_head_keys = storage.list_objects(job_head_key_prefix)
     for job_head_key in job_head_keys:
@@ -149,21 +94,22 @@
 ):
     if job.status != JobStatus.SUBMITTED:
         raise Exception("Can't create a request for a job which status is not SUBMITTED")
 
     runner = None
     try:
         job.runner_id = uuid.uuid4().hex
-        update_job(storage, job)
         instance_type = compute.get_instance_type(job)
         if instance_type is None:
             job.status = JobStatus.FAILED
             job.error_code = JobErrorCode.NO_INSTANCE_MATCHING_REQUIREMENTS
             update_job(storage, job)
             raise NoMatchingInstanceError("No instance type matching requirements")
+        job.instance_type = instance_type.instance_name
+        update_job(storage, job)
         runner = Runner(
             runner_id=job.runner_id, request_id=None, resources=instance_type.resources, job=job
         )
         runners.create_runner(storage, runner)
         runner.request_id = compute.run_instance(job, instance_type)
         runners.update_runner(storage, runner)
     except NoCapacityError:
@@ -277,18 +223,56 @@
     key = (
         f"{prefix}l;"
         f"{job.job_id};"
         f"{job.provider_name};"
         f"{job.hub_user_name};"
         f"{job.submitted_at};"
         f"{job.status.value},{job.error_code.value if job.error_code else ''},{job.container_exit_code or ''};"
-        f"{','.join([a.artifact_path.replace('/', '_') for a in (job.artifact_specs or [])])};"
+        f"{','.join([escape_head(a.artifact_path) for a in (job.artifact_specs or [])])};"
         f"{','.join([a.app_name for a in (job.app_specs or [])])};"
-        f"{job.tag_name or ''}"
+        f"{job.tag_name or ''};"
+        f"{job.instance_type or ''}"
     )
     return key
 
 
+def _parse_job_head_key(repo_id: str, full_key: str) -> JobHead:
+    tokens = full_key[len(_get_jobs_dir(repo_id)) :].split(";")
+    tokens.extend([""] * (10 - len(tokens)))  # pad with empty tokens
+    (
+        _,
+        job_id,
+        provider_name,
+        hub_user_name,
+        submitted_at,
+        status_info,
+        artifacts,
+        app_names,
+        tag_name,
+        instance_type,
+    ) = tokens
+    run_name, workflow_name, job_index = tuple(job_id.split(","))
+    status, error_code, container_exit_code = _parse_job_status_info(status_info)
+    return JobHead(
+        job_id=job_id,
+        repo_ref=RepoRef(repo_id=repo_id),
+        hub_user_name=hub_user_name,
+        run_name=run_name,
+        workflow_name=workflow_name or None,
+        provider_name=provider_name,
+        status=JobStatus(status),
+        error_code=JobErrorCode(error_code) if error_code else None,
+        container_exit_code=int(container_exit_code) if container_exit_code else None,
+        submitted_at=int(submitted_at),
+        artifact_paths=[unescape_head(path) for path in artifacts.split(",")]
+        if artifacts
+        else None,
+        tag_name=tag_name or None,
+        app_names=app_names.split(",") or None,
+        instance_type=instance_type or None,
+    )
+
+
 def _parse_job_status_info(status_info: str) -> Tuple[str, str, str]:
     if len(status_info.split(",")) == 3:
         return status_info.split(",")
     return status_info, "", ""
```

### Comparing `dstack-0.8/cli/dstack/backend/base/logs.py` & `dstack-0.8.1/cli/dstack/backend/base/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/repos.py` & `dstack-0.8.1/cli/dstack/backend/base/repos.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     LocalRepoInfo,
     RemoteRepoCredentials,
     RemoteRepoInfo,
     RepoHead,
     RepoProtocol,
     RepoSpec,
 )
-from dstack.utils.escape import Escaper
+from dstack.utils.escape import unescape_head
 
 # repo_id, last_run_at, tags_count, repo_type, repo_info
 repo_head_re = re.compile(r"([^;]+);(\d+);(\d+);(remote|local);(.*)")
 
 
 def list_repo_heads(storage: Storage) -> List[RepoHead]:
     repo_heads_prefix = _get_repo_heads_prefix()
@@ -37,19 +37,15 @@
             repo_info = RemoteRepoInfo(
                 repo_host_name=repo_spec.repo_data.repo_host_name,
                 repo_port=repo_spec.repo_data.repo_port,
                 repo_user_name=repo_spec.repo_data.repo_user_name,
                 repo_name=repo_spec.repo_data.repo_name,
             )
         elif repo_spec.repo_data.repo_type == "local":
-            repo_info = LocalRepoInfo(
-                repo_dir=Escaper({"/": "."}, escape_char="~").unescape(
-                    repo_spec.repo_data.repo_dir
-                ),
-            )
+            repo_info = LocalRepoInfo(repo_dir=unescape_head(repo_spec.repo_data.repo_dir))
         repo_head = RepoHead(
             repo_id=repo_spec.repo_ref.repo_id,
             repo_info=repo_info,
         )
     repo_head.last_run_at = last_run_at
     _create_or_update_repo_head(storage, repo_head)
 
@@ -131,16 +127,14 @@
             repo_host_name=repo_host_name,
             repo_port=repo_port or None,
             repo_user_name=repo_user_name,
             repo_name=repo_name,
         )
     elif repo_type == "local":
         repo_dir = repo_info
-        repo_info = LocalRepoInfo(
-            repo_dir=Escaper({"/": "."}, escape_char="~").unescape(repo_dir),
-        )
+        repo_info = LocalRepoInfo(repo_dir=unescape_head(repo_dir))
     return RepoHead(
         repo_id=repo_id,
         repo_info=repo_info,
         last_run_at=int(last_run_at) if last_run_at else None,
         tags_count=int(tags_count),
     )
```

### Comparing `dstack-0.8/cli/dstack/backend/base/runners.py` & `dstack-0.8.1/cli/dstack/backend/base/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/runs.py` & `dstack-0.8.1/cli/dstack/backend/base/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/secrets.py` & `dstack-0.8.1/cli/dstack/backend/base/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/base/storage.py` & `dstack-0.8.1/cli/dstack/backend/base/storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         pass
 
     @abstractmethod
     def list_objects(self, keys_prefix: str) -> List[str]:
         pass
 
     @abstractmethod
-    def list_files(self, dirpath: str) -> List[StorageFile]:
+    def list_files(self, prefix: str, recursive: bool) -> List[StorageFile]:
         pass
 
     @abstractmethod
     def download_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         """
         `source_path` - storage path relative to the storage root.
         `dest_path` - local absolute path.
```

### Comparing `dstack-0.8/cli/dstack/backend/base/tags.py` & `dstack-0.8.1/cli/dstack/backend/base/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dstack.backend.base.storage import Storage
 from dstack.core.artifact import ArtifactHead, ArtifactSpec
 from dstack.core.error import BackendError
 from dstack.core.job import Job, JobStatus
 from dstack.core.repo import Repo
 from dstack.core.tag import TagHead
 from dstack.utils.common import get_milliseconds_since_epoch
+from dstack.utils.escape import unescape_head
 
 
 def get_tag_head(storage: Storage, repo_id: str, tag_name: str) -> Optional[TagHead]:
     tag_head_key_prefix = _get_tag_head_filename_prefix(repo_id, tag_name)
     tag_head_keys = storage.list_objects(keys_prefix=tag_head_key_prefix)
     if len(tag_head_keys) == 0:
         return None
@@ -225,21 +226,13 @@
     key = f"{prefix}l;"
     return key
 
 
 def _unserialize_artifact_heads(artifact_heads):
     return (
         [
-            ArtifactHead(job_id=a.split("=")[0], artifact_path=a.split("=")[1])
+            ArtifactHead(job_id=a.split("=")[0], artifact_path=unescape_head(a.split("=")[1]))
             for a in artifact_heads.split(":")
         ]
         if artifact_heads
         else None
     )
-
-
-def _serialize_artifact_heads(tag_head):
-    return (
-        ":".join([a.job_id + "=" + a.artifact_path for a in tag_head.artifact_heads])
-        if tag_head.artifact_heads
-        else ""
-    )
```

### Comparing `dstack-0.8/cli/dstack/backend/gcp/__init__.py` & `dstack-0.8.1/cli/dstack/backend/gcp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,20 @@
             repo_id=repo_id,
             run_name=run_name,
             start_time=start_time,
             end_time=end_time,
             descending=descending,
         )
 
-    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
-        return base_artifacts.list_run_artifact_files(self._storage, repo_id, run_name)
+    def list_run_artifact_files(
+        self, repo_id: str, run_name: str, prefix: str, recursive: bool = False
+    ) -> List[Artifact]:
+        return base_artifacts.list_run_artifact_files(
+            self._storage, repo_id, run_name, prefix, recursive
+        )
 
     def download_run_artifact_files(
         self,
         repo_id: str,
         run_name: str,
         output_dir: Optional[PathLike],
         files_path: Optional[PathLike] = None,
```

### Comparing `dstack-0.8/cli/dstack/backend/gcp/compute.py` & `dstack-0.8.1/cli/dstack/backend/gcp/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/gcp/config.py` & `dstack-0.8.1/cli/dstack/backend/gcp/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/gcp/logs.py` & `dstack-0.8.1/cli/dstack/backend/gcp/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/gcp/secrets.py` & `dstack-0.8.1/cli/dstack/backend/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/gcp/storage.py` & `dstack-0.8.1/cli/dstack/backend/gcp/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,24 +51,32 @@
 
     def list_objects(self, keys_prefix: str) -> List[str]:
         # TODO pagination
         blobs = self.bucket.client.list_blobs(self.bucket.name, prefix=keys_prefix)
         object_names = [blob.name for blob in blobs]
         return object_names
 
-    def list_files(self, dirpath: str) -> List[StorageFile]:
-        prefix = dirpath
-        blobs = self.bucket.client.list_blobs(self.bucket.name, prefix=prefix)
+    def list_files(self, prefix: str, recursive: bool) -> List[StorageFile]:
+        delimiter = "/"
+        if recursive:
+            delimiter = None
+        blobs = self.bucket.client.list_blobs(self.bucket.name, prefix=prefix, delimiter=delimiter)
         files = []
         for blob in blobs:
             file = StorageFile(
-                filepath=removeprefix(blob.name, prefix),
+                filepath=blob.name,
                 filesize_in_bytes=blob.size,
             )
             files.append(file)
+        for dirname in blobs.prefixes:
+            file = StorageFile(
+                filepath=dirname,
+                filesize_in_bytes=None,
+            )
+            files.append(file)
         return files
 
     def download_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         blob = self.bucket.blob(source_path)
         blob.download_to_filename(dest_path)
         callback(os.path.getsize(dest_path))
```

### Comparing `dstack-0.8/cli/dstack/backend/gcp/utils.py` & `dstack-0.8.1/cli/dstack/backend/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/local/__init__.py` & `dstack-0.8.1/cli/dstack/backend/local/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,20 @@
         end_time: Optional[datetime] = None,
         descending: bool = False,
     ) -> Generator[LogEvent, None, None]:
         return logs.poll_logs(
             self.backend_config, self._storage, repo_id, run_name, start_time, end_time, descending
         )
 
-    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
-        return base_artifacts.list_run_artifact_files(self._storage, repo_id, run_name)
+    def list_run_artifact_files(
+        self, repo_id: str, run_name: str, prefix: Optional[str], recursive: bool = False
+    ) -> List[Artifact]:
+        return base_artifacts.list_run_artifact_files(
+            self._storage, repo_id, run_name, prefix, recursive
+        )
 
     def download_run_artifact_files(
         self,
         repo_id: str,
         run_name: str,
         output_dir: Optional[PathLike],
         files_path: Optional[PathLike] = None,
```

### Comparing `dstack-0.8/cli/dstack/backend/local/compute.py` & `dstack-0.8.1/cli/dstack/backend/local/compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.backend_config = backend_config
 
     def get_request_head(self, job: Job, request_id: Optional[str]) -> RequestHead:
         return runners.get_request_head(job, request_id)
 
     def get_instance_type(self, job: Job) -> Optional[InstanceType]:
         resources = runners.check_runner_resources(self.backend_config, job.runner_id)
-        return InstanceType(instance_name="local_runner", resources=resources)
+        return InstanceType(instance_name="", resources=resources)
 
     def run_instance(self, job: Job, instance_type: InstanceType) -> str:
         return runners.start_runner_process(self.backend_config, job.runner_id)
 
     def terminate_instance(self, request_id: str):
         runners.stop_process(request_id)
```

### Comparing `dstack-0.8/cli/dstack/backend/local/config.py` & `dstack-0.8.1/cli/dstack/backend/local/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/local/logs.py` & `dstack-0.8.1/cli/dstack/backend/local/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/local/runners.py` & `dstack-0.8.1/cli/dstack/backend/local/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/local/secrets.py` & `dstack-0.8.1/cli/dstack/backend/local/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/backend/local/storage.py` & `dstack-0.8.1/cli/dstack/backend/local/storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,22 +44,44 @@
 
     def list_objects(self, keys_prefix: str) -> List[str]:
         return _list_objects(
             Root=self.root_path,
             Prefix=keys_prefix,
         )
 
-    def list_files(self, dirpath: str) -> List[StorageFile]:
-        full_dirpath = os.path.join(self.root_path, dirpath)
+    def list_files(self, prefix: str, recursive: bool) -> List[StorageFile]:
+        prefix_path = Path(prefix)
+        if prefix.endswith("/"):
+            dirpath = prefix
+        else:
+            dirpath = prefix_path.parent
+        full_dirpath = Path(self.root_path, dirpath)
+        if not full_dirpath.exists():
+            return []
         files = []
-        for dirpath, dirnames, filenames in os.walk(full_dirpath):
-            for filename in filenames:
-                full_filepath = os.path.join(dirpath, filename)
+        if recursive:
+            for dirpath, dirnames, filenames in os.walk(full_dirpath):
+                for filename in filenames:
+                    full_filepath = Path(dirpath, filename)
+                    filesize = os.stat(full_filepath, follow_symlinks=False).st_size
+                    filepath = str(full_filepath.relative_to(self.root_path))
+                    files.append(
+                        StorageFile(
+                            filepath=filepath,
+                            filesize_in_bytes=filesize,
+                        )
+                    )
+        else:
+            for entry in os.listdir(full_dirpath):
+                full_filepath = Path(full_dirpath, entry)
                 filesize = os.stat(full_filepath, follow_symlinks=False).st_size
-                filepath = removeprefix(full_filepath, full_dirpath)
+                filepath = str(full_filepath.relative_to(self.root_path))
+                if full_filepath.is_dir():
+                    filepath = os.path.join(filepath, "")
+                    filesize = None
                 files.append(
                     StorageFile(
                         filepath=filepath,
                         filesize_in_bytes=filesize,
                     )
                 )
         return files
```

### Comparing `dstack-0.8/cli/dstack/cli/commands/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/config/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/cp/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/cp/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/init/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/init/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from argparse import Namespace
 from pathlib import Path
 from typing import Optional
 
 import giturlparse
 from git.exc import InvalidGitRepositoryError
 
-from dstack.api.repos import get_local_repo_credentials
+from dstack.api.repos import InvalidRepoCredentialsError, get_local_repo_credentials
 from dstack.cli.commands import BasicCommand
 from dstack.cli.common import add_project_argument, console
 from dstack.cli.config import config, get_hub_client
+from dstack.cli.errors import CLIError
 from dstack.core.repo import LocalRepo, RemoteRepo
 from dstack.core.userconfig import RepoUserConfig
 
 
 class InitCommand(BasicCommand):
     NAME = "init"
     DESCRIPTION = "Authorize dstack to access the current Git repo"
@@ -47,20 +48,23 @@
         self._parser.add_argument("--local", action="store_true", help="Do not use git")
 
     def _command(self, args: Namespace):
         try:
             if args.local:  # force fallback to LocalRepo
                 raise InvalidGitRepositoryError()
             repo = RemoteRepo(local_repo_dir=Path.cwd())
-            repo_credentials = get_local_repo_credentials(
-                repo_data=repo.repo_data,
-                identity_file=args.git_identity_file,
-                oauth_token=args.gh_token,
-                original_hostname=giturlparse.parse(repo.repo_url).resource,
-            )
+            try:
+                repo_credentials = get_local_repo_credentials(
+                    repo_data=repo.repo_data,
+                    identity_file=args.git_identity_file,
+                    oauth_token=args.gh_token,
+                    original_hostname=giturlparse.parse(repo.repo_url).resource,
+                )
+            except InvalidRepoCredentialsError as e:
+                raise CLIError(e.message)
         except InvalidGitRepositoryError:
             console.print(
                 f"[gray58]No git remote is used, it could affect efficiency of source code transfer[/]"
             )
             repo = LocalRepo(repo_dir=Path.cwd())
             repo_credentials = None
```

### Comparing `dstack-0.8/cli/dstack/cli/commands/logs/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/ls/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/ls/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,17 +33,14 @@
             nargs="?",
             default="",
         )
 
         self._parser.add_argument(
             "-r", "--recursive", help="Show all files recursively", action="store_true"
         )
-        self._parser.add_argument(
-            "-t", "--total", help="Show total folder size", action="store_true"
-        )
 
     @check_init
     def _command(self, args: Namespace):
         table = Table(box=None)
         table.add_column("ARTIFACT", style="bold", no_wrap=True)
         table.add_column("FILE")
         table.add_column("SIZE", style="dark_sea_green4")
@@ -51,62 +48,22 @@
         hub_client = get_hub_client(project_name=args.project)
         try:
             run_name, _ = get_tagged_run_name(hub_client, args.run_name_or_tag_name)
         except (TagNotFoundError, RunNotFoundError):
             console.print(f"Cannot find the run or tag '{args.run_name_or_tag_name}'")
             exit(1)
 
-        artifacts = hub_client.list_run_artifact_files(run_name)
+        artifacts = hub_client.list_run_artifact_files(
+            run_name, prefix=args.prefix, recursive=args.recursive
+        )
+        artifact = sorted(artifacts, key=lambda a: a.path)
         for artifact in artifacts:
-            artifact.files = sorted(
-                [
-                    f
-                    for f in artifact.files
-                    if str(Path(artifact.name, f.filepath)).startswith(args.prefix)
-                ],
-                key=lambda f: f.filepath,
-            )
-
-        if args.recursive:
-            for artifact in artifacts:
-                for i, file in enumerate(artifact.files):
-                    table.add_row(
-                        artifact.name if i == 0 else "",
-                        file.filepath,
-                        sizeof_fmt(file.filesize_in_bytes),
-                    )
-        else:
-            entries = {}
-            for artifact in artifacts:
-                if entries.get(artifact.name) is None:
-                    entries[artifact.name] = {}
-                for i, file in enumerate(artifact.files):
-                    entry_name = _get_entry_name(file.filepath, args.prefix)
-                    if entries[artifact.name].get(entry_name) is None:
-                        entries[artifact.name][entry_name] = {"size": 0, "backends": set()}
-                    entries[artifact.name][entry_name]["size"] += file.filesize_in_bytes
-
-            for artifact_name, entry_map in entries.items():
-                first_entry = True
-                for entry_name, entry_dict in entry_map.items():
-                    table.add_row(
-                        artifact_name if first_entry else "",
-                        entry_name,
-                        sizeof_fmt(entry_dict["size"])
-                        if not entry_name.endswith("/") or args.total
-                        else "",
-                    )
-                    first_entry = False
+            files = sorted(artifact.files, key=lambda f: f.filepath)
+            for i, file in enumerate(files):
+                table.add_row(
+                    artifact.name if i == 0 else "",
+                    file.filepath,
+                    sizeof_fmt(file.filesize_in_bytes)
+                    if file.filesize_in_bytes is not None
+                    else "",
+                )
         console.print(table)
-
-
-def _get_entry_name(filepath: str, prefix: str) -> str:
-    if prefix == "":
-        prefix_parts_num = 1
-    else:
-        prefix_parts_num = len(Path(prefix).parts)
-
-    path_parts = Path(filepath).parts
-    entry_name = str(Path(*path_parts[:prefix_parts_num]))
-    if len(path_parts) > prefix_parts_num:
-        entry_name += "/"
-    return entry_name
```

### Comparing `dstack-0.8/cli/dstack/cli/commands/prune/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/prune/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/ps/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/ps/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/rm/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/rm/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/run/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/run/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             exit(1)
         try:
             hub_client = get_hub_client(project_name=args.project)
             if (
                 hub_client.repo.repo_data.repo_type != "local"
                 and not hub_client.get_repo_credentials()
             ):
-                raise RepoNotInitializedError("No credentials", project_name=hub_client.project)
+                raise RepoNotInitializedError("No credentials", project_name=args.project)
 
             if not config.repo_user_config.ssh_key_path:
                 ssh_pub_key = None
             else:
                 ssh_pub_key = _read_ssh_key_pub(config.repo_user_config.ssh_key_path)
 
             try:
@@ -285,20 +285,21 @@
         time.sleep(rate)
 
 
 def ask_on_interrupt(hub_client: HubClient, run_name: str):
     global interrupt_count
     if interrupt_count == 0:
         try:
-            if Confirm.ask(f"\n[red]Stop the run '{run_name}'?[/]"):
+            console.print("\n")
+            if Confirm.ask(f"[red]Stop the run '{run_name}'?[/]"):
                 interrupt_count += 1
                 hub_client.stop_jobs(run_name, abort=False)
-                console.print("[grey58]Stopping... To abort press Ctrl+C[/]", end="")
+                console.print("\n[grey58]Stopping... To abort press Ctrl+C[/]", end="")
             else:
-                console.print("[grey58]Detaching...[/]")
+                console.print("\n[grey58]Detaching...[/]")
                 console.print("[grey58]OK[/]")
                 exit(0)
             return
         except KeyboardInterrupt:
             interrupt_count += 1
     if interrupt_count > 0:
         console.print("\n[grey58]Aborting...[/]")
```

### Comparing `dstack-0.8/cli/dstack/cli/commands/run/ssh_tunnel.py` & `dstack-0.8.1/cli/dstack/cli/commands/run/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/secrets/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/start/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/start/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/stop/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/stop/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/commands/tags/__init__.py` & `dstack-0.8.1/cli/dstack/cli/commands/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/common.py` & `dstack-0.8.1/cli/dstack/cli/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,34 @@
 
 
 def generate_runs_table(runs: List[RunHead], verbose: bool = False) -> Table:
     table = Table(box=None)
     table.add_column("RUN", style="bold", no_wrap=True)
     table.add_column("WORKFLOW", style="grey58", max_width=16)
     table.add_column("SUBMITTED", style="grey58", no_wrap=True)
-    table.add_column("OWNER", style="grey58", no_wrap=True, max_width=16)
+    table.add_column("USER", style="grey58", no_wrap=True, max_width=16)
     table.add_column("STATUS", no_wrap=True)
-    table.add_column("TAG", style="bold yellow", no_wrap=True)
+    table.add_column("INSTANCE", no_wrap=True)
     if verbose:
+        table.add_column("TAG", style="bold yellow", no_wrap=True)
         table.add_column("ERROR", no_wrap=True)
 
     for run in runs:
         submitted_at = pretty_date(round(run.submitted_at / 1000))
         row = [
             _status_color(run, run.run_name, True, False),
             _status_color(run, run.workflow_name or run.provider_name, False, False),
             _status_color(run, submitted_at, False, False),
             _status_color(run, run.hub_user_name or "", False, False),
             _pretty_print_status(run),
-            _status_color(run, run.tag_name or "", False, False),
+            _pretty_print_instance_type(run),
         ]
         if verbose:
             row += [
+                _status_color(run, run.tag_name or "", False, False),
                 _pretty_print_error_code(run),
             ]
         table.add_row(*row)
     return table
 
 
 _status_colors = {
@@ -94,14 +96,23 @@
             if job_head.error_code == JobErrorCode.CONTAINER_EXITED_WITH_ERROR:
                 return f"[red]Exit code: {job_head.container_exit_code}[/]"
             else:
                 return f"[red]{job_head.error_code.pretty_repr()}[/]"
     return ""
 
 
+def _pretty_print_instance_type(run: RunHead) -> str:
+    instances = [
+        _status_color(run, job.instance_type, False, False)
+        for job in run.job_heads
+        if job.instance_type
+    ] or [_status_color(run, "-", False, False)]
+    return "\n".join(instances)
+
+
 def check_init(func):
     def decorator(*args, **kwargs):
         try:
             func(*args, **kwargs)
         except RepoNotInitializedError as e:
             command = "dstack init"
             if e.project_name is not None:
```

### Comparing `dstack-0.8/cli/dstack/cli/config.py` & `dstack-0.8.1/cli/dstack/cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,11 +147,20 @@
             )
     else:
         project_config = cli_config_manager.get_default_project_config()
         if project_config is None:
             raise CLIError(
                 f"No default project is configured. Call `dstack start` or `dstack config`."
             )
-    repo = load_repo(config.repo_user_config)
+    repo_config = _read_repo_config_or_error_with_project_name(project_name)
+    repo = load_repo(repo_config)
     hub_client_config = HubClientConfig(url=project_config.url, token=project_config.token)
     hub_client = HubClient(config=hub_client_config, project=project_config.name, repo=repo)
     return hub_client
+
+
+def _read_repo_config_or_error_with_project_name(project_name: Optional[str]) -> RepoUserConfig:
+    try:
+        return config.repo_user_config
+    except RepoNotInitializedError as e:
+        e.project_name = project_name
+        raise e
```

### Comparing `dstack-0.8/cli/dstack/cli/handlers.py` & `dstack-0.8.1/cli/dstack/cli/handlers.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/main.py` & `dstack-0.8.1/cli/dstack/cli/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/cli/updates.py` & `dstack-0.8.1/cli/dstack/cli/updates.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/app.py` & `dstack-0.8.1/cli/dstack/core/app.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/error.py` & `dstack-0.8.1/cli/dstack/core/error.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/job.py` & `dstack-0.8.1/cli/dstack/core/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     status: JobStatus
     error_code: Optional[JobErrorCode]
     container_exit_code: Optional[int]
     submitted_at: int
     artifact_paths: Optional[List[str]]
     tag_name: Optional[str]
     app_names: Optional[List[str]]
+    instance_type: Optional[str]
 
     def get_id(self) -> Optional[str]:
         return self.job_id
 
     def set_id(self, job_id: Optional[str]):
         self.job_id = job_id
 
@@ -181,14 +182,15 @@
     submitted_at: int
     submission_num: int = 1
     image_name: str
     registry_auth: Optional[RegistryAuth]
     commands: Optional[List[str]]
     entrypoint: Optional[List[str]]
     env: Optional[Dict[str, str]]
+    home_dir: Optional[str]
     working_dir: Optional[str]
     artifact_specs: Optional[List[ArtifactSpec]]
     cache_specs: List[CacheSpec]
     port_count: Optional[int]
     ports: Optional[List[int]]
     host_name: Optional[str]
     requirements: Optional[Requirements]
@@ -247,14 +249,15 @@
             "submitted_at": self.submitted_at,
             "submission_num": self.submission_num,
             "image_name": self.image_name,
             "registry_auth": self.registry_auth.serialize() if self.registry_auth else {},
             "commands": self.commands or [],
             "entrypoint": self.entrypoint,
             "env": self.env or {},
+            "home_dir": self.home_dir or "",
             "working_dir": self.working_dir or "",
             "artifacts": artifacts,
             "cache": [item.dict() for item in self.cache_specs],
             "port_count": self.port_count if self.port_count else 0,
             "ports": [str(port) for port in self.ports] if self.ports else [],
             "host_name": self.host_name or "",
             "requirements": self.requirements.serialize() if self.requirements else {},
@@ -272,14 +275,15 @@
             if self.app_specs
             else [],
             "runner_id": self.runner_id or "",
             "request_id": self.request_id or "",
             "tag_name": self.tag_name or "",
             "ssh_key_pub": self.ssh_key_pub or "",
             "repo_code_filename": self.repo_code_filename,
+            "instance_type": self.instance_type,
         }
         if isinstance(self.repo_data, RemoteRepoData):
             job_data["repo_host_name"] = self.repo_data.repo_host_name
             job_data["repo_port"] = self.repo_data.repo_port or 0
             job_data["repo_user_name"] = self.repo_data.repo_user_name
             job_data["repo_name"] = self.repo_data.repo_name
             job_data["repo_branch"] = self.repo_data.repo_branch or ""
@@ -388,28 +392,30 @@
             submitted_at=job_data["submitted_at"],
             submission_num=job_data.get("submission_num") or 1,
             image_name=job_data["image_name"],
             registry_auth=RegistryAuth(**job_data.get("registry_auth", {})),
             commands=job_data.get("commands") or None,
             entrypoint=job_data.get("entrypoint") or None,
             env=job_data["env"] or None,
+            home_dir=job_data.get("home_dir") or None,
             working_dir=job_data.get("working_dir") or None,
             artifact_specs=artifact_specs,
             cache_specs=[CacheSpec(**item) for item in job_data.get("cache", [])],
             port_count=job_data.get("port_count") or None,
             ports=job_data.get("ports") or None,
             host_name=job_data.get("host_name") or None,
             requirements=requirements,
             dep_specs=dep_specs or None,
             master_job=master_job,
             app_specs=app_specs,
             runner_id=job_data.get("runner_id") or None,
             request_id=job_data.get("request_id") or None,
             tag_name=job_data.get("tag_name") or None,
             ssh_key_pub=job_data.get("ssh_key_pub") or None,
+            instance_type=job_data.get("instance_type") or None,
         )
         return job
 
     @property
     def repo(self) -> Repo:
         if isinstance(self.repo_data, RemoteRepoData):
             return RemoteRepo(repo_ref=self.repo_ref, repo_data=self.repo_data)
```

### Comparing `dstack-0.8/cli/dstack/core/repo/base.py` & `dstack-0.8.1/cli/dstack/core/repo/base.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/repo/head.py` & `dstack-0.8.1/cli/dstack/core/repo/head.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/repo/local.py` & `dstack-0.8.1/cli/dstack/core/repo/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Any, BinaryIO, Dict, List, Optional
 
 from typing_extensions import Literal
 
 from dstack.core.repo.base import Repo, RepoData, RepoInfo, RepoRef
 from dstack.utils.common import PathLike
-from dstack.utils.escape import Escaper
+from dstack.utils.escape import escape_head
 from dstack.utils.hash import get_sha256, slugify
 from dstack.utils.workflows import load_workflows
 
 
 class LocalRepoData(RepoData):
     repo_type: Literal["local"] = "local"
     repo_dir: str
@@ -25,15 +25,15 @@
 
 class LocalRepoInfo(RepoInfo):
     repo_type: Literal["local"] = "local"
     repo_dir: str
 
     @property
     def head_key(self) -> str:
-        repo_dir = Escaper({"/": "."}, escape_char="~").escape(self.repo_dir)
+        repo_dir = escape_head(self.repo_dir)
         return f"{self.repo_type};{repo_dir}"
 
 
 class LocalRepo(Repo):
     """Represents local folder"""
 
     repo_data: LocalRepoData
```

### Comparing `dstack-0.8/cli/dstack/core/repo/remote.py` & `dstack-0.8.1/cli/dstack/core/repo/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,17 +107,19 @@
             tracking_branch = repo.active_branch.tracking_branch()
             if tracking_branch is None:
                 raise ValueError("No remote branch is configured")
             self.repo_url = repo.remote(tracking_branch.remote_name).url
             repo_data = RemoteRepoData.from_url(self.repo_url, parse_ssh_config=True)
             repo_data.repo_branch = tracking_branch.remote_head
             repo_data.repo_hash = tracking_branch.commit.hexsha
-            repo_data.repo_diff = repo.git.diff(
-                repo_data.repo_hash
-            )  # TODO: Doesn't support unstaged changes
+            repo_data.repo_diff = repo.git.diff(repo_data.repo_hash)
+            diffs = [repo_data.repo_diff]
+            for filename in repo.untracked_files:
+                diffs.append(_add_patch(local_repo_dir, filename))
+            repo_data.repo_diff = "\n".join([d for d in diffs if d])
         elif self.repo_url is not None:
             repo_data = RemoteRepoData.from_url(self.repo_url, parse_ssh_config=True)
         elif repo_data is None:
             raise ValueError("No remote repo data provided")
 
         if repo_ref is None:
             repo_ref = RepoRef(repo_id=slugify(repo_data.repo_name, repo_data.path("/")))
@@ -153,7 +155,13 @@
     git.Repo.clone_from(
         url=repo_data.make_url(repo_credentials.protocol, repo_credentials.oauth_token),
         to_path=dst,
         env=env,
         **kwargs,
     )
     # todo checkout branch/hash
+
+
+def _add_patch(repo_dir: PathLike, filename: str) -> str:
+    return git.cmd.Git(repo_dir).diff(
+        "/dev/null", filename, no_index=True, binary=True, with_exceptions=False
+    )
```

### Comparing `dstack-0.8/cli/dstack/core/repo/spec.py` & `dstack-0.8.1/cli/dstack/core/repo/spec.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/request.py` & `dstack-0.8.1/cli/dstack/core/request.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/run.py` & `dstack-0.8.1/cli/dstack/core/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/runners.py` & `dstack-0.8.1/cli/dstack/core/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/core/tag.py` & `dstack-0.8.1/cli/dstack/core/tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from dstack.core.artifact import ArtifactHead
+from dstack.utils.escape import escape_head
 
 
 class TagHead(BaseModel):
     repo_id: str
     tag_name: str
     run_name: str
     workflow_name: Optional[str]
     provider_name: Optional[str]
     hub_user_name: str
     created_at: int
     artifact_heads: Optional[List[ArtifactHead]]
 
     def serialize_artifact_heads(self):
         return (
-            ":".join(
-                [a.job_id + "=" + a.artifact_path.replace("/", "_") for a in self.artifact_heads]
-            )
+            ":".join([a.job_id + "=" + escape_head(a.artifact_path) for a in self.artifact_heads])
             if self.artifact_heads
             else ""
         )
 
     def key(self, add_prefix=True) -> str:
         prefix = ""
         if add_prefix:
```

### Comparing `dstack-0.8/cli/dstack/hub/background/tasks/resubmit_jobs.py` & `dstack-0.8.1/cli/dstack/hub/background/tasks/resubmit_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/db/__init__.py` & `dstack-0.8.1/cli/dstack/hub/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/db/models.py` & `dstack-0.8.1/cli/dstack/hub/db/models.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/main.py` & `dstack-0.8.1/cli/dstack/hub/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/migration/env.py` & `dstack-0.8.1/cli/dstack/hub/migration/env.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/migration/versions/3b900659c822_.py` & `dstack-0.8.1/cli/dstack/hub/migration/versions/3b900659c822_.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/models/__init__.py` & `dstack-0.8.1/cli/dstack/hub/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -168,14 +168,25 @@
 
 class RunsList(BaseModel):
     repo_id: str
     run_name: Optional[str]
     include_request_heads: Optional[bool]
 
 
+class RunsStop(BaseModel):
+    repo_id: str
+    run_names: List[str]
+    abort: bool
+
+
+class RunsDelete(BaseModel):
+    repo_id: str
+    run_names: List[str]
+
+
 class JobHeadList(BaseModel):
     repo_id: str
     run_name: Optional[str]
 
 
 class JobsGet(BaseModel):
     repo_id: str
@@ -186,14 +197,16 @@
     repo_id: str
     run_name: str
 
 
 class ArtifactsList(BaseModel):
     repo_id: str
     run_name: str
+    prefix: str
+    recursive: bool
 
 
 class SecretAddUpdate(BaseModel):
     repo_id: str
     secret: Secret
```

### Comparing `dstack-0.8/cli/dstack/hub/repository/projects.py` & `dstack-0.8.1/cli/dstack/hub/repository/projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/repository/users.py` & `dstack-0.8.1/cli/dstack/hub/repository/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/artifacts.py` & `dstack-0.8.1/cli/dstack/hub/routers/artifacts.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,13 @@
 )
 
 
 @router.post("/{project_name}/artifacts/list")
 async def list_artifacts(project_name: str, body: ArtifactsList) -> List[Artifact]:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    return backend.list_run_artifact_files(repo_id=body.repo_id, run_name=body.run_name)
+    return backend.list_run_artifact_files(
+        repo_id=body.repo_id,
+        run_name=body.run_name,
+        prefix=body.prefix,
+        recursive=body.recursive,
+    )
```

### Comparing `dstack-0.8/cli/dstack/hub/routers/cache.py` & `dstack-0.8.1/cli/dstack/hub/routers/cache.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/jobs.py` & `dstack-0.8.1/cli/dstack/hub/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/link.py` & `dstack-0.8.1/cli/dstack/hub/routers/link.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/logs.py` & `dstack-0.8.1/cli/dstack/hub/routers/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/projects.py` & `dstack-0.8.1/cli/dstack/hub/routers/projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/repos.py` & `dstack-0.8.1/cli/dstack/hub/routers/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/runners.py` & `dstack-0.8.1/cli/dstack/hub/routers/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/secrets.py` & `dstack-0.8.1/cli/dstack/hub/routers/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/storage.py` & `dstack-0.8.1/cli/dstack/hub/routers/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/tags.py` & `dstack-0.8.1/cli/dstack/hub/routers/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     backend.delete_tag_head(repo_ref.repo_id, tag_head=tag)
 
 
 @router.post("/{project_name}/tags/add/run")
 async def add_tag_from_run(project_name: str, body: AddTagRun):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.add_tag_from_run(
+    backend.add_tag_from_run(  # todo pass error to CLI if tag already exists
         body.repo_id, tag_name=body.tag_name, run_name=body.run_name, run_jobs=body.run_jobs
     )
 
 
 @router.post("/{project_name}/tags/add/path")
 async def add_tag_from_path(project_name: str, body: AddTagPath):
     # project = await get_project(project_name=project_name)
```

### Comparing `dstack-0.8/cli/dstack/hub/routers/users.py` & `dstack-0.8.1/cli/dstack/hub/routers/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/util.py` & `dstack-0.8.1/cli/dstack/hub/routers/util.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/routers/workflows.py` & `dstack-0.8.1/cli/dstack/hub/routers/workflows.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from fastapi import APIRouter, Depends
 from fastapi.security import HTTPBearer
 
-from dstack.core.repo import RepoSpec
+from dstack.core.repo import RepoRef
+from dstack.hub.db.models import User
 from dstack.hub.routers.cache import get_backend
 from dstack.hub.routers.util import get_project
-from dstack.hub.security.permissions import ProjectMember
+from dstack.hub.security.permissions import Authenticated, ProjectMember
 
 router = APIRouter(
     prefix="/api/project", tags=["workflows"], dependencies=[Depends(ProjectMember())]
 )
 
 security = HTTPBearer()
 
 
 @router.post("/{project_name}/workflows/{workflow_name}/cache/delete")
-async def delete_workflow_cache(project_name: str, workflow_name: str, repo_spec: RepoSpec):
+async def delete_workflow_cache(
+    project_name: str, workflow_name: str, repo_ref: RepoRef, user: User = Depends(Authenticated())
+):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.delete_workflow_cache(repo_id, hub_user_name, workflow_name=workflow_name)
+    backend.delete_workflow_cache(repo_ref.repo_id, user.name, workflow_name=workflow_name)
```

### Comparing `dstack-0.8/cli/dstack/hub/security/permissions.py` & `dstack-0.8.1/cli/dstack/hub/security/permissions.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/services/backends/__init__.py` & `dstack-0.8.1/cli/dstack/hub/services/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/services/backends/aws.py` & `dstack-0.8.1/cli/dstack/hub/services/backends/aws.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/services/backends/base.py` & `dstack-0.8.1/cli/dstack/hub/services/backends/base.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/services/backends/gcp.py` & `dstack-0.8.1/cli/dstack/hub/services/backends/gcp.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/services/backends/local.py` & `dstack-0.8.1/cli/dstack/hub/services/backends/local.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/hub/utils/logging.py` & `dstack-0.8.1/cli/dstack/hub/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/providers/__init__.py` & `dstack-0.8.1/cli/dstack/providers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,14 +252,15 @@
                 status=JobStatus.SUBMITTED,
                 submitted_at=get_milliseconds_since_epoch(),
                 image_name=job_spec.image_name,
                 registry_auth=job_spec.registry_auth,
                 commands=job_spec.commands,
                 entrypoint=job_spec.entrypoint,
                 env=job_spec.env,
+                home_dir=self.home_dir,
                 working_dir=job_spec.working_dir,
                 artifact_specs=job_spec.artifact_specs,
                 cache_specs=self.cache_specs,
                 port_count=job_spec.port_count,
                 ports=None,
                 host_name=None,
                 requirements=job_spec.requirements,
```

### Comparing `dstack-0.8/cli/dstack/providers/_torchrun/main.py` & `dstack-0.8.1/cli/dstack/providers/_torchrun/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
-from dstack.backend.base import Backend
+import dstack.api.hub as hub
 from dstack.core.job import GpusRequirements, JobSpec, Requirements
 from dstack.providers import Provider
 
 
 class TorchrunProvider(Provider):
     def __init__(self):
         super().__init__("torchrun")
@@ -20,22 +20,22 @@
         self.working_dir = None
         self.nodes = None
         self.resources = None
         self.args = None
 
     def load(
         self,
-        backend: Backend,
+        hub_client: "hub.HubClient",
         args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
+        super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.script = self.provider_data.get("script") or self.provider_data.get("file")
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.nodes = self.provider_data.get("nodes") or 1
```

### Comparing `dstack-0.8/cli/dstack/providers/bash/main.py` & `dstack-0.8.1/cli/dstack/providers/bash/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
+import dstack.api.hub as hub
 from dstack import version
-from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class BashProvider(Provider):
     def __init__(self):
@@ -22,22 +22,22 @@
         self.ports = None
         self.commands = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
-        backend: Backend,
+        hub_client: "hub.HubClient",
         args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
+        super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.python = self._safe_python_version("python")
         self.commands = self._get_list_data("commands")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.ports = self.provider_data.get("ports")
         self.resources = self._resources()
```

### Comparing `dstack-0.8/cli/dstack/providers/code/main.py` & `dstack-0.8.1/cli/dstack/providers/code/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
+import dstack.api.hub as hub
 from dstack import version
-from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class CodeProvider(Provider):
     def __init__(self):
@@ -24,22 +24,22 @@
         self.working_dir = None
         self.resources = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
-        backend: Backend,
+        hub_client: "hub.HubClient",
         args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
+        super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.ports = self.provider_data.get("ports")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version") or "1.74.3"
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
```

### Comparing `dstack-0.8/cli/dstack/providers/docker/main.py` & `dstack-0.8.1/cli/dstack/providers/docker/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
-from dstack.backend.base import Backend
+import dstack.api.hub as hub
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class DockerProvider(Provider):
     def __init__(self):
@@ -20,30 +20,31 @@
         self.env = None
         self.working_dir = None
         self.ports = None
         self.resources = None
 
     def load(
         self,
-        backend: Backend,
+        hub_client: "hub.HubClient",
         args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
+        super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.image_name = self.provider_data["image"]
         self.registry_auth = self.provider_data.get("registry_auth")
         self.commands = self._get_list_data("commands")
         self.entrypoint = self._get_entrypoint()
         if self.commands and self.entrypoint is None:  # commands not empty
             self.entrypoint = ["/bin/sh", "-i", "-c"]
         self.artifact_specs = self._artifact_specs()
         self.env = self.provider_data.get("env")
+        self.home_dir = self.provider_data.get("home_dir")
         self.working_dir = self.provider_data.get("working_dir")
         self.ports = self.provider_data.get("ports")
         self.resources = self._resources()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
         parser = ArgumentParser(
             prog="dstack run " + (workflow_name or self.provider_name),
```

### Comparing `dstack-0.8/cli/dstack/providers/lab/main.py` & `dstack-0.8.1/cli/dstack/providers/lab/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
+import dstack.api.hub as hub
 from dstack import version
-from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class LabProvider(Provider):
     def __init__(self):
@@ -22,22 +22,22 @@
         self.working_dir = None
         self.resources = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
-        backend: Backend,
+        hub_client: "hub.HubClient",
         args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
+        super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
```

### Comparing `dstack-0.8/cli/dstack/providers/notebook/main.py` & `dstack-0.8.1/cli/dstack/providers/notebook/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
+import dstack.api.hub as hub
 from dstack import version
-from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
 from dstack.providers import Provider
 
 
 class NotebookProvider(Provider):
     def __init__(self):
@@ -22,22 +22,22 @@
         self.working_dir = None
         self.resources = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
-        backend: Backend,
+        hub_client: "hub.HubClient",
         args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
+        super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
```

### Comparing `dstack-0.8/cli/dstack/utils/common.py` & `dstack-0.8.1/cli/dstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/utils/escape.py` & `dstack-0.8.1/cli/dstack/utils/escape.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from typing import Dict
 
 
+class UnescapeError(Exception):
+    pass
+
+
 class Escaper:
     """
     Generic escaping for strings.
 
     `escape_char` is doubled
     Key from `chars` is replaced with `escape_char` and corresponding value
 
     >>> esc = Escaper({"/": "."}, escape_char="$")
     >>> esc.escape("foo/bar")
-    "foo$.bar"
+    'foo$.bar'
     >>> esc.escape("foo/$bar")
-    "foo$.$$bar"
+    'foo$.$$bar'
+    >>> esc.unescape("foo$/bar")
+    Traceback (most recent call last):
+    escape.UnescapeError: ('Unknown escape sequence', '$/')
     """
 
     def __init__(self, chars: Dict[str, str], escape_char: str):
         assert escape_char not in chars.keys()
         assert escape_char not in chars.values()
         assert len(chars) == len(set(chars.values()))
         self.chars = chars
@@ -36,14 +43,25 @@
         while start < len(value):
             esc = value.find(self.escape_char, start)
             if esc == -1:
                 parts.append(value[start:])
                 break
             parts.append(value[start:esc])
             if esc + 1 >= len(value):
-                raise ValueError("Unexpected EOL")
+                raise UnescapeError("Unexpected EOL")
             elif value[esc + 1] not in inv:
-                raise ValueError(f"Unknown escape sequence: {value[esc:esc + 2]}")
+                raise UnescapeError(f"Unknown escape sequence", value[esc : esc + 2])
             else:
                 parts.append(inv[value[esc + 1]])
             start = esc + 2
         return "".join(parts)
+
+
+_head_escaper = Escaper(chars={"/": "."}, escape_char="~")
+
+
+def escape_head(v: str) -> str:
+    return _head_escaper.escape(v)
+
+
+def unescape_head(v: str) -> str:
+    return _head_escaper.unescape(v)
```

### Comparing `dstack-0.8/cli/dstack/utils/hash.py` & `dstack-0.8.1/cli/dstack/utils/hash.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/utils/interpolator.py` & `dstack-0.8.1/cli/dstack/utils/interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/utils/random_names.py` & `dstack-0.8.1/cli/dstack/utils/random_names.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack/utils/workflows.py` & `dstack-0.8.1/cli/dstack/utils/workflows.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/dstack.egg-info/PKG-INFO` & `dstack-0.8.1/cli/dstack.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.8
+Version: 0.8.1
 Summary: The easiest way to define ML workflows and run them on any cloud platform
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
@@ -15,24 +15,24 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <div align="center">
 <h1 align="center">
   <a target="_blank" href="https://dstack.ai">
-    <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/logo.svg" width="400px"/>
+    <img alt="dstack" src="https://raw.githubusercontent.com/dstackai/dstack/master/docs/assets/images/dstack-logo.svg" width="400px"/>
   </a>
 </h1>
 
 <h4 align="center">
 ML workflows as code
 </h4>
 
 <p align="center">
-The easiest way to define ML workflows and run them on any cloud platform 
+The easiest way to run ML workflows on any cloud platform 
 </p>
 
 [![Slack](https://img.shields.io/badge/slack-join%20chat-blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
 
 <p align="center">
 <a href="https://dstack.ai/docs/quick-start" target="_blank"><b>Quick start</b></a> • 
 <a href="https://dstack.ai/docs" target="_blank"><b>Docs</b></a> • 
@@ -49,122 +49,145 @@
 
 `dstack` makes it very easy to define ML workflows
 and run them on any cloud platform. It provisions infrastructure,
 manages data, and monitors usage for you.
 
 Ideal for processing data, training models, running apps, and any other ML development tasks.
 
-## Install the CLI
+## Installation and setup
 
-Use `pip` to install `dstack`:
+To use `dstack`, install it with `pip` and start the Hub application.
 
 ```shell
 pip install dstack
+dstack start
 ```
 
-## Define workflows
+The `dstack start` command starts the Hub application, and creates the default project to run workflows locally.
 
-Define ML workflows, their output artifacts, hardware requirements, and dependencies via YAML.
+If you'll want to run workflows in the cloud (e.g. AWS, or GCP), simply log into the Hub application, and 
+create a new project.
+
+## Run your first  workflows
+
+Let's define our first ML workflow in `.dstack/workflows/hello.yaml`:
 
 ```yaml
 workflows:
   - name: train-mnist
     provider: bash
     commands:
       - pip install torchvision pytorch-lightning tensorboard
       - python examples/mnist/train_mnist.py
     artifacts:
       - path: ./lightning_logs
 ```
 
-## Run locally
+The YAML file allows you to request hardware [resources](https://dstack.ai/docs/usage/resources), run [Python](https://dstack.ai/docs/usage/python),
+save [artifacts](https://dstack.ai/docs/usage/artifacts), use [cache](https://dstack.ai/docs/usage/cache) and  
+[dependencies](https://dstack.ai/docs/usage/deps), create [dev environments](https://dstack.ai/docs/usage/dev-environments),
+run [apps](https://dstack.ai/docs/usage/apps), and many more.
 
-By default, workflows run locally on your machine.
+## Run it
+
+Go ahead and run it:
 
 ```shell
 dstack run train-mnist
 
 RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
 penguin-1  train-mnist  now        Submitted       local
 
 Provisioning... It may take up to a minute. ✓
 
 To interrupt, press Ctrl+C.
 
-GPU available: True, used: True
+GPU available: False, used: False
 
 Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-## Run remotely
+The `dstack run` command runs the workflow using the settings specified for the project configured with the
+Hub application.
+
+## Create a Hub project
+
+As mentioned above, the default project runs workflows locally.
+However, you can log into the application and create other projects that allow you to run workflows in the cloud.
+
+<img src="https://dstack.ai/assets/dstack-hub-create-project.png" width="800px" />
 
-To run workflows remotely in a configured cloud, you will need the Hub application, which can be installed either on a
-dedicated server for team work or directly on your local machine.
+If you want the project to use the cloud, you'll need to provide cloud credentials and specify settings such as the
+artifact storage bucket and the region where the workflows will run.
 
-### Start the Hub application
+<img src="https://dstack.ai/assets/dstack-hub-view-project.png" width="800px" />
 
-To start the Hub application, use this command:
+Once a project is created, copy the CLI command from the project settings and execute it in your terminal.
 
 <div class="termy">
 
 ```shell
-$ dstack hub start
-
-The hub is available at http://127.0.0.1:3000?token=b934d226-e24a-4eab-a284-eb92b353b10f
+dstack config --url http://127.0.0.1:3000 \
+  --project gcp \
+  --token b934d226-e24a-4eab-a284-eb92b353b10f
 ```
 
 </div>
 
-To login as an administrator, visit the URL in the output.
+The `dstack config` command configures `dstack` to run workflows using the settings from
+the corresponding project.
 
-### Create a project
+You can configure multiple projects and use them interchangeably (by passing the `--project` argument to the `dstack 
+run` command. Any project can be set as the default by passing `--default` to the `dstack config` command.
 
-Go ahead and create a new project.
+Configuring multiple projects can be convenient if you want to run workflows both locally and in the cloud or if 
+you would like to use multiple clouds.
 
-<img src="https://dstack.ai/assets/dstack_hub_create_project.png" width="800px"/>
 
-Choose a backend type (such as AWS or GCP), provide cloud credentials, and specify settings like
-artifact storage bucket and the region where to run workflows.
+## Manage resources
 
-<img src="https://dstack.ai/assets/dstack_hub_view_project.png" width="800px"/>
+Consider that you have configured a project that allows you to use a GPU (e.g., a local backend if you have a GPU
+locally, or an AWS or GCP backend).
 
-### Configure the CLI
+Let's update our workflow and add `resources`.
 
-Copy the CLI command from the project settings and execute it in your terminal to configure the project as a remote.
-
-<div class="termy">
-
-```shell
-$ dstack config hub --url http://127.0.0.1:3000 \
-  --project my-awesome-project \
-  --token b934d226-e24a-4eab-a284-eb92b353b10f
+```yaml
+workflows:
+  - name: train-mnist
+    provider: bash
+    commands:
+      - pip install torchvision pytorch-lightning tensorboard
+      - python examples/mnist/train_mnist.py
+    artifacts:
+      - path: ./lightning_logs
+    resources:
+      gpu:
+        name: V100
+        count: 1
 ```
 
-</div>
-
-Now, you can run workflows remotely in the created project by adding the `--remote` flag to the `dstack run` command
-and request hardware [`resources`](usage/resources.md) (like GPU, memory, interruptible instances, etc.) that you need.
+Let's run the workflow:
 
 ```shell
-dstack run train-mnist --remote --gpu 1
+dstack run train-mnist --project gcp
 
-RUN       WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
-turtle-1  train-mnist  now        Submitted       aws
+RUN        WORKFLOW     SUBMITTED  STATUS     TAG  BACKENDS
+penguin-1  train-mnist  now        Submitted       local
 
 Provisioning... It may take up to a minute. ✓
 
 To interrupt, press Ctrl+C.
 
 GPU available: True, used: True
 
 Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0]
 ```
 
-The command will automatically provision the required cloud resources in the corresponding cloud upon workflow 
-startup and tear them down upon completion.
+If your project is configured to use the cloud, the Hub application will automatically create the necessary cloud
+resources to execute the workflow and tear them down once it is finished.
 
 ## More information
 
 For additional information and examples, see the following links:
 
 * [Quick start](https://dstack.ai/docs/quick-start)
 * [Docs](https://dstack.ai/docs)
```

#### html2text {}

```diff
@@ -1,62 +1,78 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.8 Summary: The easiest way to
+Metadata-Version: 2.1 Name: dstack Version: 0.8.1 Summary: The easiest way to
 define ML workflows and run them on any cloud platform Home-page: https://
 dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
 UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
 UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
 Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
                             ****** [dstack] ******
                          *** ML workflows as code ***
-   The easiest way to define ML workflows and run them on any cloud platform
+           The easiest way to run ML workflows on any cloud platform
            [![Slack](https://img.shields.io/badge/slack-join%20chat-
 blueviolet?logo=slack&style=for-the-badge)](https://join.slack.com/t/dstackai/
                shared_invite/zt-xdnsytie-D4qU9BvJP8vkbkHXdi6clQ)
                   Quick_start â¢ Docs â¢ Tutorials â¢ Blog
   [![Last commit](https://img.shields.io/github/last-commit/dstackai/dstack)]
    (https://github.com/dstackai/dstack/commits/) [![PyPI - License](https://
    img.shields.io/pypi/l/dstack?style=flat&color=blue)](https://github.com/
                     dstackai/dstack/blob/master/LICENSE.md)
 ## What is dstack? `dstack` makes it very easy to define ML workflows and run
 them on any cloud platform. It provisions infrastructure, manages data, and
 monitors usage for you. Ideal for processing data, training models, running
-apps, and any other ML development tasks. ## Install the CLI Use `pip` to
-install `dstack`: ```shell pip install dstack ``` ## Define workflows Define ML
-workflows, their output artifacts, hardware requirements, and dependencies via
-YAML. ```yaml workflows: - name: train-mnist provider: bash commands: - pip
-install torchvision pytorch-lightning tensorboard - python examples/mnist/
-train_mnist.py artifacts: - path: ./lightning_logs ``` ## Run locally By
-default, workflows run locally on your machine. ```shell dstack run train-mnist
-RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-mnist now Submitted
-local Provisioning... It may take up to a minute. â To interrupt, press
-Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00, 280.17it/s,
-loss=1.35, v_num=0] ``` ## Run remotely To run workflows remotely in a
-configured cloud, you will need the Hub application, which can be installed
-either on a dedicated server for team work or directly on your local machine.
-### Start the Hub application To start the Hub application, use this command:
-```shell $ dstack hub start The hub is available at http://127.0.0.1:
-3000?token=b934d226-e24a-4eab-a284-eb92b353b10f ```
-To login as an administrator, visit the URL in the output. ### Create a project
-Go ahead and create a new project. [https://dstack.ai/assets/
-dstack_hub_create_project.png] Choose a backend type (such as AWS or GCP),
-provide cloud credentials, and specify settings like artifact storage bucket
-and the region where to run workflows. [https://dstack.ai/assets/
-dstack_hub_view_project.png] ### Configure the CLI Copy the CLI command from
-the project settings and execute it in your terminal to configure the project
-as a remote.
-```shell $ dstack config hub --url http://127.0.0.1:3000 \ --project my-
-awesome-project \ --token b934d226-e24a-4eab-a284-eb92b353b10f ```
-Now, you can run workflows remotely in the created project by adding the `--
-remote` flag to the `dstack run` command and request hardware [`resources`]
-(usage/resources.md) (like GPU, memory, interruptible instances, etc.) that you
-need. ```shell dstack run train-mnist --remote --gpu 1 RUN WORKFLOW SUBMITTED
-STATUS TAG BACKENDS turtle-1 train-mnist now Submitted aws Provisioning... It
-may take up to a minute. â To interrupt, press Ctrl+C. GPU available: True,
-used: True Epoch 1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0] ``` The
-command will automatically provision the required cloud resources in the
-corresponding cloud upon workflow startup and tear them down upon completion.
-## More information For additional information and examples, see the following
+apps, and any other ML development tasks. ## Installation and setup To use
+`dstack`, install it with `pip` and start the Hub application. ```shell pip
+install dstack dstack start ``` The `dstack start` command starts the Hub
+application, and creates the default project to run workflows locally. If
+you'll want to run workflows in the cloud (e.g. AWS, or GCP), simply log into
+the Hub application, and create a new project. ## Run your first workflows
+Let's define our first ML workflow in `.dstack/workflows/hello.yaml`: ```yaml
+workflows: - name: train-mnist provider: bash commands: - pip install
+torchvision pytorch-lightning tensorboard - python examples/mnist/
+train_mnist.py artifacts: - path: ./lightning_logs ``` The YAML file allows you
+to request hardware [resources](https://dstack.ai/docs/usage/resources), run
+[Python](https://dstack.ai/docs/usage/python), save [artifacts](https://
+dstack.ai/docs/usage/artifacts), use [cache](https://dstack.ai/docs/usage/
+cache) and [dependencies](https://dstack.ai/docs/usage/deps), create [dev
+environments](https://dstack.ai/docs/usage/dev-environments), run [apps](https:
+//dstack.ai/docs/usage/apps), and many more. ## Run it Go ahead and run it:
+```shell dstack run train-mnist RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS
+penguin-1 train-mnist now Submitted local Provisioning... It may take up to a
+minute. â To interrupt, press Ctrl+C. GPU available: False, used: False Epoch
+1: [00:03<00:00, 280.17it/s, loss=1.35, v_num=0] ``` The `dstack run` command
+runs the workflow using the settings specified for the project configured with
+the Hub application. ## Create a Hub project As mentioned above, the default
+project runs workflows locally. However, you can log into the application and
+create other projects that allow you to run workflows in the cloud. [https://
+dstack.ai/assets/dstack-hub-create-project.png] If you want the project to use
+the cloud, you'll need to provide cloud credentials and specify settings such
+as the artifact storage bucket and the region where the workflows will run.
+[https://dstack.ai/assets/dstack-hub-view-project.png] Once a project is
+created, copy the CLI command from the project settings and execute it in your
+terminal.
+```shell dstack config --url http://127.0.0.1:3000 \ --project gcp \ --token
+b934d226-e24a-4eab-a284-eb92b353b10f ```
+The `dstack config` command configures `dstack` to run workflows using the
+settings from the corresponding project. You can configure multiple projects
+and use them interchangeably (by passing the `--project` argument to the
+`dstack run` command. Any project can be set as the default by passing `--
+default` to the `dstack config` command. Configuring multiple projects can be
+convenient if you want to run workflows both locally and in the cloud or if you
+would like to use multiple clouds. ## Manage resources Consider that you have
+configured a project that allows you to use a GPU (e.g., a local backend if you
+have a GPU locally, or an AWS or GCP backend). Let's update our workflow and
+add `resources`. ```yaml workflows: - name: train-mnist provider: bash
+commands: - pip install torchvision pytorch-lightning tensorboard - python
+examples/mnist/train_mnist.py artifacts: - path: ./lightning_logs resources:
+gpu: name: V100 count: 1 ``` Let's run the workflow: ```shell dstack run train-
+mnist --project gcp RUN WORKFLOW SUBMITTED STATUS TAG BACKENDS penguin-1 train-
+mnist now Submitted local Provisioning... It may take up to a minute. â To
+interrupt, press Ctrl+C. GPU available: True, used: True Epoch 1: [00:03<00:00,
+280.17it/s, loss=1.35, v_num=0] ``` If your project is configured to use the
+cloud, the Hub application will automatically create the necessary cloud
+resources to execute the workflow and tear them down once it is finished. ##
+More information For additional information and examples, see the following
 links: * [Quick start](https://dstack.ai/docs/quick-start) * [Docs](https://
 dstack.ai/docs) * [Tutorials](https://dstack.ai/tutorials/dolly) * [Blog]
 (https://dstack.ai/blog) ## Licence [Mozilla Public License 2.0](LICENSE.md)
```

### Comparing `dstack-0.8/cli/dstack.egg-info/SOURCES.txt` & `dstack-0.8.1/cli/dstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/backend/base/test_logs.py` & `dstack-0.8.1/cli/tests/backend/base/test_logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/hub/common.py` & `dstack-0.8.1/cli/tests/hub/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/hub/routers/test_jobs.py` & `dstack-0.8.1/cli/tests/hub/routers/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/hub/routers/test_projects.py` & `dstack-0.8.1/cli/tests/hub/routers/test_projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/hub/routers/test_users.py` & `dstack-0.8.1/cli/tests/hub/routers/test_users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/integration/common.py` & `dstack-0.8.1/cli/tests/integration/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import errno
 import os
 import subprocess
 import time
 from contextlib import contextmanager
 from pathlib import Path
 from typing import List, Optional
 from unittest.mock import patch
@@ -83,14 +84,35 @@
     finally:
         process = psutil.Process(proc.pid)
         for child in process.children(recursive=True):
             child.kill()
         process.kill()
 
 
+# TODO: Figure out a way to read process stderr reliably.
+# proc.communicate() may hang even with timeout.
+#
+# @contextmanager
+# def terminate_on_exit(proc: subprocess.Popen) -> subprocess.Popen:
+#     try:
+#         yield proc
+#     finally:
+#         stderr = None
+#         try:
+#             stdout, stderr = proc.communicate(timeout=1)
+#         except subprocess.TimeoutExpired as e:
+#             process = psutil.Process(proc.pid)
+#             for child in process.children(recursive=True):
+#                 child.kill()
+#             process.kill()
+#             stdout, stderr = proc.communicate()
+#         if stderr is not None:
+#             print(stderr)
+
+
 def wait_hub(host: str = HUB_HOST, port: str = HUB_PORT, attempts=10):
     for _ in range(attempts):
         try:
             resp = requests.get(f"http://{host}:{port}")
         except requests.exceptions.ConnectionError:
             time.sleep(1)
             continue
```

### Comparing `dstack-0.8/cli/tests/integration/conftest.py` & `dstack-0.8.1/cli/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/integration/test_commands.py` & `dstack-0.8.1/cli/tests/integration/test_commands.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/providers/docker/test_entrypoint.py` & `dstack-0.8.1/cli/tests/providers/docker/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/providers/test_local_path.py` & `dstack-0.8.1/cli/tests/providers/test_local_path.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/utils/escape.py` & `dstack-0.8.1/cli/tests/utils/escape.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/utils/test_interpolator.py` & `dstack-0.8.1/cli/tests/utils/test_interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/utils/test_merge_workflow_data.py` & `dstack-0.8.1/cli/tests/utils/test_merge_workflow_data.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/cli/tests/utils/test_tarignore.py` & `dstack-0.8.1/cli/tests/utils/test_tarignore.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8/setup.py` & `dstack-0.8.1/setup.py`

 * *Files identical despite different names*


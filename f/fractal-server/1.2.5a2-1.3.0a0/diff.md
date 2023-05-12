# Comparing `tmp/fractal_server-1.2.5a2.tar.gz` & `tmp/fractal_server-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.5a2.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a0.tar", max compression
```

## Comparing `fractal_server-1.2.5a2.tar` & `fractal_server-1.3.0a0.tar`

### file list

```diff
@@ -1,129 +1,132 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.5a2/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.5a2/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.5a2/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-05-09 10:21:14.532581 fractal_server-1.2.5a2/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.2.5a2/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.5a2/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.5a2/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-05-09 10:07:31.178019 fractal_server-1.2.5a2/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.5a2/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2783 2023-05-09 10:07:31.178019 fractal_server-1.2.5a2/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    22641 2023-05-09 10:07:31.178019 fractal_server-1.2.5a2/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    12661 2023-05-09 10:18:18.878596 fractal_server-1.2.5a2/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11503 2023-05-09 10:07:31.182019 fractal_server-1.2.5a2/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-08 13:22:04.417311 fractal_server-1.2.5a2/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.5a2/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3175 2023-05-08 11:17:37.139725 fractal_server-1.2.5a2/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2529 2023-05-08 13:16:58.240665 fractal_server-1.2.5a2/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-05-08 13:16:58.244665 fractal_server-1.2.5a2/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.5a2/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.5a2/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.5a2/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.5a2/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8991 2023-04-28 14:21:32.268370 fractal_server-1.2.5a2/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19294 2023-04-17 13:34:24.748408 fractal_server-1.2.5a2/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5460 2023-04-17 13:34:24.748408 fractal_server-1.2.5a2/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.2.5a2/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.2.5a2/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.2.5a2/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3835 2023-04-21 11:00:14.178698 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-21 08:35:50.575851 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-04-21 11:00:14.178698 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    40272 2023-04-21 08:35:50.575851 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9749 2023-05-03 13:37:16.597419 fractal_server-1.2.5a2/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7400 2023-05-08 13:16:58.244665 fractal_server-1.2.5a2/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.5a2/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.5a2/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.5a2/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.5a2/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.5a2/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.5a2/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.5a2/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-05-09 10:11:26.675393 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-05-09 10:11:26.687393 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-05-08 12:02:12.609892 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-05-09 10:11:26.695393 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-05-09 10:08:09.097598 fractal_server-1.2.5a2/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.5a2/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-05-09 10:08:09.097598 fractal_server-1.2.5a2/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-05-09 10:08:09.097598 fractal_server-1.2.5a2/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-05-09 10:11:27.087389 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3046 2023-05-09 10:11:27.115388 fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-05-09 10:08:09.097598 fractal_server-1.2.5a2/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.2.5a2/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-05-09 10:08:09.097598 fractal_server-1.2.5a2/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12171 2023-05-08 06:31:53.082555 fractal_server-1.2.5a2/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.5a2/fractal_server/logger.py
--rw-r--r--   0        0        0     5805 2023-04-28 06:28:20.387228 fractal_server-1.2.5a2/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.5a2/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.5a2/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.5a2/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-05-08 13:16:58.244665 fractal_server-1.2.5a2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-05-08 13:16:58.244665 fractal_server-1.2.5a2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-05-08 13:16:58.244665 fractal_server-1.2.5a2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.5a2/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.5a2/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.5a2/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12869 2023-05-09 10:07:31.182019 fractal_server-1.2.5a2/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.2.5a2/fractal_server/utils.py
--rw-r--r--   0        0        0     2629 2023-05-09 10:21:14.532581 fractal_server-1.2.5a2/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.5a2/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.5a2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a0/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.3.0a0/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a0/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:12.629324 fractal_server-1.3.0a0/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.3.0a0/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a0/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a0/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a0/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     6974 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8401 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    12661 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12202 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a0/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3370 2023-05-12 09:56:36.874307 fractal_server-1.3.0a0/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2295 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2534 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5464 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8968 2023-05-12 09:56:36.874307 fractal_server-1.3.0a0/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19458 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a0/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a0/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a0/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4334 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42000 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a0/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a0/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1658 2023-05-12 09:55:08.603302 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     4943 2023-05-09 12:55:27.450288 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1135 2023-05-12 09:55:08.619302 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     3957 2023-05-09 12:55:27.454288 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1135 2023-05-12 09:54:53.927466 fractal_server-1.3.0a0/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.3.0a0/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4323 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      980 2023-05-12 09:54:53.927466 fractal_server-1.3.0a0/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2502 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.3.0a0/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a0/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a0/fractal_server/logger.py
+-rw-r--r--   0        0        0     5726 2023-05-12 12:34:32.122055 fractal_server-1.3.0a0/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a0/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a0/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a0/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      751 2023-05-12 09:56:36.874307 fractal_server-1.3.0a0/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py
+-rw-r--r--   0        0        0     8438 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py
+-rw-r--r--   0        0        0      745 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a0/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a0/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a0/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12869 2023-05-12 06:48:40.382595 fractal_server-1.3.0a0/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a0/fractal_server/utils.py
+-rw-r--r--   0        0        0     2592 2023-05-12 12:35:12.625325 fractal_server-1.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 fractal_server-1.3.0a0/setup.py
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 fractal_server-1.3.0a0/PKG-INFO
```

### Comparing `fractal_server-1.2.5a2/LICENSE` & `fractal_server-1.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/README.md` & `fractal_server-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/__main__.py` & `fractal_server-1.3.0a0/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/alembic.ini` & `fractal_server-1.3.0a0/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a0/fractal_server/app/api/v1/job.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,79 +4,93 @@
 from typing import Optional
 from zipfile import ZIP_DEFLATED
 from zipfile import ZipFile
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
+from fastapi import Response
 from fastapi import status
 from fastapi.responses import StreamingResponse
+from sqlmodel import select
 
+from ....config import get_settings
+from ....syringe import Inject
 from ...db import AsyncSession
 from ...db import get_db
 from ...models import ApplyWorkflow
 from ...models import ApplyWorkflowRead
 from ...runner._common import METADATA_FILENAME
+from ...runner._common import SHUTDOWN_FILENAME
 from ...security import current_active_user
 from ...security import User
-from .project import _get_project_check_owner
+from ._aux_functions import _get_job_check_owner
+from ._aux_functions import _get_project_check_owner
 
 
 router = APIRouter()
 
 
-@router.get("/{job_id}", response_model=ApplyWorkflowRead)
-async def get_job(
+@router.get(
+    "/project/{project_id}/job/{job_id}",
+    response_model=ApplyWorkflowRead,
+)
+async def read_job(
+    project_id: int,
     job_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[ApplyWorkflow]:
     """
     Return info on an existing job
     """
-    job = await db.get(ApplyWorkflow, job_id)
-    if not job:
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND, detail="Job not found"
-        )
-    await _get_project_check_owner(
-        project_id=job.project_id, user_id=user.id, db=db
+
+    output = await _get_job_check_owner(
+        project_id=project_id,
+        job_id=job_id,
+        user_id=user.id,
+        db=db,
     )
+    job = output["job"]
 
     job_read = ApplyWorkflowRead(**job.dict())
 
+    # FIXME: this operation is not reading from the DB, but from file
     try:
         metadata_file = Path(job_read.working_dir) / METADATA_FILENAME
         with metadata_file.open("r") as f:
             metadata = json.load(f)
         job_read.history = metadata["history"]
     except (KeyError, FileNotFoundError):
         pass
 
     await db.close()
     return job_read
 
 
-@router.get("/download/{job_id}", response_class=StreamingResponse)
+@router.get(
+    "/project/{project_id}/job/{job_id}/download/",
+    response_class=StreamingResponse,
+)
 async def download_job_logs(
+    project_id: int,
     job_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> StreamingResponse:
     """
     Download job folder
     """
-    job = await db.get(ApplyWorkflow, job_id)
-    if not job:
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND, detail="Job not found"
-        )
-    await _get_project_check_owner(
-        project_id=job.project_id, user_id=user.id, db=db
+    output = await _get_job_check_owner(
+        project_id=project_id,
+        job_id=job_id,
+        user_id=user.id,
+        db=db,
     )
+    job = output["job"]
 
     # Extract job's working_dir attribute
     working_dir_str = job.dict()["working_dir"]
     working_dir_path = Path(working_dir_str)
 
     # Create zip byte stream
     PREFIX_ZIP = working_dir_path.name
@@ -89,7 +103,72 @@
     await db.close()
 
     return StreamingResponse(
         iter([byte_stream.getvalue()]),
         media_type="application/x-zip-compressed",
         headers={"Content-Disposition": f"attachment;filename={zip_filename}"},
     )
+
+
+@router.get(
+    "/project/{project_id}/job/",
+    response_model=list[ApplyWorkflowRead],
+)
+async def get_job_list(
+    project_id: int,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_db),
+) -> Optional[list[ApplyWorkflowRead]]:
+    """
+    Get list of jobs associated to the current project
+    """
+    await _get_project_check_owner(
+        project_id=project_id, user_id=user.id, db=db
+    )
+    stm = select(ApplyWorkflow).where(ApplyWorkflow.project_id == project_id)
+    res = await db.execute(stm)
+    job_list = res.scalars().all()
+    await db.close()
+    return job_list
+
+
+@router.get(
+    "/project/{project_id}/job/{job_id}/stop/",
+    status_code=200,
+)
+async def stop_job(
+    project_id: int,
+    job_id: int,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_db),
+) -> Optional[ApplyWorkflow]:
+    """
+    Stop execution of a workflow job (only available for slurm backend)
+    """
+
+    # This endpoint is only implemented for SLURM backend
+    settings = Inject(get_settings)
+    backend = settings.FRACTAL_RUNNER_BACKEND
+    if backend == "slurm":
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                "Stopping a job execution is not implemented for "
+                f"FRACTAL_RUNNER_BACKEND={backend}."
+            ),
+        )
+
+    # Get job from DB
+    output = await _get_job_check_owner(
+        project_id=project_id,
+        job_id=job_id,
+        user_id=user.id,
+        db=db,
+    )
+    job = output["job"]
+
+    # Write shutdown file
+    shutdown_file = Path(job.working_dir) / SHUTDOWN_FILENAME
+    with shutdown_file.open("w") as f:
+        f.write(f"Trigger executor shutdown for {job.id=}, {project_id=}.")
+
+    return Response(status_code=status.HTTP_200_OK)
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a0/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a0/fractal_server/app/api/v1/workflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,227 +6,137 @@
 # Marco Franzon <marco.franzon@exact-lab.it>
 # Tommaso Comparin <tommaso.comparin@exact-lab.it>
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
-import asyncio
 from copy import deepcopy
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
-from pydantic import UUID4
 from sqlmodel import select
 
 from ...db import AsyncSession
 from ...db import get_db
-from ...models import LinkUserProject
-from ...models import Project
+from ...models import Task
 from ...models import Workflow
 from ...models import WorkflowCreate
 from ...models import WorkflowExport
+from ...models import WorkflowImport
 from ...models import WorkflowRead
-from ...models import WorkflowTask
 from ...models import WorkflowTaskCreate
 from ...models import WorkflowTaskRead
 from ...models import WorkflowTaskUpdate
 from ...models import WorkflowUpdate
 from ...security import current_active_user
 from ...security import User
-from .project import _get_project_check_owner
+from ._aux_functions import _check_workflow_exists
+from ._aux_functions import _get_project_check_owner
+from ._aux_functions import _get_workflow_check_owner
+from ._aux_functions import _get_workflow_task_check_owner
 
-router = APIRouter()
-
-
-async def _get_workflow_check_owner(
-    *,
-    workflow_id: int,
-    user_id: UUID4,
-    db: AsyncSession = Depends(get_db),
-) -> Workflow:
-    """
-    Check that user is a member of a workflow's project and return
-
-    Raises:
-        HTTPException(status_code=403_FORBIDDEN): If the user is not a
-                                                  member of the project
-        HTTPException(status_code=404_NOT_FOUND): If the project or workflow do
-                                                  not exist
-    """
-
-    workflow = await db.get(Workflow, workflow_id)
-    if not workflow:
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND, detail="Workflow not found"
-        )
 
-    project, link_user_project = await asyncio.gather(
-        db.get(Project, workflow.project_id),
-        db.get(LinkUserProject, (workflow.project_id, user_id)),
-    )
-    if not project:
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND, detail="Project not found"
-        )
-    if not link_user_project:
-        raise HTTPException(
-            status_code=status.HTTP_403_FORBIDDEN,
-            detail=f"Not allowed on project {workflow.project_id}",
-        )
-
-    return workflow
-
-
-async def _get_workflow_task_check_owner(
-    *,
-    workflow_id: int,
-    workflow_task_id: int,
-    user_id: UUID4,
-    db: AsyncSession = Depends(get_db),
-) -> tuple[WorkflowTask, Workflow]:
-    """
-    Check that user has rights to access a Workflow and a WorkflowTask and
-    return the WorkflowTask
-
-    Raises:
-        HTTPException(status_code=404_NOT_FOUND): If the WorkflowTask does not
-                                                  exist
-        HTTPException(status_code=422_UNPROCESSABLE_ENTITY): If the
-                                                             WorkflowTask is
-                                                             not associated to
-                                                             the Workflow
-    """
-
-    workflow_task = await db.get(WorkflowTask, workflow_task_id)
-
-    # If WorkflowTask is not in the db, exit
-    if not workflow_task:
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND,
-            detail="WorkflowTask not found",
-        )
-
-    # Access control for workflow
-    workflow = await _get_workflow_check_owner(  # noqa: F841
-        workflow_id=workflow_id, user_id=user_id, db=db
-    )
-
-    # If WorkflowTask is not part of the expected Workflow, exit
-    if workflow_id != workflow_task.workflow_id:
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=f"Invalid {workflow_id=} for {workflow_task_id=}",
-        )
-
-    return workflow_task, workflow
+router = APIRouter()
 
 
-async def _check_workflow_exists(
-    *,
-    name: str,
+@router.get(
+    "/project/{project_id}/workflow/",
+    response_model=list[WorkflowRead],
+)
+async def get_workflow_list(
     project_id: int,
+    user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-):
+) -> Optional[list[WorkflowRead]]:
     """
-    Check that there is no existing workflow for the same project and with the
-    same name
-
-    Arguments:
-        name: Workflow name
-        project_id: Project ID
-
-    Raises:
-        HTTPException(status_code=422_UNPROCESSABLE_ENTITY): If such a workflow
-                                                             already exists
-    """
-    stm = (
-        select(Workflow)
-        .where(Workflow.name == name)
-        .where(Workflow.project_id == project_id)
+    Get list of workflows associated to the current project
+    """
+    await _get_project_check_owner(
+        project_id=project_id, user_id=user.id, db=db
     )
+    stm = select(Workflow).where(Workflow.project_id == project_id)
     res = await db.execute(stm)
-    if res.scalars().all():
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=f"Workflow with {name=} and\
-                    {project_id=} already in use",
-        )
-
-
-# Main endpoints ("/")
+    workflow_list = res.scalars().all()
+    await db.close()
+    return workflow_list
 
 
 @router.post(
-    "/", response_model=WorkflowRead, status_code=status.HTTP_201_CREATED
+    "/project/{project_id}/workflow/",
+    response_model=WorkflowRead,
+    status_code=status.HTTP_201_CREATED,
 )
 async def create_workflow(
+    project_id: int,
     workflow: WorkflowCreate,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[WorkflowRead]:
     """
     Create a workflow, associate to a project
     """
     await _get_project_check_owner(
-        project_id=workflow.project_id,
+        project_id=project_id,
         user_id=user.id,
         db=db,
     )
     await _check_workflow_exists(
-        name=workflow.name, project_id=workflow.project_id, db=db
+        name=workflow.name, project_id=project_id, db=db
     )
 
-    db_workflow = Workflow.from_orm(workflow)
+    db_workflow = Workflow(project_id=project_id, **workflow.dict())
     db.add(db_workflow)
     await db.commit()
     await db.refresh(db_workflow)
     await db.close()
     return db_workflow
 
 
-# Workflow endpoints ("/{workflow_id}")
-
-
-@router.delete("/{workflow_id}", status_code=status.HTTP_204_NO_CONTENT)
-async def delete_workflow(
+@router.get(
+    "/project/{project_id}/workflow/{workflow_id}",
+    response_model=WorkflowRead,
+)
+async def read_workflow(
+    project_id: int,
     workflow_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> Response:
+) -> Optional[WorkflowRead]:
     """
-    Delte a workflow
+    Get info on an existing workflow
     """
 
     workflow = await _get_workflow_check_owner(
-        workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
 
-    await db.delete(workflow)
-    await db.commit()
-
-    return Response(status_code=status.HTTP_204_NO_CONTENT)
+    return workflow
 
 
-@router.patch("/{workflow_id}", response_model=WorkflowRead)
-async def patch_workflow(
+@router.patch(
+    "/project/{project_id}/workflow/{workflow_id}",
+    response_model=WorkflowRead,
+)
+async def update_workflow(
+    project_id: int,
     workflow_id: int,
     patch: WorkflowUpdate,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[WorkflowRead]:
     """
     Edit a workflow
     """
     workflow = await _get_workflow_check_owner(
-        workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
 
     for key, value in patch.dict(exclude_unset=True).items():
         if key == "reordered_workflowtask_ids":
             current_workflowtask_ids = [
                 wftask.id for wftask in workflow.task_list
             ]
@@ -249,78 +159,200 @@
     await db.commit()
     await db.refresh(workflow)
     await db.close()
 
     return workflow
 
 
-@router.get("/{workflow_id}", response_model=WorkflowRead)
-async def get_workflow(
+@router.delete(
+    "/project/{project_id}/workflow/{workflow_id}",
+    status_code=status.HTTP_204_NO_CONTENT,
+)
+async def delete_workflow(
+    project_id: int,
     workflow_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-) -> Optional[WorkflowRead]:
+) -> Response:
     """
-    Get info on an existing workflow
+    Delte a workflow
     """
 
     workflow = await _get_workflow_check_owner(
-        workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
 
+    await db.delete(workflow)
+    await db.commit()
+
+    return Response(status_code=status.HTTP_204_NO_CONTENT)
+
+
+@router.get(
+    "/project/{project_id}/workflow/{workflow_id}/export/",
+    response_model=WorkflowExport,
+)
+async def export_worfklow(
+    project_id: int,
+    workflow_id: int,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_db),
+) -> Optional[WorkflowExport]:
+    """
+    Export an existing workflow, after stripping all IDs
+    """
+    workflow = await _get_workflow_check_owner(
+        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
+    )
+    await db.close()
     return workflow
 
 
 @router.post(
-    "/{workflow_id}/add-task/",
+    "/project/{project_id}/workflow/import/",
+    response_model=WorkflowRead,
+    status_code=status.HTTP_201_CREATED,
+)
+async def import_workflow(
+    project_id: int,
+    workflow: WorkflowImport,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_db),
+) -> Optional[WorkflowRead]:
+    """
+    Import an existing workflow into a project
+
+    Also create all required objects (i.e. Workflow and WorkflowTask's) along
+    the way.
+    """
+
+    # Preliminary checks
+    await _get_project_check_owner(
+        project_id=project_id,
+        user_id=user.id,
+        db=db,
+    )
+
+    await _check_workflow_exists(
+        name=workflow.name, project_id=project_id, db=db
+    )
+
+    # Check that all required tasks are available
+    # NOTE: by now we go through the pair (source, name), but later on we may
+    # combine them into source -- see issue #293.
+    tasks = [wf_task.task for wf_task in workflow.task_list]
+    sourcename_to_id = {}
+    for task in tasks:
+        source = task.source
+        name = task.name
+        if not (source, name) in sourcename_to_id.keys():
+            stm = select(Task).where(Task.source == source)
+            tasks_by_source = (await db.execute(stm)).scalars().all()
+            if not tasks_by_source:
+                raise HTTPException(
+                    status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                    detail=(f"Found 0 tasks with {source=}."),
+                )
+            else:
+                stm = (
+                    select(Task)
+                    .where(Task.source == source)
+                    .where(Task.name == name)
+                )
+                current_task = (await db.execute(stm)).scalars().all()
+                if len(current_task) != 1:
+                    raise HTTPException(
+                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                        detail=(
+                            f"Found {len(current_task)} tasks with "
+                            f"{name =} and {source=}."
+                        ),
+                    )
+                sourcename_to_id[(source, name)] = current_task[0].id
+
+    # Create new Workflow (with empty task_list)
+    db_workflow = Workflow(
+        project_id=project_id,
+        **workflow.dict(exclude_none=True, exclude={"task_list"}),
+    )
+    db.add(db_workflow)
+    await db.commit()
+    await db.refresh(db_workflow)
+
+    # Insert tasks
+    async with db:
+        for _, wf_task in enumerate(workflow.task_list):
+            # Identify task_id
+            source = wf_task.task.source
+            name = wf_task.task.name
+            task_id = sourcename_to_id[(source, name)]
+            # Prepare new_wf_task
+            new_wf_task = WorkflowTaskCreate(
+                **wf_task.dict(exclude_none=True),
+            )
+            # Insert task
+            await db_workflow.insert_task(
+                **new_wf_task.dict(),
+                task_id=task_id,
+                db=db,
+            )
+
+    await db.close()
+    return db_workflow
+
+
+@router.post(
+    "/project/{project_id}/workflow/{workflow_id}/wftask/",
     response_model=WorkflowTaskRead,
     status_code=status.HTTP_201_CREATED,
 )
-async def add_task_to_workflow(
+async def create_workflowtask(
+    project_id: int,
     workflow_id: int,
+    task_id: int,
     new_task: WorkflowTaskCreate,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[WorkflowTaskRead]:
     """
     Add a WorkflowTask to a Workflow
     """
 
     workflow = await _get_workflow_check_owner(
-        workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
     async with db:
         workflow_task = await workflow.insert_task(
             **new_task.dict(),
+            task_id=task_id,
             db=db,
         )
 
     await db.close()
     return workflow_task
 
 
-# WorkflowTask endpoints ("/{workflow_id}/../{workflow_task_id}"
-
-
 @router.patch(
-    "/{workflow_id}/edit-task/{workflow_task_id}",
+    "/project/{project_id}/workflow/{workflow_id}/wftask/{workflow_task_id}",
     response_model=WorkflowTaskRead,
 )
-async def patch_workflow_task(
+async def update_workflowtask(
+    project_id: int,
     workflow_id: int,
     workflow_task_id: int,
     workflow_task_update: WorkflowTaskUpdate,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[WorkflowTaskRead]:
     """
     Edit a WorkflowTask of a Workflow
     """
 
     db_workflow_task, db_workflow = await _get_workflow_task_check_owner(
+        project_id=project_id,
         workflow_task_id=workflow_task_id,
         workflow_id=workflow_id,
         user_id=user.id,
         db=db,
     )
 
     for key, value in workflow_task_update.dict(exclude_unset=True).items():
@@ -342,54 +374,37 @@
     await db.refresh(db_workflow_task)
     await db.close()
 
     return db_workflow_task
 
 
 @router.delete(
-    "/{workflow_id}/rm-task/{workflow_task_id}",
+    "/project/{project_id}/workflow/{workflow_id}/wftask/{workflow_task_id}",
     status_code=status.HTTP_204_NO_CONTENT,
 )
-async def delete_task_from_workflow(
+async def delete_workflowtask(
+    project_id: int,
     workflow_id: int,
     workflow_task_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Response:
     """
     Delete a WorkflowTask of a Workflow
     """
 
     db_workflow_task, db_workflow = await _get_workflow_task_check_owner(
+        project_id=project_id,
         workflow_task_id=workflow_task_id,
         workflow_id=workflow_id,
         user_id=user.id,
         db=db,
     )
 
     await db.delete(db_workflow_task)
     await db.commit()
 
     await db.refresh(db_workflow)
     db_workflow.task_list.reorder()
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
-
-
-@router.get(
-    "/{workflow_id}/export/",
-    response_model=WorkflowExport,
-)
-async def export_worfklow(
-    workflow_id: int,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Optional[WorkflowExport]:
-    """
-    Export an existing workflow, after stripping all IDs
-    """
-    workflow = await _get_workflow_check_owner(
-        workflow_id=workflow_id, user_id=user.id, db=db
-    )
-    await db.close()
-    return workflow
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a0/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/models/job.py` & `fractal_server-1.3.0a0/fractal_server/app/models/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,16 @@
             ID of the output dataset.
         workflow_id:
             ID of the workflow being applied.
         status:
             Workflow status
         start_timestamp:
             Timestamp of when the run began.
+        end_timestamp:
+            Timestamp of when the run ended or failed.
         status:
             Status of the run.
         log:
             forward of the workflow logs. Usually this attribute is only
             populated upon failure.
 
         project:
@@ -99,9 +101,12 @@
     workflow: Workflow = Relationship()
 
     start_timestamp: datetime = Field(
         default_factory=get_timestamp,
         nullable=False,
         sa_column=Column(DateTime(timezone=True)),
     )
+    end_timestamp: Optional[datetime] = Field(
+        default=None, sa_column=Column(DateTime(timezone=True))
+    )
     status: JobStatusType = JobStatusType.SUBMITTED
     log: Optional[str] = None
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/models/project.py` & `fractal_server-1.3.0a0/fractal_server/app/models/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 from typing import Any
 from typing import Optional
 
-from pydantic import UUID4
 from sqlalchemy import Column
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
-from sqlmodel import SQLModel
 
 from ...common.schemas.project import _DatasetBase
 from ...common.schemas.project import _ProjectBase
 from ...common.schemas.project import _ResourceBase
+from .linkuserproject import LinkUserProject
 from .security import UserOAuth as User
 from .workflow import Workflow
 
 
-class LinkUserProject(SQLModel, table=True):
-    """
-    Crossing table between User and Project
-    """
-
-    project_id: int = Field(foreign_key="project.id", primary_key=True)
-    user_id: UUID4 = Field(foreign_key="user_oauth.id", primary_key=True)
-
-
 class Dataset(_DatasetBase, table=True):
     """
     Represent a dataset
 
     Attributes:
         id:
             Primary key
@@ -58,16 +48,17 @@
     def paths(self) -> list[str]:
         return [r.path for r in self.resource_list]
 
 
 class Project(_ProjectBase, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
 
-    user_member_list: list[User] = Relationship(
+    user_list: list[User] = Relationship(
         link_model=LinkUserProject,
+        back_populates="project_list",
         sa_relationship_kwargs={
             "lazy": "selectin",
         },
     )
 
     dataset_list: list[Dataset] = Relationship(
         sa_relationship_kwargs={
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/models/state.py` & `fractal_server-1.3.0a0/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/models/task.py` & `fractal_server-1.3.0a0/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a0/fractal_server/app/models/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,7 +180,11 @@
             await db.commit()
             await db.refresh(wf_task)
         return wf_task
 
     @property
     def input_type(self):
         return self.task_list[0].task.input_type
+
+    @property
+    def output_type(self):
+        return self.task_list[-1].task.output_type
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from ...utils import get_timestamp
 from ..db import DB
 from ..models import ApplyWorkflow
 from ..models import Dataset
 from ..models import JobStatusType
 from ..models import Workflow
 from ._local import process_workflow as local_process_workflow
-from .common import auto_output_dataset  # noqa: F401
 from .common import close_job_logger
 from .common import JobExecutionError
 from .common import TaskExecutionError
 from .common import validate_workflow_compatibility  # noqa: F401
 
 
 _backends = {}
@@ -84,17 +83,15 @@
 
     Args:
         workflow_id:
             ID of the workflow being applied
         input_dataset_id
             Input dataset ID
         output_dataset_id:
-            ID of the destination dataset of the workflow. If not provided,
-            overwriting of the input dataset is implied and an error is raised
-            if the dataset is in read only mode.
+            ID of the destination dataset of the workflow.
         job_id:
             Id of the job record which stores the state for the current
             workflow application.
         worker_init:
             Custom executor parameters that get parsed before the execution of
             each task.
         user_cache_dir:
@@ -212,25 +209,27 @@
             f"more logs at {str(log_file_path)}"
         )
         logger.debug(f'END workflow "{workflow.name}"')
 
         db_sync.merge(output_dataset)
 
         job.status = JobStatusType.DONE
+        job.end_timestamp = get_timestamp()
         with log_file_path.open("r") as f:
             logs = f.read()
         job.log = logs
         db_sync.merge(job)
 
     except TaskExecutionError as e:
 
         logger.debug(f'FAILED workflow "{workflow.name}", TaskExecutionError.')
         logger.info(f'Workflow "{workflow.name}" failed (TaskExecutionError).')
 
         job.status = JobStatusType.FAILED
+        job.end_timestamp = get_timestamp()
 
         exception_args_string = "\n".join(e.args)
         job.log = (
             f"TASK ERROR:"
             f"Task id: {e.workflow_task_id} ({e.task_name}), "
             f"{e.workflow_task_order=}\n"
             f"TRACEBACK:\n{exception_args_string}"
@@ -239,24 +238,26 @@
 
     except JobExecutionError as e:
 
         logger.debug(f'FAILED workflow "{workflow.name}", JobExecutionError.')
         logger.info(f'Workflow "{workflow.name}" failed (JobExecutionError).')
 
         job.status = JobStatusType.FAILED
+        job.end_timestamp = get_timestamp()
         error = e.assemble_error()
         job.log = f"JOB ERROR:\nTRACEBACK:\n{error}"
         db_sync.merge(job)
 
     except Exception as e:
 
         logger.debug(f'FAILED workflow "{workflow.name}", unknown error.')
         logger.info(f'Workflow "{workflow.name}" failed (unkwnon error).')
 
         job.status = JobStatusType.FAILED
+        job.end_timestamp = get_timestamp()
         job.log = f"UNKNOWN ERROR\nOriginal error: {str(e)}"
         db_sync.merge(job)
 
     finally:
         close_job_logger(logger)
         db_sync.commit()
         db_sync.close()
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .common import JobExecutionError
 from .common import TaskExecutionError
 from .common import TaskParameters
 from .common import write_args_file
 
 
 METADATA_FILENAME = "metadata.json"
+SHUTDOWN_FILENAME = "shutdown"
 
 
 def no_op_submit_setup_call(
     *,
     wftask: WorkflowTask,
     workflow_dir: Path,
     workflow_dir_user: Path,
@@ -432,15 +433,17 @@
         workflow_dir_user=workflow_dir_user,
     )
 
     # Submit tasks for execution. Note that `for _ in map_iter:
     # pass` explicitly calls the .result() method for each future, and
     # therefore is blocking until the task are complete.
     map_iter = executor.map(partial_call_task, component_list, **extra_setup)
-    # Wait for execution of this chunk of tasks
+    # Wait for execution of this chunk of tasks. Note: this is required *also*
+    # because otherwise the shutdown of a FractalSlurmExecutor while running
+    # map() may not work
     for _ in map_iter:
         pass  # noqa: 701
 
     # Assemble a Future[TaskParameter]
     history = f"{wftask.task.name}: {component_list}"
     try:
         task_pars_depend.metadata["history"].append(history)
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 metadata=input_metadata,
             ),
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir,
             logger_name=logger_name,
             submit_setup_call=_local_submit_setup,
         )
-    output_task_pars = output_task_pars_fut.result()
+        output_task_pars = output_task_pars_fut.result()
     output_dataset_metadata = output_task_pars.metadata
     return output_dataset_metadata
 
 
 async def process_workflow(
     *,
     workflow: Workflow,
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 metadata=input_metadata,
             ),
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir_user,
             submit_setup_call=_slurm_submit_setup,
             logger_name=logger_name,
         )
-    output_task_pars = output_task_pars_fut.result()
+        output_task_pars = output_task_pars_fut.result()
     output_dataset_metadata = output_task_pars.metadata
     return output_dataset_metadata
 
 
 async def process_workflow(
     *,
     workflow: Workflow,
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 import cloudpickle
 from cfut import SlurmExecutor
 from cfut.util import random_string
 
 from ....config import get_settings
 from ....logger import set_logger
-from ....logger import wrap_with_timing_logs
 from ....syringe import Inject
 from .._common import get_task_file_paths
 from .._common import TaskFiles
 from ..common import JobExecutionError
 from ..common import TaskExecutionError
 from ._batching import heuristics
 from ._executor_wait_thread import FractalSlurmWaitThread
@@ -167,26 +166,28 @@
             Directory for both the cfut/SLURM and fractal-server files and logs
         map_jobid_to_slurm_files:
             Dictionary with paths of slurm-related files for active jobs
     """
 
     wait_thread_cls = FractalSlurmWaitThread
     slurm_user: str
+    shutdown_file: str
     common_script_lines: list[str]
     user_cache_dir: str
     working_dir: Path
     working_dir_user: Path
     map_jobid_to_slurm_files: dict[str, tuple[str, str, str]]
     keep_pickle_files: bool
 
     def __init__(
         self,
         slurm_user: str,
-        working_dir: Optional[Path] = None,
-        working_dir_user: Optional[Path] = None,
+        working_dir: Path,
+        working_dir_user: Path,
+        shutdown_file: Optional[str] = None,
         user_cache_dir: Optional[str] = None,
         common_script_lines: Optional[list[str]] = None,
         slurm_poll_interval: Optional[int] = None,
         keep_pickle_files: bool = False,
         *args,
         **kwargs,
     ):
@@ -199,24 +200,17 @@
                 "Missing attribute FractalSlurmExecutor.slurm_user"
             )
 
         super().__init__(*args, **kwargs)
 
         self.keep_pickle_files = keep_pickle_files
         self.slurm_user = slurm_user
+
         self.common_script_lines = common_script_lines or []
-        if not working_dir:
-            settings = Inject(get_settings)
-            working_dir = settings.FRACTAL_RUNNER_WORKING_BASE_DIR
         self.working_dir = working_dir
-        if not working_dir_user:
-            if self.slurm_user:
-                raise RuntimeError(f"{self.slurm_user=}, {working_dir_user=}")
-            else:
-                working_dir_user = working_dir
         if not _path_exists_as_user(
             path=str(working_dir_user), user=self.slurm_user
         ):
             logger.info(f"Missing folder {working_dir_user=}")
         self.user_cache_dir = user_cache_dir
 
         self.working_dir_user = working_dir_user
@@ -226,20 +220,24 @@
         # cfut.SlurmWaitThread)
         if not slurm_poll_interval:
             settings = Inject(get_settings)
             slurm_poll_interval = settings.FRACTAL_SLURM_POLL_INTERVAL
         self.wait_thread.slurm_poll_interval = slurm_poll_interval
         self.wait_thread.slurm_user = self.slurm_user
 
+        self.wait_thread.shutdown_file = shutdown_file
+        self.wait_thread.shutdown_callback = self.shutdown
+
     def _cleanup(self, jobid: str) -> None:
         """
         Given a job ID as returned by _start, perform any necessary
         cleanup after the job has finished.
         """
-        self.map_jobid_to_slurm_files.pop(jobid)
+        with self.jobs_lock:
+            self.map_jobid_to_slurm_files.pop(jobid)
 
     def get_input_pickle_file_path(
         self, arg: str, prefix: Optional[str] = None
     ) -> Path:
         prefix = prefix or "cfut"
         return self.working_dir / f"{prefix}_in_{arg}.pickle"
 
@@ -476,15 +474,14 @@
                         yield res
             finally:
                 for future in fs:
                     future.cancel()
 
         return result_iterator()
 
-    @wrap_with_timing_logs
     def _submit_job(
         self,
         fun: Callable[..., Any],
         slurm_file_prefix: str,
         task_files: TaskFiles,
         slurm_config: SlurmConfig,
         single_task_submission: bool = False,
@@ -604,31 +601,31 @@
 
         # Submit job to SLURM, and get jobid
         jobid, job = self._start(job)
 
         # Add the SLURM script/out/err paths to map_jobid_to_slurm_files (this
         # must be after self._start(job), so that "%j" has already been
         # replaced with the job ID)
-        self.map_jobid_to_slurm_files[jobid] = (
-            job.slurm_script.as_posix(),
-            job.slurm_stdout.as_posix(),
-            job.slurm_stderr.as_posix(),
-        )
+        with self.jobs_lock:
+            self.map_jobid_to_slurm_files[jobid] = (
+                job.slurm_script.as_posix(),
+                job.slurm_stdout.as_posix(),
+                job.slurm_stderr.as_posix(),
+            )
 
         # Thread will wait for it to finish.
         self.wait_thread.wait(
             filenames=job.get_clean_output_pickle_files(),
             jobid=jobid,
         )
 
         with self.jobs_lock:
             self.jobs[jobid] = (fut, job)
         return fut
 
-    @wrap_with_timing_logs
     def _prepare_JobExecutionError(
         self, jobid: str, info: str
     ) -> JobExecutionError:
         """
         Prepare the JobExecutionError for a given job
 
             1. Wait for `FRACTAL_SLURM_KILLWAIT_INTERVAL` seconds, so that
@@ -646,29 +643,29 @@
                 ID of the SLURM job.
         """
         # Wait FRACTAL_SLURM_KILLWAIT_INTERVAL seconds
         settings = Inject(get_settings)
         settings.FRACTAL_SLURM_KILLWAIT_INTERVAL
         time.sleep(settings.FRACTAL_SLURM_KILLWAIT_INTERVAL)
         # Extract SLURM file paths
-        (
-            slurm_script_file,
-            slurm_stdout_file,
-            slurm_stderr_file,
-        ) = self.map_jobid_to_slurm_files[jobid]
+        with self.jobs_lock:
+            (
+                slurm_script_file,
+                slurm_stdout_file,
+                slurm_stderr_file,
+            ) = self.map_jobid_to_slurm_files[jobid]
         # Construct JobExecutionError exception
         job_exc = JobExecutionError(
             cmd_file=slurm_script_file,
             stdout_file=slurm_stdout_file,
             stderr_file=slurm_stderr_file,
             info=info,
         )
         return job_exc
 
-    @wrap_with_timing_logs
     def _completion(self, jobid: str) -> None:
         """
         Callback function to be executed whenever a job finishes.
 
         This function is executed by self.wait_thread (triggered by either
         finding an existing output pickle file `out_path` or finding that the
         SLURM job is over). Since this takes place on a different thread,
@@ -691,31 +688,33 @@
             # Copy all relevant files from self.working_dir_user to
             # self.working_dir
 
             self._copy_files_from_user_to_server(job)
 
             # Update the paths to use the files in self.working_dir (rather
             # than the user's ones in self.working_dir_user)
-            self.map_jobid_to_slurm_files[jobid]
-            (
-                slurm_script_file,
-                slurm_stdout_file,
-                slurm_stderr_file,
-            ) = self.map_jobid_to_slurm_files[jobid]
+            with self.jobs_lock:
+                self.map_jobid_to_slurm_files[jobid]
+                (
+                    slurm_script_file,
+                    slurm_stdout_file,
+                    slurm_stderr_file,
+                ) = self.map_jobid_to_slurm_files[jobid]
             new_slurm_stdout_file = str(
                 self.working_dir / Path(slurm_stdout_file).name
             )
             new_slurm_stderr_file = str(
                 self.working_dir / Path(slurm_stderr_file).name
             )
-            self.map_jobid_to_slurm_files[jobid] = (
-                slurm_script_file,
-                new_slurm_stdout_file,
-                new_slurm_stderr_file,
-            )
+            with self.jobs_lock:
+                self.map_jobid_to_slurm_files[jobid] = (
+                    slurm_script_file,
+                    new_slurm_stdout_file,
+                    new_slurm_stderr_file,
+                )
 
             in_paths = job.input_pickle_files
             out_paths = tuple(
                 self.working_dir / f.name for f in job.output_pickle_files
             )
 
             outputs = []
@@ -831,15 +830,14 @@
             except InvalidStateError:
                 logger.warning(
                     f"Future {fut} (SLURM job ID: {jobid}) was already"
                     " cancelled, exit from"
                     " FractalSlurmExecutor._completion."
                 )
 
-    @wrap_with_timing_logs
     def _copy_files_from_user_to_server(
         self,
         job: SlurmJob,
     ):
         """
         Impersonate the user and copy task-related files
 
@@ -913,15 +911,14 @@
                     raise JobExecutionError(info)
                 # Write to dest_file_path (including empty files)
                 dest_file_path = str(self.working_dir / source_file_name)
                 with open(dest_file_path, "wb") as f:
                     f.write(res.stdout)
         logger.debug("[_copy_files_from_user_to_server] End")
 
-    @wrap_with_timing_logs
     def _start(
         self,
         job: SlurmJob,
     ) -> tuple[str, SlurmJob]:
         """
         Submit function for execution on a SLURM cluster
         """
@@ -997,15 +994,14 @@
         )
         job.slurm_stderr = Path(
             job.slurm_stderr.as_posix().replace("%j", jobid_str)
         )
 
         return jobid_str, job
 
-    @wrap_with_timing_logs
     def _prepare_sbatch_script(
         self,
         *,
         list_commands: list[str],
         slurm_out_path: str,
         slurm_err_path: str,
         slurm_config: SlurmConfig,
@@ -1054,21 +1050,69 @@
                     f"{cmd} &"
                 )
         script_lines.append("wait\n")
 
         script = "\n".join(script_lines)
         return script
 
-    @wrap_with_timing_logs
     def get_default_task_files(self) -> TaskFiles:
         """
         This will be called when self.submit or self.map are called from
         outside fractal-server, and then lack some optional arguments.
         """
         import random
 
         task_files = TaskFiles(
             workflow_dir=self.working_dir,
             workflow_dir_user=self.working_dir_user,
             task_order=random.randint(10000, 99999),  # nosec
         )
         return task_files
+
+    def shutdown(self, wait=True, *, cancel_futures=False):
+        """
+        Clean up all executor variables. Note that this function is executed on
+        the self.wait_thread thread, see _completion.
+        """
+
+        logger.debug("Executor shutdown: start")
+
+        # Handle all job futures
+        slurm_jobs_to_scancel = []
+        with self.jobs_lock:
+            while self.jobs:
+                jobid, fut_and_job = self.jobs.popitem()
+                slurm_jobs_to_scancel.append(jobid)
+                fut, job = fut_and_job[:]
+                self.map_jobid_to_slurm_files.pop(jobid)
+                if not fut.cancelled():
+                    fut.set_exception(
+                        JobExecutionError(
+                            "Job cancelled due to executor shutdown."
+                        )
+                    )
+                    fut.cancel()
+
+        # Cancel SLURM jobs
+        if slurm_jobs_to_scancel:
+            scancel_string = " ".join(slurm_jobs_to_scancel)
+            logger.warning(f"Now scancel-ing SLURM jobs {scancel_string}")
+            pre_command = f"sudo --non-interactive -u {self.slurm_user}"
+            submit_command = f"scancel {scancel_string}"
+            full_command = f"{pre_command} {submit_command}"
+            logger.debug(f"Now execute `{full_command}`")
+            try:
+                subprocess.run(  # nosec
+                    shlex.split(full_command),
+                    capture_output=True,
+                    check=True,
+                    encoding="utf-8",
+                )
+            except subprocess.CalledProcessError as e:
+                error_msg = (
+                    f"Cancel command `{full_command}` failed. "
+                    f"Original error:\n{str(e)}"
+                )
+                logger.error(error_msg)
+                raise JobExecutionError(info=error_msg)
+
+        logger.debug("Executor shutdown: end")
```

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a0/fractal_server/app/runner/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing import Callable
 from typing import Optional
 
 from pydantic import BaseModel
 
 from ...logger import close_logger as close_job_logger  # noqa F401
 from ..models import Dataset
-from ..models import Project
 from ..models.workflow import Workflow
 
 
 class TaskExecutionError(RuntimeError):
     """
     Forwards errors occurred during the execution of a task
 
@@ -184,105 +183,44 @@
     metadata: dict[str, Any]
 
     class Config:
         arbitrary_types_allowed = True
         extra = "forbid"
 
 
-async def auto_output_dataset(
-    *,
-    project: Project,
-    input_dataset: Dataset,
-    workflow: Workflow,
-    overwrite_input: bool = False,
-) -> Dataset:
-    """
-    Determine the output dataset if it was not provided explicitly
-
-    Only datasets containing exactly one path can be used as output.
-
-    Note: This routine is still a stub.
-
-    Args:
-        project:
-            The project that contains the input and output datasets.
-        input_dataset:
-            The input dataset.
-        workflow:
-            The workflow to be applied to the input dataset.
-        overwrite_input:
-            Whether it is allowed to overwrite the input dataset with the
-            output data.
-
-    Raises:
-        ValueError: If the input dataset is to be overwritten and it provides
-                    more than one path.
-
-    Returns:
-        output_dataset:
-            the output dataset
-    """
-    if overwrite_input and not input_dataset.read_only:
-        input_paths = input_dataset.paths
-        if len(input_paths) != 1:
-            raise ValueError(
-                "Cannot determine output dataset "
-                "with more than one input path."
-            )
-        output_dataset = input_dataset
-    else:
-        raise NotImplementedError(
-            "Cannot determine ouput dataset with "
-            f"{overwrite_input=} and {input_dataset.read_only=}"
-        )
-
-    return output_dataset
-
-
 def validate_workflow_compatibility(
     *,
     input_dataset: Dataset,
     workflow: Workflow,
-    output_dataset: Optional[Dataset] = None,
-):
+    output_dataset: Dataset,
+) -> None:
     """
     Check compatibility of workflow and input / ouptut dataset
     """
+    # Check input_dataset type
     if (
         workflow.input_type != "Any"
         and workflow.input_type != input_dataset.type
     ):
         raise TypeError(
             f"Incompatible types `{workflow.input_type}` of workflow "
             f"`{workflow.name}` and `{input_dataset.type}` of dataset "
             f"`{input_dataset.name}`"
         )
 
-    if not output_dataset:
-        if input_dataset.read_only:
-            raise ValueError("Input dataset is read-only")
-        else:
-            input_paths = input_dataset.paths
-            if len(input_paths) != 1:
-                # Only single input can be safely transformed in an output
-                raise ValueError(
-                    "Cannot determine output path: multiple input "
-                    "paths to overwrite"
-                )
-            else:
-                output_path = input_paths[0]
-    else:
-
-        if len(output_dataset.paths) != 1:
-            raise ValueError(
-                "Cannot determine output path: Multiple paths in dataset."
-            )
-        else:
-            output_path = output_dataset.paths[0]
-    return output_path
+    # Check output_dataset type
+    if (
+        workflow.output_type != "Any"
+        and workflow.output_type != output_dataset.type
+    ):
+        raise TypeError(
+            f"Incompatible types `{workflow.output_type}` of workflow "
+            f"`{workflow.name}` and `{output_dataset.type}` of dataset "
+            f"`{output_dataset.name}`"
+        )
 
 
 def async_wrap(func: Callable) -> Callable:
     """
     Wrap a synchronous callable in an async task
 
     Ref: [issue #140](https://github.com/fractal-analytics-platform/fractal-server/issues/140)
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a0/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a0/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/README.md` & `fractal_server-1.3.0a0/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 10:08:09 2023 UTC, .py size: 1716 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,104 @@
-00000000: 6f0d 0d0a 0000 0000 891b 5a64 b406 0000  o.........Zd....
+00000000: 6f0d 0d0a 0000 0000 ed0c 5e64 6f04 0000  o.........^do...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c06 6d07 5a07 0100 6406 6407 6c08  d.l.m.Z...d.d.l.
-00000070: 6d09 5a09 0100 6406 6408 6c08 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000080: 0100 6409 5a0b 4700 640a 640b 8400 640b  ..d.Z.G.d.d...d.
-00000090: 6507 8303 5a0c 4700 640c 640d 8400 640d  e...Z.G.d.d...d.
-000000a0: 650c 8303 5a0d 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
-000000b0: 650c 8303 5a0e 6410 5300 2911 e900 0000  e...Z.d.S.).....
-000000c0: 0029 01da 0864 6174 6574 696d 6529 01da  .)...datetime)..
-000000d0: 044c 6973 7429 01da 084f 7074 696f 6e61  .List)...Optiona
-000000e0: 6c29 01da 0976 616c 6964 6174 6f72 2901  l)...validator).
-000000f0: da08 5351 4c4d 6f64 656c e901 0000 0029  ..SQLModel.....)
-00000100: 01da 0676 616c 696e 7429 01da 0676 616c  ...valint)...val
-00000110: 7374 7229 03da 1141 7070 6c79 576f 726b  str)...ApplyWork
-00000120: 666c 6f77 4261 7365 da13 4170 706c 7957  flowBase..ApplyW
-00000130: 6f72 6b66 6c6f 7743 7265 6174 65da 1141  orkflowCreate..A
-00000140: 7070 6c79 576f 726b 666c 6f77 5265 6164  pplyWorkflowRead
-00000150: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000160: 0003 0000 0040 0000 0073 4e00 0000 6500  .....@...sN...e.
-00000170: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
-00000180: 6402 3c00 6504 6505 6403 3c00 6506 6504  d.<.e.e.d.<.e.e.
-00000190: 1900 6505 6404 3c00 6504 6505 6405 3c00  ..e.d.<.e.e.d.<.
-000001a0: 6406 5a07 6508 6505 6407 3c00 6506 6509  d.Z.e.e.d.<.e.e.
-000001b0: 1900 6505 6408 3c00 6409 5300 290a 720a  ..e.d.<.d.S.).r.
-000001c0: 0000 007a fa0a 2020 2020 4261 7365 2063  ...z..    Base c
-000001d0: 6c61 7373 2066 6f72 2041 7070 6c79 576f  lass for ApplyWo
-000001e0: 726b 666c 6f77 0a0a 2020 2020 4174 7472  rkflow..    Attr
-000001f0: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-00000200: 696e 7075 745f 6461 7461 7365 745f 6964  input_dataset_id
-00000210: 3a20 5442 440a 2020 2020 2020 2020 6f75  : TBD.        ou
-00000220: 7470 7574 5f64 6174 6173 6574 5f69 643a  tput_dataset_id:
-00000230: 2054 4244 0a20 2020 2020 2020 2077 6f72   TBD.        wor
-00000240: 6b66 6c6f 775f 6964 3a20 5442 440a 2020  kflow_id: TBD.  
-00000250: 2020 2020 2020 6f76 6572 7772 6974 655f        overwrite_
-00000260: 696e 7075 743a 2054 4244 0a20 2020 2020  input: TBD.     
-00000270: 2020 2077 6f72 6b65 725f 696e 6974 3a20     worker_init: 
-00000280: 5442 440a 2020 2020 2020 2020 776f 726b  TBD.        work
-00000290: 696e 675f 6469 723a 2054 4244 0a20 2020  ing_dir: TBD.   
-000002a0: 2020 2020 2077 6f72 6b69 6e67 5f64 6972       working_dir
-000002b0: 5f75 7365 723a 2054 4244 0a20 2020 20da  _user: TBD.    .
-000002c0: 0a70 726f 6a65 6374 5f69 64da 1069 6e70  .project_id..inp
-000002d0: 7574 5f64 6174 6173 6574 5f69 64da 116f  ut_dataset_id..o
-000002e0: 7574 7075 745f 6461 7461 7365 745f 6964  utput_dataset_id
-000002f0: da0b 776f 726b 666c 6f77 5f69 6446 da0f  ..workflow_idF..
-00000300: 6f76 6572 7772 6974 655f 696e 7075 74da  overwrite_input.
-00000310: 0b77 6f72 6b65 725f 696e 6974 4e29 0ada  .worker_initN)..
-00000320: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000330: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000340: 655f 5fda 075f 5f64 6f63 5f5f da03 696e  e__..__doc__..in
-00000350: 74da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  t..__annotations
-00000360: 5f5f 7204 0000 0072 1100 0000 da04 626f  __r....r......bo
-00000370: 6f6c da03 7374 72a9 0072 1b00 0000 721b  ol..str..r....r.
-00000380: 0000 00fa 532f 686f 6d65 2f74 6f6d 6d61  ....S/home/tomma
-00000390: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
-000003a0: 616c 2d73 6572 7665 722f 6672 6163 7461  al-server/fracta
-000003b0: 6c5f 7365 7276 6572 2f63 6f6d 6d6f 6e2f  l_server/common/
-000003c0: 7363 6865 6d61 732f 6170 706c 7977 6f72  schemas/applywor
-000003d0: 6b66 6c6f 772e 7079 720a 0000 0012 0000  kflow.pyr.......
-000003e0: 0073 1000 0000 0a00 0401 080d 0801 0c01  .s..............
-000003f0: 0801 0c01 1001 720a 0000 0063 0000 0000  ......r....c....
-00000400: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000410: 4000 0000 7370 0000 0065 005a 0164 005a  @...sp...e.Z.d.Z
-00000420: 0265 0364 0164 0264 038d 0265 0464 0183  .e.d.d.d...e.d..
-00000430: 0183 015a 0565 0364 0464 0264 038d 0265  ...Z.e.d.d.d...e
-00000440: 0464 0483 0183 015a 0665 0364 0564 0264  .d.....Z.e.d.d.d
-00000450: 038d 0265 0464 0583 0183 015a 0765 0364  ...e.d.....Z.e.d
-00000460: 0664 0264 038d 0265 0464 0683 0183 015a  .d.d...e.d.....Z
-00000470: 0865 0364 0764 0264 038d 0265 0964 0783  .e.d.d.d...e.d..
-00000480: 0183 015a 0a64 0853 0029 0972 0b00 0000  ...Z.d.S.).r....
-00000490: 720d 0000 0054 2901 da0b 616c 6c6f 775f  r....T)...allow_
-000004a0: 7265 7573 6572 0e00 0000 720f 0000 0072  reuser....r....r
-000004b0: 1000 0000 7212 0000 004e 290b 7213 0000  ....r....N).r...
-000004c0: 0072 1400 0000 7215 0000 0072 0500 0000  .r....r....r....
-000004d0: 7208 0000 00da 0b5f 7072 6f6a 6563 745f  r......_project_
-000004e0: 6964 da11 5f69 6e70 7574 5f64 6174 6173  id.._input_datas
-000004f0: 6574 5f69 64da 125f 6f75 7470 7574 5f64  et_id.._output_d
-00000500: 6174 6173 6574 5f69 64da 0c5f 776f 726b  ataset_id.._work
-00000510: 666c 6f77 5f69 6472 0900 0000 da0c 5f77  flow_idr......_w
-00000520: 6f72 6b65 725f 696e 6974 721b 0000 0072  orker_initr....r
-00000530: 1b00 0000 721b 0000 0072 1c00 0000 720b  ....r....r....r.
-00000540: 0000 0028 0000 0073 2000 0000 0800 0a03  ...(...s .......
-00000550: 0601 04ff 0a03 0601 04ff 0a03 0601 04ff  ................
-00000560: 0a03 0601 04ff 0a03 0601 08ff 720b 0000  ............r...
-00000570: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000580: 0000 0300 0000 4000 0000 7362 0000 0065  ......@...sb...e
-00000590: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
-000005a0: 0065 0565 0464 023c 0065 0665 0464 033c  .e.e.d.<.e.e.d.<
-000005b0: 0065 0765 0619 0065 0464 043c 0065 0765  .e.e...e.d.<.e.e
-000005c0: 0865 0619 0019 0065 0464 053c 0065 0765  .e.....e.d.<.e.e
-000005d0: 0619 0065 0464 063c 0065 0765 0619 0065  ...e.d.<.e.e...e
-000005e0: 0464 073c 0064 0864 0984 005a 0964 0a53  .d.<.d.d...Z.d.S
-000005f0: 0029 0b72 0c00 0000 da02 6964 da0f 7374  .).r......id..st
-00000600: 6172 745f 7469 6d65 7374 616d 70da 0673  art_timestamp..s
-00000610: 7461 7475 73da 036c 6f67 da07 6869 7374  tatus..log..hist
-00000620: 6f72 79da 0b77 6f72 6b69 6e67 5f64 6972  ory..working_dir
-00000630: da10 776f 726b 696e 675f 6469 725f 7573  ..working_dir_us
-00000640: 6572 6301 0000 0000 0000 0000 0000 0002  erc.............
-00000650: 0000 0003 0000 0043 0000 0073 1a00 0000  .......C...s....
-00000660: 7c00 a000 a100 7d01 7401 7c00 6a02 8301  |.....}.t.|.j...
-00000670: 7c01 6401 3c00 7c01 5300 2902 4e72 2400  |.d.<.|.S.).Nr$.
-00000680: 0000 2903 da04 6469 6374 721a 0000 0072  ..)...dictr....r
-00000690: 2400 0000 2902 da04 7365 6c66 da01 6472  $...)...self..dr
-000006a0: 1b00 0000 721b 0000 0072 1c00 0000 da0e  ....r....r......
-000006b0: 7361 6e69 7469 7365 645f 6469 6374 4500  sanitised_dictE.
-000006c0: 0000 7306 0000 0008 010e 0104 017a 2041  ..s..........z A
-000006d0: 7070 6c79 576f 726b 666c 6f77 5265 6164  pplyWorkflowRead
-000006e0: 2e73 616e 6974 6973 6564 5f64 6963 744e  .sanitised_dictN
-000006f0: 290a 7213 0000 0072 1400 0000 7215 0000  ).r....r....r...
-00000700: 0072 1700 0000 7218 0000 0072 0200 0000  .r....r....r....
-00000710: 721a 0000 0072 0400 0000 7203 0000 0072  r....r....r....r
-00000720: 2d00 0000 721b 0000 0072 1b00 0000 721b  -...r....r....r.
-00000730: 0000 0072 1c00 0000 720c 0000 003c 0000  ...r....r....<..
-00000740: 0073 1200 0000 0a00 0801 0801 0801 0c01  .s..............
-00000750: 1001 0c01 0c01 0c02 720c 0000 004e 290f  ........r....N).
-00000760: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
-00000770: 0000 7204 0000 00da 0870 7964 616e 7469  ..r......pydanti
-00000780: 6372 0500 0000 da08 7371 6c6d 6f64 656c  cr......sqlmodel
-00000790: 7206 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
-000007a0: 7273 7208 0000 0072 0900 0000 da07 5f5f  rsr....r......__
-000007b0: 616c 6c5f 5f72 0a00 0000 720b 0000 0072  all__r....r....r
-000007c0: 0c00 0000 721b 0000 0072 1b00 0000 721b  ....r....r....r.
-000007d0: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000007e0: 653e 0100 0000 7316 0000 000c 000c 010c  e>....s.........
-000007f0: 010c 020c 010c 020c 0104 0210 0710 1614  ................
-00000800: 14                                       .
+00000070: 6d09 5a09 0100 6408 5a0a 4700 6409 640a  m.Z...d.Z.G.d.d.
+00000080: 8400 640a 6507 8303 5a0b 4700 640b 640c  ..d.e...Z.G.d.d.
+00000090: 8400 640c 650b 8303 5a0c 4700 640d 640e  ..d.e...Z.G.d.d.
+000000a0: 8400 640e 650b 8303 5a0d 640f 5300 2910  ..d.e...Z.d.S.).
+000000b0: e900 0000 0029 01da 0864 6174 6574 696d  .....)...datetim
+000000c0: 6529 01da 044c 6973 7429 01da 084f 7074  e)...List)...Opt
+000000d0: 696f 6e61 6c29 01da 0976 616c 6964 6174  ional)...validat
+000000e0: 6f72 2901 da08 5351 4c4d 6f64 656c e901  or)...SQLModel..
+000000f0: 0000 0029 01da 0676 616c 7374 7229 03da  ...)...valstr)..
+00000100: 1141 7070 6c79 576f 726b 666c 6f77 4261  .ApplyWorkflowBa
+00000110: 7365 da13 4170 706c 7957 6f72 6b66 6c6f  se..ApplyWorkflo
+00000120: 7743 7265 6174 65da 1141 7070 6c79 576f  wCreate..ApplyWo
+00000130: 726b 666c 6f77 5265 6164 6300 0000 0000  rkflowReadc.....
+00000140: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000150: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000160: 5500 6401 5a03 6504 6505 1900 6506 6402  U.d.Z.e.e...e.d.
+00000170: 3c00 6403 5300 2904 7209 0000 007a 500a  <.d.S.).r....zP.
+00000180: 2020 2020 4261 7365 2063 6c61 7373 2066      Base class f
+00000190: 6f72 2041 7070 6c79 576f 726b 666c 6f77  or ApplyWorkflow
+000001a0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+000001b0: 3a0a 2020 2020 2020 2020 776f 726b 6572  :.        worker
+000001c0: 5f69 6e69 743a 2054 4244 0a20 2020 20da  _init: TBD.    .
+000001d0: 0b77 6f72 6b65 725f 696e 6974 4e29 07da  .worker_initN)..
+000001e0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000001f0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000200: 655f 5fda 075f 5f64 6f63 5f5f 7204 0000  e__..__doc__r...
+00000210: 00da 0373 7472 da0f 5f5f 616e 6e6f 7461  ...str..__annota
+00000220: 7469 6f6e 735f 5fa9 0072 1300 0000 7213  tions__..r....r.
+00000230: 0000 00fa 532f 686f 6d65 2f74 6f6d 6d61  ....S/home/tomma
+00000240: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
+00000250: 616c 2d73 6572 7665 722f 6672 6163 7461  al-server/fracta
+00000260: 6c5f 7365 7276 6572 2f63 6f6d 6d6f 6e2f  l_server/common/
+00000270: 7363 6865 6d61 732f 6170 706c 7977 6f72  schemas/applywor
+00000280: 6b66 6c6f 772e 7079 7209 0000 0011 0000  kflow.pyr.......
+00000290: 0073 0600 0000 0a00 0401 1007 7209 0000  .s..........r...
+000002a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000002b0: 0000 0400 0000 4000 0000 7320 0000 0065  ......@...s ...e
+000002c0: 005a 0164 005a 0265 0364 0164 0264 038d  .Z.d.Z.e.d.d.d..
+000002d0: 0265 0464 0183 0183 015a 0564 0453 0029  .e.d.....Z.d.S.)
+000002e0: 0572 0a00 0000 720c 0000 0054 2901 da0b  .r....r....T)...
+000002f0: 616c 6c6f 775f 7265 7573 654e 2906 720d  allow_reuseN).r.
+00000300: 0000 0072 0e00 0000 720f 0000 0072 0500  ...r....r....r..
+00000310: 0000 7208 0000 00da 0c5f 776f 726b 6572  ..r......_worker
+00000320: 5f69 6e69 7472 1300 0000 7213 0000 0072  _initr....r....r
+00000330: 1300 0000 7214 0000 0072 0a00 0000 1c00  ....r....r......
+00000340: 0000 7308 0000 0008 000a 0306 0108 ff72  ..s............r
+00000350: 0a00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000360: 0000 0000 0003 0000 0040 0000 0073 8e00  .........@...s..
+00000370: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000380: 6401 3c00 6503 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
+00000390: 6403 3c00 6503 6504 6404 3c00 6503 6504  d.<.e.e.d.<.e.e.
+000003a0: 6405 3c00 6505 6504 6406 3c00 6506 6505  d.<.e.e.d.<.e.e.
+000003b0: 1900 6504 6407 3c00 6507 6504 6408 3c00  ..e.d.<.e.e.d.<.
+000003c0: 6506 6507 1900 6504 6409 3c00 6506 6508  e.e...e.d.<.e.e.
+000003d0: 6507 1900 1900 6504 640a 3c00 6506 6507  e.....e.d.<.e.e.
+000003e0: 1900 6504 640b 3c00 6506 6507 1900 6504  ..e.d.<.e.e...e.
+000003f0: 640c 3c00 640d 640e 8400 5a09 640f 5300  d.<.d.d...Z.d.S.
+00000400: 2910 720b 0000 00da 0269 64da 0a70 726f  ).r......id..pro
+00000410: 6a65 6374 5f69 64da 0b77 6f72 6b66 6c6f  ject_id..workflo
+00000420: 775f 6964 da10 696e 7075 745f 6461 7461  w_id..input_data
+00000430: 7365 745f 6964 da11 6f75 7470 7574 5f64  set_id..output_d
+00000440: 6174 6173 6574 5f69 64da 0f73 7461 7274  ataset_id..start
+00000450: 5f74 696d 6573 7461 6d70 da0d 656e 645f  _timestamp..end_
+00000460: 7469 6d65 7374 616d 70da 0673 7461 7475  timestamp..statu
+00000470: 73da 036c 6f67 da07 6869 7374 6f72 79da  s..log..history.
+00000480: 0b77 6f72 6b69 6e67 5f64 6972 da10 776f  .working_dir..wo
+00000490: 726b 696e 675f 6469 725f 7573 6572 6301  rking_dir_userc.
+000004a0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000004b0: 0000 0043 0000 0073 2800 0000 7c00 a000  ...C...s(...|...
+000004c0: a100 7d01 7401 7c00 6a02 8301 7c01 6401  ..}.t.|.j...|.d.
+000004d0: 3c00 7401 7c00 6a03 8301 7c01 6402 3c00  <.t.|.j...|.d.<.
+000004e0: 7c01 5300 2903 4e72 1c00 0000 721d 0000  |.S.).Nr....r...
+000004f0: 0029 04da 0464 6963 7472 1100 0000 721c  .)...dictr....r.
+00000500: 0000 0072 1d00 0000 2902 da04 7365 6c66  ...r....)...self
+00000510: da01 6472 1300 0000 7213 0000 0072 1400  ..dr....r....r..
+00000520: 0000 da0e 7361 6e69 7469 7365 645f 6469  ....sanitised_di
+00000530: 6374 3200 0000 7308 0000 0008 010e 010e  ct2...s.........
+00000540: 0104 017a 2041 7070 6c79 576f 726b 666c  ...z ApplyWorkfl
+00000550: 6f77 5265 6164 2e73 616e 6974 6973 6564  owRead.sanitised
+00000560: 5f64 6963 744e 290a 720d 0000 0072 0e00  _dictN).r....r..
+00000570: 0000 720f 0000 00da 0369 6e74 7212 0000  ..r......intr...
+00000580: 0072 0200 0000 7204 0000 0072 1100 0000  .r....r....r....
+00000590: 7203 0000 0072 2600 0000 7213 0000 0072  r....r&...r....r
+000005a0: 1300 0000 7213 0000 0072 1400 0000 720b  ....r....r....r.
+000005b0: 0000 0024 0000 0073 1c00 0000 0a00 0801  ...$...s........
+000005c0: 0801 0801 0801 0801 0801 0c01 0801 0c01  ................
+000005d0: 1001 0c01 0c01 0c02 720b 0000 004e 290e  ........r....N).
+000005e0: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
+000005f0: 0000 7204 0000 00da 0870 7964 616e 7469  ..r......pydanti
+00000600: 6372 0500 0000 da08 7371 6c6d 6f64 656c  cr......sqlmodel
+00000610: 7206 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
+00000620: 7273 7208 0000 00da 075f 5f61 6c6c 5f5f  rsr......__all__
+00000630: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00000640: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00000650: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000660: 0073 1400 0000 0c00 0c01 0c01 0c02 0c01  .s..............
+00000670: 0c02 0402 1007 100b 1408                 ..........
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 10:08:09 2023 UTC, .py size: 4484 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 891b 5a64 8411 0000  o.........Zd....
+00000000: 6f0d 0d0a 0000 0000 6e2d 5a64 e310 0000  o.......n-Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -216,99 +216,94 @@
 00000d70: 5442 440a 2020 2020 2020 2020 7061 636b  TBD.        pack
 00000d80: 6167 655f 6578 7472 6173 3a20 5442 440a  age_extras: TBD.
 00000d90: 2020 2020 da07 7061 636b 6167 65da 0776      ..package..v
 00000da0: 6572 7369 6f6e 4eda 0e70 7974 686f 6e5f  ersionN..python_
 00000db0: 7665 7273 696f 6eda 0e70 6163 6b61 6765  version..package
 00000dc0: 5f65 7874 7261 7363 0200 0000 0000 0000  _extrasc........
 00000dd0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00000de0: 7340 0000 0064 017c 0176 0072 1e74 007c  s@...d.|.v.r.t.|
+00000de0: 732a 0000 0064 017c 0176 0072 1374 007c  s*...d.|.v.r.t.|
 00000df0: 0183 017d 027c 02a0 01a1 0073 1374 0264  ...}.|.....s.t.d
-00000e00: 027c 029b 009d 0283 0182 017c 02a0 03a1  .|.........|....
-00000e10: 0073 1e74 0264 037c 029b 009d 0283 0182  .s.t.d.|........
-00000e20: 017c 0153 0029 044e fa01 2f7a 1f50 6163  .|.S.).N../z.Pac
-00000e30: 6b61 6765 2070 6174 6820 6d75 7374 2062  kage path must b
-00000e40: 6520 6162 736f 6c75 7465 3a20 7a1d 5061  e absolute: z.Pa
-00000e50: 636b 6167 6520 6669 6c65 2064 6f65 7320  ckage file does 
-00000e60: 6e6f 7420 6578 6973 743a 2029 0472 0200  not exist: ).r..
-00000e70: 0000 da0b 6973 5f61 6273 6f6c 7574 65da  ....is_absolute.
-00000e80: 0a56 616c 7565 4572 726f 72da 0665 7869  .ValueError..exi
-00000e90: 7374 7329 03da 0363 6c73 da05 7661 6c75  sts)...cls..valu
-00000ea0: 65da 0c70 6163 6b61 6765 5f70 6174 6872  e..package_pathr
-00000eb0: 1e00 0000 721e 0000 0072 1f00 0000 da15  ....r....r......
+00000e00: 027c 029b 009d 0283 0182 017c 0153 0029  .|.........|.S.)
+00000e10: 034e fa01 2f7a 1f50 6163 6b61 6765 2070  .N../z.Package p
+00000e20: 6174 6820 6d75 7374 2062 6520 6162 736f  ath must be abso
+00000e30: 6c75 7465 3a20 2903 7202 0000 00da 0b69  lute: ).r......i
+00000e40: 735f 6162 736f 6c75 7465 da0a 5661 6c75  s_absolute..Valu
+00000e50: 6545 7272 6f72 2903 da03 636c 73da 0576  eError)...cls..v
+00000e60: 616c 7565 da0c 7061 636b 6167 655f 7061  alue..package_pa
+00000e70: 7468 721e 0000 0072 1e00 0000 721f 0000  thr....r....r...
+00000e80: 00da 1570 6163 6b61 6765 5f70 6174 685f  ...package_path_
+00000e90: 6162 736f 6c75 7465 8400 0000 730e 0000  absolute....s...
+00000ea0: 0008 0208 0108 0102 0108 0104 ff04 037a  ...............z
+00000eb0: 2454 6173 6b43 6f6c 6c65 6374 5069 702e  $TaskCollectPip.
 00000ec0: 7061 636b 6167 655f 7061 7468 5f61 6273  package_path_abs
-00000ed0: 6f6c 7574 6584 0000 0073 1600 0000 0802  olute....s......
-00000ee0: 0801 0801 0201 0801 04ff 0803 0201 0801  ................
-00000ef0: 04ff 0403 7a24 5461 736b 436f 6c6c 6563  ....z$TaskCollec
-00000f00: 7450 6970 2e70 6163 6b61 6765 5f70 6174  tPip.package_pat
-00000f10: 685f 6162 736f 6c75 7465 290a 7218 0000  h_absolute).r...
-00000f20: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000f30: 721c 0000 0072 1d00 0000 7207 0000 0072  r....r....r....r
-00000f40: 3600 0000 7209 0000 0072 3f00 0000 721e  6...r....r?...r.
-00000f50: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-00000f60: 0000 7213 0000 0074 0000 0073 1000 0000  ..r....t...s....
-00000f70: 0a00 0401 080a 0c01 1001 0c01 0602 0e01  ................
-00000f80: 7213 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000f90: 0000 0000 0000 0300 0000 4000 0000 7368  ..........@...sh
-00000fa0: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000fb0: 0365 0464 0219 0065 0564 033c 0065 0665  .e.d...e.d.<.e.e
-00000fc0: 0564 043c 0065 0765 0564 053c 0065 0867  .d.<.e.e.d.<.e.g
-00000fd0: 0064 068d 015a 0965 0a65 0b65 0c19 0019  .d...Z.e.e.e....
-00000fe0: 0065 0564 073c 0065 0a65 0619 0065 0564  .e.d.<.e.e...e.d
-00000ff0: 083c 0065 0a65 0619 0065 0564 093c 0064  .<.e.e...e.d.<.d
-00001000: 0a64 0b84 005a 0d64 0c53 0029 0d72 1400  .d...Z.d.S.).r..
-00001010: 0000 7aac 0a20 2020 2054 6173 6b43 6f6c  ..z..    TaskCol
-00001020: 6c65 6374 5374 6174 7573 2063 6c61 7373  lectStatus class
-00001030: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
-00001040: 3a0a 2020 2020 2020 2020 7374 6174 7573  :.        status
-00001050: 3a20 5442 440a 2020 2020 2020 2020 7061  : TBD.        pa
-00001060: 636b 6167 653a 2054 4244 0a20 2020 2020  ckage: TBD.     
-00001070: 2020 2076 656e 765f 7061 7468 3a20 5442     venv_path: TB
-00001080: 440a 2020 2020 2020 2020 7461 736b 5f6c  D.        task_l
-00001090: 6973 743a 2054 4244 0a20 2020 2020 2020  ist: TBD.       
-000010a0: 206c 6f67 3a20 5442 440a 2020 2020 2020   log: TBD.      
-000010b0: 2020 696e 666f 3a20 5442 440a 2020 2020    info: TBD.    
-000010c0: 2905 da07 7065 6e64 696e 67da 0a69 6e73  )...pending..ins
-000010d0: 7461 6c6c 696e 67da 0a63 6f6c 6c65 6374  talling..collect
-000010e0: 696e 67da 0466 6169 6cda 024f 4bda 0673  ing..fail..OK..s
-000010f0: 7461 7475 7372 3400 0000 da09 7665 6e76  tatusr4.....venv
-00001100: 5f70 6174 6872 3000 0000 da09 7461 736b  _pathr0.....task
-00001110: 5f6c 6973 74da 036c 6f67 da04 696e 666f  _list..log..info
-00001120: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001130: 0003 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
-00001140: a000 a100 7d01 7401 7c00 6a02 8301 7c01  ....}.t.|.j...|.
-00001150: 6401 3c00 7c01 5300 2902 7a51 0a20 2020  d.<.|.S.).zQ.   
-00001160: 2020 2020 2052 6574 7572 6e20 6073 656c       Return `sel
-00001170: 662e 6469 6374 2829 6020 6166 7465 7220  f.dict()` after 
-00001180: 6361 7374 696e 6720 6073 656c 662e 7665  casting `self.ve
-00001190: 6e76 5f70 6174 6860 2074 6f20 6120 7374  nv_path` to a st
-000011a0: 7269 6e67 0a20 2020 2020 2020 2072 4600  ring.        rF.
-000011b0: 0000 2903 da04 6469 6374 721c 0000 0072  ..)...dictr....r
-000011c0: 4600 0000 2902 da04 7365 6c66 da01 6472  F...)...self..dr
-000011d0: 1e00 0000 721e 0000 0072 1f00 0000 da0e  ....r....r......
-000011e0: 7361 6e69 7469 7365 645f 6469 6374 a700  sanitised_dict..
-000011f0: 0000 7306 0000 0008 040e 0104 017a 2054  ..s..........z T
-00001200: 6173 6b43 6f6c 6c65 6374 5374 6174 7573  askCollectStatus
-00001210: 2e73 616e 6974 6973 6564 5f64 6963 744e  .sanitised_dictN
-00001220: 290e 7218 0000 0072 1900 0000 721a 0000  ).r....r....r...
-00001230: 0072 1b00 0000 7206 0000 0072 1d00 0000  .r....r....r....
-00001240: 721c 0000 0072 0200 0000 720a 0000 0072  r....r....r....r
-00001250: 4700 0000 7207 0000 0072 0500 0000 7210  G...r....r....r.
-00001260: 0000 0072 4d00 0000 721e 0000 0072 1e00  ...rM...r....r..
-00001270: 0000 721e 0000 0072 1f00 0000 7214 0000  ..r....r....r...
-00001280: 0093 0000 0073 1200 0000 0a00 0401 0c0c  .....s..........
-00001290: 0801 0801 1a01 0c01 0c01 0c02 7214 0000  ............r...
-000012a0: 004e 291a da07 7061 7468 6c69 6272 0200  .N)...pathlibr..
-000012b0: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
-000012c0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-000012d0: 0000 00da 0870 7964 616e 7469 6372 0800  .....pydanticr..
-000012e0: 0000 7209 0000 00da 0873 716c 6d6f 6465  ..r......sqlmode
-000012f0: 6c72 0a00 0000 720b 0000 00da 0b5f 7661  lr....r......_va
-00001300: 6c69 6461 746f 7273 720d 0000 00da 075f  lidatorsr......_
-00001310: 5f61 6c6c 5f5f 7215 0000 0072 0f00 0000  _all__r....r....
-00001320: 7211 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
-00001330: 0e00 0000 7233 0000 0072 1300 0000 7214  ....r3...r....r.
-00001340: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
-00001350: 0000 721f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001360: 3e01 0000 0073 2a00 0000 0c00 0c01 0c01  >....s*.........
-00001370: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c02  ................
-00001380: 0402 100b 101c 1015 1005 1004 1009 1013  ................
-00001390: 1004 141f                                ....
+00000ed0: 6f6c 7574 6529 0a72 1800 0000 7219 0000  olute).r....r...
+00000ee0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000ef0: 721d 0000 0072 0700 0000 7236 0000 0072  r....r....r6...r
+00000f00: 0900 0000 723e 0000 0072 1e00 0000 721e  ....r>...r....r.
+00000f10: 0000 0072 1e00 0000 721f 0000 0072 1300  ...r....r....r..
+00000f20: 0000 7400 0000 7310 0000 000a 0004 0108  ..t...s.........
+00000f30: 0a0c 0110 010c 0106 020e 0172 1300 0000  ...........r....
+00000f40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000f50: 0003 0000 0040 0000 0073 6800 0000 6500  .....@...sh...e.
+00000f60: 5a01 6400 5a02 5500 6401 5a03 6504 6402  Z.d.Z.U.d.Z.e.d.
+00000f70: 1900 6505 6403 3c00 6506 6505 6404 3c00  ..e.d.<.e.e.d.<.
+00000f80: 6507 6505 6405 3c00 6508 6700 6406 8d01  e.e.d.<.e.g.d...
+00000f90: 5a09 650a 650b 650c 1900 1900 6505 6407  Z.e.e.e.....e.d.
+00000fa0: 3c00 650a 6506 1900 6505 6408 3c00 650a  <.e.e...e.d.<.e.
+00000fb0: 6506 1900 6505 6409 3c00 640a 640b 8400  e...e.d.<.d.d...
+00000fc0: 5a0d 640c 5300 290d 7214 0000 007a ac0a  Z.d.S.).r....z..
+00000fd0: 2020 2020 5461 736b 436f 6c6c 6563 7453      TaskCollectS
+00000fe0: 7461 7475 7320 636c 6173 730a 0a20 2020  tatus class..   
+00000ff0: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
+00001000: 2020 2020 2073 7461 7475 733a 2054 4244       status: TBD
+00001010: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
+00001020: 3a20 5442 440a 2020 2020 2020 2020 7665  : TBD.        ve
+00001030: 6e76 5f70 6174 683a 2054 4244 0a20 2020  nv_path: TBD.   
+00001040: 2020 2020 2074 6173 6b5f 6c69 7374 3a20       task_list: 
+00001050: 5442 440a 2020 2020 2020 2020 6c6f 673a  TBD.        log:
+00001060: 2054 4244 0a20 2020 2020 2020 2069 6e66   TBD.        inf
+00001070: 6f3a 2054 4244 0a20 2020 2029 05da 0770  o: TBD.    )...p
+00001080: 656e 6469 6e67 da0a 696e 7374 616c 6c69  ending..installi
+00001090: 6e67 da0a 636f 6c6c 6563 7469 6e67 da04  ng..collecting..
+000010a0: 6661 696c da02 4f4b da06 7374 6174 7573  fail..OK..status
+000010b0: 7234 0000 00da 0976 656e 765f 7061 7468  r4.....venv_path
+000010c0: 7230 0000 00da 0974 6173 6b5f 6c69 7374  r0.....task_list
+000010d0: da03 6c6f 67da 0469 6e66 6f63 0100 0000  ..log..infoc....
+000010e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000010f0: 4300 0000 731a 0000 007c 00a0 00a1 007d  C...s....|.....}
+00001100: 0174 017c 006a 0283 017c 0164 013c 007c  .t.|.j...|.d.<.|
+00001110: 0153 0029 027a 510a 2020 2020 2020 2020  .S.).zQ.        
+00001120: 5265 7475 726e 2060 7365 6c66 2e64 6963  Return `self.dic
+00001130: 7428 2960 2061 6674 6572 2063 6173 7469  t()` after casti
+00001140: 6e67 2060 7365 6c66 2e76 656e 765f 7061  ng `self.venv_pa
+00001150: 7468 6020 746f 2061 2073 7472 696e 670a  th` to a string.
+00001160: 2020 2020 2020 2020 7245 0000 0029 03da          rE...)..
+00001170: 0464 6963 7472 1c00 0000 7245 0000 0029  .dictr....rE...)
+00001180: 02da 0473 656c 66da 0164 721e 0000 0072  ...self..dr....r
+00001190: 1e00 0000 721f 0000 00da 0e73 616e 6974  ....r......sanit
+000011a0: 6973 6564 5f64 6963 74a3 0000 0073 0600  ised_dict....s..
+000011b0: 0000 0804 0e01 0401 7a20 5461 736b 436f  ........z TaskCo
+000011c0: 6c6c 6563 7453 7461 7475 732e 7361 6e69  llectStatus.sani
+000011d0: 7469 7365 645f 6469 6374 4e29 0e72 1800  tised_dictN).r..
+000011e0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+000011f0: 0072 0600 0000 721d 0000 0072 1c00 0000  .r....r....r....
+00001200: 7202 0000 0072 0a00 0000 7246 0000 0072  r....r....rF...r
+00001210: 0700 0000 7205 0000 0072 1000 0000 724c  ....r....r....rL
+00001220: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
+00001230: 0000 721f 0000 0072 1400 0000 8f00 0000  ..r....r........
+00001240: 7312 0000 000a 0004 010c 0c08 0108 011a  s...............
+00001250: 010c 010c 010c 0272 1400 0000 4e29 1ada  .......r....N)..
+00001260: 0770 6174 686c 6962 7202 0000 00da 0674  .pathlibr......t
+00001270: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
+00001280: 0500 0000 7206 0000 0072 0700 0000 da08  ....r....r......
+00001290: 7079 6461 6e74 6963 7208 0000 0072 0900  pydanticr....r..
+000012a0: 0000 da08 7371 6c6d 6f64 656c 720a 0000  ....sqlmodelr...
+000012b0: 0072 0b00 0000 da0b 5f76 616c 6964 6174  .r......_validat
+000012c0: 6f72 7372 0d00 0000 da07 5f5f 616c 6c5f  orsr......__all_
+000012d0: 5f72 1500 0000 720f 0000 0072 1100 0000  _r....r....r....
+000012e0: 7212 0000 0072 1000 0000 720e 0000 0072  r....r....r....r
+000012f0: 3300 0000 7213 0000 0072 1400 0000 721e  3...r....r....r.
+00001300: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+00001310: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001320: 732a 0000 000c 000c 010c 010c 010c 010c  s*..............
+00001330: 010c 020c 010c 010c 010c 0204 0210 0b10  ................
+00001340: 1c10 1510 0510 0410 0910 1310 0414 1b    ...............
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 998 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,71 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 e603 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 ed0c 5e64 d403 0000  o.........^d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6405 6407 6c07 6d09 5a09  m.Z...d.d.l.m.Z.
-00000070: 0100 6408 5a0a 4700 6409 640a 8400 640a  ..d.Z.G.d.d...d.
-00000080: 6504 6a0b 6500 6a0c 1900 8303 5a0d 4700  e.j.e.j.....Z.G.
-00000090: 640b 640c 8400 640c 6504 6a0e 8303 5a0f  d.d...d.e.j...Z.
-000000a0: 4700 640d 640e 8400 640e 6504 6a10 8303  G.d.d...d.e.j...
-000000b0: 5a11 6401 5300 290f e900 0000 004e 2901  Z.d.S.)......N).
-000000c0: da08 4f70 7469 6f6e 616c 2901 da07 7363  ..Optional)...sc
-000000d0: 6865 6d61 7329 01da 0976 616c 6964 6174  hemas)...validat
-000000e0: 6f72 e901 0000 0029 01da 1176 616c 5f61  or.....)...val_a
-000000f0: 6273 6f6c 7574 655f 7061 7468 2901 da06  bsolute_path)...
-00000100: 7661 6c73 7472 2903 da08 5573 6572 5265  valstr)...UserRe
-00000110: 6164 da0a 5573 6572 5570 6461 7465 da0a  ad..UserUpdate..
-00000120: 5573 6572 4372 6561 7465 6300 0000 0000  UserCreatec.....
-00000130: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000140: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
-00000150: 5500 6503 6504 1900 6505 6401 3c00 6503  U.e.e...e.d.<.e.
-00000160: 6504 1900 6505 6402 3c00 6403 5300 2904  e...e.d.<.d.S.).
-00000170: 7208 0000 00da 0a73 6c75 726d 5f75 7365  r......slurm_use
-00000180: 72da 0963 6163 6865 5f64 6972 4e29 06da  r..cache_dirN)..
-00000190: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000001a0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000001b0: 655f 5f72 0200 0000 da03 7374 72da 0f5f  e__r......str.._
-000001c0: 5f61 6e6e 6f74 6174 696f 6e73 5f5f a900  _annotations__..
-000001d0: 7212 0000 0072 1200 0000 fa4a 2f68 6f6d  r....r.....J/hom
-000001e0: 652f 746f 6d6d 6173 6f2f 4672 6163 7461  e/tommaso/Fracta
-000001f0: 6c2f 6672 6163 7461 6c2d 7365 7276 6572  l/fractal-server
-00000200: 2f66 7261 6374 616c 5f73 6572 7665 722f  /fractal_server/
-00000210: 636f 6d6d 6f6e 2f73 6368 656d 6173 2f75  common/schemas/u
-00000220: 7365 722e 7079 7208 0000 0012 0000 0073  ser.pyr........s
-00000230: 0600 0000 0a00 0c01 1001 7208 0000 0063  ..........r....c
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0400 0000 4000 0000 f34e 0000 0065 005a  ....@....N...e.Z
-00000260: 0164 005a 0255 0065 0365 0419 0065 0564  .d.Z.U.e.e...e.d
-00000270: 013c 0065 0365 0419 0065 0564 023c 0065  .<.e.e...e.d.<.e
-00000280: 0664 0164 0364 048d 0265 0764 0183 0183  .d.d.d...e.d....
-00000290: 015a 0865 0664 0264 0364 048d 0265 0964  .Z.e.d.d.d...e.d
-000002a0: 0283 0183 015a 0a64 0553 0029 0672 0900  .....Z.d.S.).r..
-000002b0: 0000 720b 0000 0072 0c00 0000 54a9 01da  ..r....r....T...
-000002c0: 0b61 6c6c 6f77 5f72 6575 7365 4ea9 0b72  .allow_reuseN..r
-000002d0: 0d00 0000 720e 0000 0072 0f00 0000 7202  ....r....r....r.
-000002e0: 0000 0072 1000 0000 7211 0000 0072 0400  ...r....r....r..
-000002f0: 0000 7207 0000 00da 0b5f 736c 7572 6d5f  ..r......_slurm_
-00000300: 7573 6572 7206 0000 00da 0a5f 6361 6368  userr......_cach
-00000310: 655f 6469 7272 1200 0000 7212 0000 0072  e_dirr....r....r
-00000320: 1200 0000 7213 0000 0072 0900 0000 1700  ....r....r......
-00000330: 0000 f312 0000 000a 000c 010c 010a 0306  ................
-00000340: 0104 ff0a 0306 0108 ff72 0900 0000 6300  .........r....c.
-00000350: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000360: 0000 0040 0000 0072 1400 0000 2906 720a  ...@...r....).r.
-00000370: 0000 0072 0b00 0000 720c 0000 0054 7215  ...r....r....Tr.
-00000380: 0000 004e 7217 0000 0072 1200 0000 7212  ...Nr....r....r.
-00000390: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
-000003a0: 0000 2400 0000 721a 0000 0072 0a00 0000  ..$...r....r....
-000003b0: 2912 da04 7575 6964 da06 7479 7069 6e67  )...uuid..typing
-000003c0: 7202 0000 00da 0d66 6173 7461 7069 5f75  r......fastapi_u
-000003d0: 7365 7273 7203 0000 00da 0870 7964 616e  sersr......pydan
-000003e0: 7469 6372 0400 0000 da0b 5f76 616c 6964  ticr......_valid
-000003f0: 6174 6f72 7372 0600 0000 7207 0000 00da  atorsr....r.....
-00000400: 075f 5f61 6c6c 5f5f da08 4261 7365 5573  .__all__..BaseUs
-00000410: 6572 da04 5555 4944 7208 0000 00da 0e42  er..UUIDr......B
-00000420: 6173 6555 7365 7255 7064 6174 6572 0900  aseUserUpdater..
-00000430: 0000 da0e 4261 7365 5573 6572 4372 6561  ....BaseUserCrea
-00000440: 7465 720a 0000 0072 1200 0000 7212 0000  ter....r....r...
-00000450: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
-00000460: 6475 6c65 3e01 0000 0073 1400 0000 0800  dule>....s......
-00000470: 0c01 0c02 0c01 0c02 0c01 0403 1807 1205  ................
-00000480: 160d                                     ..
+00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6404 6405 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
+00000060: 6406 6c06 6d08 5a08 0100 6407 5a09 4700  d.l.m.Z...d.Z.G.
+00000070: 6408 6409 8400 6409 6503 6a0a 650b 1900  d.d...d.e.j.e...
+00000080: 8303 5a0c 4700 640a 640b 8400 640b 6503  ..Z.G.d.d...d.e.
+00000090: 6a0d 8303 5a0e 4700 640c 640d 8400 640d  j...Z.G.d.d...d.
+000000a0: 6503 6a0f 8303 5a10 640e 5300 290f e900  e.j...Z.d.S.)...
+000000b0: 0000 0029 01da 084f 7074 696f 6e61 6c29  ...)...Optional)
+000000c0: 01da 0773 6368 656d 6173 2901 da09 7661  ...schemas)...va
+000000d0: 6c69 6461 746f 72e9 0100 0000 2901 da11  lidator.....)...
+000000e0: 7661 6c5f 6162 736f 6c75 7465 5f70 6174  val_absolute_pat
+000000f0: 6829 01da 0676 616c 7374 7229 03da 0855  h)...valstr)...U
+00000100: 7365 7252 6561 64da 0a55 7365 7255 7064  serRead..UserUpd
+00000110: 6174 65da 0a55 7365 7243 7265 6174 6563  ate..UserCreatec
+00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000130: 0300 0000 4000 0000 7326 0000 0065 005a  ....@...s&...e.Z
+00000140: 0164 005a 0255 0065 0365 0419 0065 0564  .d.Z.U.e.e...e.d
+00000150: 013c 0065 0365 0419 0065 0564 023c 0064  .<.e.e...e.d.<.d
+00000160: 0353 0029 0472 0800 0000 da0a 736c 7572  .S.).r......slur
+00000170: 6d5f 7573 6572 da09 6361 6368 655f 6469  m_user..cache_di
+00000180: 724e 2906 da08 5f5f 6e61 6d65 5f5f da0a  rN)...__name__..
+00000190: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000001a0: 616c 6e61 6d65 5f5f 7202 0000 00da 0373  alname__r......s
+000001b0: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
+000001c0: 735f 5fa9 0072 1200 0000 7212 0000 00fa  s__..r....r.....
+000001d0: 4a2f 686f 6d65 2f74 6f6d 6d61 736f 2f46  J/home/tommaso/F
+000001e0: 7261 6374 616c 2f66 7261 6374 616c 2d73  ractal/fractal-s
+000001f0: 6572 7665 722f 6672 6163 7461 6c5f 7365  erver/fractal_se
+00000200: 7276 6572 2f63 6f6d 6d6f 6e2f 7363 6865  rver/common/sche
+00000210: 6d61 732f 7573 6572 2e70 7972 0800 0000  mas/user.pyr....
+00000220: 1100 0000 7306 0000 000a 000c 0110 0172  ....s..........r
+00000230: 0800 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000240: 0000 0000 0004 0000 0040 0000 00f3 4e00  .........@....N.
+00000250: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000260: 1900 6505 6401 3c00 6503 6504 1900 6505  ..e.d.<.e.e...e.
+00000270: 6402 3c00 6506 6401 6403 6404 8d02 6507  d.<.e.d.d.d...e.
+00000280: 6401 8301 8301 5a08 6506 6402 6403 6404  d.....Z.e.d.d.d.
+00000290: 8d02 6509 6402 8301 8301 5a0a 6405 5300  ..e.d.....Z.d.S.
+000002a0: 2906 7209 0000 0072 0b00 0000 720c 0000  ).r....r....r...
+000002b0: 0054 a901 da0b 616c 6c6f 775f 7265 7573  .T....allow_reus
+000002c0: 654e a90b 720d 0000 0072 0e00 0000 720f  eN..r....r....r.
+000002d0: 0000 0072 0200 0000 7210 0000 0072 1100  ...r....r....r..
+000002e0: 0000 7204 0000 0072 0700 0000 da0b 5f73  ..r....r......_s
+000002f0: 6c75 726d 5f75 7365 7272 0600 0000 da0a  lurm_userr......
+00000300: 5f63 6163 6865 5f64 6972 7212 0000 0072  _cache_dirr....r
+00000310: 1200 0000 7212 0000 0072 1300 0000 7209  ....r....r....r.
+00000320: 0000 0016 0000 00f3 1200 0000 0a00 0c01  ................
+00000330: 0c01 0a03 0601 04ff 0a03 0601 08ff 7209  ..............r.
+00000340: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000350: 0000 0000 0400 0000 4000 0000 7214 0000  ........@...r...
+00000360: 0029 0672 0a00 0000 720b 0000 0072 0c00  .).r....r....r..
+00000370: 0000 5472 1500 0000 4e72 1700 0000 7212  ..Tr....Nr....r.
+00000380: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000390: 0000 720a 0000 0023 0000 0072 1a00 0000  ..r....#...r....
+000003a0: 720a 0000 004e 2911 da06 7479 7069 6e67  r....N)...typing
+000003b0: 7202 0000 00da 0d66 6173 7461 7069 5f75  r......fastapi_u
+000003c0: 7365 7273 7203 0000 00da 0870 7964 616e  sersr......pydan
+000003d0: 7469 6372 0400 0000 da0b 5f76 616c 6964  ticr......_valid
+000003e0: 6174 6f72 7372 0600 0000 7207 0000 00da  atorsr....r.....
+000003f0: 075f 5f61 6c6c 5f5f da08 4261 7365 5573  .__all__..BaseUs
+00000400: 6572 da03 696e 7472 0800 0000 da0e 4261  er..intr......Ba
+00000410: 7365 5573 6572 5570 6461 7465 7209 0000  seUserUpdater...
+00000420: 00da 0e42 6173 6555 7365 7243 7265 6174  ...BaseUserCreat
+00000430: 6572 0a00 0000 7212 0000 0072 1200 0000  er....r....r....
+00000440: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
+00000450: 756c 653e 0100 0000 7312 0000 000c 000c  ule>....s.......
+00000460: 020c 010c 020c 0104 0316 0712 0516 0d    ...............
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 10:08:09 2023 UTC, .py size: 2709 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 891b 5a64 950a 0000  o.........Zd....
+00000000: 6f0d 0d0a 0000 0000 6e2d 5a64 c609 0000  o.......n-Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -59,197 +59,190 @@
 000003a0: 7261 6374 616c 2f66 7261 6374 616c 2d73  ractal/fractal-s
 000003b0: 6572 7665 722f 6672 6163 7461 6c5f 7365  erver/fractal_se
 000003c0: 7276 6572 2f63 6f6d 6d6f 6e2f 7363 6865  rver/common/sche
 000003d0: 6d61 732f 776f 726b 666c 6f77 2e70 7972  mas/workflow.pyr
 000003e0: 1800 0000 1e00 0000 7306 0000 000a 0018  ........s.......
 000003f0: 021c 0172 1800 0000 6300 0000 0000 0000  ...r....c.......
 00000400: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00000410: 0073 4e00 0000 6500 5a01 6400 5a02 5500  .sN...e.Z.d.Z.U.
-00000420: 6503 6504 1900 6505 6401 3c00 6504 6505  e.e...e.d.<.e.e.
-00000430: 6402 3c00 6506 6401 6403 6404 8d02 6507  d.<.e.d.d.d...e.
-00000440: 6401 6405 6406 8d02 8301 5a08 6506 6402  d.d.d.....Z.e.d.
-00000450: 6403 6404 8d02 6507 6402 8301 8301 5a09  d.d...e.d.....Z.
-00000460: 6407 5300 2908 7213 0000 00da 056f 7264  d.S.).r......ord
-00000470: 6572 da07 7461 736b 5f69 6454 a901 da0b  er..task_idT....
-00000480: 616c 6c6f 775f 7265 7573 6572 0100 0000  allow_reuser....
-00000490: 2901 da07 6d69 6e5f 7661 6c4e 290a 721b  )...min_valN).r.
-000004a0: 0000 0072 1c00 0000 721d 0000 0072 0500  ...r....r....r..
-000004b0: 0000 da03 696e 7472 1f00 0000 7206 0000  ....intr....r...
-000004c0: 0072 0900 0000 da06 5f6f 7264 6572 da08  .r......_order..
-000004d0: 5f74 6173 6b5f 6964 7220 0000 0072 2000  _task_idr ...r .
-000004e0: 0000 7220 0000 0072 2100 0000 7213 0000  ..r ...r!...r...
-000004f0: 0024 0000 0073 0a00 0000 0a00 0c01 0801  .$...s..........
-00000500: 1802 1801 7213 0000 0063 0000 0000 0000  ....r....c......
-00000510: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000520: 0000 733a 0000 0065 005a 0164 005a 0255  ..s:...e.Z.d.Z.U
-00000530: 0065 0365 0464 013c 0065 0565 0319 0065  .e.e.d.<.e.e...e
-00000540: 0464 023c 0065 0365 0464 033c 0065 0365  .d.<.e.e.d.<.e.e
-00000550: 0464 043c 0065 0665 0464 053c 0064 0653  .d.<.e.e.d.<.d.S
-00000560: 0029 0772 1600 0000 da02 6964 7222 0000  .).r......idr"..
-00000570: 00da 0b77 6f72 6b66 6c6f 775f 6964 7223  ...workflow_idr#
-00000580: 0000 00da 0474 6173 6b4e 2907 721b 0000  .....taskN).r...
-00000590: 0072 1c00 0000 721d 0000 0072 2700 0000  .r....r....r'...
-000005a0: 721f 0000 0072 0500 0000 720d 0000 0072  r....r....r....r
-000005b0: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-000005c0: 0000 0072 1600 0000 2c00 0000 730c 0000  ...r....,...s...
-000005d0: 000a 0008 010c 0108 0108 010c 0172 1600  .............r..
-000005e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000005f0: 0000 0003 0000 0040 0000 00f3 1600 0000  .......@........
-00000600: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000610: 3c00 6402 5300 2903 7214 0000 0072 2c00  <.d.S.).r....r,.
-00000620: 0000 4e29 0572 1b00 0000 721c 0000 0072  ..N).r....r....r
-00000630: 1d00 0000 720c 0000 0072 1f00 0000 7220  ....r....r....r 
-00000640: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000650: 0000 7214 0000 0034 0000 00f3 0400 0000  ..r....4........
-00000660: 0a00 0c01 7214 0000 0063 0000 0000 0000  ....r....c......
-00000670: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000680: 0000 722d 0000 0029 0372 1500 0000 722c  ..r-...).r....r,
-00000690: 0000 004e 2905 721b 0000 0072 1c00 0000  ...N).r....r....
-000006a0: 721d 0000 0072 0b00 0000 721f 0000 0072  r....r....r....r
-000006b0: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-000006c0: 0000 0072 1500 0000 3800 0000 722e 0000  ...r....8...r...
-000006d0: 0072 1500 0000 6300 0000 0000 0000 0000  .r....c.........
-000006e0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000006f0: 1c00 0000 6500 5a01 6400 5a02 6503 6401  ....e.Z.d.Z.e.d.
-00000700: 8301 6402 6403 8400 8301 5a04 6404 5300  ..d.d.....Z.d.S.
-00000710: 2905 7217 0000 0072 1900 0000 6302 0000  ).r....r....c...
-00000720: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000730: 0043 0000 0073 1400 0000 6401 7c01 7600  .C...s....d.|.v.
-00000740: 7208 7400 6402 8301 8201 7c01 5300 2903  r.t.d.....|.S.).
-00000750: 4eda 1570 6172 616c 6c65 6c69 7a61 7469  N..parallelizati
-00000760: 6f6e 5f6c 6576 656c 7a3b 4f76 6572 7269  on_levelz;Overri
-00000770: 6469 6e67 2074 6173 6b20 7061 7261 6c6c  ding task parall
-00000780: 656c 697a 6174 696f 6e20 6c65 7665 6c20  elization level 
-00000790: 6375 7272 656e 746c 7920 6e6f 7420 616c  currently not al
-000007a0: 6c6f 7765 6429 01da 0a56 616c 7565 4572  lowed)...ValueEr
-000007b0: 726f 7229 02da 0363 6c73 da01 6d72 2000  ror)...cls..mr .
-000007c0: 0000 7220 0000 0072 2100 0000 da1e 6368  ..r ...r!.....ch
-000007d0: 6563 6b5f 6e6f 5f70 6172 616c 6c65 6c69  eck_no_paralleli
-000007e0: 7361 7469 6f6e 5f6c 6576 656c 3e00 0000  sation_level>...
-000007f0: 730a 0000 0008 0202 0102 0104 ff04 037a  s..............z
-00000800: 3157 6f72 6b66 6c6f 7754 6173 6b55 7064  1WorkflowTaskUpd
-00000810: 6174 652e 6368 6563 6b5f 6e6f 5f70 6172  ate.check_no_par
-00000820: 616c 6c65 6c69 7361 7469 6f6e 5f6c 6576  allelisation_lev
-00000830: 656c 4e29 0572 1b00 0000 721c 0000 0072  elN).r....r....r
-00000840: 1d00 0000 7206 0000 0072 3300 0000 7220  ....r....r3...r 
-00000850: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000860: 0000 7217 0000 003c 0000 0073 0600 0000  ..r....<...s....
-00000870: 0800 0602 0e01 7217 0000 0063 0000 0000  ......r....c....
-00000880: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000890: 4000 0000 722d 0000 0029 03da 0d5f 576f  @...r-...)..._Wo
-000008a0: 726b 666c 6f77 4261 7365 da04 6e61 6d65  rkflowBase..name
-000008b0: 4e29 0572 1b00 0000 721c 0000 0072 1d00  N).r....r....r..
-000008c0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-000008d0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-000008e0: 7234 0000 0047 0000 0072 2e00 0000 7234  r4...G...r....r4
-000008f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000900: 0000 0000 0300 0000 4000 0000 732a 0000  ........@...s*..
-00000910: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-00000920: 013c 0065 0365 0464 023c 0065 0565 0619  .<.e.e.d.<.e.e..
-00000930: 0065 0464 033c 0064 0453 0029 0572 0f00  .e.d.<.d.S.).r..
-00000940: 0000 722a 0000 00da 0a70 726f 6a65 6374  ..r*.....project
-00000950: 5f69 64da 0974 6173 6b5f 6c69 7374 4e29  _id..task_listN)
-00000960: 0772 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000970: 7227 0000 0072 1f00 0000 7204 0000 0072  r'...r....r....r
-00000980: 1600 0000 7220 0000 0072 2000 0000 7220  ....r ...r ...r 
-00000990: 0000 0072 2100 0000 720f 0000 004b 0000  ...r!...r....K..
-000009a0: 0073 0800 0000 0a00 0801 0801 1001 720f  .s............r.
-000009b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000009c0: 0000 0000 0400 0000 4000 0000 733e 0000  ........@...s>..
-000009d0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-000009e0: 013c 0065 0564 0264 0364 048d 0265 0664  .<.e.d.d.d...e.d
-000009f0: 0283 0183 015a 0765 0564 0164 0364 048d  .....Z.e.d.d.d..
-00000a00: 0265 0864 0183 0183 015a 0964 0553 0029  .e.d.....Z.d.S.)
-00000a10: 0672 0e00 0000 7236 0000 0072 3500 0000  .r....r6...r5...
-00000a20: 5472 2400 0000 4e29 0a72 1b00 0000 721c  Tr$...N).r....r.
-00000a30: 0000 0072 1d00 0000 7227 0000 0072 1f00  ...r....r'...r..
-00000a40: 0000 7206 0000 0072 0a00 0000 da05 5f6e  ..r....r......_n
-00000a50: 616d 6572 0900 0000 da0b 5f70 726f 6a65  amer......_proje
-00000a60: 6374 5f69 6472 2000 0000 7220 0000 0072  ct_idr ...r ...r
-00000a70: 2000 0000 7221 0000 0072 0e00 0000 5100   ...r!...r....Q.
-00000a80: 0000 730c 0000 000a 0008 0114 030a 0106  ..s.............
-00000a90: 0108 ff72 0e00 0000 6300 0000 0000 0000  ...r....c.......
-00000aa0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000ab0: 0073 4e00 0000 6500 5a01 6400 5a02 5500  .sN...e.Z.d.Z.U.
-00000ac0: 6503 6504 1900 6505 6401 3c00 6503 6506  e.e...e.d.<.e.e.
-00000ad0: 6507 1900 1900 6505 6402 3c00 6508 6401  e.....e.d.<.e.d.
-00000ae0: 6403 6404 8d02 6509 6401 8301 8301 5a0a  d.d...e.d.....Z.
-00000af0: 6508 6402 8301 6405 6406 8400 8301 5a0b  e.d...d.d.....Z.
-00000b00: 6407 5300 2908 7210 0000 0072 3500 0000  d.S.).r....r5...
-00000b10: da1a 7265 6f72 6465 7265 645f 776f 726b  ..reordered_work
-00000b20: 666c 6f77 7461 736b 5f69 6473 5472 2400  flowtask_idsTr$.
-00000b30: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000b40: 0000 0004 0000 0043 0000 0073 3a00 0000  .......C...s:...
-00000b50: 7400 6401 6402 8400 7c01 4400 8301 8301  t.d.d...|.D.....
-00000b60: 720d 7401 6403 8301 8201 7402 7c01 8301  r.t.d.....t.|...
-00000b70: 7402 7403 7c01 8301 8301 6b03 721b 7401  t.t.|.....k.r.t.
-00000b80: 6404 8301 8201 7c01 5300 2905 4e63 0100  d.....|.S.).Nc..
-00000b90: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000ba0: 0000 7300 0000 7318 0000 0081 007c 005d  ..s...s......|.]
-00000bb0: 077d 017c 0164 006b 0056 0001 0071 0264  .}.|.d.k.V...q.d
-00000bc0: 0153 0029 0272 0100 0000 4e72 2000 0000  .S.).r....Nr ...
-00000bd0: 2902 da02 2e30 da01 6972 2000 0000 7220  )....0..ir ...r 
-00000be0: 0000 0072 2100 0000 da09 3c67 656e 6578  ...r!.....<genex
-00000bf0: 7072 3e64 0000 0073 0400 0000 0280 1600  pr>d...s........
-00000c00: 7a3b 576f 726b 666c 6f77 5570 6461 7465  z;WorkflowUpdate
-00000c10: 2e63 6865 636b 5f70 6f73 6974 6976 655f  .check_positive_
-00000c20: 616e 645f 756e 6971 7565 2e3c 6c6f 6361  and_unique.<loca
-00000c30: 6c73 3e2e 3c67 656e 6578 7072 3e7a 2d4e  ls>.<genexpr>z-N
-00000c40: 6567 6174 6976 6520 6069 6460 2069 6e20  egative `id` in 
-00000c50: 6072 656f 7264 6572 6564 5f77 6f72 6b66  `reordered_workf
-00000c60: 6c6f 7774 6173 6b5f 6964 7360 7a2c 6072  lowtask_ids`z,`r
-00000c70: 656f 7264 6572 6564 5f77 6f72 6b66 6c6f  eordered_workflo
-00000c80: 7774 6173 6b5f 6964 7360 2068 6173 2072  wtask_ids` has r
-00000c90: 6570 6574 6974 696f 6e73 2904 da03 616e  epetitions)...an
-00000ca0: 7972 3000 0000 da03 6c65 6eda 0373 6574  yr0.....len..set
-00000cb0: 2902 7231 0000 00da 0576 616c 7565 7220  ).r1.....valuer 
-00000cc0: 0000 0072 2000 0000 7221 0000 00da 1963  ...r ...r!.....c
-00000cd0: 6865 636b 5f70 6f73 6974 6976 655f 616e  heck_positive_an
-00000ce0: 645f 756e 6971 7565 6200 0000 730a 0000  d_uniqueb...s...
-00000cf0: 0012 0208 0114 0108 0104 017a 2857 6f72  ...........z(Wor
-00000d00: 6b66 6c6f 7755 7064 6174 652e 6368 6563  kflowUpdate.chec
-00000d10: 6b5f 706f 7369 7469 7665 5f61 6e64 5f75  k_positive_and_u
-00000d20: 6e69 7175 654e 290c 721b 0000 0072 1c00  niqueN).r....r..
-00000d30: 0000 721d 0000 0072 0500 0000 721e 0000  ..r....r....r...
-00000d40: 0072 1f00 0000 7204 0000 0072 2700 0000  .r....r....r'...
-00000d50: 7206 0000 0072 0a00 0000 7238 0000 0072  r....r....r8...r
-00000d60: 4200 0000 7220 0000 0072 2000 0000 7220  B...r ...r ...r 
-00000d70: 0000 0072 2100 0000 7210 0000 005b 0000  ...r!...r....[..
-00000d80: 0073 0c00 0000 0a00 0c01 1001 1403 0602  .s..............
-00000d90: 0e01 7210 0000 0063 0000 0000 0000 0000  ..r....c........
-00000da0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000db0: 732e 0000 0065 005a 0164 005a 0255 0065  s....e.Z.d.Z.U.e
-00000dc0: 0365 0419 0065 0564 013c 0065 0664 0264  .e...e.d.<.e.d.d
-00000dd0: 0364 048d 0265 0764 0283 0183 015a 0864  .d...e.d.....Z.d
-00000de0: 0553 0029 0672 1100 0000 7237 0000 0072  .S.).r....r7...r
-00000df0: 3500 0000 5472 2400 0000 4e29 0972 1b00  5...Tr$...N).r..
-00000e00: 0000 721c 0000 0072 1d00 0000 7204 0000  ..r....r....r...
-00000e10: 0072 1400 0000 721f 0000 0072 0600 0000  .r....r....r....
-00000e20: 720a 0000 0072 3800 0000 7220 0000 0072  r....r8...r ...r
-00000e30: 2000 0000 7220 0000 0072 2100 0000 7211   ...r ...r!...r.
-00000e40: 0000 006b 0000 0073 0600 0000 0a00 0c01  ...k...s........
-00000e50: 1803 7211 0000 0063 0000 0000 0000 0000  ..r....c........
-00000e60: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000e70: 731a 0000 0065 005a 0164 005a 0255 0065  s....e.Z.d.Z.U.e
-00000e80: 0365 0419 0065 0564 013c 0064 0253 0029  .e...e.d.<.d.S.)
-00000e90: 0372 1200 0000 7237 0000 004e 2906 721b  .r....r7...N).r.
-00000ea0: 0000 0072 1c00 0000 721d 0000 0072 0400  ...r....r....r..
-00000eb0: 0000 7215 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000ec0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-00000ed0: 7212 0000 0072 0000 0073 0400 0000 0a00  r....r...s......
-00000ee0: 1001 7212 0000 004e 291d da06 7479 7069  ..r....N)...typi
-00000ef0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
-00000f00: 0072 0500 0000 da08 7079 6461 6e74 6963  .r......pydantic
-00000f10: 7206 0000 00da 0873 716c 6d6f 6465 6c72  r......sqlmodelr
-00000f20: 0700 0000 da0b 5f76 616c 6964 6174 6f72  ......_validator
-00000f30: 7372 0900 0000 720a 0000 0072 2c00 0000  sr....r....r,...
-00000f40: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000f50: 075f 5f61 6c6c 5f5f 7218 0000 0072 1300  .__all__r....r..
-00000f60: 0000 7216 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000f70: 0072 1700 0000 7234 0000 0072 0f00 0000  .r....r4...r....
-00000f80: 720e 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000f90: 1200 0000 7220 0000 0072 2000 0000 7220  ....r ...r ...r 
-00000fa0: 0000 0072 2100 0000 da08 3c6d 6f64 756c  ...r!.....<modul
-00000fb0: 653e 0100 0000 7330 0000 000c 000c 010c  e>....s0........
-00000fc0: 010c 010c 020c 010c 020c 010c 010c 010c  ................
-00000fd0: 0104 0310 0e10 0610 0810 0810 0410 0410  ................
-00000fe0: 0b10 0410 0610 0a10 1014 07              ...........
+00000410: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+00000420: 6503 6504 1900 6505 6401 3c00 6506 6401  e.e...e.d.<.e.d.
+00000430: 6402 6403 8d02 6507 6401 6404 6405 8d02  d.d...e.d.d.d...
+00000440: 8301 5a08 6406 5300 2907 7213 0000 00da  ..Z.d.S.).r.....
+00000450: 056f 7264 6572 54a9 01da 0b61 6c6c 6f77  .orderT....allow
+00000460: 5f72 6575 7365 7201 0000 0029 01da 076d  _reuser....)...m
+00000470: 696e 5f76 616c 4e29 0972 1b00 0000 721c  in_valN).r....r.
+00000480: 0000 0072 1d00 0000 7205 0000 00da 0369  ...r....r......i
+00000490: 6e74 721f 0000 0072 0600 0000 7209 0000  ntr....r....r...
+000004a0: 00da 065f 6f72 6465 7272 2000 0000 7220  ..._orderr ...r 
+000004b0: 0000 0072 2000 0000 7221 0000 0072 1300  ...r ...r!...r..
+000004c0: 0000 2400 0000 7306 0000 000a 000c 011c  ..$...s.........
+000004d0: 0272 1300 0000 6300 0000 0000 0000 0000  .r....c.........
+000004e0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+000004f0: 3a00 0000 6500 5a01 6400 5a02 5500 6503  :...e.Z.d.Z.U.e.
+00000500: 6504 6401 3c00 6505 6503 1900 6504 6402  e.d.<.e.e...e.d.
+00000510: 3c00 6503 6504 6403 3c00 6503 6504 6404  <.e.e.d.<.e.e.d.
+00000520: 3c00 6506 6504 6405 3c00 6406 5300 2907  <.e.e.d.<.d.S.).
+00000530: 7216 0000 00da 0269 6472 2200 0000 da0b  r......idr".....
+00000540: 776f 726b 666c 6f77 5f69 64da 0774 6173  workflow_id..tas
+00000550: 6b5f 6964 da04 7461 736b 4e29 0772 1b00  k_id..taskN).r..
+00000560: 0000 721c 0000 0072 1d00 0000 7226 0000  ..r....r....r&..
+00000570: 0072 1f00 0000 7205 0000 0072 0d00 0000  .r....r....r....
+00000580: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+00000590: 2100 0000 7216 0000 002a 0000 0073 0c00  !...r....*...s..
+000005a0: 0000 0a00 0801 0c01 0801 0801 0c01 7216  ..............r.
+000005b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000005c0: 0000 0000 0300 0000 4000 0000 f316 0000  ........@.......
+000005d0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
+000005e0: 013c 0064 0253 0029 0372 1400 0000 722b  .<.d.S.).r....r+
+000005f0: 0000 004e 2905 721b 0000 0072 1c00 0000  ...N).r....r....
+00000600: 721d 0000 0072 0c00 0000 721f 0000 0072  r....r....r....r
+00000610: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
+00000620: 0000 0072 1400 0000 3200 0000 f304 0000  ...r....2.......
+00000630: 000a 000c 0172 1400 0000 6300 0000 0000  .....r....c.....
+00000640: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000650: 0000 0072 2c00 0000 2903 7215 0000 0072  ...r,...).r....r
+00000660: 2b00 0000 4e29 0572 1b00 0000 721c 0000  +...N).r....r...
+00000670: 0072 1d00 0000 720b 0000 0072 1f00 0000  .r....r....r....
+00000680: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+00000690: 2100 0000 7215 0000 0036 0000 0072 2d00  !...r....6...r-.
+000006a0: 0000 7215 0000 0063 0000 0000 0000 0000  ..r....c........
+000006b0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000006c0: 731c 0000 0065 005a 0164 005a 0265 0364  s....e.Z.d.Z.e.d
+000006d0: 0183 0164 0264 0384 0083 015a 0464 0453  ...d.d.....Z.d.S
+000006e0: 0029 0572 1700 0000 7219 0000 0063 0200  .).r....r....c..
+000006f0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000700: 0000 4300 0000 7314 0000 0064 017c 0176  ..C...s....d.|.v
+00000710: 0072 0874 0064 0283 0182 017c 0153 0029  .r.t.d.....|.S.)
+00000720: 034e da15 7061 7261 6c6c 656c 697a 6174  .N..parallelizat
+00000730: 696f 6e5f 6c65 7665 6c7a 3b4f 7665 7272  ion_levelz;Overr
+00000740: 6964 696e 6720 7461 736b 2070 6172 616c  iding task paral
+00000750: 6c65 6c69 7a61 7469 6f6e 206c 6576 656c  lelization level
+00000760: 2063 7572 7265 6e74 6c79 206e 6f74 2061   currently not a
+00000770: 6c6c 6f77 6564 2901 da0a 5661 6c75 6545  llowed)...ValueE
+00000780: 7272 6f72 2902 da03 636c 73da 016d 7220  rror)...cls..mr 
+00000790: 0000 0072 2000 0000 7221 0000 00da 1e63  ...r ...r!.....c
+000007a0: 6865 636b 5f6e 6f5f 7061 7261 6c6c 656c  heck_no_parallel
+000007b0: 6973 6174 696f 6e5f 6c65 7665 6c3c 0000  isation_level<..
+000007c0: 0073 0a00 0000 0802 0201 0201 04ff 0403  .s..............
+000007d0: 7a31 576f 726b 666c 6f77 5461 736b 5570  z1WorkflowTaskUp
+000007e0: 6461 7465 2e63 6865 636b 5f6e 6f5f 7061  date.check_no_pa
+000007f0: 7261 6c6c 656c 6973 6174 696f 6e5f 6c65  rallelisation_le
+00000800: 7665 6c4e 2905 721b 0000 0072 1c00 0000  velN).r....r....
+00000810: 721d 0000 0072 0600 0000 7232 0000 0072  r....r....r2...r
+00000820: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
+00000830: 0000 0072 1700 0000 3a00 0000 7306 0000  ...r....:...s...
+00000840: 0008 0006 020e 0172 1700 0000 6300 0000  .......r....c...
+00000850: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000860: 0040 0000 0072 2c00 0000 2903 da0d 5f57  .@...r,...)..._W
+00000870: 6f72 6b66 6c6f 7742 6173 65da 046e 616d  orkflowBase..nam
+00000880: 654e 2905 721b 0000 0072 1c00 0000 721d  eN).r....r....r.
+00000890: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+000008a0: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+000008b0: 0072 3300 0000 4500 0000 722d 0000 0072  .r3...E...r-...r
+000008c0: 3300 0000 6300 0000 0000 0000 0000 0000  3...c...........
+000008d0: 0000 0000 0003 0000 0040 0000 0073 2a00  .........@...s*.
+000008e0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+000008f0: 6401 3c00 6503 6504 6402 3c00 6505 6506  d.<.e.e.d.<.e.e.
+00000900: 1900 6504 6403 3c00 6404 5300 2905 720f  ..e.d.<.d.S.).r.
+00000910: 0000 0072 2800 0000 da0a 7072 6f6a 6563  ...r(.....projec
+00000920: 745f 6964 da09 7461 736b 5f6c 6973 744e  t_id..task_listN
+00000930: 2907 721b 0000 0072 1c00 0000 721d 0000  ).r....r....r...
+00000940: 0072 2600 0000 721f 0000 0072 0400 0000  .r&...r....r....
+00000950: 7216 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
+00000960: 2000 0000 7221 0000 0072 0f00 0000 4900   ...r!...r....I.
+00000970: 0000 7308 0000 000a 0008 0108 0110 0172  ..s............r
+00000980: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000990: 0000 0000 0004 0000 0040 0000 0073 2000  .........@...s .
+000009a0: 0000 6500 5a01 6400 5a02 6503 6401 6402  ..e.Z.d.Z.e.d.d.
+000009b0: 6403 8d02 6504 6401 8301 8301 5a05 6404  d...e.d.....Z.d.
+000009c0: 5300 2905 720e 0000 0072 3400 0000 5472  S.).r....r4...Tr
+000009d0: 2300 0000 4e29 0672 1b00 0000 721c 0000  #...N).r....r...
+000009e0: 0072 1d00 0000 7206 0000 0072 0a00 0000  .r....r....r....
+000009f0: da05 5f6e 616d 6572 2000 0000 7220 0000  .._namer ...r ..
+00000a00: 0072 2000 0000 7221 0000 0072 0e00 0000  .r ...r!...r....
+00000a10: 4f00 0000 7304 0000 0008 0018 0272 0e00  O...s........r..
+00000a20: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000a30: 0000 0004 0000 0040 0000 0073 4e00 0000  .......@...sN...
+00000a40: 6500 5a01 6400 5a02 5500 6503 6504 1900  e.Z.d.Z.U.e.e...
+00000a50: 6505 6401 3c00 6503 6506 6507 1900 1900  e.d.<.e.e.e.....
+00000a60: 6505 6402 3c00 6508 6401 6403 6404 8d02  e.d.<.e.d.d.d...
+00000a70: 6509 6401 8301 8301 5a0a 6508 6402 8301  e.d.....Z.e.d...
+00000a80: 6405 6406 8400 8301 5a0b 6407 5300 2908  d.d.....Z.d.S.).
+00000a90: 7210 0000 0072 3400 0000 da1a 7265 6f72  r....r4.....reor
+00000aa0: 6465 7265 645f 776f 726b 666c 6f77 7461  dered_workflowta
+00000ab0: 736b 5f69 6473 5472 2300 0000 6302 0000  sk_idsTr#...c...
+00000ac0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000ad0: 0043 0000 0073 3a00 0000 7400 6401 6402  .C...s:...t.d.d.
+00000ae0: 8400 7c01 4400 8301 8301 720d 7401 6403  ..|.D.....r.t.d.
+00000af0: 8301 8201 7402 7c01 8301 7402 7403 7c01  ....t.|...t.t.|.
+00000b00: 8301 8301 6b03 721b 7401 6404 8301 8201  ....k.r.t.d.....
+00000b10: 7c01 5300 2905 4e63 0100 0000 0000 0000  |.S.).Nc........
+00000b20: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
+00000b30: 7318 0000 0081 007c 005d 077d 017c 0164  s......|.].}.|.d
+00000b40: 006b 0056 0001 0071 0264 0153 0029 0272  .k.V...q.d.S.).r
+00000b50: 0100 0000 4e72 2000 0000 2902 da02 2e30  ....Nr ...)....0
+00000b60: da01 6972 2000 0000 7220 0000 0072 2100  ..ir ...r ...r!.
+00000b70: 0000 da09 3c67 656e 6578 7072 3e5d 0000  ....<genexpr>]..
+00000b80: 0073 0400 0000 0280 1600 7a3b 576f 726b  .s........z;Work
+00000b90: 666c 6f77 5570 6461 7465 2e63 6865 636b  flowUpdate.check
+00000ba0: 5f70 6f73 6974 6976 655f 616e 645f 756e  _positive_and_un
+00000bb0: 6971 7565 2e3c 6c6f 6361 6c73 3e2e 3c67  ique.<locals>.<g
+00000bc0: 656e 6578 7072 3e7a 2d4e 6567 6174 6976  enexpr>z-Negativ
+00000bd0: 6520 6069 6460 2069 6e20 6072 656f 7264  e `id` in `reord
+00000be0: 6572 6564 5f77 6f72 6b66 6c6f 7774 6173  ered_workflowtas
+00000bf0: 6b5f 6964 7360 7a2c 6072 656f 7264 6572  k_ids`z,`reorder
+00000c00: 6564 5f77 6f72 6b66 6c6f 7774 6173 6b5f  ed_workflowtask_
+00000c10: 6964 7360 2068 6173 2072 6570 6574 6974  ids` has repetit
+00000c20: 696f 6e73 2904 da03 616e 7972 2f00 0000  ions)...anyr/...
+00000c30: da03 6c65 6eda 0373 6574 2902 7230 0000  ..len..set).r0..
+00000c40: 00da 0576 616c 7565 7220 0000 0072 2000  ...valuer ...r .
+00000c50: 0000 7221 0000 00da 1963 6865 636b 5f70  ..r!.....check_p
+00000c60: 6f73 6974 6976 655f 616e 645f 756e 6971  ositive_and_uniq
+00000c70: 7565 5b00 0000 730a 0000 0012 0208 0114  ue[...s.........
+00000c80: 0108 0104 017a 2857 6f72 6b66 6c6f 7755  .....z(WorkflowU
+00000c90: 7064 6174 652e 6368 6563 6b5f 706f 7369  pdate.check_posi
+00000ca0: 7469 7665 5f61 6e64 5f75 6e69 7175 654e  tive_and_uniqueN
+00000cb0: 290c 721b 0000 0072 1c00 0000 721d 0000  ).r....r....r...
+00000cc0: 0072 0500 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000cd0: 7204 0000 0072 2600 0000 7206 0000 0072  r....r&...r....r
+00000ce0: 0a00 0000 7237 0000 0072 4000 0000 7220  ....r7...r@...r 
+00000cf0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00000d00: 0000 7210 0000 0054 0000 0073 0c00 0000  ..r....T...s....
+00000d10: 0a00 0c01 1001 1403 0602 0e01 7210 0000  ............r...
+00000d20: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000d30: 0000 0400 0000 4000 0000 732e 0000 0065  ......@...s....e
+00000d40: 005a 0164 005a 0255 0065 0365 0419 0065  .Z.d.Z.U.e.e...e
+00000d50: 0564 013c 0065 0664 0264 0364 048d 0265  .d.<.e.d.d.d...e
+00000d60: 0764 0283 0183 015a 0864 0553 0029 0672  .d.....Z.d.S.).r
+00000d70: 1100 0000 7236 0000 0072 3400 0000 5472  ....r6...r4...Tr
+00000d80: 2300 0000 4e29 0972 1b00 0000 721c 0000  #...N).r....r...
+00000d90: 0072 1d00 0000 7204 0000 0072 1400 0000  .r....r....r....
+00000da0: 721f 0000 0072 0600 0000 720a 0000 0072  r....r....r....r
+00000db0: 3700 0000 7220 0000 0072 2000 0000 7220  7...r ...r ...r 
+00000dc0: 0000 0072 2100 0000 7211 0000 0064 0000  ...r!...r....d..
+00000dd0: 0073 0600 0000 0a00 0c01 1803 7211 0000  .s..........r...
+00000de0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000df0: 0000 0300 0000 4000 0000 731a 0000 0065  ......@...s....e
+00000e00: 005a 0164 005a 0255 0065 0365 0419 0065  .Z.d.Z.U.e.e...e
+00000e10: 0564 013c 0064 0253 0029 0372 1200 0000  .d.<.d.S.).r....
+00000e20: 7236 0000 004e 2906 721b 0000 0072 1c00  r6...N).r....r..
+00000e30: 0000 721d 0000 0072 0400 0000 7215 0000  ..r....r....r...
+00000e40: 0072 1f00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
+00000e50: 7220 0000 0072 2100 0000 7212 0000 006b  r ...r!...r....k
+00000e60: 0000 0073 0400 0000 0a00 1001 7212 0000  ...s........r...
+00000e70: 004e 291d da06 7479 7069 6e67 7202 0000  .N)...typingr...
+00000e80: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
+00000e90: da08 7079 6461 6e74 6963 7206 0000 00da  ..pydanticr.....
+00000ea0: 0873 716c 6d6f 6465 6c72 0700 0000 da0b  .sqlmodelr......
+00000eb0: 5f76 616c 6964 6174 6f72 7372 0900 0000  _validatorsr....
+00000ec0: 720a 0000 0072 2b00 0000 720b 0000 0072  r....r+...r....r
+00000ed0: 0c00 0000 720d 0000 00da 075f 5f61 6c6c  ....r......__all
+00000ee0: 5f5f 7218 0000 0072 1300 0000 7216 0000  __r....r....r...
+00000ef0: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
+00000f00: 7233 0000 0072 0f00 0000 720e 0000 0072  r3...r....r....r
+00000f10: 1000 0000 7211 0000 0072 1200 0000 7220  ....r....r....r 
+00000f20: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00000f30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000f40: 7330 0000 000c 000c 010c 010c 010c 020c  s0..............
+00000f50: 010c 020c 010c 010c 010c 0104 0310 0e10  ................
+00000f60: 0610 0610 0810 0410 0410 0b10 0410 0610  ................
+00000f70: 0510 1014 07                             .....
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.3.0a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/task.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,18 +133,14 @@
     def package_path_absolute(cls, value):
         if "/" in value:
             package_path = Path(value)
             if not package_path.is_absolute():
                 raise ValueError(
                     f"Package path must be absolute: {package_path}"
                 )
-            if not package_path.exists():
-                raise ValueError(
-                    f"Package file does not exist: {package_path}"
-                )
         return value
 
 
 class TaskCollectStatus(_TaskCollectBase):
     """
     TaskCollectStatus class
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import uuid
 from typing import Optional
 
 from fastapi_users import schemas
 from pydantic import validator
 
 from ._validators import val_absolute_path
 from ._validators import valstr
@@ -11,15 +10,15 @@
 __all__ = (
     "UserRead",
     "UserUpdate",
     "UserCreate",
 )
 
 
-class UserRead(schemas.BaseUser[uuid.UUID]):
+class UserRead(schemas.BaseUser[int]):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
 
 
 class UserUpdate(schemas.BaseUserUpdate):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a0/fractal_server/common/schemas/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 
     meta: Optional[Dict[str, Any]] = None
     args: Optional[Dict[str, Any]] = None
 
 
 class WorkflowTaskCreate(_WorkflowTaskBase):
     order: Optional[int]
-    task_id: int
     # Validators
     _order = validator("order", allow_reuse=True)(valint("order", min_val=0))
-    _task_id = validator("task_id", allow_reuse=True)(valint("task_id"))
 
 
 class WorkflowTaskRead(_WorkflowTaskBase):
     id: int
     order: Optional[int]
     workflow_id: int
     task_id: int
@@ -75,21 +73,16 @@
 class WorkflowRead(_WorkflowBase):
     id: int
     project_id: int
     task_list: List[WorkflowTaskRead]
 
 
 class WorkflowCreate(_WorkflowBase):
-    project_id: int
-
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
-    _project_id = validator("project_id", allow_reuse=True)(
-        valint("project_id")
-    )
 
 
 class WorkflowUpdate(_WorkflowBase):
     name: Optional[str]
     reordered_workflowtask_ids: Optional[List[int]]
 
     # Validators
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 10:08:09 2023 UTC, .py size: 1065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,74 @@
-00000000: 6f0d 0d0a 0000 0000 891b 5a64 2904 0000  o.........Zd)...
+00000000: 6f0d 0d0a 0000 0000 5583 2e64 0d02 0000  o.......U..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
-000000a0: 7272 6f72 2901 da13 4170 706c 7957 6f72  rror)...ApplyWor
-000000b0: 6b66 6c6f 7743 7265 6174 6563 0000 0000  kflowCreatec....
-000000c0: 0000 0000 0000 0000 0a00 0000 0900 0000  ................
-000000d0: 4300 0000 737e 0100 0074 0064 0164 0164  C...s~...t.d.d.d
-000000e0: 0264 0364 0464 058d 057d 0074 0164 1169  .d.d.d...}.t.d.i
-000000f0: 007c 00a4 018e 017d 0174 027c 0183 0101  .|.....}.t.|....
-00000100: 007c 016a 037d 0264 007d 037c 027c 0375  .|.j.}.d.}.|.|.u
-00000110: 007d 047c 0473 5374 04a0 0564 067c 0466  .}.|.sSt...d.|.f
-00000120: 0164 077c 027c 0366 02a1 0464 0874 06a0  .d.|.|.f...d.t..
-00000130: 07a1 0076 0073 3474 04a0 087c 01a1 0172  ...v.s4t...|...r
-00000140: 3974 04a0 097c 01a1 016e 0164 0874 04a0  9t...|...n.d.t..
-00000150: 097c 02a1 0174 04a0 097c 03a1 0164 099c  .|...t...|...d..
-00000160: 0316 007d 0564 0a64 0b7c 0569 0116 007d  ...}.d.d.|.i...}
-00000170: 0674 0a74 04a0 0b7c 06a1 0183 0182 0164  .t.t...|.......d
-00000180: 0004 007d 0204 007d 047d 0364 027c 0064  ...}...}.}.d.|.d
-00000190: 0c3c 0074 0164 1169 007c 00a4 018e 017d  .<.t.d.i.|.....}
-000001a0: 0174 027c 0183 0101 007c 016a 037d 027c  .t.|.....|.j.}.|
-000001b0: 0273 8e64 0d64 0874 06a0 07a1 0076 0073  .s.d.d.t.....v.s
-000001c0: 7974 04a0 087c 01a1 0172 7e74 04a0 097c  yt...|...r~t...|
-000001d0: 01a1 016e 0164 0874 04a0 097c 02a1 0164  ...n.d.t...|...d
-000001e0: 0e9c 0216 007d 0774 0a74 04a0 0b7c 07a1  .....}.t.t...|..
-000001f0: 0183 0182 0164 007d 0264 0f44 005d 2a7d  .....d.}.d.D.]*}
-00000200: 087c 00a0 0ca1 007d 0964 107c 097c 083c  .|.....}.d.|.|.<
-00000210: 0074 027c 0983 0101 0074 0da0 0e74 0fa1  .t.|.....t...t..
-00000220: 018f 0f01 0074 0164 1169 007c 09a4 018e  .....t.d.i.|....
-00000230: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000240: 0831 0073 b777 0101 0001 0001 0059 0001  .1.s.w.......Y..
-00000250: 0071 9264 0053 0029 124e e901 0000 00e9  .q.d.S.).N......
-00000260: 0300 0000 547a 0b57 4f52 4b45 5220 494e  ....Tz.WORKER IN
-00000270: 4954 2905 da0a 7072 6f6a 6563 745f 6964  IT)...project_id
-00000280: da10 696e 7075 745f 6461 7461 7365 745f  ..input_dataset_
-00000290: 6964 da0b 776f 726b 666c 6f77 5f69 64da  id..workflow_id.
-000002a0: 0f6f 7665 7277 7269 7465 5f69 6e70 7574  .overwrite_input
-000002b0: da0b 776f 726b 6572 5f69 6e69 7429 01da  ..worker_init)..
-000002c0: 0269 7329 017a 3925 2870 7932 2973 0a7b  .is).z9%(py2)s.{
-000002d0: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
-000002e0: 732e 6f75 7470 7574 5f64 6174 6173 6574  s.output_dataset
-000002f0: 5f69 640a 7d20 6973 2025 2870 7935 2973  _id.} is %(py5)s
-00000300: da03 6a6f 6229 03da 0370 7930 da03 7079  ..job)...py0..py
-00000310: 32da 0370 7935 7a0e 6173 7365 7274 2025  2..py5z.assert %
-00000320: 2870 7937 2973 da03 7079 37da 116f 7574  (py7)s..py7..out
-00000330: 7075 745f 6461 7461 7365 745f 6964 7a35  put_dataset_idz5
-00000340: 6173 7365 7274 2025 2870 7932 2973 0a7b  assert %(py2)s.{
-00000350: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
-00000360: 732e 6f75 7470 7574 5f64 6174 6173 6574  s.output_dataset
-00000370: 5f69 640a 7d29 0272 0e00 0000 720f 0000  _id.}).r....r...
-00000380: 0029 0472 0700 0000 7208 0000 0072 1200  .).r....r....r..
-00000390: 0000 7209 0000 00e9 ffff ffff a900 2910  ..r...........).
-000003a0: da04 6469 6374 7204 0000 0072 0200 0000  ..dictr....r....
-000003b0: 7212 0000 00da 0a40 7079 7465 7374 5f61  r......@pytest_a
-000003c0: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
-000003d0: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
-000003e0: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
-000003f0: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
-00000400: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
-00000410: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000420: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000430: 7469 6f6e da04 636f 7079 da06 7079 7465  tion..copy..pyte
-00000440: 7374 da06 7261 6973 6573 7203 0000 0029  st..raisesr....)
-00000450: 0ada 0a76 616c 6964 5f61 7267 7372 0d00  ...valid_argsr..
-00000460: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
-00000470: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
-00000480: 795f 6173 7365 7274 33da 0b40 7079 5f66  y_assert3..@py_f
-00000490: 6f72 6d61 7436 da0b 4070 795f 666f 726d  ormat6..@py_form
-000004a0: 6174 38da 0b40 7079 5f66 6f72 6d61 7433  at8..@py_format3
-000004b0: da03 6b65 79da 0c69 6e76 616c 6964 5f61  ..key..invalid_a
-000004c0: 7267 7372 1400 0000 7214 0000 00fa 562f  rgsr....r.....V/
-000004d0: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-000004e0: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
-000004f0: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
-00000500: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
-00000510: 7465 7374 5f61 7070 6c79 776f 726b 666c  test_applyworkfl
-00000520: 6f77 2e70 79da 1a74 6573 745f 6170 706c  ow.py..test_appl
-00000530: 795f 776f 726b 666c 6f77 5f63 7265 6174  y_workflow_creat
-00000540: 6508 0000 0073 2e00 0000 0202 0201 0201  e....s..........
-00000550: 0201 0201 0201 06fb 0e07 0801 8a01 0802  ................
-00000560: 0e01 0801 5001 0802 0806 0801 0801 0c01  ....P...........
-00000570: 1001 1cff 0280 04f7 722b 0000 0029 0eda  ........r+...)..
-00000580: 0862 7569 6c74 696e 7372 1800 0000 da19  .builtinsr......
-00000590: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-000005a0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-000005b0: 7469 6f6e da07 7265 7772 6974 6572 1600  tion..rewriter..
-000005c0: 0000 721f 0000 00da 0864 6576 746f 6f6c  ..r......devtool
-000005d0: 7372 0200 0000 da17 7079 6461 6e74 6963  sr......pydantic
-000005e0: 2e65 7272 6f72 5f77 7261 7070 6572 7372  .error_wrappersr
-000005f0: 0300 0000 da07 7363 6865 6d61 7372 0400  ......schemasr..
-00000600: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
-00000610: 0072 1400 0000 722a 0000 00da 083c 6d6f  .r....r*.....<mo
-00000620: 6475 6c65 3e01 0000 0073 0a00 0000 2200  dule>....s....".
-00000630: 0c01 0c01 0c02 0c03                      ........
+000000a0: 7272 6f72 2901 da0d 5072 6f6a 6563 7443  rror)...ProjectC
+000000b0: 7265 6174 6563 0000 0000 0000 0000 0000  reatec..........
+000000c0: 0000 0600 0000 0800 0000 4300 0000 7306  ..........C...s.
+000000d0: 0100 0074 0064 0164 028d 017d 0074 017c  ...t.d.d...}.t.|
+000000e0: 0083 0101 0064 037d 0174 0064 047c 019b  .....d.}.t.d.|..
+000000f0: 0064 049d 0364 028d 017d 0074 017c 0083  .d...d...}.t.|..
+00000100: 0101 007c 006a 027d 027c 027c 016b 027d  ...|.j.}.|.|.k.}
+00000110: 037c 0373 6274 03a0 0464 057c 0366 0164  .|.sbt...d.|.f.d
+00000120: 067c 027c 0166 02a1 0464 0774 05a0 06a1  .|.|.f...d.t....
+00000130: 0076 0073 3674 03a0 077c 00a1 0172 3b74  .v.s6t...|...r;t
+00000140: 03a0 087c 00a1 016e 0164 0774 03a0 087c  ...|...n.d.t...|
+00000150: 02a1 0164 0874 05a0 06a1 0076 0073 4b74  ...d.t.....v.sKt
+00000160: 03a0 077c 01a1 0172 5074 03a0 087c 01a1  ...|...rPt...|..
+00000170: 016e 0164 0864 099c 0316 007d 0464 0a64  .n.d.d.....}.d.d
+00000180: 0b7c 0469 0116 007d 0574 0974 03a0 0a7c  .|.i...}.t.t...|
+00000190: 05a1 0183 0182 0164 0004 007d 027d 0374  .......d...}.}.t
+000001a0: 0ba0 0c74 0da1 018f 0e01 0074 0064 0464  ...t.......t.d.d
+000001b0: 028d 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+000001c0: 0064 0053 0031 0073 7c77 0101 0001 0001  .d.S.1.s|w......
+000001d0: 0059 0001 0064 0053 0029 0c4e 7a0a 6d79  .Y...d.S.).Nz.my
+000001e0: 2070 726f 6a65 6374 2901 da04 6e61 6d65   project)...name
+000001f0: 7a11 736f 6d65 2070 726f 6a65 6374 206e  z.some project n
+00000200: 616d 657a 0220 2029 01fa 023d 3d29 017a  amez.  )...==).z
+00000210: 2c25 2870 7932 2973 0a7b 2528 7079 3229  ,%(py2)s.{%(py2)
+00000220: 7320 3d20 2528 7079 3029 732e 6e61 6d65  s = %(py0)s.name
+00000230: 0a7d 203d 3d20 2528 7079 3429 73da 0170  .} == %(py4)s..p
+00000240: da04 4e41 4d45 2903 da03 7079 30da 0370  ..NAME)...py0..p
+00000250: 7932 da03 7079 347a 0e61 7373 6572 7420  y2..py4z.assert 
+00000260: 2528 7079 3629 73da 0370 7936 290e 7204  %(py6)s..py6).r.
+00000270: 0000 0072 0200 0000 7205 0000 00da 0a40  ...r....r......@
+00000280: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
+00000290: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
+000002a0: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
+000002b0: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
+000002c0: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
+000002d0: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
+000002e0: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
+000002f0: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
+00000300: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
+00000310: 0029 0672 0700 0000 7208 0000 00da 0b40  .).r....r......@
+00000320: 7079 5f61 7373 6572 7431 da0b 4070 795f  py_assert1..@py_
+00000330: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
+00000340: 6d61 7435 da0b 4070 795f 666f 726d 6174  mat5..@py_format
+00000350: 37a9 0072 1b00 0000 fa50 2f68 6f6d 652f  7..r.....P/home/
+00000360: 746f 6d6d 6173 6f2f 4672 6163 7461 6c2f  tommaso/Fractal/
+00000370: 6672 6163 7461 6c2d 7365 7276 6572 2f66  fractal-server/f
+00000380: 7261 6374 616c 5f73 6572 7665 722f 636f  ractal_server/co
+00000390: 6d6d 6f6e 2f74 6573 7473 2f74 6573 745f  mmon/tests/test_
+000003a0: 7072 6f6a 6563 742e 7079 da13 7465 7374  project.py..test
+000003b0: 5f70 726f 6a65 6374 5f63 7265 6174 6508  _project_create.
+000003c0: 0000 0073 1200 0000 0a02 0801 0402 1201  ...s............
+000003d0: 0801 9c01 0c02 0c01 22ff 721d 0000 0029  ........".r....)
+000003e0: 0eda 0862 7569 6c74 696e 7372 0f00 0000  ...builtinsr....
+000003f0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+00000400: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+00000410: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+00000420: 0d00 0000 7215 0000 00da 0864 6576 746f  ....r......devto
+00000430: 6f6c 7372 0200 0000 da17 7079 6461 6e74  olsr......pydant
+00000440: 6963 2e65 7272 6f72 5f77 7261 7070 6572  ic.error_wrapper
+00000450: 7372 0300 0000 da07 7363 6865 6d61 7372  sr......schemasr
+00000460: 0400 0000 721d 0000 0072 1b00 0000 721b  ....r....r....r.
+00000470: 0000 0072 1b00 0000 721c 0000 00da 083c  ...r....r......<
+00000480: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
+00000490: 2200 0c01 0c01 0c02 0c03                 ".........
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr  6 08:31:17 2023 UTC, .py size: 525 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5583 2e64 0d02 0000  o.......U..d....
+00000000: 6f0d 0d0a 0000 0000 aae4 5864 0d02 0000  o.........Xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 10:08:09 2023 UTC, .py size: 2838 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 891b 5a64 160b 0000  o.........Zd....
+00000000: 6f0d 0d0a 0000 0000 6e2d 5a64 240a 0000  o.......n-Zd$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
@@ -27,165 +27,157 @@
 000001a0: 6561 7465 2901 da12 576f 726b 666c 6f77  eate)...Workflow
 000001b0: 5461 736b 496d 706f 7274 2901 da10 576f  TaskImport)...Wo
 000001c0: 726b 666c 6f77 5461 736b 5265 6164 2901  rkflowTaskRead).
 000001d0: da12 576f 726b 666c 6f77 5461 736b 5570  ..WorkflowTaskUp
 000001e0: 6461 7465 2901 da0e 576f 726b 666c 6f77  date)...Workflow
 000001f0: 5570 6461 7465 6300 0000 0000 0000 0000  Updatec.........
 00000200: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
-00000210: d000 0000 7400 6401 6402 8d01 7d00 7401  ....t.d.d...}.t.
+00000210: 8000 0000 7400 6401 6402 8d01 7d00 7401  ....t.d.d...}.t.
 00000220: 7c00 8301 0100 7402 a003 7404 a101 8f0d  |.....t...t.....
 00000230: 0100 7400 6403 6402 8d01 0100 5700 6400  ..t.d.d.....W.d.
 00000240: 0400 0400 8303 0100 6e08 3100 731e 7701  ........n.1.s.w.
-00000250: 0100 0100 0100 5900 0100 7400 6401 6401  ......Y...t.d.d.
-00000260: 6404 8d02 7d00 7400 6401 6405 6404 8d02  d...}.t.d.d.d...
-00000270: 7d00 7402 a003 7404 a101 8f0e 0100 7400  }.t...t.......t.
-00000280: 6401 6403 6404 8d02 0100 5700 6400 0400  d.d.d.....W.d...
-00000290: 0400 8303 0100 6e08 3100 7345 7701 0100  ......n.1.sEw...
-000002a0: 0100 0100 5900 0100 7402 a003 7404 a101  ....Y...t...t...
-000002b0: 8f0f 0100 7400 6401 6400 6404 8d02 0100  ....t.d.d.d.....
-000002c0: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
-000002d0: 3100 7361 7701 0100 0100 0100 5900 0100  1.saw.......Y...
-000002e0: 6400 5300 2906 4ee9 0100 0000 2901 da07  d.S.).N.....)...
-000002f0: 7461 736b 5f69 64e9 ffff ffff 2902 720f  task_id.....).r.
-00000300: 0000 00da 056f 7264 6572 7201 0000 0029  .....orderr....)
-00000310: 0572 0900 0000 7202 0000 00da 0670 7974  .r....r......pyt
-00000320: 6573 74da 0672 6169 7365 7372 0300 0000  est..raisesr....
-00000330: a901 da01 74a9 0072 1600 0000 fa51 2f68  ....t..r.....Q/h
-00000340: 6f6d 652f 746f 6d6d 6173 6f2f 4672 6163  ome/tommaso/Frac
-00000350: 7461 6c2f 6672 6163 7461 6c2d 7365 7276  tal/fractal-serv
-00000360: 6572 2f66 7261 6374 616c 5f73 6572 7665  er/fractal_serve
-00000370: 722f 636f 6d6d 6f6e 2f74 6573 7473 2f74  r/common/tests/t
-00000380: 6573 745f 776f 726b 666c 6f77 2e70 79da  est_workflow.py.
-00000390: 1974 6573 745f 776f 726b 666c 6f77 5f74  .test_workflow_t
-000003a0: 6173 6b5f 6372 6561 7465 1100 0000 731a  ask_create....s.
-000003b0: 0000 000a 0208 010c 020c 011c ff0c 030c  ................
-000003c0: 010c 010e 011c ff0c 020e 0122 ff72 1800  ...........".r..
-000003d0: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
-000003e0: 0000 0008 0000 0043 0000 0073 5600 0000  .......C...sV...
-000003f0: 7400 7401 6401 6402 8d01 6403 8d01 7d00  t.t.d.d...d...}.
-00000400: 7402 a003 7404 a101 8f10 0100 7400 7401  t...t.......t.t.
-00000410: 6404 6405 8d01 6403 8d01 7d00 5700 6400  d.d...d...}.W.d.
-00000420: 0400 0400 8303 0100 6e08 3100 7320 7701  ........n.1.s w.
-00000430: 0100 0100 0100 5900 0100 7405 7c00 8301  ......Y...t.|...
-00000440: 0100 6400 5300 2906 4eda 0465 6c73 65a9  ..d.S.).N..else.
-00000450: 01da 0973 6f6d 6574 6869 6e67 2901 da04  ...something)...
-00000460: 6d65 7461 da03 6e65 7729 01da 1570 6172  meta..new)...par
-00000470: 616c 6c65 6c69 7a61 7469 6f6e 5f6c 6576  allelization_lev
-00000480: 656c 2906 720c 0000 00da 0464 6963 7472  el).r......dictr
-00000490: 1200 0000 7213 0000 0072 0300 0000 7202  ....r....r....r.
-000004a0: 0000 0072 1400 0000 7216 0000 0072 1600  ...r....r....r..
-000004b0: 0000 7217 0000 00da 1974 6573 745f 776f  ..r......test_wo
-000004c0: 726b 666c 6f77 5f74 6173 6b5f 7570 6461  rkflow_task_upda
-000004d0: 7465 2100 0000 730a 0000 0010 020c 0212  te!...s.........
-000004e0: 011c ff0c 0272 2000 0000 6300 0000 0000  .....r ...c.....
-000004f0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00000500: 0000 0073 1800 0000 7400 6401 6402 6403  ...s....t.d.d.d.
-00000510: 8d02 7d00 7401 7c00 8301 0100 6400 5300  ..}.t.|.....d.S.
-00000520: 2904 4eda 0877 6f72 6b66 6c6f 7772 0e00  ).N..workflowr..
-00000530: 0000 2902 da04 6e61 6d65 da0a 7072 6f6a  ..)...name..proj
-00000540: 6563 745f 6964 2902 7206 0000 0072 0200  ect_id).r....r..
-00000550: 0000 a901 da01 7772 1600 0000 7216 0000  ......wr....r...
-00000560: 0072 1700 0000 da14 7465 7374 5f77 6f72  .r......test_wor
-00000570: 6b66 6c6f 775f 6372 6561 7465 2a00 0000  kflow_create*...
-00000580: 7304 0000 000c 010c 0172 2600 0000 6300  s........r&...c.
-00000590: 0000 0000 0000 0000 0000 0003 0000 0008  ................
-000005a0: 0000 0043 0000 0073 6a00 0000 7400 6401  ...C...sj...t.d.
-000005b0: 6402 6403 8d02 7d00 7401 7c00 6404 8d01  d.d...}.t.|.d...
-000005c0: 7d01 7402 6405 7c01 6701 6406 8d02 7d02  }.t.d.|.g.d...}.
-000005d0: 7403 7c02 8301 0100 7404 a005 7406 a101  t.|.....t...t...
-000005e0: 8f10 0100 7402 6407 7c01 6701 6406 8d02  ....t.d.|.g.d...
-000005f0: 0100 5700 6400 0400 0400 8303 0100 6400  ..W.d.........d.
-00000600: 5300 3100 732e 7701 0100 0100 0100 5900  S.1.s.w.......Y.
-00000610: 0100 6400 5300 2908 4e72 2200 0000 da06  ..d.S.).Nr".....
-00000620: 736f 7572 6365 2902 7222 0000 0072 2700  source).r"...r'.
-00000630: 0000 2901 da04 7461 736b 7221 0000 0029  ..)...taskr!...)
-00000640: 0272 2200 0000 da09 7461 736b 5f6c 6973  .r".....task_lis
-00000650: 74da 0120 2907 7204 0000 0072 0a00 0000  t.. ).r....r....
-00000660: 7207 0000 0072 0200 0000 7212 0000 0072  r....r....r....r
-00000670: 1300 0000 7203 0000 0029 0372 1500 0000  ....r....).r....
-00000680: da03 7766 7472 2500 0000 7216 0000 0072  ..wftr%...r....r
-00000690: 1600 0000 7217 0000 00da 1474 6573 745f  ....r......test_
-000006a0: 776f 726b 666c 6f77 5f69 6d70 6f72 742f  workflow_import/
-000006b0: 0000 0073 0e00 0000 0c02 0a01 0e01 0801  ...s............
-000006c0: 0c02 1001 22ff 722c 0000 0063 0000 0000  ....".r,...c....
-000006d0: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-000006e0: 4300 0000 731c 0000 0074 0064 0164 0264  C...s....t.d.d.d
-000006f0: 0167 0064 038d 047d 0074 017c 0083 0101  .g.d...}.t.|....
-00000700: 0064 0053 0029 044e 720e 0000 0072 2100  .d.S.).Nr....r!.
-00000710: 0000 a904 da02 6964 7222 0000 0072 2300  ......idr"...r#.
-00000720: 0000 7229 0000 0029 0272 0800 0000 7202  ..r)...).r....r.
-00000730: 0000 0072 2400 0000 7216 0000 0072 1600  ...r$...r....r..
-00000740: 0000 7217 0000 00da 2274 6573 745f 776f  ..r....."test_wo
-00000750: 726b 666c 6f77 5f72 6561 645f 656d 7074  rkflow_read_empt
-00000760: 795f 7461 736b 5f6c 6973 743a 0000 0073  y_task_list:...s
-00000770: 0400 0000 1001 0c01 722f 0000 0063 0000  ........r/...c..
-00000780: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-00000790: 0000 4300 0000 735c 0000 0074 0064 0164  ..C...s\...t.d.d
-000007a0: 0264 0364 0464 0564 0674 0164 0764 088d  .d.d.d.d.t.d.d..
-000007b0: 0164 098d 077d 0074 0264 0a64 0a64 0a7c  .d...}.t.d.d.d.|
-000007c0: 0064 0b8d 047d 0174 0264 0c64 0a64 0a7c  .d...}.t.d.d.d.|
-000007d0: 0064 0b8d 047d 0274 0364 0a64 0d64 0a7c  .d...}.t.d.d.d.|
-000007e0: 017c 0267 0264 0e8d 047d 0374 047c 0383  .|.g.d...}.t.|..
-000007f0: 0101 0064 0053 0029 0f4e e909 0000 0072  ...d.S.).N.....r
-00000800: 2200 0000 7227 0000 00da 0763 6f6d 6d61  "...r'.....comma
-00000810: 6e64 da0a 696e 7075 745f 7479 7065 da0b  nd..input_type..
-00000820: 6f75 7470 7574 5f74 7970 6572 1900 0000  output_typer....
-00000830: 721a 0000 0029 0772 2e00 0000 7222 0000  r....).r....r"..
-00000840: 0072 2700 0000 7231 0000 0072 3200 0000  .r'...r1...r2...
-00000850: 7233 0000 0072 1c00 0000 720e 0000 0029  r3...r....r....)
-00000860: 0472 2e00 0000 720f 0000 00da 0b77 6f72  .r....r......wor
-00000870: 6b66 6c6f 775f 6964 7228 0000 00e9 0200  kflow_idr(......
-00000880: 0000 7221 0000 0072 2d00 0000 2905 7205  ..r!...r-...).r.
-00000890: 0000 0072 1f00 0000 720b 0000 0072 0800  ...r....r....r..
-000008a0: 0000 7202 0000 0029 04da 0274 31da 0477  ..r....)...t1..w
-000008b0: 6674 31da 0477 6674 3272 2500 0000 7216  ft1..wft2r%...r.
-000008c0: 0000 0072 1600 0000 7217 0000 00da 2674  ...r....r.....&t
-000008d0: 6573 745f 776f 726b 666c 6f77 5f72 6561  est_workflow_rea
-000008e0: 645f 6e6f 6e5f 656d 7074 795f 7461 736b  d_non_empty_task
-000008f0: 5f6c 6973 743f 0000 0073 1e00 0000 0202  _list?...s......
-00000900: 0201 0201 0201 0201 0201 0201 0801 06f9  ................
-00000910: 100a 1001 0202 0c01 06ff 0c03 7239 0000  ............r9..
-00000920: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000930: 0000 0800 0000 4300 0000 73a2 0000 0074  ......C...s....t
-00000940: 0064 0167 0064 02a2 0164 038d 0201 0074  .d.g.d...d.....t
-00000950: 0064 0164 048d 0101 0074 0067 0064 02a2  .d.d.....t.g.d..
-00000960: 0164 058d 0101 0074 01a0 0274 03a1 018f  .d.....t...t....
-00000970: 1001 0074 0064 0167 0064 06a2 0164 038d  ...t.d.g.d...d..
-00000980: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000990: 0831 0073 2c77 0101 0001 0001 0059 0001  .1.s,w.......Y..
-000009a0: 0074 01a0 0274 03a1 018f 1101 0074 0064  .t...t.......t.d
-000009b0: 0167 0064 07a2 0164 038d 0201 0057 0064  .g.d...d.....W.d
-000009c0: 0004 0004 0083 0301 0064 0053 0031 0073  .........d.S.1.s
-000009d0: 4a77 0101 0001 0001 0059 0001 0064 0053  Jw.......Y...d.S
-000009e0: 0029 084e 7221 0000 0029 0472 0100 0000  .).Nr!...).r....
-000009f0: 720e 0000 00e9 0300 0000 7235 0000 0029  r.........r5...)
-00000a00: 0272 2200 0000 da1a 7265 6f72 6465 7265  .r".....reordere
-00000a10: 645f 776f 726b 666c 6f77 7461 736b 5f69  d_workflowtask_i
-00000a20: 6473 2901 7222 0000 0029 0172 3b00 0000  ds).r"...).r;...
-00000a30: 2903 720e 0000 0072 3a00 0000 720e 0000  ).r....r:...r...
-00000a40: 0029 0372 0e00 0000 723a 0000 0072 1000  .).r....r:...r..
-00000a50: 0000 2904 720d 0000 0072 1200 0000 7213  ..).r....r....r.
-00000a60: 0000 0072 0300 0000 7216 0000 0072 1600  ...r....r....r..
-00000a70: 0000 7216 0000 0072 1700 0000 da14 7465  ..r....r......te
-00000a80: 7374 5f77 6f72 6b66 6c6f 775f 7570 6461  st_workflow_upda
-00000a90: 7465 5400 0000 7312 0000 0010 010a 010e  teT...s.........
-00000aa0: 010c 0112 011c ff0c 0212 0122 ff72 3c00  ...........".r<.
-00000ab0: 0000 291d da08 6275 696c 7469 6e73 da0c  ..)...builtins..
-00000ac0: 4070 795f 6275 696c 7469 6e73 da19 5f70  @py_builtins.._p
-00000ad0: 7974 6573 742e 6173 7365 7274 696f 6e2e  ytest.assertion.
-00000ae0: 7265 7772 6974 65da 0961 7373 6572 7469  rewrite..asserti
-00000af0: 6f6e da07 7265 7772 6974 65da 0a40 7079  on..rewrite..@py
-00000b00: 7465 7374 5f61 7272 1200 0000 da08 6465  test_arr......de
-00000b10: 7674 6f6f 6c73 7202 0000 00da 1770 7964  vtoolsr......pyd
-00000b20: 616e 7469 632e 6572 726f 725f 7772 6170  antic.error_wrap
-00000b30: 7065 7273 7203 0000 00da 0773 6368 656d  persr......schem
-00000b40: 6173 7204 0000 0072 0500 0000 7206 0000  asr....r....r...
-00000b50: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00000b60: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000b70: 0d00 0000 7218 0000 0072 2000 0000 7226  ....r....r ...r&
-00000b80: 0000 0072 2c00 0000 722f 0000 0072 3900  ...r,...r/...r9.
-00000b90: 0000 723c 0000 0072 1600 0000 7216 0000  ..r<...r....r...
-00000ba0: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
-00000bb0: 6475 6c65 3e01 0000 0073 2800 0000 2200  dule>....s(...".
-00000bc0: 0c01 0c01 0c02 0c01 0c01 0c01 0c01 0c01  ................
-00000bd0: 0c01 0c01 0c01 0c01 0803 0810 0809 0805  ................
-00000be0: 080b 0805 0c15                           ......
+00000250: 0100 0100 0100 5900 0100 7402 a003 7404  ......Y...t...t.
+00000260: a101 8f0e 0100 7400 6400 6402 8d01 0100  ......t.d.d.....
+00000270: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+00000280: 3100 7339 7701 0100 0100 0100 5900 0100  1.s9w.......Y...
+00000290: 6400 5300 2904 4ee9 0100 0000 2901 da05  d.S.).N.....)...
+000002a0: 6f72 6465 72e9 ffff ffff 2905 7209 0000  order.....).r...
+000002b0: 0072 0200 0000 da06 7079 7465 7374 da06  .r......pytest..
+000002c0: 7261 6973 6573 7203 0000 00a9 01da 0174  raisesr........t
+000002d0: a900 7215 0000 00fa 512f 686f 6d65 2f74  ..r.....Q/home/t
+000002e0: 6f6d 6d61 736f 2f46 7261 6374 616c 2f66  ommaso/Fractal/f
+000002f0: 7261 6374 616c 2d73 6572 7665 722f 6672  ractal-server/fr
+00000300: 6163 7461 6c5f 7365 7276 6572 2f63 6f6d  actal_server/com
+00000310: 6d6f 6e2f 7465 7374 732f 7465 7374 5f77  mon/tests/test_w
+00000320: 6f72 6b66 6c6f 772e 7079 da19 7465 7374  orkflow.py..test
+00000330: 5f77 6f72 6b66 6c6f 775f 7461 736b 5f63  _workflow_task_c
+00000340: 7265 6174 6511 0000 0073 1000 0000 0a02  reate....s......
+00000350: 0801 0c02 0c01 1cff 0c02 0c01 22ff 7217  ............".r.
+00000360: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000370: 0100 0000 0800 0000 4300 0000 7356 0000  ........C...sV..
+00000380: 0074 0074 0164 0164 028d 0164 038d 017d  .t.t.d.d...d...}
+00000390: 0074 02a0 0374 04a1 018f 1001 0074 0074  .t...t.......t.t
+000003a0: 0164 0464 058d 0164 038d 017d 0057 0064  .d.d...d...}.W.d
+000003b0: 0004 0004 0083 0301 006e 0831 0073 2077  .........n.1.s w
+000003c0: 0101 0001 0001 0059 0001 0074 057c 0083  .......Y...t.|..
+000003d0: 0101 0064 0053 0029 064e da04 656c 7365  ...d.S.).N..else
+000003e0: a901 da09 736f 6d65 7468 696e 6729 01da  ....something)..
+000003f0: 046d 6574 61da 036e 6577 2901 da15 7061  .meta..new)...pa
+00000400: 7261 6c6c 656c 697a 6174 696f 6e5f 6c65  rallelization_le
+00000410: 7665 6c29 0672 0c00 0000 da04 6469 6374  vel).r......dict
+00000420: 7211 0000 0072 1200 0000 7203 0000 0072  r....r....r....r
+00000430: 0200 0000 7213 0000 0072 1500 0000 7215  ....r....r....r.
+00000440: 0000 0072 1600 0000 da19 7465 7374 5f77  ...r......test_w
+00000450: 6f72 6b66 6c6f 775f 7461 736b 5f75 7064  orkflow_task_upd
+00000460: 6174 651c 0000 0073 0a00 0000 1002 0c02  ate....s........
+00000470: 1201 1cff 0c02 721f 0000 0063 0000 0000  ......r....c....
+00000480: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000490: 4300 0000 7316 0000 0074 0064 0164 028d  C...s....t.d.d..
+000004a0: 017d 0074 017c 0083 0101 0064 0053 0029  .}.t.|.....d.S.)
+000004b0: 034e da08 776f 726b 666c 6f77 a901 da04  .N..workflow....
+000004c0: 6e61 6d65 2902 7206 0000 0072 0200 0000  name).r....r....
+000004d0: a901 da01 7772 1500 0000 7215 0000 0072  ....wr....r....r
+000004e0: 1600 0000 da14 7465 7374 5f77 6f72 6b66  ......test_workf
+000004f0: 6c6f 775f 6372 6561 7465 2500 0000 7304  low_create%...s.
+00000500: 0000 000a 010c 0172 2500 0000 6300 0000  .......r%...c...
+00000510: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00000520: 0043 0000 0073 6a00 0000 7400 6401 6402  .C...sj...t.d.d.
+00000530: 6403 8d02 7d00 7401 7c00 6404 8d01 7d01  d...}.t.|.d...}.
+00000540: 7402 6405 7c01 6701 6406 8d02 7d02 7403  t.d.|.g.d...}.t.
+00000550: 7c02 8301 0100 7404 a005 7406 a101 8f10  |.....t...t.....
+00000560: 0100 7402 6407 7c01 6701 6406 8d02 0100  ..t.d.|.g.d.....
+00000570: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+00000580: 3100 732e 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00000590: 6400 5300 2908 4e72 2200 0000 da06 736f  d.S.).Nr".....so
+000005a0: 7572 6365 2902 7222 0000 0072 2600 0000  urce).r"...r&...
+000005b0: 2901 da04 7461 736b 7220 0000 0029 0272  )...taskr ...).r
+000005c0: 2200 0000 da09 7461 736b 5f6c 6973 74da  ".....task_list.
+000005d0: 0120 2907 7204 0000 0072 0a00 0000 7207  . ).r....r....r.
+000005e0: 0000 0072 0200 0000 7211 0000 0072 1200  ...r....r....r..
+000005f0: 0000 7203 0000 0029 0372 1400 0000 da03  ..r....).r......
+00000600: 7766 7472 2400 0000 7215 0000 0072 1500  wftr$...r....r..
+00000610: 0000 7216 0000 00da 1474 6573 745f 776f  ..r......test_wo
+00000620: 726b 666c 6f77 5f69 6d70 6f72 742a 0000  rkflow_import*..
+00000630: 0073 0e00 0000 0c02 0a01 0e01 0801 0c02  .s..............
+00000640: 1001 22ff 722b 0000 0063 0000 0000 0000  ..".r+...c......
+00000650: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
+00000660: 0000 731c 0000 0074 0064 0164 0264 0167  ..s....t.d.d.d.g
+00000670: 0064 038d 047d 0074 017c 0083 0101 0064  .d...}.t.|.....d
+00000680: 0053 0029 044e 720e 0000 0072 2000 0000  .S.).Nr....r ...
+00000690: a904 da02 6964 7222 0000 00da 0a70 726f  ....idr".....pro
+000006a0: 6a65 6374 5f69 6472 2800 0000 2902 7208  ject_idr(...).r.
+000006b0: 0000 0072 0200 0000 7223 0000 0072 1500  ...r....r#...r..
+000006c0: 0000 7215 0000 0072 1600 0000 da22 7465  ..r....r....."te
+000006d0: 7374 5f77 6f72 6b66 6c6f 775f 7265 6164  st_workflow_read
+000006e0: 5f65 6d70 7479 5f74 6173 6b5f 6c69 7374  _empty_task_list
+000006f0: 3500 0000 7304 0000 0010 010c 0172 2f00  5...s........r/.
+00000700: 0000 6300 0000 0000 0000 0000 0000 0004  ..c.............
+00000710: 0000 000a 0000 0043 0000 0073 5c00 0000  .......C...s\...
+00000720: 7400 6401 6402 6403 6404 6405 6406 7401  t.d.d.d.d.d.d.t.
+00000730: 6407 6408 8d01 6409 8d07 7d00 7402 640a  d.d...d...}.t.d.
+00000740: 640a 640a 7c00 640b 8d04 7d01 7402 640c  d.d.|.d...}.t.d.
+00000750: 640a 640a 7c00 640b 8d04 7d02 7403 640a  d.d.|.d...}.t.d.
+00000760: 640d 640a 7c01 7c02 6702 640e 8d04 7d03  d.d.|.|.g.d...}.
+00000770: 7404 7c03 8301 0100 6400 5300 290f 4ee9  t.|.....d.S.).N.
+00000780: 0900 0000 7222 0000 0072 2600 0000 da07  ....r"...r&.....
+00000790: 636f 6d6d 616e 64da 0a69 6e70 7574 5f74  command..input_t
+000007a0: 7970 65da 0b6f 7574 7075 745f 7479 7065  ype..output_type
+000007b0: 7218 0000 0072 1900 0000 2907 722d 0000  r....r....).r-..
+000007c0: 0072 2200 0000 7226 0000 0072 3100 0000  .r"...r&...r1...
+000007d0: 7232 0000 0072 3300 0000 721b 0000 0072  r2...r3...r....r
+000007e0: 0e00 0000 2904 722d 0000 00da 0774 6173  ....).r-.....tas
+000007f0: 6b5f 6964 da0b 776f 726b 666c 6f77 5f69  k_id..workflow_i
+00000800: 6472 2700 0000 e902 0000 0072 2000 0000  dr'........r ...
+00000810: 722c 0000 0029 0572 0500 0000 721e 0000  r,...).r....r...
+00000820: 0072 0b00 0000 7208 0000 0072 0200 0000  .r....r....r....
+00000830: 2904 da02 7431 da04 7766 7431 da04 7766  )...t1..wft1..wf
+00000840: 7432 7224 0000 0072 1500 0000 7215 0000  t2r$...r....r...
+00000850: 0072 1600 0000 da26 7465 7374 5f77 6f72  .r.....&test_wor
+00000860: 6b66 6c6f 775f 7265 6164 5f6e 6f6e 5f65  kflow_read_non_e
+00000870: 6d70 7479 5f74 6173 6b5f 6c69 7374 3a00  mpty_task_list:.
+00000880: 0000 731e 0000 0002 0202 0102 0102 0102  ..s.............
+00000890: 0102 0102 0108 0106 f910 0a10 0102 020c  ................
+000008a0: 0106 ff0c 0372 3a00 0000 6300 0000 0000  .....r:...c.....
+000008b0: 0000 0000 0000 0000 0000 0008 0000 0043  ...............C
+000008c0: 0000 0073 a200 0000 7400 6401 6700 6402  ...s....t.d.g.d.
+000008d0: a201 6403 8d02 0100 7400 6401 6404 8d01  ..d.....t.d.d...
+000008e0: 0100 7400 6700 6402 a201 6405 8d01 0100  ..t.g.d...d.....
+000008f0: 7401 a002 7403 a101 8f10 0100 7400 6401  t...t.......t.d.
+00000900: 6700 6406 a201 6403 8d02 0100 5700 6400  g.d...d.....W.d.
+00000910: 0400 0400 8303 0100 6e08 3100 732c 7701  ........n.1.s,w.
+00000920: 0100 0100 0100 5900 0100 7401 a002 7403  ......Y...t...t.
+00000930: a101 8f11 0100 7400 6401 6700 6407 a201  ......t.d.g.d...
+00000940: 6403 8d02 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00000950: 0100 6400 5300 3100 734a 7701 0100 0100  ..d.S.1.sJw.....
+00000960: 0100 5900 0100 6400 5300 2908 4e72 2000  ..Y...d.S.).Nr .
+00000970: 0000 2904 7201 0000 0072 0e00 0000 e903  ..).r....r......
+00000980: 0000 0072 3600 0000 2902 7222 0000 00da  ...r6...).r"....
+00000990: 1a72 656f 7264 6572 6564 5f77 6f72 6b66  .reordered_workf
+000009a0: 6c6f 7774 6173 6b5f 6964 7372 2100 0000  lowtask_idsr!...
+000009b0: 2901 723c 0000 0029 0372 0e00 0000 723b  ).r<...).r....r;
+000009c0: 0000 0072 0e00 0000 2903 720e 0000 0072  ...r....).r....r
+000009d0: 3b00 0000 7210 0000 0029 0472 0d00 0000  ;...r....).r....
+000009e0: 7211 0000 0072 1200 0000 7203 0000 0072  r....r....r....r
+000009f0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000a00: 0000 00da 1474 6573 745f 776f 726b 666c  .....test_workfl
+00000a10: 6f77 5f75 7064 6174 654f 0000 0073 1200  ow_updateO...s..
+00000a20: 0000 1001 0a01 0e01 0c01 1201 1cff 0c02  ................
+00000a30: 1201 22ff 723d 0000 0029 1dda 0862 7569  ..".r=...)...bui
+00000a40: 6c74 696e 73da 0c40 7079 5f62 7569 6c74  ltins..@py_built
+00000a50: 696e 73da 195f 7079 7465 7374 2e61 7373  ins.._pytest.ass
+00000a60: 6572 7469 6f6e 2e72 6577 7269 7465 da09  ertion.rewrite..
+00000a70: 6173 7365 7274 696f 6eda 0772 6577 7269  assertion..rewri
+00000a80: 7465 da0a 4070 7974 6573 745f 6172 7211  te..@pytest_arr.
+00000a90: 0000 00da 0864 6576 746f 6f6c 7372 0200  .....devtoolsr..
+00000aa0: 0000 da17 7079 6461 6e74 6963 2e65 7272  ....pydantic.err
+00000ab0: 6f72 5f77 7261 7070 6572 7372 0300 0000  or_wrappersr....
+00000ac0: da07 7363 6865 6d61 7372 0400 0000 7205  ..schemasr....r.
+00000ad0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
+00000ae0: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000af0: 0072 0c00 0000 720d 0000 0072 1700 0000  .r....r....r....
+00000b00: 721f 0000 0072 2500 0000 722b 0000 0072  r....r%...r+...r
+00000b10: 2f00 0000 723a 0000 0072 3d00 0000 7215  /...r:...r=...r.
+00000b20: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000b30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000b40: 7328 0000 0022 000c 010c 010c 020c 010c  s(..."..........
+00000b50: 010c 010c 010c 010c 010c 010c 010c 0108  ................
+00000b60: 0308 0b08 0908 0508 0b08 050c 15         .............
```

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a0/fractal_server/common/tests/test_workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,39 +12,34 @@
 from schemas import WorkflowTaskRead
 from schemas import WorkflowTaskUpdate
 from schemas import WorkflowUpdate
 
 
 def test_workflow_task_create():
     # Successful creation
-    t = WorkflowTaskCreate(task_id=1)
+    t = WorkflowTaskCreate(order=1)
     debug(t)
-    # Missing arguments
+    # Invalid arguments
     with pytest.raises(ValidationError):
-        WorkflowTaskCreate(task_id=-1)
-    # Several values of order
-    t = WorkflowTaskCreate(task_id=1, order=1)
-    t = WorkflowTaskCreate(task_id=1, order=0)
+        WorkflowTaskCreate(order=-1)
     with pytest.raises(ValidationError):
-        WorkflowTaskCreate(task_id=1, order=-1)
-    with pytest.raises(ValidationError):
-        WorkflowTaskCreate(task_id=1, order=None)
+        WorkflowTaskCreate(order=None)
 
 
 def test_workflow_task_update():
     # Successful creation
     t = WorkflowTaskUpdate(meta=dict(something="else"))
     # Forbidden key-value update
     with pytest.raises(ValidationError):
         t = WorkflowTaskUpdate(meta=dict(parallelization_level="new"))
     debug(t)
 
 
 def test_workflow_create():
-    w = WorkflowCreate(name="workflow", project_id=1)
+    w = WorkflowCreate(name="workflow")
     debug(w)
 
 
 def test_workflow_import():
     # Successful creation
     t = TaskImport(name="name", source="source")
     wft = WorkflowTaskImport(task=t)
```

### Comparing `fractal_server-1.2.5a2/fractal_server/config.py` & `fractal_server-1.3.0a0/fractal_server/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,15 +265,16 @@
     not specified, the same interpreter that runs the server is used.
     """
 
     FRACTAL_SLURM_POLL_INTERVAL: Optional[int] = 60
     """
     Interval to wait (in seconds) before checking whether unfinished job are
     still running on SLURM (see `SlurmWaitThread` in
-    [`clusterfutures`](https://github.com/sampsyo/clusterfutures/blob/master/cfut/__init__.py)).
+    [`clusterfutures`]
+    (https://github.com/sampsyo/clusterfutures/blob/master/cfut/__init__.py)).
     """
 
     FRACTAL_SLURM_KILLWAIT_INTERVAL: Optional[int] = 45
     """
     Interval to wait (in seconds) when the execution of a SLURM-backend job
     failed, before raising a `JobExecutionError`. Must be larger than [SLURM
     `KillWait` timer](https://slurm.schedmd.com/slurm.conf.html#OPT_KillWait),
@@ -284,18 +285,21 @@
     """
     Interval to wait (in seconds) when the SLURM backend does not find an
     output pickle file, which could be for multiple reasons (the SLURM job was
     cancelled, or writing the file is taking long). After this interval, the
     file is considered as missing.
     """
 
-    # NOTE: we currently set FRACTAL_PARSL_MONITORING to False, due to
-    # https://github.com/fractal-analytics-platform/fractal-server/issues/148
-    FRACTAL_PARSL_MONITORING: bool = False
-    FRACTAL_PARSL_CONFIG: str = "local"
+    FRACTAL_CORS_ALLOW_ORIGIN: str = (
+        "http://127.0.0.1:5173;http://localhost:5173"
+    )
+    """
+    Allowed origins for CORS middleware configuration.
+    Default values correspond to `vite` defaults.
+    """
 
     ###########################################################################
     # BUSINESS LOGIC
     ###########################################################################
 
     def check(self):
         """
```

### Comparing `fractal_server-1.2.5a2/fractal_server/logger.py` & `fractal_server-1.3.0a0/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/main.py` & `fractal_server-1.3.0a0/fractal_server/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,23 +145,18 @@
 
     Returns:
         app:
             The fully initialised application.
     """
     app = FastAPI()
     collect_routers(app)
-
+    settings = Inject(get_settings)
     app.add_middleware(
         CORSMiddleware,
-        allow_origins=[
-            "http://127.0.0.1:5173",
-            "http://localhost:5173",
-            "http://127.0.0.1:4173",
-            "http://localhost:4173",
-        ],
+        allow_origins=settings.FRACTAL_CORS_ALLOW_ORIGIN.split(";"),
         allow_methods=["GET", "POST", "PUT", "PATCH", "DELETE", "OPTIONS"],
         allow_headers=[
             "set-cookie",
             "Set-Cookie",
             "Content-Type",
             "Access-Control-Allow-Headers",
             "X-Requested-With",
```

### Comparing `fractal_server-1.2.5a2/fractal_server/migrations/env.py` & `fractal_server-1.3.0a0/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a0/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.3.0a0/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-"""Add user.cache_dir
+"""add ApplyWorkflow.end_timestamp
 
-Revision ID: 385aa8c18489
-Revises: 47072e0106ce
-Create Date: 2023-04-06 10:13:43.234442
+Revision ID: bb1cca2acc40
+Revises: fda995215ae9
+Create Date: 2023-05-12 10:15:50.102921
 
 """
 import sqlalchemy as sa
-import sqlmodel
 from alembic import op
 
 
 # revision identifiers, used by Alembic.
-revision = "385aa8c18489"
-down_revision = "47072e0106ce"
+revision = "bb1cca2acc40"
+down_revision = "fda995215ae9"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     op.add_column(
-        "user_oauth",
-        sa.Column(
-            "cache_dir", sqlmodel.sql.sqltypes.AutoString(), nullable=True
-        ),
+        "applyworkflow",
+        sa.Column("end_timestamp", sa.DateTime(timezone=True), nullable=True),
     )
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_column("user_oauth", "cache_dir")
+    op.drop_column("applyworkflow", "end_timestamp")
     # ### end Alembic commands ###
```

### Comparing `fractal_server-1.2.5a2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.3.0a0/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-"""Initial schema
+"""New initial schema
 
-Revision ID: 47072e0106ce
+Revision ID: e8f4051440be
 Revises:
-Create Date: 2023-03-16 08:37:00.138811
+Create Date: 2023-05-08 09:23:14.013706
 
 """
 import sqlalchemy as sa
-import sqlalchemy_utils
 import sqlmodel
 from alembic import op
 
 
 # revision identifiers, used by Alembic.
-revision = "47072e0106ce"
+revision = "e8f4051440be"
 down_revision = None
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     op.create_table(
         "project",
         sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
-        sa.Column(
-            "project_dir", sqlmodel.sql.sqltypes.AutoString(), nullable=False
-        ),
         sa.Column("read_only", sa.Boolean(), nullable=False),
         sa.Column("id", sa.Integer(), nullable=False),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_table(
         "state",
         sa.Column("data", sa.JSON(), nullable=True),
@@ -55,29 +51,30 @@
         sa.Column(
             "output_type", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_table(
         "user_oauth",
-        sa.Column(
-            "id", sqlalchemy_utils.types.uuid.UUIDType(), nullable=False
-        ),
+        sa.Column("id", sa.Integer(), nullable=False),
         sa.Column("email", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
         sa.Column(
             "hashed_password",
             sqlmodel.sql.sqltypes.AutoString(),
             nullable=False,
         ),
         sa.Column("is_active", sa.Boolean(), nullable=False),
         sa.Column("is_superuser", sa.Boolean(), nullable=False),
         sa.Column("is_verified", sa.Boolean(), nullable=False),
         sa.Column(
             "slurm_user", sqlmodel.sql.sqltypes.AutoString(), nullable=True
         ),
+        sa.Column(
+            "cache_dir", sqlmodel.sql.sqltypes.AutoString(), nullable=True
+        ),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_index(
         op.f("ix_user_oauth_email"), "user_oauth", ["email"], unique=True
     )
     op.create_table(
         "dataset",
@@ -92,29 +89,29 @@
             ["project.id"],
         ),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_table(
         "linkuserproject",
         sa.Column("project_id", sa.Integer(), nullable=False),
-        sa.Column("user_id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
+        sa.Column("user_id", sa.Integer(), nullable=False),
         sa.ForeignKeyConstraint(
             ["project_id"],
             ["project.id"],
         ),
         sa.ForeignKeyConstraint(
             ["user_id"],
             ["user_oauth.id"],
         ),
         sa.PrimaryKeyConstraint("project_id", "user_id"),
     )
     op.create_table(
         "oauthaccount",
-        sa.Column("id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
-        sa.Column("user_id", sqlmodel.sql.sqltypes.GUID(), nullable=False),
+        sa.Column("id", sa.Integer(), nullable=False),
+        sa.Column("user_id", sa.Integer(), nullable=False),
         sa.Column(
             "oauth_name", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
         sa.Column(
             "access_token", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
         sa.Column("expires_at", sa.Integer(), nullable=True),
@@ -211,18 +208,18 @@
         ),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_table(
         "workflowtask",
         sa.Column("meta", sa.JSON(), nullable=True),
         sa.Column("args", sa.JSON(), nullable=True),
-        sa.Column("order", sa.Integer(), nullable=True),
         sa.Column("id", sa.Integer(), nullable=False),
         sa.Column("workflow_id", sa.Integer(), nullable=True),
         sa.Column("task_id", sa.Integer(), nullable=True),
+        sa.Column("order", sa.Integer(), nullable=True),
         sa.ForeignKeyConstraint(
             ["task_id"],
             ["task.id"],
         ),
         sa.ForeignKeyConstraint(
             ["workflow_id"],
             ["workflow.id"],
```

### Comparing `fractal_server-1.2.5a2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.3.0a0/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-"""Drop project.project_dir
+"""Drop ApplyWorkflow.overwrite_input
 
-Revision ID: 6dede8d6fd9d
-Revises: 385aa8c18489
-Create Date: 2023-04-06 10:32:52.972906
+Revision ID: fda995215ae9
+Revises: e8f4051440be
+Create Date: 2023-05-11 17:02:46.208476
 
 """
 import sqlalchemy as sa
 from alembic import op
 
 
 # revision identifiers, used by Alembic.
-revision = "6dede8d6fd9d"
-down_revision = "385aa8c18489"
+revision = "fda995215ae9"
+down_revision = "e8f4051440be"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_column("project", "project_dir")
+    op.drop_column("applyworkflow", "overwrite_input")
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
     op.add_column(
-        "project", sa.Column("project_dir", sa.VARCHAR(), nullable=False)
+        "applyworkflow",
+        sa.Column("overwrite_input", sa.BOOLEAN(), nullable=False),
     )
     # ### end Alembic commands ###
```

### Comparing `fractal_server-1.2.5a2/fractal_server/syringe.py` & `fractal_server-1.3.0a0/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a0/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/fractal_server/utils.py` & `fractal_server-1.3.0a0/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a2/pyproject.toml` & `fractal_server-1.3.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.5a2"
+version = "1.3.0a0"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -15,15 +15,14 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.20.0"
 fastapi = "^0.95.0"
 sqlmodel = "^0.0.8"
 aiosqlite = "^0.17.0"
 fastapi-users = {extras = ["oauth"], version = "^10.1"}
-fastapi-users-db-sqlmodel = "^0.2.0"
 alembic = "^1.9.1"
 uvicorn = "^0.20.0"
 sqlalchemy = "^1.4"
 SQLAlchemy-Utils = "^0.38.3"
 
 clusterfutures = { version = "^0.5", optional = true}
 
@@ -71,15 +70,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.5a2"
+current_version = "1.3.0a0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.5a2/setup.py` & `fractal_server-1.3.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 package_data = \
 {'': ['*'], 'fractal_server.common': ['.github/workflows/*']}
 
 install_requires = \
 ['SQLAlchemy-Utils>=0.38.3,<0.39.0',
  'aiosqlite>=0.17.0,<0.18.0',
  'alembic>=1.9.1,<2.0.0',
- 'fastapi-users-db-sqlmodel>=0.2.0,<0.3.0',
  'fastapi-users[oauth]>=10.1,<11.0',
  'fastapi>=0.95.0,<0.96.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'sqlalchemy>=1.4,<2.0',
  'sqlmodel>=0.0.8,<0.0.9',
  'uvicorn>=0.20.0,<0.21.0']
 
@@ -40,15 +39,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.5a2',
+    'version': '1.3.0a0',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.5a2/PKG-INFO` & `fractal_server-1.3.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.5a2
+Version: 1.3.0a0
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -17,15 +17,14 @@
 Provides-Extra: slurm
 Requires-Dist: SQLAlchemy-Utils (>=0.38.3,<0.39.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "postgres"
 Requires-Dist: clusterfutures (>=0.5,<0.6) ; extra == "slurm"
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
-Requires-Dist: fastapi-users-db-sqlmodel (>=0.2.0,<0.3.0)
 Requires-Dist: fastapi-users[oauth] (>=10.1,<11.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
```


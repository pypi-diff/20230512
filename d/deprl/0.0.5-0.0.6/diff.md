# Comparing `tmp/deprl-0.0.5.tar.gz` & `tmp/deprl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprl-0.0.5.tar", max compression
+gzip compressed data, was "deprl-0.0.6.tar", max compression
```

## Comparing `deprl-0.0.5.tar` & `deprl-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1083 2023-04-19 09:11:34.327760 deprl-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     6881 2023-04-28 12:48:24.334114 deprl-0.0.5/README.md
--rw-r--r--   0        0        0      461 2023-05-11 10:40:58.337940 deprl-0.0.5/deprl/__init__.py
--rw-r--r--   0        0        0     5819 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/custom_agents.py
--rw-r--r--   0        0        0     8859 2023-04-08 11:41:40.942841 deprl-0.0.5/deprl/custom_distributed.py
--rw-r--r--   0        0        0     3639 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/custom_mpo_torch.py
--rw-r--r--   0        0        0     3476 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/custom_test_environment.py
--rw-r--r--   0        0        0     1244 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/custom_torso.py
--rw-r--r--   0        0        0     5818 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/custom_trainer.py
--rw-r--r--   0        0        0     7373 2023-04-08 11:41:40.942841 deprl-0.0.5/deprl/dep_controller.py
--rw-r--r--   0        0        0      132 2023-04-08 11:41:40.942841 deprl-0.0.5/deprl/env_wrappers/__init__.py
--rw-r--r--   0        0        0     5534 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/env_wrappers/wrappers.py
--rw-r--r--   0        0        0     7722 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/main.py
--rw-r--r--   0        0        0      704 2023-04-08 11:41:40.942841 deprl-0.0.5/deprl/param_files/default_agents.json
--rw-r--r--   0        0        0     9038 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/play.py
--rw-r--r--   0        0        0     9383 2023-04-24 13:15:26.620578 deprl-0.0.5/deprl/play_analysis.py
--rw-r--r--   0        0        0       73 2023-04-08 11:41:40.942841 deprl-0.0.5/deprl/utils/__init__.py
--rw-r--r--   0        0        0      608 2023-04-08 11:41:40.942841 deprl-0.0.5/deprl/utils/utils.py
--rw-r--r--   0        0        0       39 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/__init__.py
--rwxr-xr-x   0        0        0       80 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/.gitignore
--rw-r--r--   0        0        0     1110 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/LICENSE
--rw-r--r--   0        0        0      207 2023-05-11 10:40:42.082155 deprl-0.0.5/deprl/vendor/tonic/__init__.py
--rw-r--r--   0        0        0      178 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/agents/__init__.py
--rw-r--r--   0        0        0      946 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/agents/agent.py
--rw-r--r--   0        0        0     3954 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/agents/basic.py
--rw-r--r--   0        0        0      293 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/environments/__init__.py
--rw-r--r--   0        0        0     5641 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/environments/builders.py
--rw-r--r--   0        0        0     6612 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/environments/distributed.py
--rw-r--r--   0        0        0     1914 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/environments/wrappers.py
--rw-r--r--   0        0        0      175 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/explorations/__init__.py
--rw-r--r--   0        0        0     2939 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/explorations/noisy.py
--rw-r--r--   0        0        0     2081 2023-05-11 16:13:46.545684 deprl-0.0.5/deprl/vendor/tonic/log.py
--rw-r--r--   0        0        0     8754 2023-04-21 17:51:40.339710 deprl-0.0.5/deprl/vendor/tonic/play.py
--rw-r--r--   0        0        0    18152 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/plot.py
--rw-r--r--   0        0        0      167 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/replays/__init__.py
--rw-r--r--   0        0        0     3636 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/replays/buffers.py
--rw-r--r--   0        0        0     2815 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/replays/segments.py
--rw-r--r--   0        0        0      821 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/replays/utils.py
--rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/__init__.py
--rw-r--r--   0        0        0      303 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/__init__.py
--rw-r--r--   0        0        0     4630 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/a2c.py
--rw-r--r--   0        0        0      519 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/agent.py
--rw-r--r--   0        0        0     1456 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/d4pg.py
--rw-r--r--   0        0        0     4327 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/ddpg.py
--rw-r--r--   0        0        0     4089 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/mpo.py
--rw-r--r--   0        0        0     2452 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/ppo.py
--rw-r--r--   0        0        0     1868 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/sac.py
--rw-r--r--   0        0        0     2181 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/td3.py
--rw-r--r--   0        0        0     1448 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/td4.py
--rw-r--r--   0        0        0     3754 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/trpo.py
--rw-r--r--   0        0        0      819 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     6247 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/actor_critics.py
--rw-r--r--   0        0        0     4849 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/actors.py
--rw-r--r--   0        0        0     3046 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/critics.py
--rw-r--r--   0        0        0      734 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/encoders.py
--rw-r--r--   0        0        0      627 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1339 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/normalizers/returns.py
--rw-r--r--   0        0        0     1260 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/__init__.py
--rw-r--r--   0        0        0    19301 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/actors.py
--rw-r--r--   0        0        0    13820 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/critics.py
--rw-r--r--   0        0        0     4232 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
--rw-r--r--   0        0        0      193 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/utils.py
--rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/__init__.py
--rw-r--r--   0        0        0      277 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/__init__.py
--rw-r--r--   0        0        0     5287 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/a2c.py
--rw-r--r--   0        0        0      841 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/agent.py
--rw-r--r--   0        0        0     1522 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/d4pg.py
--rw-r--r--   0        0        0     4551 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/ddpg.py
--rw-r--r--   0        0        0     4446 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/mpo.py
--rw-r--r--   0        0        0     2608 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/ppo.py
--rw-r--r--   0        0        0     2102 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/sac.py
--rw-r--r--   0        0        0     2315 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/td3.py
--rw-r--r--   0        0        0     4077 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/agents/trpo.py
--rw-r--r--   0        0        0      817 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/models/__init__.py
--rw-r--r--   0        0        0     5824 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/models/actor_critics.py
--rw-r--r--   0        0        0     4874 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/models/actors.py
--rw-r--r--   0        0        0     3177 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/models/critics.py
--rw-r--r--   0        0        0     1084 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/models/encoders.py
--rw-r--r--   0        0        0      791 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/normalizers/__init__.py
--rw-r--r--   0        0        0     2615 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1429 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/normalizers/returns.py
--rw-r--r--   0        0        0     1156 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/updaters/__init__.py
--rw-r--r--   0        0        0    20504 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/updaters/actors.py
--rw-r--r--   0        0        0    11054 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/updaters/critics.py
--rw-r--r--   0        0        0     4317 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/updaters/optimizers.py
--rw-r--r--   0        0        0      156 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/torch/updaters/utils.py
--rw-r--r--   0        0        0     5722 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/train.py
--rw-r--r--   0        0        0      213 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/utils/__init__.py
--rw-r--r--   0        0        0      822 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/utils/csv_utils.py
--rw-r--r--   0        0        0     8867 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/utils/logger.py
--rw-r--r--   0        0        0     5477 2023-04-21 17:51:40.343710 deprl-0.0.5/deprl/vendor/tonic/utils/trainer.py
--rw-r--r--   0        0        0     1229 2023-05-11 16:18:37.841866 deprl-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 deprl-0.0.5/setup.py
--rw-r--r--   0        0        0     7665 1970-01-01 00:00:00.000000 deprl-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-19 09:11:34.327760 deprl-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     6881 2023-04-28 12:48:24.334114 deprl-0.0.6/README.md
+-rw-r--r--   0        0        0      495 2023-05-12 11:35:17.598376 deprl-0.0.6/deprl/__init__.py
+-rw-r--r--   0        0        0     5819 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/custom_agents.py
+-rw-r--r--   0        0        0     8859 2023-04-08 11:41:40.942841 deprl-0.0.6/deprl/custom_distributed.py
+-rw-r--r--   0        0        0     3639 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/custom_mpo_torch.py
+-rw-r--r--   0        0        0     3476 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/custom_test_environment.py
+-rw-r--r--   0        0        0     1244 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/custom_torso.py
+-rw-r--r--   0        0        0     5818 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/custom_trainer.py
+-rw-r--r--   0        0        0     7373 2023-04-08 11:41:40.942841 deprl-0.0.6/deprl/dep_controller.py
+-rw-r--r--   0        0        0      132 2023-04-08 11:41:40.942841 deprl-0.0.6/deprl/env_wrappers/__init__.py
+-rw-r--r--   0        0        0     5534 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/env_wrappers/wrappers.py
+-rw-r--r--   0        0        0     7722 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/main.py
+-rw-r--r--   0        0        0      704 2023-04-08 11:41:40.942841 deprl-0.0.6/deprl/param_files/default_agents.json
+-rw-r--r--   0        0        0     9038 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/play.py
+-rw-r--r--   0        0        0    10150 2023-05-12 11:16:59.953045 deprl-0.0.6/deprl/play_plot.py
+-rw-r--r--   0        0        0       85 2023-05-12 11:35:18.734361 deprl-0.0.6/deprl/utils/__init__.py
+-rw-r--r--   0        0        0     2982 2023-05-12 11:35:18.734361 deprl-0.0.6/deprl/utils/utils.py
+-rw-r--r--   0        0        0       39 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/__init__.py
+-rwxr-xr-x   0        0        0       80 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/.gitignore
+-rw-r--r--   0        0        0     1110 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/LICENSE
+-rw-r--r--   0        0        0      207 2023-05-11 10:40:42.082155 deprl-0.0.6/deprl/vendor/tonic/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/agents/__init__.py
+-rw-r--r--   0        0        0     1144 2023-05-12 11:33:18.923960 deprl-0.0.6/deprl/vendor/tonic/agents/agent.py
+-rw-r--r--   0        0        0     3954 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/agents/basic.py
+-rw-r--r--   0        0        0      293 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/environments/__init__.py
+-rw-r--r--   0        0        0     5641 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/environments/builders.py
+-rw-r--r--   0        0        0     6612 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/environments/distributed.py
+-rw-r--r--   0        0        0     1914 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/environments/wrappers.py
+-rw-r--r--   0        0        0      175 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/explorations/__init__.py
+-rw-r--r--   0        0        0     2939 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/explorations/noisy.py
+-rw-r--r--   0        0        0     2081 2023-05-11 16:13:46.545684 deprl-0.0.6/deprl/vendor/tonic/log.py
+-rw-r--r--   0        0        0     8754 2023-04-21 17:51:40.339710 deprl-0.0.6/deprl/vendor/tonic/play.py
+-rw-r--r--   0        0        0    18152 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/plot.py
+-rw-r--r--   0        0        0      167 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/replays/__init__.py
+-rw-r--r--   0        0        0     3636 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/replays/buffers.py
+-rw-r--r--   0        0        0     2815 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/replays/segments.py
+-rw-r--r--   0        0        0      821 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/replays/utils.py
+-rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/__init__.py
+-rw-r--r--   0        0        0      303 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/__init__.py
+-rw-r--r--   0        0        0     4630 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/a2c.py
+-rw-r--r--   0        0        0      519 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/agent.py
+-rw-r--r--   0        0        0     1456 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/d4pg.py
+-rw-r--r--   0        0        0     4327 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/ddpg.py
+-rw-r--r--   0        0        0     4089 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/mpo.py
+-rw-r--r--   0        0        0     2452 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/ppo.py
+-rw-r--r--   0        0        0     1868 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/sac.py
+-rw-r--r--   0        0        0     2181 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/td3.py
+-rw-r--r--   0        0        0     1448 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/td4.py
+-rw-r--r--   0        0        0     3754 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/trpo.py
+-rw-r--r--   0        0        0      819 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     6247 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/actor_critics.py
+-rw-r--r--   0        0        0     4849 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/actors.py
+-rw-r--r--   0        0        0     3046 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/critics.py
+-rw-r--r--   0        0        0      734 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/encoders.py
+-rw-r--r--   0        0        0      627 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/utils.py
+-rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1339 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/normalizers/returns.py
+-rw-r--r--   0        0        0     1260 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/__init__.py
+-rw-r--r--   0        0        0    19301 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/actors.py
+-rw-r--r--   0        0        0    13820 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/critics.py
+-rw-r--r--   0        0        0     4232 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
+-rw-r--r--   0        0        0      193 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/utils.py
+-rw-r--r--   0        0        0      103 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/__init__.py
+-rw-r--r--   0        0        0     5287 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/a2c.py
+-rw-r--r--   0        0        0     1184 2023-05-12 11:35:17.638375 deprl-0.0.6/deprl/vendor/tonic/torch/agents/agent.py
+-rw-r--r--   0        0        0     1522 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/d4pg.py
+-rw-r--r--   0        0        0     4551 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/ddpg.py
+-rw-r--r--   0        0        0     4446 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/mpo.py
+-rw-r--r--   0        0        0     2608 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/ppo.py
+-rw-r--r--   0        0        0     2102 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/sac.py
+-rw-r--r--   0        0        0     2315 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/td3.py
+-rw-r--r--   0        0        0     4077 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/agents/trpo.py
+-rw-r--r--   0        0        0      817 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/models/__init__.py
+-rw-r--r--   0        0        0     5824 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/models/actor_critics.py
+-rw-r--r--   0        0        0     4874 2023-05-12 09:59:41.471381 deprl-0.0.6/deprl/vendor/tonic/torch/models/actors.py
+-rw-r--r--   0        0        0     3177 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/models/critics.py
+-rw-r--r--   0        0        0     1084 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/models/encoders.py
+-rw-r--r--   0        0        0      791 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/models/utils.py
+-rw-r--r--   0        0        0       88 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/normalizers/__init__.py
+-rw-r--r--   0        0        0     2615 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1429 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/normalizers/returns.py
+-rw-r--r--   0        0        0     1156 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/updaters/__init__.py
+-rw-r--r--   0        0        0    20504 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/updaters/actors.py
+-rw-r--r--   0        0        0    11054 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/updaters/critics.py
+-rw-r--r--   0        0        0     4317 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/updaters/optimizers.py
+-rw-r--r--   0        0        0      156 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/torch/updaters/utils.py
+-rw-r--r--   0        0        0     5722 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/train.py
+-rw-r--r--   0        0        0      213 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/utils/__init__.py
+-rw-r--r--   0        0        0      822 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/utils/csv_utils.py
+-rw-r--r--   0        0        0     8867 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/utils/logger.py
+-rw-r--r--   0        0        0     5477 2023-04-21 17:51:40.343710 deprl-0.0.6/deprl/vendor/tonic/utils/trainer.py
+-rw-r--r--   0        0        0     1229 2023-05-12 11:41:16.557587 deprl-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 deprl-0.0.6/setup.py
+-rw-r--r--   0        0        0     7665 1970-01-01 00:00:00.000000 deprl-0.0.6/PKG-INFO
```

### Comparing `deprl-0.0.5/LICENSE.txt` & `deprl-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/README.md` & `deprl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/custom_agents.py` & `deprl-0.0.6/deprl/custom_agents.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/custom_distributed.py` & `deprl-0.0.6/deprl/custom_distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/custom_mpo_torch.py` & `deprl-0.0.6/deprl/custom_mpo_torch.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/custom_test_environment.py` & `deprl-0.0.6/deprl/custom_test_environment.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/custom_torso.py` & `deprl-0.0.6/deprl/custom_torso.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/custom_trainer.py` & `deprl-0.0.6/deprl/custom_trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/dep_controller.py` & `deprl-0.0.6/deprl/dep_controller.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/env_wrappers/wrappers.py` & `deprl-0.0.6/deprl/env_wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/main.py` & `deprl-0.0.6/deprl/main.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/param_files/default_agents.json` & `deprl-0.0.6/deprl/param_files/default_agents.json`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/play.py` & `deprl-0.0.6/deprl/play.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/play_analysis.py` & `deprl-0.0.6/deprl/vendor/tonic/play.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,62 @@
 """Script used to play with trained agents."""
 
 import argparse
 import os
 
 import numpy as np
+import tonic  # noqa
 import yaml
 
-from deprl import env_wrappers
-
-from .vendor.tonic import logger
-from matplotlib import pyplot as plt
-
 
 def play_gym(agent, environment):
     """Launches an agent in a Gym-based environment."""
-    environment = env_wrappers.apply_wrapper(environment)
-    observations = environment.reset()
-    tendon_states = environment.tendon_states
+
+    environment = tonic.environments.distribute(lambda: environment)
+
+    observations = environment.start()
     environment.render()
 
     score = 0
     length = 0
     min_reward = float("inf")
     max_reward = -float("inf")
     global_min_reward = float("inf")
     global_max_reward = -float("inf")
     steps = 0
     episodes = 0
-    data = []
+
     while True:
-        actions = agent.test_step(
-            observations, tendon_states=tendon_states, steps=1e6
-        )
-        if len(actions.shape) > 1:
-            actions = actions[0, :]
-        observations, reward, done, info = environment.step(actions)
-        data.append(environment.sim.data.qpos[:].copy())
-        tendon_states = environment.tendon_states
+        actions = agent.test_step(observations, steps)
+        observations, infos = environment.step(actions)
+        agent.test_update(**infos, steps=steps)
         environment.render()
 
         steps += 1
+        reward = infos["rewards"][0]
         score += reward
         min_reward = min(min_reward, reward)
         max_reward = max(max_reward, reward)
         global_min_reward = min(global_min_reward, reward)
         global_max_reward = max(global_max_reward, reward)
         length += 1
 
-        if done or length >= environment.max_episode_steps:
+        if infos["resets"][0]:
+            term = infos["terminations"][0]
             episodes += 1
-            fig, axs = plt.subplots(data[0].shape[0], 1, figsize=(10, 10))
-            for i in range(data[0].shape[0]):
-                y = [x[i] for x in data]
-                axs[i].plot(y)
-            plt.show()
-            data = []
 
             print()
             print(f"Episodes: {episodes:,}")
             print(f"Score: {score:,.3f}")
             print(f"Length: {length:,}")
-            print(f"Terminal: {done:}")
+            print(f"Terminal: {term:}")
             print(f"Min reward: {min_reward:,.3f}")
             print(f"Max reward: {max_reward:,.3f}")
             print(f"Global min reward: {min_reward:,.3f}")
             print(f"Global max reward: {max_reward:,.3f}")
-            environment.reset()
 
             score = 0
             length = 0
             min_reward = float("inf")
             max_reward = -float("inf")
 
 
@@ -89,15 +76,14 @@
             self.infos = None
             self.steps = 0
             self.episodes = 0
             self.min_reward = float("inf")
             self.max_reward = -float("inf")
             self.global_min_reward = float("inf")
             self.global_max_reward = -float("inf")
-            self.max_vel = 0
 
         def reset(self):
             """Mimics a dm_control reset for the viewer."""
 
             self.observations = self.environment.reset()[None]
 
             self.score = 0
@@ -140,54 +126,45 @@
                 rewards=np.array([rew]),
                 resets=np.array([done]),
                 terminations=np.array([term]),
             )
 
             return self.unwrapped.last_time_step
 
-        @property
-        def tendon_states(self):
-            return self.environment.tendon_states
-
     # Wrap the environment for the viewer.
-    environment = env_wrappers.apply_wrapper(environment)
     environment = Wrapper(environment)
 
     def policy(timestep):
         """Mimics a dm_control policy for the viewer."""
+
         if environment.infos is not None:
             agent.test_update(**environment.infos, steps=environment.steps)
             environment.steps += 1
-        tendon_states = environment.tendon_states
-        return agent.test_step(
-            environment.observations,
-            tendon_states=tendon_states,
-            steps=environment.steps,
-        )
+        return agent.test_step(environment.observations, environment.steps)
 
     # Launch the viewer with the wrapped environment and policy.
     viewer.launch(environment, policy)
 
 
 def play(path, checkpoint, seed, header, agent, environment):
     """Reloads an agent and an environment from a previous experiment."""
 
     checkpoint_path = None
 
     if path:
-        logger.log(f"Loading experiment from {path}")
+        tonic.logger.log(f"Loading experiment from {path}")
 
         # Use no checkpoint, the agent is freshly created.
         if checkpoint == "none" or agent is not None:
-            logger.log("Not loading any weights")
+            tonic.logger.log("Not loading any weights")
 
         else:
             checkpoint_path = os.path.join(path, "checkpoints")
             if not os.path.isdir(checkpoint_path):
-                logger.error(f"{checkpoint_path} is not a directory")
+                tonic.logger.error(f"{checkpoint_path} is not a directory")
                 checkpoint_path = None
 
             # List all the checkpoints.
             checkpoint_ids = []
             for file in os.listdir(checkpoint_path):
                 if file[:5] == "step_":
                     checkpoint_id = file.split(".")[0]
@@ -205,22 +182,22 @@
                 else:
                     checkpoint_id = int(checkpoint)
                     if checkpoint_id in checkpoint_ids:
                         checkpoint_path = os.path.join(
                             checkpoint_path, f"step_{checkpoint_id}"
                         )
                     else:
-                        logger.error(
+                        tonic.logger.error(
                             f"Checkpoint {checkpoint_id} "
                             f"not found in {checkpoint_path}"
                         )
                         checkpoint_path = None
 
             else:
-                logger.error(f"No checkpoint found in {checkpoint_path}")
+                tonic.logger.error(f"No checkpoint found in {checkpoint_path}")
                 checkpoint_path = None
 
         # Load the experiment configuration.
         arguments_path = os.path.join(path, "config.yaml")
         with open(arguments_path, "r") as config_file:
             config = yaml.load(config_file, Loader=yaml.FullLoader)
         config = argparse.Namespace(**config)
@@ -239,31 +216,37 @@
         raise ValueError("No agent specified.")
     agent = eval(agent)
 
     # Build the environment.
     environment = eval(environment)
     environment.seed(seed)
 
-    # Adapt mpo specific settings
-    if "config" in locals():
-        if "mpo_args" in config:
-            agent.set_params(**config.mpo_args)
     # Initialize the agent.
     agent.initialize(
         observation_space=environment.observation_space,
         action_space=environment.action_space,
         seed=seed,
     )
 
     # Load the weights of the agent form a checkpoint.
     if checkpoint_path:
         agent.load(checkpoint_path)
-    if "ontrol" in type(environment).__name__:
+
+    # Play with the agent in the environment.
+    if isinstance(environment, tonic.environments.wrappers.ActionRescaler):
+        environment_type = environment.env.__class__.__name__
+    else:
+        environment_type = environment.__class__.__name__
+
+    if environment_type == "ControlSuiteEnvironment":
         play_control_suite(agent, environment)
-    play_gym(agent, environment)
+    else:
+        if "Bullet" in environment_type:
+            environment.render()
+        play_gym(agent, environment)
 
 
 if __name__ == "__main__":
     # Argument parsing.
     parser = argparse.ArgumentParser()
     parser.add_argument("--path")
     parser.add_argument("--checkpoint", default="last")
```

### Comparing `deprl-0.0.5/deprl/vendor/tonic/LICENSE` & `deprl-0.0.6/deprl/vendor/tonic/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/agents/agent.py` & `deprl-0.0.6/deprl/vendor/tonic/agents/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,7 +28,14 @@
     def save(self, path):
         """Saves the agent weights during training."""
         pass
 
     def load(self, path):
         """Reloads the agent weights from a checkpoint."""
         pass
+
+    def load_policy(self, path):
+        """Reloads the agent weights from a checkpoint."""
+        pass
+
+    def __call__(self, observation):
+        return self.test_step(observation, steps=1e6)
```

### Comparing `deprl-0.0.5/deprl/vendor/tonic/agents/basic.py` & `deprl-0.0.6/deprl/vendor/tonic/agents/basic.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/environments/builders.py` & `deprl-0.0.6/deprl/vendor/tonic/environments/builders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/environments/distributed.py` & `deprl-0.0.6/deprl/vendor/tonic/environments/distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/environments/wrappers.py` & `deprl-0.0.6/deprl/vendor/tonic/environments/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/explorations/noisy.py` & `deprl-0.0.6/deprl/vendor/tonic/explorations/noisy.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/log.py` & `deprl-0.0.6/deprl/vendor/tonic/log.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/play.py` & `deprl-0.0.6/deprl/play_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,96 @@
 """Script used to play with trained agents."""
 
 import argparse
 import os
 
 import numpy as np
-import tonic  # noqa
 import yaml
 
+from deprl import env_wrappers
+
+from .vendor.tonic import logger
+import matplotlib.pyplot as plt
 
-def play_gym(agent, environment):
-    """Launches an agent in a Gym-based environment."""
 
-    environment = tonic.environments.distribute(lambda: environment)
+def plot_rwd_dict(rwd_dict):
+    fig, axs = plt.subplots(len(rwd_dict.keys()) + 2, 1, figsize=(10, 10))
+    # fig, axs = plt.subplots(5, 1, figsize=(10, 10))
+    i = 0
+    for k, v in rwd_dict.items():
+        axs[i].plot(v, label=k)
+        axs[i].set_title(k)
+        axs[i].grid()
+        i += 1
+        print(f'{k}: {np.sum(v)}')
 
-    observations = environment.start()
+    plt.show()
+
+def play_gym(agent, environment):
+    """Launches an agent in a Gym-based environment."""
+    environment = env_wrappers.apply_wrapper(environment)
+    observations = environment.reset()
+    tendon_states = environment.tendon_states
     environment.render()
 
     score = 0
     length = 0
     min_reward = float("inf")
     max_reward = -float("inf")
     global_min_reward = float("inf")
     global_max_reward = -float("inf")
     steps = 0
     episodes = 0
+    rwd_dict = {k: [] for k in environment.rwd_dict.keys()}
+    rwd_dict['hiprot_l'] = []
+    rwd_dict['hiprot_r'] = []
+    rwd_dict['hipadd_l'] = []
+    rwd_dict['hipadd_r'] = []
+
 
     while True:
-        actions = agent.test_step(observations, steps)
-        observations, infos = environment.step(actions)
-        agent.test_update(**infos, steps=steps)
+        actions = agent.test_step(
+            observations, tendon_states=tendon_states, steps=1e6
+        )
+        if len(actions.shape) > 1:
+            actions = actions[0, :]
+        observations, reward, done, info = environment.step(actions)
+        tendon_states = environment.tendon_states
         environment.render()
 
         steps += 1
-        reward = infos["rewards"][0]
         score += reward
         min_reward = min(min_reward, reward)
         max_reward = max(max_reward, reward)
         global_min_reward = min(global_min_reward, reward)
         global_max_reward = max(global_max_reward, reward)
         length += 1
+        # environment.max_episode_steps = 1000000
+        for k,v in environment.rwd_dict.items():
+            rwd_dict[k].append(v)
+        rwd_dict['hiprot_l'].append(environment.env._get_angle(['hip_rotation_l'])[0].copy())
+        rwd_dict['hiprot_r'].append(environment.env._get_angle(['hip_rotation_r'])[0].copy())
+        rwd_dict['hipadd_l'].append(environment.env._get_angle(['hip_adduction_l'])[0].copy())
+        rwd_dict['hipadd_r'].append(environment.env._get_angle(['hip_adduction_r'])[0].copy())
 
-        if infos["resets"][0]:
-            term = infos["terminations"][0]
+        if done or length >= environment.max_episode_steps:
             episodes += 1
 
             print()
             print(f"Episodes: {episodes:,}")
             print(f"Score: {score:,.3f}")
             print(f"Length: {length:,}")
-            print(f"Terminal: {term:}")
+            print(f"Terminal: {done:}")
             print(f"Min reward: {min_reward:,.3f}")
             print(f"Max reward: {max_reward:,.3f}")
             print(f"Global min reward: {min_reward:,.3f}")
             print(f"Global max reward: {max_reward:,.3f}")
+            environment.reset()
+            plot_rwd_dict(rwd_dict)
+
 
             score = 0
             length = 0
             min_reward = float("inf")
             max_reward = -float("inf")
 
 
@@ -76,14 +110,15 @@
             self.infos = None
             self.steps = 0
             self.episodes = 0
             self.min_reward = float("inf")
             self.max_reward = -float("inf")
             self.global_min_reward = float("inf")
             self.global_max_reward = -float("inf")
+            self.max_vel = 0
 
         def reset(self):
             """Mimics a dm_control reset for the viewer."""
 
             self.observations = self.environment.reset()[None]
 
             self.score = 0
@@ -126,45 +161,54 @@
                 rewards=np.array([rew]),
                 resets=np.array([done]),
                 terminations=np.array([term]),
             )
 
             return self.unwrapped.last_time_step
 
+        @property
+        def tendon_states(self):
+            return self.environment.tendon_states
+
     # Wrap the environment for the viewer.
+    environment = env_wrappers.apply_wrapper(environment)
     environment = Wrapper(environment)
 
     def policy(timestep):
         """Mimics a dm_control policy for the viewer."""
-
         if environment.infos is not None:
             agent.test_update(**environment.infos, steps=environment.steps)
             environment.steps += 1
-        return agent.test_step(environment.observations, environment.steps)
+        tendon_states = environment.tendon_states
+        return agent.test_step(
+            environment.observations,
+            tendon_states=tendon_states,
+            steps=environment.steps,
+        )
 
     # Launch the viewer with the wrapped environment and policy.
     viewer.launch(environment, policy)
 
 
 def play(path, checkpoint, seed, header, agent, environment):
     """Reloads an agent and an environment from a previous experiment."""
 
     checkpoint_path = None
 
     if path:
-        tonic.logger.log(f"Loading experiment from {path}")
+        logger.log(f"Loading experiment from {path}")
 
         # Use no checkpoint, the agent is freshly created.
         if checkpoint == "none" or agent is not None:
-            tonic.logger.log("Not loading any weights")
+            logger.log("Not loading any weights")
 
         else:
             checkpoint_path = os.path.join(path, "checkpoints")
             if not os.path.isdir(checkpoint_path):
-                tonic.logger.error(f"{checkpoint_path} is not a directory")
+                logger.error(f"{checkpoint_path} is not a directory")
                 checkpoint_path = None
 
             # List all the checkpoints.
             checkpoint_ids = []
             for file in os.listdir(checkpoint_path):
                 if file[:5] == "step_":
                     checkpoint_id = file.split(".")[0]
@@ -182,22 +226,22 @@
                 else:
                     checkpoint_id = int(checkpoint)
                     if checkpoint_id in checkpoint_ids:
                         checkpoint_path = os.path.join(
                             checkpoint_path, f"step_{checkpoint_id}"
                         )
                     else:
-                        tonic.logger.error(
+                        logger.error(
                             f"Checkpoint {checkpoint_id} "
                             f"not found in {checkpoint_path}"
                         )
                         checkpoint_path = None
 
             else:
-                tonic.logger.error(f"No checkpoint found in {checkpoint_path}")
+                logger.error(f"No checkpoint found in {checkpoint_path}")
                 checkpoint_path = None
 
         # Load the experiment configuration.
         arguments_path = os.path.join(path, "config.yaml")
         with open(arguments_path, "r") as config_file:
             config = yaml.load(config_file, Loader=yaml.FullLoader)
         config = argparse.Namespace(**config)
@@ -216,37 +260,31 @@
         raise ValueError("No agent specified.")
     agent = eval(agent)
 
     # Build the environment.
     environment = eval(environment)
     environment.seed(seed)
 
+    # Adapt mpo specific settings
+    if "config" in locals():
+        if "mpo_args" in config:
+            agent.set_params(**config.mpo_args)
     # Initialize the agent.
     agent.initialize(
         observation_space=environment.observation_space,
         action_space=environment.action_space,
         seed=seed,
     )
 
     # Load the weights of the agent form a checkpoint.
     if checkpoint_path:
         agent.load(checkpoint_path)
-
-    # Play with the agent in the environment.
-    if isinstance(environment, tonic.environments.wrappers.ActionRescaler):
-        environment_type = environment.env.__class__.__name__
-    else:
-        environment_type = environment.__class__.__name__
-
-    if environment_type == "ControlSuiteEnvironment":
+    if "ontrol" in type(environment).__name__:
         play_control_suite(agent, environment)
-    else:
-        if "Bullet" in environment_type:
-            environment.render()
-        play_gym(agent, environment)
+    play_gym(agent, environment)
 
 
 if __name__ == "__main__":
     # Argument parsing.
     parser = argparse.ArgumentParser()
     parser.add_argument("--path")
     parser.add_argument("--checkpoint", default="last")
```

### Comparing `deprl-0.0.5/deprl/vendor/tonic/plot.py` & `deprl-0.0.6/deprl/vendor/tonic/plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/replays/buffers.py` & `deprl-0.0.6/deprl/vendor/tonic/replays/buffers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/replays/segments.py` & `deprl-0.0.6/deprl/vendor/tonic/replays/segments.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/replays/utils.py` & `deprl-0.0.6/deprl/vendor/tonic/replays/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/a2c.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/agent.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/d4pg.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/ddpg.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/mpo.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/ppo.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/sac.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/td3.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/td4.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/td4.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/agents/trpo.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/__init__.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/actor_critics.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/actors.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/critics.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/encoders.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/models/utils.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/normalizers/returns.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/__init__.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/actors.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/critics.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/tensorflow/updaters/optimizers.py` & `deprl-0.0.6/deprl/vendor/tonic/tensorflow/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/a2c.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/agent.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,7 +24,17 @@
     def load(self, path):
         path = path + ".pt"
         logger.log(f"\nLoading weights from {path}")
         if torch.cuda.is_available():
             self.model.load_state_dict(torch.load(path))
         else:
             self.model.load_state_dict(torch.load(path, map_location="cpu"))
+
+    def load_policy(self, path):
+        path = path + ".pt"
+        logger.log(f"\nLoading weights from {path}")
+        if torch.cuda.is_available():
+            self.model.actor.load_state_dict(torch.load(path))
+        else:
+            self.model.actor.load_state_dict(
+                torch.load(path, map_location="cpu")
+            )
```

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/d4pg.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/ddpg.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/mpo.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/ppo.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/sac.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/td3.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/agents/trpo.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/models/__init__.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/models/actor_critics.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/models/actors.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/models/critics.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/models/encoders.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/models/utils.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/normalizers/mean_stds.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/normalizers/returns.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/updaters/__init__.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/updaters/actors.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/updaters/critics.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/torch/updaters/optimizers.py` & `deprl-0.0.6/deprl/vendor/tonic/torch/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/train.py` & `deprl-0.0.6/deprl/vendor/tonic/train.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/utils/csv_utils.py` & `deprl-0.0.6/deprl/vendor/tonic/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/utils/logger.py` & `deprl-0.0.6/deprl/vendor/tonic/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/deprl/vendor/tonic/utils/trainer.py` & `deprl-0.0.6/deprl/vendor/tonic/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.0.5/pyproject.toml` & `deprl-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deprl"
-version = "0.0.5"
+version = "0.0.6"
 description = "DEP-RL, a method for robust control of musculoskeletal systems."
 authors = ["Pierre Schumacher <pierre.schumacher@tuebingen.mpg.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

### Comparing `deprl-0.0.5/setup.py` & `deprl-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'torch>=1.13.1']
 
 entry_points = \
 {'console_scripts': ['log = deprl.vendor.tonic.log:main']}
 
 setup_kwargs = {
     'name': 'deprl',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'DEP-RL, a method for robust control of musculoskeletal systems.',
     'long_description': '# DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems\n\n This repo contains the code for the paper [DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems](https://openreview.net/forum?id=C-xa_D3oTj6) paper, published at ICLR 2023 with perfect review scores (8, 8, 8, 10) and a notable-top-25% rating. See [here](https://sites.google.com/view/dep-rl) for videos.\n\nThe work was performed by Pierre Schumacher, Daniel F.B. Haeufle, Dieter Büchler, Syn Schmitt and Georg Martius.\n\nIf you just want to see the code for DEP, take a look at `deprl/dep_controller.py`, `deprl/custom_agents.py` and `deprl/env_wrapper/wrappers.py`\n\n<p align="center">\n<img src=https://user-images.githubusercontent.com/24903880/229783811-44c422e9-3cc3-42e4-b657-d21be9af6458.gif width=250>\n<img src=https://user-images.githubusercontent.com/24903880/229783729-d068e87c-cb0b-43c7-91d5-ff2ba836f05b.gif width=214>\n\n <img src=https://user-images.githubusercontent.com/24903880/229783370-ee95b9c3-06a0-4ef3-9b60-78e88c4eae38.gif width=214>\n</p>\n\n\n## Abstract\nMuscle-actuated organisms are capable of learning an unparalleled diversity of\ndexterous movements despite their vast amount of muscles. Reinforcement learning (RL) on large musculoskeletal models, however, has not been able to show\nsimilar performance. We conjecture that ineffective exploration in large overactuated action spaces is a key problem. This is supported by our finding that common\nexploration noise strategies are inadequate in synthetic examples of overactuated\nsystems. We identify differential extrinsic plasticity (DEP), a method from the\ndomain of self-organization, as being able to induce state-space covering exploration within seconds of interaction. By integrating DEP into RL, we achieve fast\nlearning of reaching and locomotion in musculoskeletal systems, outperforming\ncurrent approaches in all considered tasks in sample efficiency and robustness.\n\n\n## Installation\n\nWe provide a python package for easy installation:\n```\npip install deprl\n```\nIf you would like to use `jax` with CUDA support, which significantly speeds up learning, we recommend running:\n```\npip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html\n```\nor similar afterwards.\n\nThe humanreacher environment can be installed with\n```\npip install git+https://github.com/P-Schumacher/warmup.git\n```\n\nOstrichRL can be installed from [here](https://github.com/vittorione94/ostrichrl).\n\n\n## Experiments\n\nThe major experiments (humanreacher reaching and ostrich running) can be repeated with the config files.\nSimply run from the root folder:\n```\npython -m deprl.main experiments/ostrich_running_dep.json\npython -m deprl.main experiments/humanreacher.json\n```\nto train an agent. Model checkpoints will be saved in the `output` directory.\nThe progress can be monitored with:\n```\npython -m tonic.plot --path output/folder/\n```\n\nTo execute a trained policy, use:\n\n```\npython -m deprl.play --path output/folder/\n```\n\nSee the [TonicRL](https://github.com/fabiopardo/tonic) documentation for details.\n\nBe aware that ostrich training can be seed-dependant, as seen in the plots of the original publication.\n\n## Pure DEP\nIf you want to see pure DEP in action, just run the following bash files after installing the ostrichrl and warmup environments.\n```\nbash play_files/play_dep_humanreacher.sh\nbash play_files/play_dep_ostrich.sh\nbash play_files/play_dep_dmcontrol_quadruped.sh\n```\n\nYou might see a more interesting ostrich behavior by disabling episode resets in the ostrich environment first.\n## Environments\n\nThe ostrich environment can be found [here](https://github.com/vittorione94/ostrichrl) and is installed automatically via poetry.\n\nThe arm-environment [warmup](https://github.com/P-Schumacher/warmup) is also automatically installed by poetry and can be used like any other gym environment:\n\n```\nimport gym\nimport warmup\n\nenv = gym.make("humanreacher-v0")\n\nfor ep in range(5):\n     ep_steps = 0\n     state = env.reset()\n     while True:\n         next_state, reward, done, info = env.step(env.action_space.sample())\n         env.render()\n         if done or (ep_steps >= env.max_episode_steps):\n             break\n         ep_steps += 1\n\n```\n\nThe humanoid environments were simulated with [SCONE](https://scone.software/doku.php?id=start). A ready-to-use RL package will be released in cooperation with GOATSTREAM at a later date.\n\n## Source Code Installation\n\nWe recommend an installation with [poetry](https://python-poetry.org/) to ensure reproducibility.\nWhile [TonicRL](https://github.com/fabiopardo/tonic) with PyTorch is used for the RL algorithms, DEP itself is implemented in JAX. We *strongly* recommend GPU-usage to speed up the computation of DEP. On systems without GPUs, give the tensorflow version of TonicRL a try! We alternatively provide a pip_requirements file.\n1. Make sure to install poetry and deactivate all virtual environments.\n2. Clone the environment\n```\ngit clone https://github.com/martius-lab/depRL\n```\n\n3. Go to the root folder and run\n```\npoetry install\npoetry shell\n```\n\nThat\'s it!\n\nThe build has been tested with:\n```\nUbuntu 20.04 and Ubuntu 22.04\nCUDA 12.0\npoetry 1.4.0\n```\n### Troubleshooting\n* A common error with poetry is a faulty interaction with the python keyring, resulting in a `Failed to unlock the collection!`-error. It could also happen that the dependency solving takes very long (more than 60s), this is caused by the same error.\n  If it happens, try to append\n```\nexport PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring\n```\nto your bashrc. You can also try to prepend it to the poetry command: `PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring poetry install`.\n* If you have an error related to your `ptxas` version, this means that your cuda environment is not setup correctly and you should install the cuda-toolkit. The easiest way is to do this via conda if you don\'t have admin rights on your workstation.\n  I recommend running\n```\nconda install -c conda-forge cudatoolkit-dev\n```\n* In any other case, first try to delete the `poetry.lock` file and the virtual env `.venv`, then run `poetry install` again.\n\n\nFeel free to open an issue if you encounter any problems.\n\n## Citation\n\nPlease use the following citation if you make use of our work:\n\n```\n@inproceedings{schumacher2023:deprl,\n  title = {DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems},\n  author = {Schumacher, Pierre and Haeufle, Daniel F.B. and B{\\"u}chler, Dieter and Schmitt, Syn and Martius, Georg},\n  booktitle = {Proceedings of the Eleventh International Conference on Learning Representations (ICLR)},\n  month = may,\n  year = {2023},\n  doi = {},\n  url = {https://openreview.net/forum?id=C-xa_D3oTj6},\n  month_numeric = {5}\n}\n```\n',
     'author': 'Pierre Schumacher',
     'author_email': 'pierre.schumacher@tuebingen.mpg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deprl-0.0.5/PKG-INFO` & `deprl-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprl
-Version: 0.0.5
+Version: 0.0.6
 Summary: DEP-RL, a method for robust control of musculoskeletal systems.
 License: MIT
 Author: Pierre Schumacher
 Author-email: pierre.schumacher@tuebingen.mpg.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


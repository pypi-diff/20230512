# Comparing `tmp/dev-gpt-0.18.40.dev6.tar.gz` & `tmp/dev-gpt-0.18.41.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.40.dev6.tar", last modified: Fri May 12 14:24:08 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.41.dev1.tar", last modified: Fri May 12 14:25:15 2023, max compression
```

## Comparing `dev-gpt-0.18.40.dev6.tar` & `dev-gpt-0.18.41.dev1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.861571 dev-gpt-0.18.40.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-05-12 14:24:08.861571 dev-gpt-0.18.40.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 14:24:07.000000 dev-gpt-0.18.40.dev6/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/auto_refine_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/extract_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/get_user_input_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/pm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/pm/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/pm/task_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/prompt_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.853571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.857571 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-05-12 14:24:08.000000 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-12 14:24:08.000000 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:24:08.000000 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 14:24:08.000000 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 14:24:08.000000 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 14:24:08.000000 dev-gpt-0.18.40.dev6/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:24:08.861571 dev-gpt-0.18.40.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.861571 dev-gpt-0.18.40.dev6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.861571 dev-gpt-0.18.40.dev6/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:08.861571 dev-gpt-0.18.40.dev6/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/unit/test_construct_sub_task_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-12 14:24:00.000000 dev-gpt-0.18.40.dev6/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.228566 dev-gpt-0.18.41.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-05-12 14:25:15.228566 dev-gpt-0.18.41.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.216566 dev-gpt-0.18.41.dev1/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 14:25:14.000000 dev-gpt-0.18.41.dev1/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.216566 dev-gpt-0.18.41.dev1/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.220566 dev-gpt-0.18.41.dev1/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.220566 dev-gpt-0.18.41.dev1/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.220566 dev-gpt-0.18.41.dev1/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.220566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/auto_refine_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/extract_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/get_user_input_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/pm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/pm/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/pm/task_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/prompt_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.212566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.216566 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-05-12 14:25:15.000000 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-12 14:25:15.000000 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:25:15.000000 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 14:25:15.000000 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 14:25:15.000000 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 14:25:15.000000 dev-gpt-0.18.41.dev1/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:25:15.228566 dev-gpt-0.18.41.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.224566 dev-gpt-0.18.41.dev1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:15.228566 dev-gpt-0.18.41.dev1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/unit/test_construct_sub_task_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-12 14:25:07.000000 dev-gpt-0.18.41.dev1/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.40.dev6/LICENSE` & `dev-gpt-0.18.41.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/PKG-INFO` & `dev-gpt-0.18.41.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.40.dev6
+Version: 0.18.41.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.40.dev6 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.41.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.40.dev6/README.md` & `dev-gpt-0.18.41.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.41.dev1/dev_gpt/apis/gpt.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.41.dev1/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.41.dev1/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/cli.py` & `dev-gpt-0.18.41.dev1/dev_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/constants.py` & `dev-gpt-0.18.41.dev1/dev_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/__init__.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/auto_refine_description.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/auto_refine_description.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/extract_information.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/extract_information.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/get_user_input_if_needed.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/get_user_input_if_needed.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/question_answering.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/question_answering.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/translation.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/translation.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/pm/pm.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/pm/pm.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/pm/task_tree_schema.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/pm/task_tree_schema.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/templates_user.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.41.dev1/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/utils/io.py` & `dev-gpt-0.18.41.dev1/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.41.dev1/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.41.dev1/dev_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.40.dev6
+Version: 0.18.41.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.40.dev6 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.41.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.40.dev6/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.41.dev1/dev_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/setup.py` & `dev-gpt-0.18.41.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/test/conftest.py` & `dev-gpt-0.18.41.dev1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/test/integration/test_generator.py` & `dev-gpt-0.18.41.dev1/test/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/test/unit/test_api.py` & `dev-gpt-0.18.41.dev1/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.40.dev6/test/unit/test_response_parsing.py` & `dev-gpt-0.18.41.dev1/test/unit/test_response_parsing.py`

 * *Files identical despite different names*


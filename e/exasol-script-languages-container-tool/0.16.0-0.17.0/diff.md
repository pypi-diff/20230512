# Comparing `tmp/exasol-script-languages-container-tool-0.16.0.tar.gz` & `tmp/exasol_script_languages_container_tool-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol-script-languages-container-tool-0.16.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_tool-0.17.0.tar", max compression
```

## Comparing `exasol-script-languages-container-tool-0.16.0.tar` & `exasol_script_languages_container_tool-0.17.0.tar`

### file list

```diff
@@ -1,89 +1,93 @@
--rw-r--r--   0        0        0     1063 2023-03-20 13:54:59.720430 exasol-script-languages-container-tool-0.16.0/LICENSE
--rw-r--r--   0        0        0     7271 2023-03-20 13:54:59.720430 exasol-script-languages-container-tool-0.16.0/README.md
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/__init__.py
--rw-r--r--   0        0        0      393 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/__init__.py
--rw-r--r--   0        0        0     3825 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/build.py
--rw-r--r--   0        0        0     2357 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/clean.py
--rw-r--r--   0        0        0     3781 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/export.py
--rw-r--r--   0        0        0     1066 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py
--rw-r--r--   0        0        0     1070 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py
--rw-r--r--   0        0        0     3057 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/push.py
--rw-r--r--   0        0        0    11899 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py
--rw-r--r--   0        0        0     3551 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/save.py
--rw-r--r--   0        0        0     3657 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/security_scan.py
--rw-r--r--   0        0        0     4519 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/upload.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/options/__init__.py
--rw-r--r--   0        0        0      820 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/options/flavor_options.py
--rw-r--r--   0        0        0      617 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/options/goal_options.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/__init__.py
--rw-r--r--   0        0        0      394 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/__init__.py
--rw-r--r--   0        0        0       50 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/api_errors.py
--rw-r--r--   0        0        0     3049 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/build.py
--rw-r--r--   0        0        0     2588 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/clean.py
--rw-r--r--   0        0        0     3214 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/export.py
--rw-r--r--   0        0        0     1681 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py
--rw-r--r--   0        0        0      733 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py
--rw-r--r--   0        0        0     3186 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/push.py
--rw-r--r--   0        0        0     9072 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py
--rw-r--r--   0        0        0     3240 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/save.py
--rw-r--r--   0        0        0     3264 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/security_scan.py
--rw-r--r--   0        0        0     4081 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/upload.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/__init__.py
--rw-r--r--   0        0        0     1487 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py
--rw-r--r--   0        0        0     1311 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py
--rw-r--r--   0        0        0     4219 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/clean/__init__.py
--rw-r--r--   0        0        0     4470 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/__init__.py
--rw-r--r--   0        0        0      525 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py
--rw-r--r--   0        0        0     9855 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py
--rw-r--r--   0        0        0     1366 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py
--rw-r--r--   0        0        0     1736 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py
--rw-r--r--   0        0        0     3701 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py
--rw-r--r--   0        0        0      756 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py
--rw-r--r--   0        0        0     2958 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/push/__init__.py
--rw-r--r--   0        0        0     1702 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/save/__init__.py
--rw-r--r--   0        0        0     1600 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py
--rw-r--r--   0        0        0      231 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save_parameter.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/security_scan/__init__.py
--rw-r--r--   0        0        0     5728 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py
--rw-r--r--   0        0        0      223 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan_parameter.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/__init__.py
--rw-r--r--   0        0        0      553 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py
--rw-r--r--   0        0        0     1973 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py
--rw-r--r--   0        0        0     6871 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py
--rw-r--r--   0        0        0     2246 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py
--rw-r--r--   0        0        0     1961 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py
--rw-r--r--   0        0        0     2840 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py
--rw-r--r--   0        0        0     2235 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py
--rw-r--r--   0        0        0     3179 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py
--rw-r--r--   0        0        0     1450 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py
--rw-r--r--   0        0        0     8499 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py
--rw-r--r--   0        0        0     1420 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py
--rw-r--r--   0        0        0     9449 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py
--rw-r--r--   0        0        0     1010 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/__init__.py
--rw-r--r--   0        0        0     2663 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py
--rw-r--r--   0        0        0     4863 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py
--rw-r--r--   0        0        0      630 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py
--rw-r--r--   0        0        0     1312 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py
--rw-r--r--   0        0        0     1545 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py
--rw-r--r--   0        0        0     2995 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py
--rw-r--r--   0        0        0      248 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers_parameter.py
--rw-r--r--   0        0        0        0 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/utils/__init__.py
--rw-r--r--   0        0        0      922 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py
--rw-r--r--   0        0        0      915 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py
--rwxr-xr-x   0        0        0      278 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/main.py
--rwxr-xr-x   0        0        0      459 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/construct_docker_runner_image_name.sh
--rwxr-xr-x   0        0        0     1061 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh
--rwxr-xr-x   0        0        0     5629 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh
--rwxr-xr-x   0        0        0     2903 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh
--rwxr-xr-x   0        0        0     1502 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh
--rwxr-xr-x   0        0        0     4495 2023-03-20 13:54:59.724430 exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh
--rw-r--r--   0        0        0     1054 2023-03-20 13:54:59.728430 exasol-script-languages-container-tool-0.16.0/pyproject.toml
--rw-r--r--   0        0        0     9458 1970-01-01 00:00:00.000000 exasol-script-languages-container-tool-0.16.0/setup.py
--rw-r--r--   0        0        0     8211 1970-01-01 00:00:00.000000 exasol-script-languages-container-tool-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/LICENSE
+-rw-r--r--   0        0        0     7271 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3825 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build.py
+-rw-r--r--   0        0        0     2998 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py
+-rw-r--r--   0        0        0     2357 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/clean.py
+-rw-r--r--   0        0        0     3781 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/export.py
+-rw-r--r--   0        0        0     1066 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py
+-rw-r--r--   0        0        0     1070 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py
+-rw-r--r--   0        0        0     3057 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push.py
+-rw-r--r--   0        0        0     3017 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py
+-rw-r--r--   0        0        0    11821 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py
+-rw-r--r--   0        0        0     3551 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/save.py
+-rw-r--r--   0        0        0     3657 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/security_scan.py
+-rw-r--r--   0        0        0     4519 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/upload.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/__init__.py
+-rw-r--r--   0        0        0      820 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/flavor_options.py
+-rw-r--r--   0        0        0      617 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/goal_options.py
+-rw-r--r--   0        0        0      346 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/test_container_options.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/api_errors.py
+-rw-r--r--   0        0        0     3049 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build.py
+-rw-r--r--   0        0        0     2725 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build_test_container.py
+-rw-r--r--   0        0        0     2588 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/clean.py
+-rw-r--r--   0        0        0     3214 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/export.py
+-rw-r--r--   0        0        0     1681 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py
+-rw-r--r--   0        0        0      733 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py
+-rw-r--r--   0        0        0     3186 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/push.py
+-rw-r--r--   0        0        0     2738 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/push_test_container.py
+-rw-r--r--   0        0        0     9072 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py
+-rw-r--r--   0        0        0     3240 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/save.py
+-rw-r--r--   0        0        0     3264 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/security_scan.py
+-rw-r--r--   0        0        0     4081 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/upload.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py
+-rw-r--r--   0        0        0     1311 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py
+-rw-r--r--   0        0        0     4219 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/clean/__init__.py
+-rw-r--r--   0        0        0     4470 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/__init__.py
+-rw-r--r--   0        0        0      525 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py
+-rw-r--r--   0        0        0     9855 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py
+-rw-r--r--   0        0        0     1366 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py
+-rw-r--r--   0        0        0     1736 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py
+-rw-r--r--   0        0        0     3701 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py
+-rw-r--r--   0        0        0      756 2023-05-12 15:00:49.660850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py
+-rw-r--r--   0        0        0     2958 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/push/__init__.py
+-rw-r--r--   0        0        0     1702 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/__init__.py
+-rw-r--r--   0        0        0     1600 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py
+-rw-r--r--   0        0        0      231 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save_parameter.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/__init__.py
+-rw-r--r--   0        0        0     5728 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py
+-rw-r--r--   0        0        0      223 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan_parameter.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py
+-rw-r--r--   0        0        0     1973 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py
+-rw-r--r--   0        0        0     6871 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py
+-rw-r--r--   0        0        0     2246 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py
+-rw-r--r--   0        0        0     1961 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py
+-rw-r--r--   0        0        0     2840 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py
+-rw-r--r--   0        0        0     2235 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py
+-rw-r--r--   0        0        0     3179 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py
+-rw-r--r--   0        0        0     1450 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py
+-rw-r--r--   0        0        0     8499 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py
+-rw-r--r--   0        0        0     1420 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py
+-rw-r--r--   0        0        0     9449 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py
+-rw-r--r--   0        0        0     1010 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/__init__.py
+-rw-r--r--   0        0        0     2663 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py
+-rw-r--r--   0        0        0     4863 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py
+-rw-r--r--   0        0        0      630 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py
+-rw-r--r--   0        0        0     1312 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py
+-rw-r--r--   0        0        0     1545 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py
+-rw-r--r--   0        0        0     2995 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py
+-rw-r--r--   0        0        0      248 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers_parameter.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py
+-rw-r--r--   0        0        0      915 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py
+-rwxr-xr-x   0        0        0      278 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/main.py
+-rwxr-xr-x   0        0        0      459 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/construct_docker_runner_image_name.sh
+-rwxr-xr-x   0        0        0     1061 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh
+-rwxr-xr-x   0        0        0     5629 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh
+-rwxr-xr-x   0        0        0     2903 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh
+-rwxr-xr-x   0        0        0     1502 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh
+-rwxr-xr-x   0        0        0     4495 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh
+-rw-r--r--   0        0        0     1055 2023-05-12 15:00:49.664850 exasol_script_languages_container_tool-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     8262 1970-01-01 00:00:00.000000 exasol_script_languages_container_tool-0.17.0/PKG-INFO
```

### Comparing `exasol-script-languages-container-tool-0.16.0/LICENSE` & `exasol_script_languages_container_tool-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/README.md` & `exasol_script_languages_container_tool-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/build.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/clean.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/export.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/push.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/push.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from exasol_script_languages_container_tool.cli.options.goal_options import release_options
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.build_options import build_options
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import docker_repository_options
 from exasol_integration_test_docker_environment.cli.options.system_options import system_options
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import test_environment_options, \
     docker_db_options, external_db_options
+
+from exasol_script_languages_container_tool.cli.options.test_container_options import test_container_options
 from exasol_script_languages_container_tool.lib import api
 from exasol_script_languages_container_tool.lib.api import api_errors
 
 
 @cli.command(short_help="Runs integration tests.")
 @add_options(flavor_options)
 @add_options(release_options)
@@ -66,17 +68,15 @@
 @click.option('--reuse-uploaded-container/--no-reuse-uploaded-container', default=False,
               help="Reuse the uploaded script-langauge-container in a reused database.")
 @click.option('--reuse-test-container/--no-reuse-test-container', default=False,
               help="Reuse the test container which is used for test execution.")
 @click.option('--reuse-test-environment/--no-reuse-test-environment', default=False,
               help="Reuse the whole test environment with docker network, test container, "
                    "database, database setup and uploaded container")
-@click.option('--test-container-folder', type=click.Path(exists=True, file_okay=False, dir_okay=True),
-              default="./test_container",
-              help="Test folder containing 'Dockerfile', tests and test-data.")
+@add_options(test_container_options)
 @add_options(build_options)
 @add_options(docker_repository_options)
 @add_options(system_options)
 def run_db_test(flavor_path: Tuple[str, ...],
                 release_goal: Tuple[str, ...],
                 generic_language_test: Tuple[str, ...],
                 test_folder: Tuple[str, ...],
```

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/save.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/save.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/security_scan.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/commands/upload.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/options/flavor_options.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/flavor_options.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/cli/options/goal_options.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/cli/options/goal_options.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/build.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/build.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/clean.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/clean.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/export.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/export.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/push.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/push.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/save.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/save.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/security_scan.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/api/upload.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/api/upload.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh` & `exasol_script_languages_container_tool-0.17.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-tool-0.16.0/pyproject.toml` & `exasol_script_languages_container_tool-0.17.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-script-languages-container-tool"
-version = "0.16.0"
+version = "0.17.0"
 description = "Script Languages Container Tool"
 
 license = "MIT"
 
 authors = [
     "Torsten Kilias <torsten.kilias@exasol.com>"
 ]
@@ -17,19 +17,19 @@
 keywords = ['exasol', 'udf', 'script-languages']
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 importlib_metadata = ">=4.6.0"
 importlib-resources = ">=5.4.0"
 networkx = "2.8.2" # We pinned networkx to this version, because in newer versions it throws an exception, see https://github.com/exasol/integration-test-docker-environment/issues/228
-exasol-integration-test-docker-environment = "^1.4.0"
+exasol-integration-test-docker-environment = "^1.6.0"
 typeguard = "<3.0.0"
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 toml = ">=0.10.2"
 
 
 [tool.poetry.scripts]
-exaslct = 'exasol_script_languages_container_tool.main:main'
+exaslct = 'exasol_script_languages_container_tool.main:main'
```

### Comparing `exasol-script-languages-container-tool-0.16.0/setup.py` & `exasol_script_languages_container_tool-0.17.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,188 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: exasol-script-languages-container-tool
+Version: 0.17.0
+Summary: Script Languages Container Tool
+Home-page: https://github.com/exasol/script-languages-container-tool
+License: MIT
+Keywords: exasol,udf,script-languages
+Author: Torsten Kilias
+Author-email: torsten.kilias@exasol.com
+Requires-Python: >=3.8,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: exasol-integration-test-docker-environment (>=1.6.0,<2.0.0)
+Requires-Dist: importlib-resources (>=5.4.0)
+Requires-Dist: importlib_metadata (>=4.6.0)
+Requires-Dist: networkx (==2.8.2)
+Requires-Dist: typeguard (<3.0.0)
+Project-URL: Repository, https://github.com/exasol/script-languages-container-tool
+Description-Content-Type: text/markdown
 
-packages = \
-['exasol_script_languages_container_tool',
- 'exasol_script_languages_container_tool.cli',
- 'exasol_script_languages_container_tool.cli.commands',
- 'exasol_script_languages_container_tool.cli.options',
- 'exasol_script_languages_container_tool.lib',
- 'exasol_script_languages_container_tool.lib.api',
- 'exasol_script_languages_container_tool.lib.tasks',
- 'exasol_script_languages_container_tool.lib.tasks.build',
- 'exasol_script_languages_container_tool.lib.tasks.clean',
- 'exasol_script_languages_container_tool.lib.tasks.export',
- 'exasol_script_languages_container_tool.lib.tasks.install_starter_scripts',
- 'exasol_script_languages_container_tool.lib.tasks.push',
- 'exasol_script_languages_container_tool.lib.tasks.save',
- 'exasol_script_languages_container_tool.lib.tasks.security_scan',
- 'exasol_script_languages_container_tool.lib.tasks.test',
- 'exasol_script_languages_container_tool.lib.tasks.upload',
- 'exasol_script_languages_container_tool.lib.utils']
-
-package_data = \
-{'': ['*'], 'exasol_script_languages_container_tool': ['starter_scripts/*']}
-
-install_requires = \
-['exasol-integration-test-docker-environment>=1.4.0,<2.0.0',
- 'importlib-resources>=5.4.0',
- 'importlib_metadata>=4.6.0',
- 'networkx==2.8.2',
- 'typeguard<3.0.0']
-
-entry_points = \
-{'console_scripts': ['exaslct = '
-                     'exasol_script_languages_container_tool.main:main']}
-
-setup_kwargs = {
-    'name': 'exasol-script-languages-container-tool',
-    'version': '0.16.0',
-    'description': 'Script Languages Container Tool',
-    'long_description': "# Script-Languages-Container-Tool\n\n## Overview\n\nThe Script-Languages-Container-Tool (exaslct) is the build tool for the script language container.\nYou can build, export and upload script-language container from so-called flavors \nwhich are description how to build the script language container. You can find pre-defined flavors \nin the [script-languages-release](https://github.com/exasol/script-languages-release) repository. \nThere we also described how you could customize these flavors to your needs.\n\n## In a Nutshell\n\n### Prerequisites\n\n#### For installation\n\nIn order to install this tool, your system needs to provide \nthe following prerequisites:\n\n* Software\n    * Linux\n      * [bash](https://www.gnu.org/software/bash/) >= 4.2\n    * MacOsX\n      * [bash](https://www.gnu.org/software/bash/) > 3.2\n    * [coreutils](https://www.gnu.org/software/coreutils/)\n      * sha512sum\n      * sed\n    * [curl](https://curl.se/)\n    * Python 3 (>=3.8)\n      * Pip\n\n\n#### For running\n\nIn order to use this tool, your system needs to fulfill the following prerequisites:\n\n* Software\n    * Linux\n      * [bash](https://www.gnu.org/software/bash/) >= 4.2\n      * [coreutils](https://www.gnu.org/software/coreutils/)\n        * readlink with -f option\n        * realpath  \n        * dirname\n    * MacOsX (Please see limitations on [MacOsX](#macosx-limitations))\n      * [bash](https://www.gnu.org/software/bash/) >= 3.2\n      * [coreutils](https://www.gnu.org/software/coreutils/)\n        * greadlink with -f option\n        * realpath  \n        * dirname\n    * [Docker](https://docs.docker.com/) >= 17.05 \n      * with support for [multi-stage builds required](https://docs.docker.com/develop/develop-images/multistage-build/)\n      * host volume mounts need to be allowed\n\n* System Setup  \n    * We recommend at least 50 GB free disk space on the partition \n      where Docker stores its images, on linux Docker typically stores \n      the images at /var/lib/docker.\n    * For the partition where the output directory (default: ./.build_output)\n      is located we recommend additionally at least 10 GB free disk space.\n\nFurther, prerequisites might be necessary for specific tasks. These are listed under the corresponding section.\n\n### Installation\n\nYou have two options to use this project:\n - as a pure Python project\n - using the _start scripts_ which pull the correct container image from Dockerhub and execute it within the Docker container\n\n#### Pure Python\n\nFind the wheel package for a specific [release](https://github.com/exasol/script-languages-container-tool/releases) under assets.\n\nInstall the python package with `python3 -m pip install https://github.com/exasol/script-languages-container-tool/releases/download/$VERSION/exasol_script_languages_container_tool-$VERSION-py3-none-any.whl`. Replace $VERSION with the latest version or the specific version you are interested in.\n\n#### Starter scripts\n\nYou need to install the Python package only once to install the starter scripts (see the [previous section](#installation)).\n\nInstall the starter scripts which allow to run exaslct within a docker image:\n`python3 -m exasol_script_languages_container_tool.main install-starter-scripts --install-path $YOUR_INSTALL_PATH`\n\nThis will create a subfolder with the scripts itself and a symlink `exaslct` in $YOUR_INSTALL_PATH, which can be used as entry point.\n\n### Usage\n\nFor simplicity the following examples use the starter script version (`exaslct`). If you want to use the pure Python package, simply replace `exaslct` with `python3 -m exasol_script_languages_container_tool.main` in all examples. \n\n#### How to build an existing flavor?\n\nCreate the language container and export it to the local file system\n\n```bash\n./exaslct export --flavor-path=flavors/<flavor-name> --export-path <export-path>\n```\n\nor upload it directly into the BucketFS (currently http only, https follows soon)\n\n```bash\n./exaslct upload --flavor-path=flavors/<flavor-name> --database-host <hostname-or-ip> --bucketfs-port <port> \\ \n                   --bucketfs-username w --bucketfs-password <password>  --bucketfs-name <bucketfs-name> \\\n                   --bucket-name <bucket-name> --path-in-bucket <path/in/bucket>\n```\n\nOnce it is successfully uploaded, it will print the ALTER SESSION statement\nthat can be used to activate the script language container in the database.\n\n#### How to activate a script language container in the database\n\nIf you uploaded a container manually, you can generate the language activation statement with\n\n```bash\n./exaslct generate-language-activation --flavor-path=flavors/<flavor-name> --bucketfs-name <bucketfs-name> \\\n                                         --bucket-name <bucket-name> --path-in-bucket <path/in/bucket> --container-name <container-name>\n```\n\nwhere \\<container-name> is the name of the uploaded archive without its file extension. To activate the language, execute the generated statement in your database session to activate the container for the current session or system wide.\n\nThis command will print a SQL statement to activate the language similar to the following one:\n\n```bash\nALTER SESSION SET SCRIPT_LANGUAGES='<LANGUAGE_ALIAS>=localzmq+protobuf:///<bucketfs-name>/<bucket-name>/<path-in-bucket>/<container-name>?lang=<language>#buckets/<bucketfs-name>/<bucket-name>/<path-in-bucket>/<container-name>/exaudf/exaudfclient[_py3]';\n```\n\n**Please, refer to the [User Guide](doc/user_guide/user_guide.md) for more detailed information, how to use exalsct.**\n\n## Features\n\n* Build a script language container as docker images\n* Export a script language container as an archive which can be used for extending Exasol UDFs\n* Upload a script language container as an archive to the Exasol DB's BucketFS\n* Generating the activation command for a script language container\n* Can use Docker registries, such as Docker Hub, as a cache to avoid rebuilding image without changes\n* Can push Docker images to Docker registries\n* Run tests for you container against an Exasol DB (docker-db or external db)\n\n## Limitations\n\n* Caution with symbolic links: \n  If you use symbolic links inside any directory of the command line arguments\n  they must not point to files or directories outside the root of the path of the \n  command line argument (i.e. --flavor-path ./flavors/my_flavor/ => There must be no symbolic\n  link inside ./flavors/my_flavor point to anywhere outside of ./flavors/my_flavor).\n  Background: Local directories paths must be mounted manually to the docker container. \n  We currently support only the mounting of the given command line arguments, but we do not analyze\n  the content of those directories.\n  Plan is to fix this limitation with [#35](https://github.com/exasol/script-languages-container-tool/issues/35)\n\n\n### MacOsX Limitations\n  \n* On MacOsX all arguments (flavors path, output directory, etc.) must point to locations within the current directory (background is that the MacOsX version does not support mount binding additional directories).\n\n## Table of Contents\n\n### Information for Users\n\n* [User Guide](doc/user_guide/user_guide.md)\n* [Changelog](doc/changes/changelog.md)\n\n## Information for Developers\n\n* [Developer Guide](doc/developer_guide/developer_guide.md)\n* [Dependencies](doc/dependencies.md)\n",
-    'author': 'Torsten Kilias',
-    'author_email': 'torsten.kilias@exasol.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/exasol/script-languages-container-tool',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4',
-}
+# Script-Languages-Container-Tool
 
+## Overview
+
+The Script-Languages-Container-Tool (exaslct) is the build tool for the script language container.
+You can build, export and upload script-language container from so-called flavors 
+which are description how to build the script language container. You can find pre-defined flavors 
+in the [script-languages-release](https://github.com/exasol/script-languages-release) repository. 
+There we also described how you could customize these flavors to your needs.
+
+## In a Nutshell
+
+### Prerequisites
+
+#### For installation
+
+In order to install this tool, your system needs to provide 
+the following prerequisites:
+
+* Software
+    * Linux
+      * [bash](https://www.gnu.org/software/bash/) >= 4.2
+    * MacOsX
+      * [bash](https://www.gnu.org/software/bash/) > 3.2
+    * [coreutils](https://www.gnu.org/software/coreutils/)
+      * sha512sum
+      * sed
+    * [curl](https://curl.se/)
+    * Python 3 (>=3.8)
+      * Pip
+
+
+#### For running
+
+In order to use this tool, your system needs to fulfill the following prerequisites:
+
+* Software
+    * Linux
+      * [bash](https://www.gnu.org/software/bash/) >= 4.2
+      * [coreutils](https://www.gnu.org/software/coreutils/)
+        * readlink with -f option
+        * realpath  
+        * dirname
+    * MacOsX (Please see limitations on [MacOsX](#macosx-limitations))
+      * [bash](https://www.gnu.org/software/bash/) >= 3.2
+      * [coreutils](https://www.gnu.org/software/coreutils/)
+        * greadlink with -f option
+        * realpath  
+        * dirname
+    * [Docker](https://docs.docker.com/) >= 17.05 
+      * with support for [multi-stage builds required](https://docs.docker.com/develop/develop-images/multistage-build/)
+      * host volume mounts need to be allowed
+
+* System Setup  
+    * We recommend at least 50 GB free disk space on the partition 
+      where Docker stores its images, on linux Docker typically stores 
+      the images at /var/lib/docker.
+    * For the partition where the output directory (default: ./.build_output)
+      is located we recommend additionally at least 10 GB free disk space.
+
+Further, prerequisites might be necessary for specific tasks. These are listed under the corresponding section.
+
+### Installation
+
+You have two options to use this project:
+ - as a pure Python project
+ - using the _start scripts_ which pull the correct container image from Dockerhub and execute it within the Docker container
+
+#### Pure Python
+
+Find the wheel package for a specific [release](https://github.com/exasol/script-languages-container-tool/releases) under assets.
+
+Install the python package with `python3 -m pip install https://github.com/exasol/script-languages-container-tool/releases/download/$VERSION/exasol_script_languages_container_tool-$VERSION-py3-none-any.whl`. Replace $VERSION with the latest version or the specific version you are interested in.
+
+#### Starter scripts
+
+You need to install the Python package only once to install the starter scripts (see the [previous section](#installation)).
+
+Install the starter scripts which allow to run exaslct within a docker image:
+`python3 -m exasol_script_languages_container_tool.main install-starter-scripts --install-path $YOUR_INSTALL_PATH`
+
+This will create a subfolder with the scripts itself and a symlink `exaslct` in $YOUR_INSTALL_PATH, which can be used as entry point.
+
+### Usage
+
+For simplicity the following examples use the starter script version (`exaslct`). If you want to use the pure Python package, simply replace `exaslct` with `python3 -m exasol_script_languages_container_tool.main` in all examples. 
+
+#### How to build an existing flavor?
+
+Create the language container and export it to the local file system
+
+```bash
+./exaslct export --flavor-path=flavors/<flavor-name> --export-path <export-path>
+```
+
+or upload it directly into the BucketFS (currently http only, https follows soon)
+
+```bash
+./exaslct upload --flavor-path=flavors/<flavor-name> --database-host <hostname-or-ip> --bucketfs-port <port> \ 
+                   --bucketfs-username w --bucketfs-password <password>  --bucketfs-name <bucketfs-name> \
+                   --bucket-name <bucket-name> --path-in-bucket <path/in/bucket>
+```
+
+Once it is successfully uploaded, it will print the ALTER SESSION statement
+that can be used to activate the script language container in the database.
+
+#### How to activate a script language container in the database
+
+If you uploaded a container manually, you can generate the language activation statement with
+
+```bash
+./exaslct generate-language-activation --flavor-path=flavors/<flavor-name> --bucketfs-name <bucketfs-name> \
+                                         --bucket-name <bucket-name> --path-in-bucket <path/in/bucket> --container-name <container-name>
+```
+
+where \<container-name> is the name of the uploaded archive without its file extension. To activate the language, execute the generated statement in your database session to activate the container for the current session or system wide.
+
+This command will print a SQL statement to activate the language similar to the following one:
+
+```bash
+ALTER SESSION SET SCRIPT_LANGUAGES='<LANGUAGE_ALIAS>=localzmq+protobuf:///<bucketfs-name>/<bucket-name>/<path-in-bucket>/<container-name>?lang=<language>#buckets/<bucketfs-name>/<bucket-name>/<path-in-bucket>/<container-name>/exaudf/exaudfclient[_py3]';
+```
+
+**Please, refer to the [User Guide](doc/user_guide/user_guide.md) for more detailed information, how to use exalsct.**
+
+## Features
+
+* Build a script language container as docker images
+* Export a script language container as an archive which can be used for extending Exasol UDFs
+* Upload a script language container as an archive to the Exasol DB's BucketFS
+* Generating the activation command for a script language container
+* Can use Docker registries, such as Docker Hub, as a cache to avoid rebuilding image without changes
+* Can push Docker images to Docker registries
+* Run tests for you container against an Exasol DB (docker-db or external db)
+
+## Limitations
+
+* Caution with symbolic links: 
+  If you use symbolic links inside any directory of the command line arguments
+  they must not point to files or directories outside the root of the path of the 
+  command line argument (i.e. --flavor-path ./flavors/my_flavor/ => There must be no symbolic
+  link inside ./flavors/my_flavor point to anywhere outside of ./flavors/my_flavor).
+  Background: Local directories paths must be mounted manually to the docker container. 
+  We currently support only the mounting of the given command line arguments, but we do not analyze
+  the content of those directories.
+  Plan is to fix this limitation with [#35](https://github.com/exasol/script-languages-container-tool/issues/35)
+
+
+### MacOsX Limitations
+  
+* On MacOsX all arguments (flavors path, output directory, etc.) must point to locations within the current directory (background is that the MacOsX version does not support mount binding additional directories).
+
+## Table of Contents
+
+### Information for Users
+
+* [User Guide](doc/user_guide/user_guide.md)
+* [Changelog](doc/changes/changelog.md)
+
+## Information for Developers
+
+* [Developer Guide](doc/developer_guide/developer_guide.md)
+* [Dependencies](doc/dependencies.md)
 
-setup(**setup_kwargs)
```


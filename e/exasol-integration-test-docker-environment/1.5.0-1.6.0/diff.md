# Comparing `tmp/exasol-integration-test-docker-environment-1.5.0.tar.gz` & `tmp/exasol_integration_test_docker_environment-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol-integration-test-docker-environment-1.5.0.tar", max compression
+gzip compressed data, was "exasol_integration_test_docker_environment-1.6.0.tar", max compression
```

## Comparing `exasol-integration-test-docker-environment-1.5.0.tar` & `exasol_integration_test_docker_environment-1.6.0.tar`

### file list

```diff
@@ -1,234 +1,234 @@
--rw-r--r--   0        0        0     1063 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/LICENSE
--rw-r--r--   0        0        0      737 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/README.rst
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/__init__.py
--rw-r--r--   0        0        0       51 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/abstract_method_exception.py
--rw-r--r--   0        0        0      370 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/certificate_resources/container/Dockerfile
--rw-r--r--   0        0        0     1254 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh
--rwxr-xr-x   0        0        0      570 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/__init__.py
--rw-r--r--   0        0        0      523 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/cli.py
--rw-r--r--   0        0        0       86 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/commands/__init__.py
--rw-r--r--   0        0        0      744 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/commands/health.py
--rw-r--r--   0        0        0     4992 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/__init__.py
--rw-r--r--   0        0        0     1655 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/build_options.py
--rw-r--r--   0        0        0     3106 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py
--rw-r--r--   0        0        0      376 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/push_options.py
--rw-r--r--   0        0        0     1214 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/system_options.py
--rw-r--r--   0        0        0     3086 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py
--rw-r--r--   0        0        0     1970 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/termination_handler.py
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.827012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/init_db.sh
--rw-r--r--   0        0        0     6440 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/init_db.sh
--rw-r--r--   0        0        0     7182 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf
--rwxr-xr-x   0        0        0      318 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/init_db.sh
--rw-r--r--   0        0        0     2576 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/doctor.py
--rw-r--r--   0        0        0      165 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/__init__.py
--rw-r--r--   0        0        0      544 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/__init__.py
--rw-r--r--   0        0        0      500 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/api_errors.py
--rw-r--r--   0        0        0     3234 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py
--rw-r--r--   0        0        0     8293 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/common.py
--rw-r--r--   0        0        0     1328 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/health.py
--rw-r--r--   0        0        0     3342 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py
--rw-r--r--   0        0        0     6341 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py
--rw-r--r--   0        0        0     6845 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/__init__.py
--rw-r--r--   0        0        0      110 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/abstract_task_future.py
--rw-r--r--   0        0        0    16982 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/base_task.py
--rw-r--r--   0        0        0     4654 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py
--rw-r--r--   0        0        0      459 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/docker_base_task.py
--rw-r--r--   0        0        0      340 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/docker_parameter.py
--rw-r--r--   0        0        0     1516 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py
--rw-r--r--   0        0        0      325 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/frozendict_to_dict.py
--rw-r--r--   0        0        0     1007 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/info.py
--rw-r--r--   0        0        0     1165 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py
--rw-r--r--   0        0        0      737 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py
--rw-r--r--   0        0        0     2711 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py
--rw-r--r--   0        0        0      495 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/pickle_target.py
--rw-r--r--   0        0        0     1261 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py
--rw-r--r--   0        0        0     3472 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py
--rw-r--r--   0        0        0     1775 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py
--rw-r--r--   0        0        0     1021 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py
--rw-r--r--   0        0        0      173 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/task_state.py
--rw-r--r--   0        0        0     4619 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py
--rw-r--r--   0        0        0      282 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/wrong_task_state_exception.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/config/__init__.py
--rw-r--r--   0        0        0      675 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/config/build_config.py
--rw-r--r--   0        0        0     1297 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/config/docker_config.py
--rw-r--r--   0        0        0      440 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/config/log_config.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/__init__.py
--rw-r--r--   0        0        0      656 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/container_info.py
--rw-r--r--   0        0        0      810 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py
--rw-r--r--   0        0        0      507 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/database_info.py
--rw-r--r--   0        0        0      330 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/docker_network_info.py
--rw-r--r--   0        0        0      508 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/docker_volume_info.py
--rw-r--r--   0        0        0      840 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/environment_info.py
--rw-r--r--   0        0        0       91 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/environment_type.py
--rw-r--r--   0        0        0     1773 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py
--rw-r--r--   0        0        0     1010 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/container/__init__.py
--rw-r--r--   0        0        0      492 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/container/utils.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/__init__.py
--rw-r--r--   0        0        0     2778 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/__init__.py
--rw-r--r--   0        0        0     6144 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py
--rw-r--r--   0        0        0    11405 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py
--rw-r--r--   0        0        0     2977 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py
--rw-r--r--   0        0        0     5074 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py
--rw-r--r--   0        0        0      724 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py
--rw-r--r--   0        0        0     1024 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py
--rw-r--r--   0        0        0     2916 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/__init__.py
--rw-r--r--   0        0        0     3306 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py
--rw-r--r--   0        0        0     3697 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py
--rw-r--r--   0        0        0     2323 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py
--rw-r--r--   0        0        0     1734 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py
--rw-r--r--   0        0        0      659 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py
--rw-r--r--   0        0        0     1846 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py
--rw-r--r--   0        0        0    11297 2023-03-21 15:35:19.831012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py
--rw-r--r--   0        0        0     2224 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py
--rw-r--r--   0        0        0      861 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py
--rw-r--r--   0        0        0     4017 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/__init__.py
--rw-r--r--   0        0        0     2683 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py
--rw-r--r--   0        0        0     1334 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py
--rw-r--r--   0        0        0      160 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_push_parameter.py
--rw-r--r--   0        0        0     2107 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py
--rw-r--r--   0        0        0      800 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py
--rw-r--r--   0        0        0      426 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/required_task_info.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/__init__.py
--rw-r--r--   0        0        0     3106 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py
--rw-r--r--   0        0        0     1335 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py
--rw-r--r--   0        0        0      815 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py
--rw-r--r--   0        0        0     1998 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py
--rw-r--r--   0        0        0      371 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/utils.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/networks/__init__.py
--rw-r--r--   0        0        0      478 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/networks/utils.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/volumes/__init__.py
--rw-r--r--   0        0        0      473 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/volumes/utils.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/__init__.py
--rw-r--r--   0        0        0     1111 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py
--rw-r--r--   0        0        0     1587 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py
--rw-r--r--   0        0        0      911 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/__init__.py
--rw-r--r--   0        0        0    13026 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py
--rw-r--r--   0        0        0     3652 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/__init__.py
--rw-r--r--   0        0        0     3485 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py
--rw-r--r--   0        0        0     6359 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/__init__.py
--rw-r--r--   0        0        0      283 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/bucketfs_sync_checker.py
--rw-r--r--   0        0        0     2274 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py
--rw-r--r--   0        0        0      938 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py
--rw-r--r--   0        0        0     2560 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py
--rw-r--r--   0        0        0      443 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/time_based_bucketfs_sync_waiter.py
--rw-r--r--   0        0        0     7785 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/__init__.py
--rw-r--r--   0        0        0     2186 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py
--rw-r--r--   0        0        0     3021 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py
--rw-r--r--   0        0        0     1128 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py
--rw-r--r--   0        0        0     6010 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py
--rw-r--r--   0        0        0     1627 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py
--rw-r--r--   0        0        0     1787 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/__init__.py
--rw-r--r--   0        0        0      794 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py
--rw-r--r--   0        0        0     1364 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py
--rw-r--r--   0        0        0     1003 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py
--rw-r--r--   0        0        0      894 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py
--rw-r--r--   0        0        0     4769 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py
--rw-r--r--   0        0        0     5045 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py
--rw-r--r--   0        0        0    10631 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py
--rw-r--r--   0        0        0    15657 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py
--rw-r--r--   0        0        0     2628 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py
--rw-r--r--   0        0        0     4888 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py
--rw-r--r--   0        0        0     2905 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/utils/__init__.py
--rw-r--r--   0        0        0     3362 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py
--rwxr-xr-x   0        0        0      347 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/main.py
--rw-r--r--   0        0        0      681 2023-03-21 15:35:19.835012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/templates/luigi_log.conf
--rw-r--r--   0        0        0        0 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/__init__.py
--rw-r--r--   0        0        0     2445 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py
--rw-r--r--   0        0        0     4600 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/api_test_environment.py
--rw-r--r--   0        0        0     2691 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/docker_registry.py
--rw-r--r--   0        0        0     1407 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py
--rw-r--r--   0        0        0     8830 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py
--rw-r--r--   0        0        0      559 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/luigi_utils.py
--rw-r--r--   0        0        0      824 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py
--rw-r--r--   0        0        0     1988 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/utils.py
--rw-r--r--   0        0        0      331 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/ext/01_nodoc
--rw-r--r--   0        0        0     1815 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     6147 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/pytest_itde/__init__.py
--rw-r--r--   0        0        0     3335 2023-03-21 15:35:19.839012 exasol-integration-test-docker-environment-1.5.0/pytest_itde/config.py
--rw-r--r--   0        0        0     7006 1970-01-01 00:00:00.000000 exasol-integration-test-docker-environment-1.5.0/setup.py
--rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 exasol-integration-test-docker-environment-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/LICENSE
+-rw-r--r--   0        0        0      737 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/README.rst
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/abstract_method_exception.py
+-rw-r--r--   0        0        0      370 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/container/Dockerfile
+-rw-r--r--   0        0        0     1254 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh
+-rwxr-xr-x   0        0        0      570 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/cli.py
+-rw-r--r--   0        0        0       86 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/__init__.py
+-rw-r--r--   0        0        0      744 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/health.py
+-rw-r--r--   0        0        0     5323 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/__init__.py
+-rw-r--r--   0        0        0     1655 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/build_options.py
+-rw-r--r--   0        0        0     3106 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py
+-rw-r--r--   0        0        0      376 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/push_options.py
+-rw-r--r--   0        0        0     1660 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/system_options.py
+-rw-r--r--   0        0        0     3086 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py
+-rw-r--r--   0        0        0     1970 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/termination_handler.py
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/init_db.sh
+-rw-r--r--   0        0        0     2576 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/doctor.py
+-rw-r--r--   0        0        0      165 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/api_errors.py
+-rw-r--r--   0        0        0     3459 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py
+-rw-r--r--   0        0        0    11718 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/common.py
+-rw-r--r--   0        0        0     1328 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/health.py
+-rw-r--r--   0        0        0     3567 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py
+-rw-r--r--   0        0        0     6576 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py
+-rw-r--r--   0        0        0     7081 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/__init__.py
+-rw-r--r--   0        0        0      110 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/abstract_task_future.py
+-rw-r--r--   0        0        0    16982 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/base_task.py
+-rw-r--r--   0        0        0     4654 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py
+-rw-r--r--   0        0        0      459 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/docker_base_task.py
+-rw-r--r--   0        0        0      340 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/docker_parameter.py
+-rw-r--r--   0        0        0     1516 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py
+-rw-r--r--   0        0        0      325 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/frozendict_to_dict.py
+-rw-r--r--   0        0        0     1007 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/info.py
+-rw-r--r--   0        0        0     1165 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py
+-rw-r--r--   0        0        0      737 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py
+-rw-r--r--   0        0        0     3405 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py
+-rw-r--r--   0        0        0      495 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/pickle_target.py
+-rw-r--r--   0        0        0     1261 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py
+-rw-r--r--   0        0        0     3472 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py
+-rw-r--r--   0        0        0     1775 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py
+-rw-r--r--   0        0        0     1055 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py
+-rw-r--r--   0        0        0      173 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_state.py
+-rw-r--r--   0        0        0     4619 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py
+-rw-r--r--   0        0        0      282 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/wrong_task_state_exception.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/__init__.py
+-rw-r--r--   0        0        0      675 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/build_config.py
+-rw-r--r--   0        0        0     1297 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/docker_config.py
+-rw-r--r--   0        0        0      440 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/log_config.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/__init__.py
+-rw-r--r--   0        0        0      656 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/container_info.py
+-rw-r--r--   0        0        0      810 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py
+-rw-r--r--   0        0        0      507 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/database_info.py
+-rw-r--r--   0        0        0      330 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/docker_network_info.py
+-rw-r--r--   0        0        0      508 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/docker_volume_info.py
+-rw-r--r--   0        0        0      840 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/environment_info.py
+-rw-r--r--   0        0        0       91 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/environment_type.py
+-rw-r--r--   0        0        0     1773 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py
+-rw-r--r--   0        0        0     1010 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/container/__init__.py
+-rw-r--r--   0        0        0      492 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/container/utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/__init__.py
+-rw-r--r--   0        0        0     2778 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/__init__.py
+-rw-r--r--   0        0        0     6144 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py
+-rw-r--r--   0        0        0    11405 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py
+-rw-r--r--   0        0        0     2977 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py
+-rw-r--r--   0        0        0     5074 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py
+-rw-r--r--   0        0        0      724 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py
+-rw-r--r--   0        0        0     1024 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py
+-rw-r--r--   0        0        0     2916 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/__init__.py
+-rw-r--r--   0        0        0     3306 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py
+-rw-r--r--   0        0        0     3697 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py
+-rw-r--r--   0        0        0     2323 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py
+-rw-r--r--   0        0        0     1734 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py
+-rw-r--r--   0        0        0      659 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py
+-rw-r--r--   0        0        0     1846 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py
+-rw-r--r--   0        0        0    11297 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py
+-rw-r--r--   0        0        0     2224 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py
+-rw-r--r--   0        0        0      861 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py
+-rw-r--r--   0        0        0     4017 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/__init__.py
+-rw-r--r--   0        0        0     2683 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py
+-rw-r--r--   0        0        0     1334 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py
+-rw-r--r--   0        0        0      160 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_push_parameter.py
+-rw-r--r--   0        0        0     2107 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py
+-rw-r--r--   0        0        0      800 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py
+-rw-r--r--   0        0        0      426 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/required_task_info.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/__init__.py
+-rw-r--r--   0        0        0     3106 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py
+-rw-r--r--   0        0        0     1335 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py
+-rw-r--r--   0        0        0      815 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py
+-rw-r--r--   0        0        0     1998 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py
+-rw-r--r--   0        0        0      371 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/networks/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/networks/utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/volumes/__init__.py
+-rw-r--r--   0        0        0      473 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/volumes/utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py
+-rw-r--r--   0        0        0     1587 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py
+-rw-r--r--   0        0        0      911 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/__init__.py
+-rw-r--r--   0        0        0    13026 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py
+-rw-r--r--   0        0        0     3571 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/__init__.py
+-rw-r--r--   0        0        0     3485 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py
+-rw-r--r--   0        0        0     6359 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/__init__.py
+-rw-r--r--   0        0        0      283 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/bucketfs_sync_checker.py
+-rw-r--r--   0        0        0     2274 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py
+-rw-r--r--   0        0        0      938 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py
+-rw-r--r--   0        0        0     2560 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py
+-rw-r--r--   0        0        0      443 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/time_based_bucketfs_sync_waiter.py
+-rw-r--r--   0        0        0     8069 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/__init__.py
+-rw-r--r--   0        0        0     2186 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py
+-rw-r--r--   0        0        0     3021 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py
+-rw-r--r--   0        0        0     1128 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py
+-rw-r--r--   0        0        0     6010 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py
+-rw-r--r--   0        0        0     1627 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py
+-rw-r--r--   0        0        0     1787 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/__init__.py
+-rw-r--r--   0        0        0      794 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py
+-rw-r--r--   0        0        0     1364 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py
+-rw-r--r--   0        0        0      831 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py
+-rw-r--r--   0        0        0      894 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py
+-rw-r--r--   0        0        0      771 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py
+-rw-r--r--   0        0        0     4769 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py
+-rw-r--r--   0        0        0     5045 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py
+-rw-r--r--   0        0        0    10576 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py
+-rw-r--r--   0        0        0    15657 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py
+-rw-r--r--   0        0        0     2628 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py
+-rw-r--r--   0        0        0     4888 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py
+-rw-r--r--   0        0        0     2905 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/utils/__init__.py
+-rw-r--r--   0        0        0     3362 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py
+-rwxr-xr-x   0        0        0      347 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/main.py
+-rw-r--r--   0        0        0      774 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/templates/luigi_log.conf
+-rw-r--r--   0        0        0        0 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/__init__.py
+-rw-r--r--   0        0        0     2445 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py
+-rw-r--r--   0        0        0     4600 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_test_environment.py
+-rw-r--r--   0        0        0     2691 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/docker_registry.py
+-rw-r--r--   0        0        0     1407 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py
+-rw-r--r--   0        0        0     8830 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py
+-rw-r--r--   0        0        0      559 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/luigi_utils.py
+-rw-r--r--   0        0        0      824 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py
+-rw-r--r--   0        0        0     1988 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/utils.py
+-rw-r--r--   0        0        0      331 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/ext/01_nodoc
+-rw-r--r--   0        0        0     1815 2023-05-12 07:21:48.623348 exasol_integration_test_docker_environment-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6147 2023-05-12 07:21:48.623348 exasol_integration_test_docker_environment-1.6.0/pytest_itde/__init__.py
+-rw-r--r--   0        0        0     3335 2023-05-12 07:21:48.623348 exasol_integration_test_docker_environment-1.6.0/pytest_itde/config.py
+-rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 exasol_integration_test_docker_environment-1.6.0/PKG-INFO
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/LICENSE` & `exasol_integration_test_docker_environment-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/README.rst` & `exasol_integration_test_docker_environment-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/cli.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/cli.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/commands/health.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/health.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from exasol_integration_test_docker_environment.cli.cli import cli
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import (
     docker_repository_options,
 )
 from exasol_integration_test_docker_environment.cli.options.system_options import (
     output_directory_option,
     system_options,
-    tempory_base_directory_option,
+    tempory_base_directory_option, luigi_logging_options,
 )
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import (
     docker_db_options,
 )
 from exasol_integration_test_docker_environment.cli.termination_handler import (
     TerminationHandler,
 )
@@ -74,38 +74,41 @@
     help="The docker runtime used to start all containers",
 )
 @add_options(docker_db_options)
 @add_options(docker_repository_options)
 @add_options([output_directory_option])
 @add_options([tempory_base_directory_option])
 @add_options(system_options)
+@add_options(luigi_logging_options)
 def spawn_test_environment(
-    environment_name: str,
-    database_port_forward: Optional[int],
-    bucketfs_port_forward: Optional[int],
-    db_mem_size: str,
-    db_disk_size: str,
-    nameserver: Tuple[str, ...],
-    docker_runtime: Optional[str],
-    docker_db_image_version: str,
-    docker_db_image_name: str,
-    create_certificates: bool,
-    additional_db_parameter: Tuple[str, ...],
-    source_docker_repository_name: str,
-    source_docker_tag_prefix: str,
-    source_docker_username: Optional[str],
-    source_docker_password: Optional[str],
-    target_docker_repository_name: str,
-    target_docker_tag_prefix: str,
-    target_docker_username: Optional[str],
-    target_docker_password: Optional[str],
-    output_directory: str,
-    temporary_base_directory: str,
-    workers: int,
-    task_dependencies_dot_file: Optional[str],
+        environment_name: str,
+        database_port_forward: Optional[int],
+        bucketfs_port_forward: Optional[int],
+        db_mem_size: str,
+        db_disk_size: str,
+        nameserver: Tuple[str, ...],
+        docker_runtime: Optional[str],
+        docker_db_image_version: str,
+        docker_db_image_name: str,
+        create_certificates: bool,
+        additional_db_parameter: Tuple[str, ...],
+        source_docker_repository_name: str,
+        source_docker_tag_prefix: str,
+        source_docker_username: Optional[str],
+        source_docker_password: Optional[str],
+        target_docker_repository_name: str,
+        target_docker_tag_prefix: str,
+        target_docker_username: Optional[str],
+        target_docker_password: Optional[str],
+        output_directory: str,
+        temporary_base_directory: str,
+        workers: int,
+        task_dependencies_dot_file: Optional[str],
+        log_level: Optional[str],
+        use_job_specific_log_file: bool
 ):
     """
     This command spawn a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     """
     with TerminationHandler():
         try:
@@ -129,14 +132,16 @@
                 target_docker_tag_prefix,
                 target_docker_username,
                 target_docker_password,
                 output_directory,
                 temporary_base_directory,
                 workers,
                 task_dependencies_dot_file,
+                log_level=log_level,
+                use_job_specific_log_file=use_job_specific_log_file,
             )
         except ArgumentConstraintError as e:
             handle_wrong_argument_error(*e.args)
 
 
 def handle_wrong_argument_error(argument_name, message):
     formatted = f"--{argument_name}".replace("_", "-")
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/build_options.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/build_options.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/system_options.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/system_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,27 @@
 output_directory_option = click.option('--output-directory', type=click.Path(file_okay=False, dir_okay=True),
                                        default=DEFAULT_OUTPUT_DIRECTORY,
                                        show_default=True,
                                        help="Output directory where the system stores all output and log files.")
 
 tempory_base_directory_option = click.option('--temporary-base-directory',
                                              type=click.Path(file_okay=False,
-                                                      dir_okay=True),
+                                                             dir_okay=True),
                                              default="/tmp",
                                              show_default=True,
                                              help="Directory where the system creates temporary directories.")
 
 system_options = [
     click.option('--workers', type=int,
                  default=5, show_default=True,
                  help="Number of parallel workers"),
     click.option('--task-dependencies-dot-file', type=click.Path(file_okay=True),
-                 default=None, help="Path where to store the Task Dependency Graph as dot file")
+                 default=None, help="Path where to store the Task Dependency Graph as dot file"),
+]
+
+luigi_logging_options = [
+    click.option('--log-level', type=click.Choice(['DEBUG', 'INFO', 'WARNING', 'ERROR', 'FATAL']),
+                 default=None, help="Log level used for console logging"),
+    click.option('--use-job-specific-log-file', type=bool,
+                 default=True, help="Use a job specific log file which write the debug log "
+                                    "to the job directory in the build directory")
 ]
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/cli/termination_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/termination_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/doctor.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/doctor.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/__init__.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.lib.api.common import set_build_config, \
     set_docker_repository_config, run_task, generate_root_task, no_cli_function
-from exasol_integration_test_docker_environment.cli.options.docker_repository_options import DEFAULT_DOCKER_REPOSITORY_NAME
+from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
+    DEFAULT_DOCKER_REPOSITORY_NAME
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
     TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 from exasol_integration_test_docker_environment.lib.test_environment.analyze_test_container import AnalyzeTestContainer, \
     DockerTestContainerBuild
 
@@ -27,15 +28,18 @@
         source_docker_username: Optional[str] = None,
         source_docker_password: Optional[str] = None,
         target_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         target_docker_tag_prefix: str = '',
         target_docker_username: Optional[str] = None,
         target_docker_password: Optional[str] = None,
         workers: int = 5,
-        task_dependencies_dot_file: Optional[str] = None) -> ImageInfo:
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = False
+) -> ImageInfo:
     """
     This function builds all stages of the test container for the test environment.
     If stages are cached in a docker registry, the function is going to pull them,
     instead of building them.
     It returns the image info of the test-container.
     """
     set_build_config(force_rebuild,
@@ -51,9 +55,11 @@
 
     set_docker_repository_config(source_docker_password, source_docker_repository_name, source_docker_username,
                                  source_docker_tag_prefix, "source")
     set_docker_repository_config(target_docker_password, target_docker_repository_name, target_docker_username,
                                  target_docker_tag_prefix, "target")
     task_creator = lambda: generate_root_task(task_class=DockerTestContainerBuild,
                                               test_container_content=test_container_content)
-    image_infos = run_task(task_creator, workers, task_dependencies_dot_file)
+    image_infos = run_task(task_creator, workers, task_dependencies_dot_file,
+                           log_level=log_level,
+                           use_job_specific_log_file=use_job_specific_log_file)
     return image_infos["test-container"]
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/common.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,55 @@
+import contextlib
 import getpass
 import json
 import logging
 import os
+import warnings
 from datetime import datetime
 from pathlib import Path
 from typing import (
     Callable,
     Tuple,
     Set,
-    Optional, Any
+    Optional, Any, Dict, Iterator
 )
 
 import luigi
 import networkx
+from luigi.parameter import UnconsumedParameterWarning
+from luigi.setup_logging import InterfaceLogging
 from networkx import DiGraph
 
 from exasol_integration_test_docker_environment.lib import extract_modulename_for_build_steps
 from exasol_integration_test_docker_environment.lib.api.api_errors import TaskRuntimeError
 from exasol_integration_test_docker_environment.lib.base.dependency_logger_base_task import DependencyLoggerBaseTask
 from exasol_integration_test_docker_environment.lib.base.luigi_log_config import get_luigi_log_config, get_log_path
 from exasol_integration_test_docker_environment.lib.base.task_dependency import TaskDependency, DependencyState
 
 
+class JobCounterSingleton(object):
+    """
+    We use here a Singleton to avoid a unprotected global variable.
+    However, this counter needs to be global counter to guarantee unique job ids.
+    This is needed in case of task that finish in less than a second, to avoid duplicated job ids
+    """
+
+    _instance = None
+
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super(JobCounterSingleton, cls).__new__(cls)
+            cls._instance._counter = 0
+        return cls._instance
+
+    def get_next_value(self) -> int:
+        self._counter += 1
+        return self._counter
+
+
 def set_build_config(force_rebuild: bool,
                      force_rebuild_from: Tuple[str, ...],
                      force_pull: bool,
                      log_build_context_content: bool,
                      output_directory: str,
                      temporary_base_directory: str,
                      cache_directory: str,
@@ -82,50 +106,106 @@
         module_name_for_build_steps = extract_modulename_for_build_steps(path)
         spec = importlib.util.spec_from_file_location(module_name_for_build_steps, path_to_build_steps)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
 
 
 def generate_root_task(task_class, *args, **kwargs) -> DependencyLoggerBaseTask:
+    job_counter = JobCounterSingleton().get_next_value()
     strftime = datetime.now().strftime('%Y_%m_%d_%H_%M_%S')
-    params = {"job_id": f"{strftime}_{task_class.__name__}"}
+    params = {"job_id": f"{strftime}_{job_counter}_{task_class.__name__}"}
     params.update(kwargs)
     return task_class(**params)
 
 
-def run_task(task_creator: Callable[[], DependencyLoggerBaseTask], workers: int,
-             task_dependencies_dot_file: Optional[str]) \
+def run_task(task_creator: Callable[[], DependencyLoggerBaseTask], workers: int = 2,
+             task_dependencies_dot_file: Optional[str] = None,
+             log_level: str = None, use_job_specific_log_file: bool = False) \
         -> Any:
     setup_worker()
     task = task_creator()
     success = False
+    log_file_path = get_log_path(task.job_id)
     try:
-        with get_luigi_log_config(get_log_path()) as luigi_config:
-            no_scheduling_errors = luigi.build([task], workers=workers,
-                                               local_scheduler=True,
-                                               logging_conf_file=f'{luigi_config}')
+        no_scheduling_errors = \
+            _run_task_with_logging_config(
+                task, log_file_path, log_level, use_job_specific_log_file, workers)
         success = not task.failed_target.exists() and no_scheduling_errors
-        generate_graph_from_task_dependencies(task, task_dependencies_dot_file)
-
-        if success:
-            return task.get_result()
-        elif task.failed_target.exists():
-            logging.error(f"Task {task} failed. failed target exists.")
-            raise TaskRuntimeError(msg=f"Task {task} (or any of it's subtasks) failed.",
-                                   inner=list(task.collect_failures().keys()))
-        elif not no_scheduling_errors:
-            logging.error(f"Task {task} failed. : luigi reported a scheduling error.")
-            raise TaskRuntimeError(msg=f"Task {task} failed. reason: luigi reported a scheduling error.")
+        return _handle_task_result(no_scheduling_errors, success, task,
+                                   task_dependencies_dot_file)
     except BaseException as e:
         logging.error("Going to abort the task %s" % task)
         raise e
     finally:
+        if use_job_specific_log_file:
+            logging.info(
+                f"The detailed log of the integration-test-docker-environment can be found at: {log_file_path}")
         task.cleanup(success)
 
 
+def _run_task_with_logging_config(
+        task: DependencyLoggerBaseTask,
+        log_file_path: Path,
+        log_level: Optional[str],
+        use_job_specific_log_file: bool,
+        workers: int) -> bool:
+    with _configure_logging(log_file_path, log_level, use_job_specific_log_file) as run_kwargs:
+        no_scheduling_errors = luigi.build([task], workers=workers,
+                                           local_scheduler=True, **run_kwargs)
+        return no_scheduling_errors
+
+
+def _handle_task_result(no_scheduling_errors, success, task, task_dependencies_dot_file: Optional[str]) -> Any:
+    generate_graph_from_task_dependencies(task, task_dependencies_dot_file)
+    if success:
+        return task.get_result()
+    elif task.failed_target.exists():
+        logging.error(f"Task {task} failed. failed target exists.")
+        raise TaskRuntimeError(msg=f"Task {task} (or any of it's subtasks) failed.",
+                               inner=list(task.collect_failures().keys()))
+    elif not no_scheduling_errors:
+        logging.error(f"Task {task} failed. : luigi reported a scheduling error.")
+        raise TaskRuntimeError(msg=f"Task {task} failed. reason: luigi reported a scheduling error.")
+
+
+@contextlib.contextmanager
+def _configure_logging(
+        log_file_path: Path,
+        log_level: Optional[str],
+        use_job_specific_log_file: bool) -> Iterator[Dict[str, str]]:
+    with get_luigi_log_config(log_file_target=log_file_path,
+                              log_level=log_level,
+                              use_job_specific_log_file=use_job_specific_log_file) as luigi_config:
+        no_configure_logging, run_kwargs = _configure_logging_parameter(
+            log_level=log_level,
+            luigi_config=luigi_config,
+            use_job_specific_log_file=use_job_specific_log_file)
+        # We need to set InterfaceLogging._configured to false,
+        # because otherwise luigi doesn't accept the new config.
+        InterfaceLogging._configured = False
+        luigi.configuration.get_config().set('core', 'no_configure_logging', str(no_configure_logging))
+        with warnings.catch_warnings():
+            # This filter is necessary, because luigi uses the config no_configure_logging,
+            # but doesn't define it, which seems to be a bug in luigi
+            warnings.filterwarnings(action="ignore",
+                                    category=UnconsumedParameterWarning,
+                                    message=".*no_configure_logging.*")
+            yield run_kwargs
+
+
+def _configure_logging_parameter(log_level: str, luigi_config: Path, use_job_specific_log_file: bool) \
+        -> Tuple[bool, Dict[str, str]]:
+    if use_job_specific_log_file:
+        no_configure_logging = False
+        run_kwargs = {"logging_conf_file": f'{luigi_config}'}
+    else:
+        no_configure_logging = True
+        run_kwargs = {}
+    return no_configure_logging, run_kwargs
+
 def generate_graph_from_task_dependencies(task: DependencyLoggerBaseTask, task_dependencies_dot_file: Optional[str]):
     if task_dependencies_dot_file is not None:
         print(f"Generate Task Dependency Graph to {task_dependencies_dot_file}")
         print()
         dependencies = collect_dependencies(task)
         g = DiGraph()
         for dependency in dependencies:
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/health.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/health.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.lib.api.common import set_docker_repository_config, \
     run_task, set_build_config, generate_root_task, no_cli_function
-from exasol_integration_test_docker_environment.cli.options.docker_repository_options import DEFAULT_DOCKER_REPOSITORY_NAME
+from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
+    DEFAULT_DOCKER_REPOSITORY_NAME
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
     TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 from exasol_integration_test_docker_environment.lib.test_environment.analyze_test_container import \
     AnalyzeTestContainer, DockerTestContainerPush
 
@@ -29,15 +30,18 @@
         source_docker_username: Optional[str] = None,
         source_docker_password: Optional[str] = None,
         target_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         target_docker_tag_prefix: str = '',
         target_docker_username: Optional[str] = None,
         target_docker_password: Optional[str] = None,
         workers: int = 5,
-        task_dependencies_dot_file: Optional[str] = None) -> ImageInfo:
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = False
+) -> ImageInfo:
     """
     This function pushes all stages of the test container for the test environment.
     If the stages do not exist locally, the system will build or pull them before the push.
     """
     set_build_config(force_rebuild,
                      force_rebuild_from,
                      force_pull,
@@ -53,9 +57,11 @@
                                  source_docker_tag_prefix, "source")
     set_docker_repository_config(target_docker_password, target_docker_repository_name, target_docker_username,
                                  target_docker_tag_prefix, "target")
     task_creator = lambda: generate_root_task(task_class=DockerTestContainerPush,
                                               test_container_content=test_container_content,
                                               force_push=force_push,
                                               push_all=push_all)
-    image_infos = run_task(task_creator, workers, task_dependencies_dot_file)
+    image_infos = run_task(task_creator, workers, task_dependencies_dot_file,
+                           log_level=log_level,
+                           use_job_specific_log_file=use_job_specific_log_file)
     return image_infos[0]
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 from typing import Tuple, Optional, Callable
 import humanfriendly
 
 from exasol_integration_test_docker_environment.lib.api.common import set_build_config, set_docker_repository_config, \
     run_task, generate_root_task, cli_function
-from exasol_integration_test_docker_environment.cli.options.docker_repository_options import DEFAULT_DOCKER_REPOSITORY_NAME
+from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
+    DEFAULT_DOCKER_REPOSITORY_NAME
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import LATEST_DB_VERSION
 from exasol_integration_test_docker_environment.lib.api.api_errors import ArgumentConstraintError
 from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
 from exasol_integration_test_docker_environment.lib.docker.container.utils import remove_docker_container
 from exasol_integration_test_docker_environment.lib.docker.volumes.utils import remove_docker_volumes
 from exasol_integration_test_docker_environment.lib.docker.networks.utils import remove_docker_networks
@@ -42,15 +43,18 @@
         target_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         target_docker_tag_prefix: str = '',
         target_docker_username: Optional[str] = None,
         target_docker_password: Optional[str] = None,
         output_directory: str = DEFAULT_OUTPUT_DIRECTORY,
         temporary_base_directory: str = "/tmp",
         workers: int = 5,
-        task_dependencies_dot_file: Optional[str] = None) -> Tuple[EnvironmentInfo, Callable[[], None]]:
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = False
+) -> Tuple[EnvironmentInfo, Callable[[], None]]:
     """
     This function spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     The function returns an environment_info object, describing the environment, and a cleanup-method, which
     can be used to stop the environment.
     raises: TaskRuntimeError if spawning the test environment fails
 
@@ -92,9 +96,11 @@
                                               no_test_container_cleanup_after_failure=False,
                                               no_database_cleanup_after_success=True,
                                               no_database_cleanup_after_failure=False,
                                               create_certificates=create_certificates,
                                               test_container_content=None,
                                               additional_db_parameter=additional_db_parameter
                                               )
-    environment_info = run_task(task_creator, workers, task_dependencies_dot_file)
+    environment_info = run_task(task_creator, workers, task_dependencies_dot_file,
+                                log_level=log_level,
+                                use_job_specific_log_file=use_job_specific_log_file)
     return environment_info, functools.partial(_cleanup, environment_info)
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 from typing import Tuple, Optional, Callable
 import humanfriendly
 
 from exasol_integration_test_docker_environment.lib.api.common import set_build_config, set_docker_repository_config, \
     run_task, generate_root_task, no_cli_function
-from exasol_integration_test_docker_environment.cli.options.docker_repository_options import DEFAULT_DOCKER_REPOSITORY_NAME
+from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
+    DEFAULT_DOCKER_REPOSITORY_NAME
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import LATEST_DB_VERSION
 from exasol_integration_test_docker_environment.lib.api.api_errors import ArgumentConstraintError
 from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
 from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
     TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.container.utils import remove_docker_container
@@ -32,15 +33,15 @@
 def spawn_test_environment_with_test_container(
         environment_name: str,
         test_container_content: TestContainerContentDescription,
         database_port_forward: Optional[int] = None,
         bucketfs_port_forward: Optional[int] = None,
         db_mem_size: str = "2 GiB",
         db_disk_size: str = "2 GiB",
-        nameserver: Tuple[str,...] = tuple(),
+        nameserver: Tuple[str, ...] = tuple(),
         docker_runtime: Optional[str] = None,
         docker_db_image_version: str = LATEST_DB_VERSION,
         docker_db_image_name: str = "exasol/docker-db",
         create_certificates: bool = False,
         additional_db_parameter: Tuple[str, ...] = tuple(),
         source_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         source_docker_tag_prefix: str = '',
@@ -49,15 +50,18 @@
         target_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         target_docker_tag_prefix: str = '',
         target_docker_username: Optional[str] = None,
         target_docker_password: Optional[str] = None,
         output_directory: str = DEFAULT_OUTPUT_DIRECTORY,
         temporary_base_directory: str = "/tmp",
         workers: int = 5,
-        task_dependencies_dot_file: Optional[str] = None) \
+        task_dependencies_dot_file: Optional[str] = None,
+        log_level: Optional[str] = None,
+        use_job_specific_log_file: bool = False
+) \
         -> Tuple[EnvironmentInfo, Callable[[], None]]:
     """
     This function spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     The function returns an environment_info object, describing the environment, and a cleanup-method, which
     can be used to stop the environment.
     raises: TaskRuntimeError if spawning the test environment fails
@@ -100,9 +104,11 @@
                                               no_test_container_cleanup_after_failure=False,
                                               no_database_cleanup_after_success=True,
                                               no_database_cleanup_after_failure=False,
                                               create_certificates=create_certificates,
                                               test_container_content=test_container_content,
                                               additional_db_parameter=additional_db_parameter
                                               )
-    environment_info = run_task(task_creator, workers, task_dependencies_dot_file)
+    environment_info = run_task(task_creator, workers, task_dependencies_dot_file,
+                                log_level=log_level,
+                                use_job_specific_log_file=use_job_specific_log_file)
     return environment_info, functools.partial(_cleanup, environment_info)
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/info.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/info.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import logging
+
+
 class TaskLoggerWrapper():
-    def __init__(self, logger, task_id):
+    def __init__(self, logger: logging.Logger, task_id):
         self.task_id = task_id
         self.logger = logger
 
     def get_message(self, msg):
         return f"{self.task_id}: {msg}"
 
     def debug(self, msg, *args, **kwargs):
@@ -23,8 +26,8 @@
 
     def exception(self, msg, *args, exc_info=True, **kwargs):
         self.logger.exception(self.get_message(msg), *args, **kwargs)
 
     def critical(self, msg, *args, **kwargs):
         self.logger.critical(self.get_message(msg), *args, **kwargs)
 
-    fatal = critical
+    fatal = critical
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/config/build_config.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/build_config.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/config/docker_config.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/docker_config.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/container_info.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/container_info.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/environment_info.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/environment_info.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/__init__.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Set, Dict
 
-from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
+from exasol_integration_test_docker_environment.lib.config.build_config import build_config
 from exasol_integration_test_docker_environment.lib.config.docker_config import target_docker_repository_config, \
     source_docker_repository_config
-from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
-    TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.images.create.docker_build_base import DockerBuildBase
 from exasol_integration_test_docker_environment.lib.docker.images.create.docker_image_analyze_task import \
     DockerAnalyzeImageTask
 from exasol_integration_test_docker_environment.lib.docker.images.push.docker_push_parameter import DockerPushParameter
 from exasol_integration_test_docker_environment.lib.docker.images.push.push_task_creator_for_build_tasks import \
     PushTaskCreatorFromBuildTasks
+from exasol_integration_test_docker_environment.lib.test_environment.parameter.test_container_parameter import \
+    TestContainerParameter
 
 
-class AnalyzeTestContainer(DockerAnalyzeImageTask):
-    test_container_content = JsonPickleParameter(TestContainerContentDescription)
+class AnalyzeTestContainer(DockerAnalyzeImageTask, TestContainerParameter):
 
     def get_target_repository_name(self) -> str:
         return f"""{target_docker_repository_config().repository_name}"""
 
     def get_source_repository_name(self) -> str:
         return f"""{source_docker_repository_config().repository_name}"""
 
@@ -38,20 +37,19 @@
         return {mapping.target: str(mapping.source) for mapping
                 in self.test_container_content.build_files_and_directories}
 
     def get_dockerfile(self):
         return str(self.test_container_content.docker_file)
 
     def is_rebuild_requested(self) -> bool:
-        return False
+        config = build_config()
+        return config.force_rebuild
 
 
-class DockerTestContainerBuildBase(DockerBuildBase):
-
-    test_container_content = JsonPickleParameter(TestContainerContentDescription)
+class DockerTestContainerBuildBase(DockerBuildBase, TestContainerParameter):
 
     def get_goal_class_map(self) -> Dict[str, DockerAnalyzeImageTask]:
         goal_class_map = {"test-container": self.create_child_task(task_class=AnalyzeTestContainer,
                                                                    test_container_content=self.test_container_content)}
         return goal_class_map
 
     def get_default_goals(self) -> Set[str]:
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dataclasses
 from pathlib import Path
 from typing import Tuple
 
 import luigi
 from docker.models.containers import Container
 from exasol_bucketfs_utils_python import list_files, upload
 from exasol_bucketfs_utils_python.bucket_config import BucketConfig
@@ -17,14 +18,20 @@
 from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
 from exasol_integration_test_docker_environment.lib.test_environment.database_setup.docker_db_log_based_bucket_sync_checker import \
     DockerDBLogBasedBucketFSSyncChecker
 from exasol_integration_test_docker_environment.lib.test_environment.database_setup.time_based_bucketfs_sync_waiter import \
     TimeBasedBucketFSSyncWaiter
 
 
+@dataclasses.dataclass
+class UploadResult:
+    upload_target: str
+    reused: bool
+
+
 class UploadFileToBucketFS(DockerBaseTask):
     environment_name = luigi.Parameter()
     test_environment_info = JsonPickleParameter(
         EnvironmentInfo, significant=False)  # type: EnvironmentInfo
     reuse_uploaded = luigi.BoolParameter(False, significant=False)
     bucketfs_write_password = luigi.Parameter(
         significant=False, visibility=luigi.parameter.ParameterVisibility.HIDDEN)
@@ -49,18 +56,26 @@
             if not self.should_be_reused(upload_target):
                 self.upload_and_wait(database_container,
                                      file_to_upload,
                                      upload_target,
                                      log_file,
                                      pattern_to_wait_for,
                                      sync_time_estimation)
+                self.return_object(UploadResult(
+                    upload_target=upload_target,
+                    reused=False
+                ))
             else:
                 self.logger.warning("Reusing uploaded target %s instead of file %s",
                                     upload_target, file_to_upload)
                 self.write_logs("Reusing")
+                self.return_object(UploadResult(
+                    upload_target=upload_target,
+                    reused=True
+                ))
 
     def upload_and_wait(self, database_container,
                         file_to_upload: str, upload_target: str,
                         log_file: str, pattern_to_wait_for: str,
                         sync_time_estimation: int):
         still_running_logger = StillRunningLogger(self.logger,
                                                   "file upload of %s to %s"
@@ -93,35 +108,33 @@
         else:
             return TimeBasedBucketFSSyncWaiter(sync_time_estimation)
 
     def should_be_reused(self, upload_target: str):
         return self.reuse_uploaded and self.exist_file_in_bucketfs(upload_target)
 
     @staticmethod
-    def split_upload_target(upload_target: str) -> Tuple[str, str]:
+    def split_upload_target(upload_target: str) -> Tuple[str, str, str]:
         upload_parts = upload_target.split("/")
         bucket_name = upload_parts[0]
-        upload_target_in_bucket = "/".join(upload_parts[1:])
-        return bucket_name, upload_target_in_bucket
+        path_in_bucket = "/".join(upload_parts[1:-1])
+        file_in_bucket = upload_parts[-1]
+        return bucket_name, path_in_bucket, file_in_bucket
 
     def exist_file_in_bucketfs(self, upload_target: str) -> bool:
         self.logger.info("Check if file %s exist in bucketfs", upload_target)
-        bucket_name, upload_target = self.split_upload_target(upload_target)
+        bucket_name, path_in_bucket, file_in_bucket = self.split_upload_target(upload_target)
 
         bucket_config = self.generate_bucket_config(bucket_name)
         try:
             files = list_files.list_files_in_bucketfs(
                 bucket_config=bucket_config,
-                bucket_file_path=upload_target)
-            if upload_target not in files:
-                raise RuntimeError(f"Unexpected behavior of list_files.list_files_in_bucketfs. "
-                                   f"bucket_file_path='{upload_target}' was requested, but not returned.")
+                bucket_file_path=path_in_bucket)
+            return file_in_bucket in files
         except FileNotFoundError as ex:
             return False
-        return True
 
     def generate_bucket_config(self, bucket_name: str) -> BucketConfig:
         connection_config = BucketFSConnectionConfig(
             host=self._database_info.host, port=int(self._database_info.bucketfs_port),
             user="w", pwd=str(self.bucketfs_write_password),
             is_https=False)
         bucketfs_config = BucketFSConfig(
@@ -131,20 +144,20 @@
             bucket_name=bucket_name,
             bucketfs_config=bucketfs_config)
         return bucket_config
 
     def upload_file(self, file_to_upload: str, upload_target: str):
         self.logger.info("upload file %s to %s",
                          file_to_upload, upload_target)
-        bucket_name, upload_target = self.split_upload_target(upload_target)
+        bucket_name, path_in_bucket, file_in_bucket = self.split_upload_target(upload_target)
 
         bucket_config = self.generate_bucket_config(bucket_name)
         upload.upload_file_to_bucketfs(
             bucket_config=bucket_config,
-            bucket_file_path=upload_target,
+            bucket_file_path=f"{path_in_bucket}/{file_in_bucket}",
             local_file_path=Path(file_to_upload))
         return f"File '{file_to_upload}' to '{upload_target}'"
 
     def write_logs(self, output):
         log_file = Path(self.get_log_path(), "log")
         with log_file.open("w") as file:
             file.write(output)
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,35 @@
 from docker.transport import unixconn
 
 from exasol_integration_test_docker_environment.lib import PACKAGE_NAME
 from exasol_integration_test_docker_environment.lib.base.docker_base_task import DockerBaseTask
 from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
 from exasol_integration_test_docker_environment.lib.data.container_info import ContainerInfo
 from exasol_integration_test_docker_environment.lib.data.docker_network_info import DockerNetworkInfo
-from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
-    TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageState, ImageInfo
 from exasol_integration_test_docker_environment.lib.test_environment.analyze_test_container import \
     DockerTestContainerBuild
 from exasol_integration_test_docker_environment.lib.test_environment.docker_container_copy import \
     copy_script_to_container
+from exasol_integration_test_docker_environment.lib.test_environment.parameter.test_container_parameter import \
+    TestContainerParameter
 
 
-class SpawnTestContainer(DockerBaseTask):
+class SpawnTestContainer(DockerBaseTask, TestContainerParameter):
     environment_name = luigi.Parameter()
     test_container_name = luigi.Parameter()
     network_info = JsonPickleParameter(
         DockerNetworkInfo, significant=False)  # type: DockerNetworkInfo
     ip_address_index_in_subnet = luigi.IntParameter(significant=False)
     attempt = luigi.IntParameter(1)
     reuse_test_container = luigi.BoolParameter(False, significant=False)
     no_test_container_cleanup_after_success = luigi.BoolParameter(False, significant=False)
     no_test_container_cleanup_after_failure = luigi.BoolParameter(False, significant=False)
     docker_runtime = luigi.OptionalParameter(None, significant=False)
     certificate_volume_name = luigi.OptionalParameter(None, significant=False)
-    test_container_content = JsonPickleParameter(TestContainerContentDescription)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.ip_address_index_in_subnet < 0:
             raise Exception(
                 "ip_address_index_in_subnet needs to be greater than 0 got %s"
                 % self.ip_address_index_in_subnet)
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/templates/luigi_log.conf` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/templates/luigi_log.conf`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [loggers]
-keys=root,luigi
+keys=root,luigi_interface,luigi
 
 [handlers]
 keys=consoleHandler,fileHandler
 
 [formatters]
 keys=fileFormatter,consoleFormatter
 
 [logger_root]
+handlers=consoleHandler
+
+[logger_luigi_interface]
 level=DEBUG
 handlers=consoleHandler,fileHandler
+qualname=luigi-interface
+propagate=0
 
 [logger_luigi]
 level=DEBUG
 handlers=consoleHandler,fileHandler
-qualname=luigi-interface
+qualname=luigi
 propagate=0
 
 [handler_consoleHandler]
 class=StreamHandler
 level={{console_log_level}}
 formatter=consoleFormatter
 args=(sys.stdout,)
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/api_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/docker_registry.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/docker_registry.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/luigi_utils.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/luigi_utils.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/exasol_integration_test_docker_environment/testing/utils.py` & `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/utils.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/pyproject.toml` & `exasol_integration_test_docker_environment-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "exasol-integration-test-docker-environment"
 packages = [
     { include = "exasol_integration_test_docker_environment" },
     { include = "pytest_itde" }
 ]
-version = "1.5.0"
+version = "1.6.0"
 description = "Integration Test Docker Environment for Exasol"
 
 license = "MIT"
 
 authors = [
     "Torsten Kilias <torsten.kilias@exasol.com>"
 ]
```

### Comparing `exasol-integration-test-docker-environment-1.5.0/pytest_itde/__init__.py` & `exasol_integration_test_docker_environment-1.6.0/pytest_itde/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/pytest_itde/config.py` & `exasol_integration_test_docker_environment-1.6.0/pytest_itde/config.py`

 * *Files identical despite different names*

### Comparing `exasol-integration-test-docker-environment-1.5.0/PKG-INFO` & `exasol_integration_test_docker_environment-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: exasol-integration-test-docker-environment
-Version: 1.5.0
+Version: 1.6.0
 Summary: Integration Test Docker Environment for Exasol
 Home-page: https://github.com/exasol/integration-test-docker-environment
 License: MIT
 Keywords: exasol,docker,testing
 Author: Torsten Kilias
 Author-email: torsten.kilias@exasol.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.0)
-Requires-Dist: docker (>=4.0.0); sys_platform != "win32"
+Requires-Dist: docker (>=4.0.0) ; sys_platform != "win32"
 Requires-Dist: exasol-bucketfs (>=0.6.0,<2.0.0)
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: humanfriendly (>=4.18)
 Requires-Dist: importlib_resources (>=5.4.0)
 Requires-Dist: jinja2 (>=2.10.1)
 Requires-Dist: jsonpickle (>=1.1)
 Requires-Dist: luigi (>=2.8.4)
```


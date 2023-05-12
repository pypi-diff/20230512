# Comparing `tmp/cloudshell-cli-5.0.0.zip` & `tmp/cloudshell-cli-5.0.1.zip`

## zipinfo {}

```diff
@@ -1,88 +1,88 @@
-Zip file size: 59595 bytes, number of entries: 86
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell_cli.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/
--rw-r--r--  2.0 unx       34 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/MANIFEST.in
--rw-r--r--  2.0 unx       30 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/README.txt
--rw-r--r--  2.0 unx    11358 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/LICENSE
--rw-r--r--  2.0 unx     1138 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tox.ini
--rw-r--r--  2.0 unx       60 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/dev_requirements.txt
--rw-r--r--  2.0 unx      292 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/PKG-INFO
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/test_requirements.txt
--rw-r--r--  2.0 unx      852 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/setup.py
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/version.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/setup.cfg
--rw-r--r--  2.0 unx       58 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/requirements.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/__init__.py
--rw-r--r--  2.0 unx      103 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/conftest.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/command_template/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/
--rw-r--r--  2.0 unx     4297 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_command_mode.py
--rw-r--r--  2.0 unx     1717 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_configurator.py
--rw-r--r--  2.0 unx     2668 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_node.py
--rw-r--r--  2.0 unx     7215 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_session_pool_manager.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/__init__.py
--rw-r--r--  2.0 unx     2815 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_command_mode_helper.py
--rw-r--r--  2.0 unx     2638 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_session_manager.py
--rw-r--r--  2.0 unx    11465 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_cli_service_impl.py
--rw-r--r--  2.0 unx     6061 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/test_session_pool_context_manager.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/command_template/__init__.py
--rw-r--r--  2.0 unx     2689 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/command_template/test_command_template.py
--rw-r--r--  2.0 unx      395 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/test_expect_session_py3.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/__init__.py
--rw-r--r--  2.0 unx     3739 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/test_telnet_session.py
--rw-r--r--  2.0 unx     2178 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/test_connection_params.py
--rw-r--r--  2.0 unx    21646 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/test_ssh_session.py
--rw-r--r--  2.0 unx    14734 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/tests/cli/session/test_expect_session.py
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell_cli.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2486 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell_cli.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      292 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell_cli.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       58 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell_cli.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell_cli.egg-info/top_level.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/command_template/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/factory/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/
--rw-r--r--  2.0 unx     1275 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/types.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/__init__.py
--rw-r--r--  2.0 unx     4603 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/configurator.py
--rw-r--r--  2.0 unx     2067 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/command_template/command_template_executor.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/command_template/__init__.py
--rw-r--r--  2.0 unx     1687 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/command_template/command_template.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/helper/
--rw-r--r--  2.0 unx     1312 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/console_telnet.py
--rw-r--r--  2.0 unx      442 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/console_ssh.py
--rw-r--r--  2.0 unx     1282 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/connection_params.py
--rw-r--r--  2.0 unx     1906 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/tcp_session.py
--rw-r--r--  2.0 unx     4523 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/ssh_session.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/__init__.py
--rw-r--r--  2.0 unx      430 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/session_exceptions.py
--rw-r--r--  2.0 unx     2555 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/scpi_session.py
--rw-r--r--  2.0 unx     3730 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/tl1_session.py
--rw-r--r--  2.0 unx     3167 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/telnet_session.py
--rw-r--r--  2.0 unx    13316 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/expect_session.py
--rw-r--r--  2.0 unx     1691 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/session.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/helper/__init__.py
--rw-r--r--  2.0 unx      726 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/session/helper/normalize_buffer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/factory/__init__.py
--rw-r--r--  2.0 unx     3447 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/factory/session_factory.py
--rw-r--r--  2.0 unx      321 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/auth_model.py
--rwxr-xr-x  2.0 unx     5596 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/command_mode.py
--rw-r--r--  2.0 unx     2323 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/session_manager_impl.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/__init__.py
--rw-r--r--  2.0 unx     4920 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/cli_service_impl.py
--rw-r--r--  2.0 unx     1909 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/node.py
--rw-r--r--  2.0 unx      156 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/console_model.py
--rw-r--r--  2.0 unx     3989 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool_manager.py
--rw-r--r--  2.0 unx       62 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/cli_exception.py
--rw-r--r--  2.0 unx     1105 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/cli.py
--rw-r--r--  2.0 unx      948 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/session_manager.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/cli_service.py
--rw-r--r--  2.0 unx      707 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool.py
--rw-r--r--  2.0 unx     2731 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/command_mode_helper.py
--rw-r--r--  2.0 unx     2365 b- defN 23-Mar-24 16:00 cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool_context_manager.py
-86 files, 178149 bytes uncompressed, 44075 bytes compressed:  75.3%
+Zip file size: 59594 bytes, number of entries: 86
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell_cli.egg-info/
+-rw-r--r--  2.0 unx       30 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/README.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/test_requirements.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/version.txt
+-rw-r--r--  2.0 unx       34 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/MANIFEST.in
+-rw-r--r--  2.0 unx       58 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/requirements.txt
+-rw-r--r--  2.0 unx      292 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/PKG-INFO
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/LICENSE
+-rw-r--r--  2.0 unx      852 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/setup.py
+-rw-r--r--  2.0 unx       60 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/dev_requirements.txt
+-rw-r--r--  2.0 unx     1138 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tox.ini
+-rw-r--r--  2.0 unx       38 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/setup.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/
+-rw-r--r--  2.0 unx      103 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/conftest.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/command_template/
+-rw-r--r--  2.0 unx     4297 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_command_mode.py
+-rw-r--r--  2.0 unx    11465 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_cli_service_impl.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_node.py
+-rw-r--r--  2.0 unx     7215 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_session_pool_manager.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/__init__.py
+-rw-r--r--  2.0 unx     2638 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_session_manager.py
+-rw-r--r--  2.0 unx     6061 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_session_pool_context_manager.py
+-rw-r--r--  2.0 unx     1717 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_configurator.py
+-rw-r--r--  2.0 unx     2815 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/test_command_mode_helper.py
+-rw-r--r--  2.0 unx     2178 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/test_connection_params.py
+-rw-r--r--  2.0 unx    21646 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/test_ssh_session.py
+-rw-r--r--  2.0 unx    14734 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/test_expect_session.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/__init__.py
+-rw-r--r--  2.0 unx      395 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/test_expect_session_py3.py
+-rw-r--r--  2.0 unx     3739 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/session/test_telnet_session.py
+-rw-r--r--  2.0 unx     2689 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/command_template/test_command_template.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/tests/cli/command_template/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/command_template/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/factory/
+-rw-r--r--  2.0 unx     4603 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/configurator.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/__init__.py
+-rw-r--r--  2.0 unx     1275 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/types.py
+-rw-r--r--  2.0 unx      707 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool.py
+-rw-r--r--  2.0 unx       62 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/cli_exception.py
+-rw-r--r--  2.0 unx     1909 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/node.py
+-rwxr-xr-x  2.0 unx     5596 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/command_mode.py
+-rw-r--r--  2.0 unx      948 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/session_manager.py
+-rw-r--r--  2.0 unx     3989 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool_manager.py
+-rw-r--r--  2.0 unx     4920 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/cli_service_impl.py
+-rw-r--r--  2.0 unx     2731 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/command_mode_helper.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/cli_service.py
+-rw-r--r--  2.0 unx     1105 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/cli.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/__init__.py
+-rw-r--r--  2.0 unx      156 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/console_model.py
+-rw-r--r--  2.0 unx      321 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/auth_model.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool_context_manager.py
+-rw-r--r--  2.0 unx     2323 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/service/session_manager_impl.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/helper/
+-rw-r--r--  2.0 unx     3730 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/tl1_session.py
+-rw-r--r--  2.0 unx     4483 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/ssh_session.py
+-rw-r--r--  2.0 unx     1282 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/connection_params.py
+-rw-r--r--  2.0 unx     3167 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/telnet_session.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/__init__.py
+-rw-r--r--  2.0 unx     1312 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/console_telnet.py
+-rw-r--r--  2.0 unx     2555 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/scpi_session.py
+-rw-r--r--  2.0 unx      430 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/session_exceptions.py
+-rw-r--r--  2.0 unx    13316 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/expect_session.py
+-rw-r--r--  2.0 unx     1906 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/tcp_session.py
+-rw-r--r--  2.0 unx     1691 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/session.py
+-rw-r--r--  2.0 unx      442 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/console_ssh.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/helper/__init__.py
+-rw-r--r--  2.0 unx      726 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/session/helper/normalize_buffer.py
+-rw-r--r--  2.0 unx     1687 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/command_template/command_template.py
+-rw-r--r--  2.0 unx     2067 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/command_template/command_template_executor.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/command_template/__init__.py
+-rw-r--r--  2.0 unx     3447 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/factory/session_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell/cli/factory/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell_cli.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       58 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell_cli.egg-info/requires.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell_cli.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      292 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell_cli.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     2486 b- defN 23-May-12 08:56 cloudshell-cli-5.0.1/cloudshell_cli.egg-info/SOURCES.txt
+86 files, 178109 bytes uncompressed, 44074 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,259 +1,259 @@
-Filename: cloudshell-cli-5.0.0/
+Filename: cloudshell-cli-5.0.1/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/
+Filename: cloudshell-cli-5.0.1/tests/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell_cli.egg-info/
+Filename: cloudshell-cli-5.0.1/cloudshell/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/
+Filename: cloudshell-cli-5.0.1/cloudshell_cli.egg-info/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/MANIFEST.in
+Filename: cloudshell-cli-5.0.1/README.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/README.txt
+Filename: cloudshell-cli-5.0.1/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/LICENSE
+Filename: cloudshell-cli-5.0.1/version.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tox.ini
+Filename: cloudshell-cli-5.0.1/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/dev_requirements.txt
+Filename: cloudshell-cli-5.0.1/requirements.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/PKG-INFO
+Filename: cloudshell-cli-5.0.1/PKG-INFO
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/test_requirements.txt
+Filename: cloudshell-cli-5.0.1/LICENSE
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/setup.py
+Filename: cloudshell-cli-5.0.1/setup.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/version.txt
+Filename: cloudshell-cli-5.0.1/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/setup.cfg
+Filename: cloudshell-cli-5.0.1/tox.ini
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/requirements.txt
+Filename: cloudshell-cli-5.0.1/setup.cfg
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/
+Filename: cloudshell-cli-5.0.1/tests/cli/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/__init__.py
+Filename: cloudshell-cli-5.0.1/tests/conftest.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/conftest.py
+Filename: cloudshell-cli-5.0.1/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/command_template/
+Filename: cloudshell-cli-5.0.1/tests/cli/session/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/
+Filename: cloudshell-cli-5.0.1/tests/cli/command_template/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_command_mode.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_command_mode.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_configurator.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_cli_service_impl.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_node.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_node.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_session_pool_manager.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_session_pool_manager.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/__init__.py
+Filename: cloudshell-cli-5.0.1/tests/cli/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_command_mode_helper.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_session_manager.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_session_manager.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_session_pool_context_manager.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_cli_service_impl.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_configurator.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/test_session_pool_context_manager.py
+Filename: cloudshell-cli-5.0.1/tests/cli/test_command_mode_helper.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/command_template/__init__.py
+Filename: cloudshell-cli-5.0.1/tests/cli/session/test_connection_params.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/command_template/test_command_template.py
+Filename: cloudshell-cli-5.0.1/tests/cli/session/test_ssh_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/test_expect_session_py3.py
+Filename: cloudshell-cli-5.0.1/tests/cli/session/test_expect_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/__init__.py
+Filename: cloudshell-cli-5.0.1/tests/cli/session/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/test_telnet_session.py
+Filename: cloudshell-cli-5.0.1/tests/cli/session/test_expect_session_py3.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/test_connection_params.py
+Filename: cloudshell-cli-5.0.1/tests/cli/session/test_telnet_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/test_ssh_session.py
+Filename: cloudshell-cli-5.0.1/tests/cli/command_template/test_command_template.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/tests/cli/session/test_expect_session.py
+Filename: cloudshell-cli-5.0.1/tests/cli/command_template/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell_cli.egg-info/dependency_links.txt
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell_cli.egg-info/SOURCES.txt
+Filename: cloudshell-cli-5.0.1/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell_cli.egg-info/PKG-INFO
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell_cli.egg-info/requires.txt
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell_cli.egg-info/top_level.txt
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/command_template/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/factory/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/configurator.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/command_template/
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/types.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/factory/
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/cli_exception.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/types.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/node.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/command_mode.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/configurator.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/session_manager.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/command_template/command_template_executor.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool_manager.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/command_template/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/cli_service_impl.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/command_template/command_template.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/command_mode_helper.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/helper/
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/cli_service.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/console_telnet.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/cli.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/console_ssh.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/connection_params.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/console_model.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/tcp_session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/auth_model.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/ssh_session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool_context_manager.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/service/session_manager_impl.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/session_exceptions.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/helper/
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/scpi_session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/tl1_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/tl1_session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/ssh_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/telnet_session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/connection_params.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/expect_session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/telnet_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/session.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/helper/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/console_telnet.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/session/helper/normalize_buffer.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/scpi_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/factory/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/session_exceptions.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/factory/session_factory.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/expect_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/auth_model.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/tcp_session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/command_mode.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/session.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/session_manager_impl.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/console_ssh.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/__init__.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/helper/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/cli_service_impl.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/session/helper/normalize_buffer.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/node.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/command_template/command_template.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/console_model.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/command_template/command_template_executor.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool_manager.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/command_template/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/cli_exception.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/factory/session_factory.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/cli.py
+Filename: cloudshell-cli-5.0.1/cloudshell/cli/factory/__init__.py
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/session_manager.py
+Filename: cloudshell-cli-5.0.1/cloudshell_cli.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/cli_service.py
+Filename: cloudshell-cli-5.0.1/cloudshell_cli.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool.py
+Filename: cloudshell-cli-5.0.1/cloudshell_cli.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/command_mode_helper.py
+Filename: cloudshell-cli-5.0.1/cloudshell_cli.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool_context_manager.py
+Filename: cloudshell-cli-5.0.1/cloudshell_cli.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-cli-5.0.0/LICENSE` & `cloudshell-cli-5.0.1/LICENSE`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tox.ini` & `cloudshell-cli-5.0.1/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/setup.py` & `cloudshell-cli-5.0.1/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_command_mode.py` & `cloudshell-cli-5.0.1/tests/cli/test_command_mode.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_configurator.py` & `cloudshell-cli-5.0.1/tests/cli/test_configurator.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_node.py` & `cloudshell-cli-5.0.1/tests/cli/test_node.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_session_pool_manager.py` & `cloudshell-cli-5.0.1/tests/cli/test_session_pool_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_command_mode_helper.py` & `cloudshell-cli-5.0.1/tests/cli/test_command_mode_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_session_manager.py` & `cloudshell-cli-5.0.1/tests/cli/test_session_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_cli_service_impl.py` & `cloudshell-cli-5.0.1/tests/cli/test_cli_service_impl.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/test_session_pool_context_manager.py` & `cloudshell-cli-5.0.1/tests/cli/test_session_pool_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/command_template/test_command_template.py` & `cloudshell-cli-5.0.1/tests/cli/command_template/test_command_template.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/session/test_telnet_session.py` & `cloudshell-cli-5.0.1/tests/cli/session/test_telnet_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/session/test_connection_params.py` & `cloudshell-cli-5.0.1/tests/cli/session/test_connection_params.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/session/test_ssh_session.py` & `cloudshell-cli-5.0.1/tests/cli/session/test_ssh_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/tests/cli/session/test_expect_session.py` & `cloudshell-cli-5.0.1/tests/cli/session/test_expect_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell_cli.egg-info/SOURCES.txt` & `cloudshell-cli-5.0.1/cloudshell_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/types.py` & `cloudshell-cli-5.0.1/cloudshell/cli/types.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/configurator.py` & `cloudshell-cli-5.0.1/cloudshell/cli/configurator.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/command_template/command_template_executor.py` & `cloudshell-cli-5.0.1/cloudshell/cli/command_template/command_template_executor.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/command_template/command_template.py` & `cloudshell-cli-5.0.1/cloudshell/cli/command_template/command_template.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/console_telnet.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/console_telnet.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/connection_params.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/connection_params.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/tcp_session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/tcp_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/ssh_session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/ssh_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,20 @@
         self.pkey_passphrase = pkey_passphrase
 
         self._handler = None
         self._current_channel = None
         self._buffer_size = self.BUFFER_SIZE
 
     def __eq__(self, other) -> bool:
-        return all(
-            [
-                ConnectionParams.__eq__(self, other),
-                self.username == other.username,
-                self.password == other.password,
-                self.pkey == other.pkey,
-                self.pkey_passphrase == other.pkey_passphrase,
-            ]
+        return (
+            ConnectionParams.__eq__(self, other)
+            and self.username == other.username
+            and self.password == other.password
+            and self.pkey == other.pkey
+            and self.pkey_passphrase == other.pkey_passphrase
         )
 
     def __del__(self) -> None:
         self.disconnect()
 
     def _create_handler(self) -> None:
         self._handler = paramiko.SSHClient()
```

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/scpi_session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/scpi_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/tl1_session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/tl1_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/telnet_session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/telnet_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/expect_session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/expect_session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/session.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/session.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/session/helper/normalize_buffer.py` & `cloudshell-cli-5.0.1/cloudshell/cli/session/helper/normalize_buffer.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/factory/session_factory.py` & `cloudshell-cli-5.0.1/cloudshell/cli/factory/session_factory.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/command_mode.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/command_mode.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/session_manager_impl.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/session_manager_impl.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/cli_service_impl.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/cli_service_impl.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/node.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/node.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool_manager.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/cli.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/cli.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/session_manager.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/session_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/cli_service.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/cli_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/command_mode_helper.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/command_mode_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cli-5.0.0/cloudshell/cli/service/session_pool_context_manager.py` & `cloudshell-cli-5.0.1/cloudshell/cli/service/session_pool_context_manager.py`

 * *Files identical despite different names*


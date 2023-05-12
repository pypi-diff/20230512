# Comparing `tmp/testgear-python-commons-2.1.2.tar.gz` & `tmp/testgear-python-commons-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-python-commons-2.1.2.tar", last modified: Fri Apr 21 14:54:27 2023, max compression
+gzip compressed data, was "testgear-python-commons-2.1.3.tar", last modified: Fri May 12 09:41:19 2023, max compression
```

## Comparing `testgear-python-commons-2.1.2.tar` & `testgear-python-commons-2.1.3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/
--rw-rw-rw-   0        0        0      563 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/README.md
--rw-rw-rw-   0        0        0      113 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-04-21 13:52:57.000000 testgear-python-commons-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.414215 testgear-python-commons-2.1.2/src/
--rw-rw-rw-   0        0        0      882 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.414215 testgear-python-commons-2.1.2/src/testgear_python_commons/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/__init__.py
--rw-rw-rw-   0        0        0     7773 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/app_properties.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/src/testgear_python_commons/client/
--rw-rw-rw-   0        0        0      176 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/__init__.py
--rw-rw-rw-   0        0        0     5302 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/api_client.py
--rw-rw-rw-   0        0        0     2012 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/client_configuration.py
--rw-rw-rw-   0        0        0    10032 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/client/converter.py
--rw-rw-rw-   0        0        0     4715 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/decorators.py
--rw-rw-rw-   0        0        0     4144 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/dynamic_methods.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/src/testgear_python_commons/models/
--rw-rw-rw-   0        0        0       97 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/__init__.py
--rw-rw-rw-   0        0        0       91 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/adapter_mode.py
--rw-rw-rw-   0        0        0      180 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/link_type.py
--rw-rw-rw-   0        0        0      116 2023-04-21 13:47:37.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/models/outcome_type.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.428821 testgear-python-commons-2.1.2/src/testgear_python_commons/services/
--rw-rw-rw-   0        0        0      387 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/__init__.py
--rw-rw-rw-   0        0        0     2159 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager.py
--rw-rw-rw-   0        0        0     1265 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager_configuration.py
--rw-rw-rw-   0        0        0     1601 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/logger.py
--rw-rw-rw-   0        0        0     1717 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/plugin_manager.py
--rw-rw-rw-   0        0        0    13482 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/services/utils.py
--rw-rw-rw-   0        0        0     5281 2023-04-21 13:52:32.000000 testgear-python-commons-2.1.2/src/testgear_python_commons/step.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:54:27.414215 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/
--rw-rw-rw-   0        0        0      563 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-04-21 14:54:27.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-04-21 14:54:26.000000 testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.500736 testgear-python-commons-2.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.500736 testgear-python-commons-2.1.3/src/testgear_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/src/testgear_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/src/testgear_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/models/outcome_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/src/testgear_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-12 09:41:06.000000 testgear-python-commons-2.1.3/src/testgear_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:19.504737 testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-12 09:41:19.000000 testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-12 09:41:19.000000 testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:41:19.000000 testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 09:41:19.000000 testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 09:41:19.000000 testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/top_level.txt
```

### Comparing `testgear-python-commons-2.1.2/PKG-INFO` & `testgear-python-commons-2.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: testgear-python-commons
-Version: 2.1.2
-Summary: Python commons for Test Gear
-Home-page: https://github.com/testgear-tms/adapters-python/
-Author: Integration team
-Author-email: integrations@test-gear.io
-License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Metadata-Version: 2.1
+Name: testgear-python-commons
+Version: 2.1.3
+Summary: Python commons for Test Gear
+Home-page: https://github.com/testgear-tms/adapters-python/
+Author: Integration team
+Author-email: integrations@test-gear.io
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `testgear-python-commons-2.1.2/setup.py` & `testgear-python-commons-2.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import find_packages, setup
-
-setup(
-    name='testgear-python-commons',
-    version='2.1.2',
-    description='Python commons for Test Gear',
-    url='https://github.com/testgear-tms/adapters-python/',
-    author='Integration team',
-    author_email='integrations@test-gear.io',
-    license='Apache-2.0',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
-    ],
-    py_modules=['testgear', 'testgear_python_commons'],
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
-    install_requires=['pluggy', 'testgear-api-client==3.0.0']
-)
+from setuptools import find_packages, setup
+
+setup(
+    name='testgear-python-commons',
+    version='2.1.3',
+    description='Python commons for Test Gear',
+    url='https://github.com/testgear-tms/adapters-python/',
+    author='Integration team',
+    author_email='integrations@test-gear.io',
+    license='Apache-2.0',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
+    ],
+    py_modules=['testgear', 'testgear_python_commons'],
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
+    install_requires=['pluggy', 'testgear-api-client==3.0.0']
+)
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/app_properties.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/app_properties.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import configparser
-import logging
-import os
-import re
-import warnings
-
-from testgear_python_commons.models.adapter_mode import AdapterMode
-
-
-class AppProperties:
-    __properties_file = 'connection_config'
-    __env_prefix = 'TMS'
-
-    @staticmethod
-    def load_properties(option=None):
-        properties = AppProperties.load_file_properties(
-            option.set_config_file if hasattr(option, 'set_config_file') else None)
-
-        properties.update(AppProperties.load_env_properties())
-
-        if option:
-            properties.update(AppProperties.load_cli_properties(option))
-
-        AppProperties.__check_properties(properties)
-
-        return properties
-
-    @classmethod
-    def load_file_properties(cls, file_name: str = None):
-        properties = {}
-
-        path = os.path.abspath('')
-        root = path[:path.index(os.sep)]
-
-        if file_name:
-            cls.__properties_file = file_name
-
-        if os.environ.get(f'{cls.__env_prefix}_CONFIG_FILE'):
-            cls.__properties_file = os.environ.get(f'{cls.__env_prefix}_CONFIG_FILE')
-
-        while not os.path.isfile(
-                path + os.sep + f'{cls.__properties_file}.ini') and path != root:
-            path = path[:path.rindex(os.sep)]
-
-        path = path + os.sep + f'{cls.__properties_file}.ini'
-
-        if os.path.isfile(path):
-            parser = configparser.RawConfigParser()
-
-            parser.read(path)
-
-            if parser.has_section('testgear'):
-                for key, value in parser.items('testgear'):
-                    properties[key] = cls.__search_in_environ(value)
-
-            if parser.has_section('debug'):
-                if parser.has_option('debug', 'tmsproxy'):
-                    properties['tmsproxy'] = cls.__search_in_environ(
-                        parser.get('debug', 'tmsproxy'))
-
-                if parser.has_option('debug', '__dev'):
-                    properties['logs'] = cls.__search_in_environ(
-                        parser.get('debug', '__dev')).lower()
-
-            if 'privatetoken' in properties:
-                warnings.warn(
-                    'The configuration file specifies a private token. It is not safe.'
-                    ' Use TMS_PRIVATE_TOKEN environment variable',
-                    category=Warning,
-                    stacklevel=2)
-                warnings.simplefilter('default', Warning)
-
-        return properties
-
-    @staticmethod
-    def load_cli_properties(option):
-        cli_properties = {}
-
-        if hasattr(option, 'set_url') and option.set_url:
-            cli_properties['url'] = option.set_url
-
-        if hasattr(option, 'set_private_token') and option.set_private_token:
-            cli_properties['privatetoken'] = option.set_private_token
-
-        if hasattr(option, 'set_project_id') and option.set_project_id:
-            cli_properties['projectid'] = option.set_project_id
-
-        if hasattr(option, 'set_configuration_id') and option.set_configuration_id:
-            cli_properties['configurationid'] = option.set_configuration_id
-
-        if hasattr(option, 'set_test_run_id') and option.set_test_run_id:
-            cli_properties['testrunid'] = option.set_test_run_id
-
-        if hasattr(option, 'set_test_run_name') and option.set_test_run_name:
-            cli_properties['testrunname'] = option.set_test_run_name
-
-        if hasattr(option, 'set_tms_proxy') and option.set_tms_proxy:
-            cli_properties['tmsproxy'] = option.set_tms_proxy
-
-        if hasattr(option, 'set_adapter_mode') and option.set_adapter_mode:
-            cli_properties['adaptermode'] = option.set_adapter_mode
-
-        if hasattr(option, 'set_cert_validation') and option.set_cert_validation:
-            cli_properties['certvalidation'] = option.set_cert_validation
-
-        if hasattr(option, 'set_automatic_creation_test_cases') and option.set_automatic_creation_test_cases:
-            cli_properties['automaticcreationtestcases'] = option.set_automatic_creation_test_cases
-
-        return cli_properties
-
-    @classmethod
-    def load_env_properties(cls):
-        env_properties = {}
-
-        if f'{cls.__env_prefix}_URL' in os.environ.keys():
-            env_properties['url'] = os.environ.get(f'{cls.__env_prefix}_URL')
-
-        if f'{cls.__env_prefix}_PRIVATE_TOKEN' in os.environ.keys():
-            env_properties['privatetoken'] = os.environ.get(f'{cls.__env_prefix}_PRIVATE_TOKEN')
-
-        if f'{cls.__env_prefix}_PROJECT_ID' in os.environ.keys():
-            env_properties['projectid'] = os.environ.get(f'{cls.__env_prefix}_PROJECT_ID')
-
-        if f'{cls.__env_prefix}_CONFIGURATION_ID' in os.environ.keys():
-            env_properties['configurationid'] = os.environ.get(f'{cls.__env_prefix}_CONFIGURATION_ID')
-
-        if f'{cls.__env_prefix}_TEST_RUN_ID' in os.environ.keys():
-            env_properties['testrunid'] = os.environ.get(f'{cls.__env_prefix}_TEST_RUN_ID')
-
-        if f'{cls.__env_prefix}_TEST_RUN_NAME' in os.environ.keys():
-            env_properties['testrunname'] = os.environ.get(f'{cls.__env_prefix}_TEST_RUN_NAME')
-
-        if f'{cls.__env_prefix}_PROXY' in os.environ.keys():
-            env_properties['tmsproxy'] = os.environ.get(f'{cls.__env_prefix}_PROXY')
-
-        if f'{cls.__env_prefix}_ADAPTER_MODE' in os.environ.keys():
-            env_properties['adaptermode'] = os.environ.get(f'{cls.__env_prefix}_ADAPTER_MODE')
-
-        if f'{cls.__env_prefix}_CERT_VALIDATION' in os.environ.keys():
-            env_properties['certvalidation'] = os.environ.get(f'{cls.__env_prefix}_CERT_VALIDATION')
-
-        if f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES' in os.environ.keys():
-            env_properties['automaticcreationtestcases'] = os.environ.get(
-                f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
-
-        return env_properties
-
-    @staticmethod
-    def __check_properties(properties: dict):
-        adapter_mode = properties.get('adaptermode')
-
-        if adapter_mode == AdapterMode.NEW_TEST_RUN:
-            if properties.get('projectid') is None:
-                logging.error('Adapter mode "2" is enabled. The project ID is needed, but it was not found!')
-                raise SystemExit
-        elif adapter_mode in (
-                AdapterMode.RUN_ALL_TESTS,
-                AdapterMode.USE_FILTER,
-                None):
-            if properties.get('testrunid') is None:
-                logging.error(f'Adapter mode "{adapter_mode if adapter_mode else "0"}" is enabled. '
-                              f'The test run ID is needed, but it was not found!')
-                raise SystemExit
-        else:
-            logging.error(f'Unknown adapter mode "{adapter_mode}"!')
-            raise SystemExit
-
-        if properties.get('url') is None:
-            logging.error('URL was not found!')
-            raise SystemExit
-
-        if properties.get('privatetoken') is None:
-            logging.error('Private token was not found!')
-            raise SystemExit
-
-        if properties.get('configurationid') is None:
-            logging.error('Configuration ID was not found!')
-            raise SystemExit
-
-        if properties.get('certvalidation'):
-            properties['certvalidation'] = properties['certvalidation'].lower()
-
-        if properties.get('automaticcreationtestcases'):
-            properties['automaticcreationtestcases'] = properties['automaticcreationtestcases'].lower()
-
-    @staticmethod
-    def __search_in_environ(var_name: str):
-        if re.fullmatch(r'{[a-zA-Z_]\w*}', var_name) and var_name[1:-1] in os.environ:
-            return os.environ[var_name[1:-1]]
-
-        return var_name
+import configparser
+import logging
+import os
+import re
+import warnings
+
+from testgear_python_commons.models.adapter_mode import AdapterMode
+
+
+class AppProperties:
+    __properties_file = 'connection_config'
+    __env_prefix = 'TMS'
+
+    @staticmethod
+    def load_properties(option=None):
+        properties = AppProperties.load_file_properties(
+            option.set_config_file if hasattr(option, 'set_config_file') else None)
+
+        properties.update(AppProperties.load_env_properties())
+
+        if option:
+            properties.update(AppProperties.load_cli_properties(option))
+
+        AppProperties.__check_properties(properties)
+
+        return properties
+
+    @classmethod
+    def load_file_properties(cls, file_name: str = None):
+        properties = {}
+
+        path = os.path.abspath('')
+        root = path[:path.index(os.sep)]
+
+        if file_name:
+            cls.__properties_file = file_name
+
+        if os.environ.get(f'{cls.__env_prefix}_CONFIG_FILE'):
+            cls.__properties_file = os.environ.get(f'{cls.__env_prefix}_CONFIG_FILE')
+
+        while not os.path.isfile(
+                path + os.sep + f'{cls.__properties_file}.ini') and path != root:
+            path = path[:path.rindex(os.sep)]
+
+        path = path + os.sep + f'{cls.__properties_file}.ini'
+
+        if os.path.isfile(path):
+            parser = configparser.RawConfigParser()
+
+            parser.read(path)
+
+            if parser.has_section('testgear'):
+                for key, value in parser.items('testgear'):
+                    properties[key] = cls.__search_in_environ(value)
+
+            if parser.has_section('debug'):
+                if parser.has_option('debug', 'tmsproxy'):
+                    properties['tmsproxy'] = cls.__search_in_environ(
+                        parser.get('debug', 'tmsproxy'))
+
+                if parser.has_option('debug', '__dev'):
+                    properties['logs'] = cls.__search_in_environ(
+                        parser.get('debug', '__dev')).lower()
+
+            if 'privatetoken' in properties:
+                warnings.warn(
+                    'The configuration file specifies a private token. It is not safe.'
+                    ' Use TMS_PRIVATE_TOKEN environment variable',
+                    category=Warning,
+                    stacklevel=2)
+                warnings.simplefilter('default', Warning)
+
+        return properties
+
+    @staticmethod
+    def load_cli_properties(option):
+        cli_properties = {}
+
+        if hasattr(option, 'set_url') and option.set_url:
+            cli_properties['url'] = option.set_url
+
+        if hasattr(option, 'set_private_token') and option.set_private_token:
+            cli_properties['privatetoken'] = option.set_private_token
+
+        if hasattr(option, 'set_project_id') and option.set_project_id:
+            cli_properties['projectid'] = option.set_project_id
+
+        if hasattr(option, 'set_configuration_id') and option.set_configuration_id:
+            cli_properties['configurationid'] = option.set_configuration_id
+
+        if hasattr(option, 'set_test_run_id') and option.set_test_run_id:
+            cli_properties['testrunid'] = option.set_test_run_id
+
+        if hasattr(option, 'set_test_run_name') and option.set_test_run_name:
+            cli_properties['testrunname'] = option.set_test_run_name
+
+        if hasattr(option, 'set_tms_proxy') and option.set_tms_proxy:
+            cli_properties['tmsproxy'] = option.set_tms_proxy
+
+        if hasattr(option, 'set_adapter_mode') and option.set_adapter_mode:
+            cli_properties['adaptermode'] = option.set_adapter_mode
+
+        if hasattr(option, 'set_cert_validation') and option.set_cert_validation:
+            cli_properties['certvalidation'] = option.set_cert_validation
+
+        if hasattr(option, 'set_automatic_creation_test_cases') and option.set_automatic_creation_test_cases:
+            cli_properties['automaticcreationtestcases'] = option.set_automatic_creation_test_cases
+
+        return cli_properties
+
+    @classmethod
+    def load_env_properties(cls):
+        env_properties = {}
+
+        if f'{cls.__env_prefix}_URL' in os.environ.keys():
+            env_properties['url'] = os.environ.get(f'{cls.__env_prefix}_URL')
+
+        if f'{cls.__env_prefix}_PRIVATE_TOKEN' in os.environ.keys():
+            env_properties['privatetoken'] = os.environ.get(f'{cls.__env_prefix}_PRIVATE_TOKEN')
+
+        if f'{cls.__env_prefix}_PROJECT_ID' in os.environ.keys():
+            env_properties['projectid'] = os.environ.get(f'{cls.__env_prefix}_PROJECT_ID')
+
+        if f'{cls.__env_prefix}_CONFIGURATION_ID' in os.environ.keys():
+            env_properties['configurationid'] = os.environ.get(f'{cls.__env_prefix}_CONFIGURATION_ID')
+
+        if f'{cls.__env_prefix}_TEST_RUN_ID' in os.environ.keys():
+            env_properties['testrunid'] = os.environ.get(f'{cls.__env_prefix}_TEST_RUN_ID')
+
+        if f'{cls.__env_prefix}_TEST_RUN_NAME' in os.environ.keys():
+            env_properties['testrunname'] = os.environ.get(f'{cls.__env_prefix}_TEST_RUN_NAME')
+
+        if f'{cls.__env_prefix}_PROXY' in os.environ.keys():
+            env_properties['tmsproxy'] = os.environ.get(f'{cls.__env_prefix}_PROXY')
+
+        if f'{cls.__env_prefix}_ADAPTER_MODE' in os.environ.keys():
+            env_properties['adaptermode'] = os.environ.get(f'{cls.__env_prefix}_ADAPTER_MODE')
+
+        if f'{cls.__env_prefix}_CERT_VALIDATION' in os.environ.keys():
+            env_properties['certvalidation'] = os.environ.get(f'{cls.__env_prefix}_CERT_VALIDATION')
+
+        if f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES' in os.environ.keys():
+            env_properties['automaticcreationtestcases'] = os.environ.get(
+                f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
+
+        return env_properties
+
+    @staticmethod
+    def __check_properties(properties: dict):
+        adapter_mode = properties.get('adaptermode')
+
+        if adapter_mode == AdapterMode.NEW_TEST_RUN:
+            if properties.get('projectid') is None:
+                logging.error('Adapter mode "2" is enabled. The project ID is needed, but it was not found!')
+                raise SystemExit
+        elif adapter_mode in (
+                AdapterMode.RUN_ALL_TESTS,
+                AdapterMode.USE_FILTER,
+                None):
+            if properties.get('testrunid') is None:
+                logging.error(f'Adapter mode "{adapter_mode if adapter_mode else "0"}" is enabled. '
+                              f'The test run ID is needed, but it was not found!')
+                raise SystemExit
+        else:
+            logging.error(f'Unknown adapter mode "{adapter_mode}"!')
+            raise SystemExit
+
+        if properties.get('url') is None:
+            logging.error('URL was not found!')
+            raise SystemExit
+
+        if properties.get('privatetoken') is None:
+            logging.error('Private token was not found!')
+            raise SystemExit
+
+        if properties.get('configurationid') is None:
+            logging.error('Configuration ID was not found!')
+            raise SystemExit
+
+        if properties.get('certvalidation'):
+            properties['certvalidation'] = properties['certvalidation'].lower()
+
+        if properties.get('automaticcreationtestcases'):
+            properties['automaticcreationtestcases'] = properties['automaticcreationtestcases'].lower()
+
+    @staticmethod
+    def __search_in_environ(var_name: str):
+        if re.fullmatch(r'{[a-zA-Z_]\w*}', var_name) and var_name[1:-1] in os.environ:
+            return os.environ[var_name[1:-1]]
+
+        return var_name
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/client/api_client.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/client/api_client.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import logging
-import os
-from datetime import datetime
-
-from testgear_api_client import ApiClient, Configuration
-from testgear_api_client.apis import AttachmentsApi, AutoTestsApi, TestRunsApi
-from testgear_api_client.models import (
-    AttachmentPutModel,
-    WorkItemIdModel
-)
-
-from testgear_python_commons.client.client_configuration import ClientConfiguration
-from testgear_python_commons.client.converter import Converter
-from testgear_python_commons.services.logger import adapter_logger
-
-
-class ApiClientWorker:
-    def __init__(self, config: ClientConfiguration):
-        client_config = Configuration(host=config.get_url())
-
-        if config.get_cert_validation() == 'false':
-            client_config.verify_ssl = False
-
-        self.__api_client = ApiClient(
-            configuration=client_config,
-            header_name='Authorization',
-            header_value='PrivateToken ' + config.get_private_token()
-        )
-        self.__config = config
-
-    @adapter_logger
-    def create_test_run(self):
-        test_run_api = TestRunsApi(api_client=self.__api_client)
-
-        test_run_name = f'TestRun_{datetime.today().strftime("%Y-%m-%dT%H:%M:%S")}' if \
-            not self.__config.get_test_run_name() else self.__config.get_test_run_name()
-        model = Converter.test_run_to_test_run_short_model(
-            self.__config.get_project_id(),
-            test_run_name
-        )
-
-        response = test_run_api.create_empty(test_run_v2_post_short_model=model)
-
-        return Converter.get_id_from_create_test_run_response(response)
-
-    @adapter_logger
-    def set_test_run_id(self, test_run_id: str):
-        self.__config.set_test_run_id(test_run_id)
-
-    @adapter_logger
-    def get_autotests_by_test_run_id(self):
-        test_run_api = TestRunsApi(api_client=self.__api_client)
-
-        response = test_run_api.get_test_run_by_id(self.__config.get_test_run_id())
-
-        return Converter.get_resolved_autotests_from_get_test_run_response(
-            response,
-            self.__config.get_configuration_id())
-
-    @adapter_logger
-    def write_test(self, test_result: dict):
-        test_run_api = TestRunsApi(api_client=self.__api_client)
-        autotest_api = AutoTestsApi(api_client=self.__api_client)
-
-        autotest = autotest_api.get_all_auto_tests(project_id=self.__config.get_project_id(),
-                                                   external_id=test_result['externalID'])
-
-        if autotest:
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was found')
-
-            model = Converter.test_result_to_autotest_put_model(
-                test_result,
-                self.__config.get_project_id())
-
-            autotest_api.update_auto_test(auto_test_put_model=model)
-            autotest_global_id = autotest[0]['id']
-
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was updated')
-        else:
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was not found')
-
-            model = Converter.test_result_to_autotest_post_model(
-                test_result,
-                self.__config.get_project_id())
-
-            autotest_response = autotest_api.create_auto_test(auto_test_post_model=model)
-            autotest_global_id = autotest_response['id']
-
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was created')
-
-        if autotest_global_id:
-            for work_item_id in test_result['workItemsID']:
-                try:
-                    autotest_api.link_auto_test_to_work_item(
-                        autotest_global_id,
-                        work_item_id_model=WorkItemIdModel(id=work_item_id))
-
-                    logging.debug(f'Autotest "{test_result["autoTestName"]}" was linked with workItem "{work_item_id}"')
-                except Exception as exc:
-                    logging.error(f'Link with workItem "{work_item_id}" status: {exc.status}\n{exc.body}')
-
-        model = Converter.test_result_to_testrun_result_post_model(
-            test_result,
-            self.__config.get_configuration_id())
-
-        test_run_api.set_auto_test_results_for_test_run(
-            id=self.__config.get_test_run_id(),
-            auto_test_results_for_test_run_model=[model])
-
-        logging.debug(f'Result of the autotest "{test_result["autoTestName"]}" was set '
-                      f'in the test run "{self.__config.get_test_run_id()}"')
-
-    @adapter_logger
-    def load_attachments(self, attach_paths: list or tuple):
-        attachments_api = AttachmentsApi(api_client=self.__api_client)
-
-        attachments = []
-        for path in attach_paths:
-            if os.path.isfile(path):
-                try:
-                    attachment_response = attachments_api.api_v2_attachments_post(file=open(path, "rb"))
-
-                    attachments.append(AttachmentPutModel(attachment_response['id']))
-
-                    logging.debug(f'Attachment "{path}" was uploaded')
-                except Exception as exc:
-                    logging.error(f'Upload attachment "{path}" status: {exc.status}\n{exc.body}')
-            else:
-                logging.error(f'File "{path}" was not found!')
-        return attachments
+import logging
+import os
+from datetime import datetime
+
+from testgear_api_client import ApiClient, Configuration
+from testgear_api_client.apis import AttachmentsApi, AutoTestsApi, TestRunsApi
+from testgear_api_client.models import (
+    AttachmentPutModel,
+    WorkItemIdModel
+)
+
+from testgear_python_commons.client.client_configuration import ClientConfiguration
+from testgear_python_commons.client.converter import Converter
+from testgear_python_commons.services.logger import adapter_logger
+
+
+class ApiClientWorker:
+    def __init__(self, config: ClientConfiguration):
+        client_config = Configuration(host=config.get_url())
+
+        if config.get_cert_validation() == 'false':
+            client_config.verify_ssl = False
+
+        self.__api_client = ApiClient(
+            configuration=client_config,
+            header_name='Authorization',
+            header_value='PrivateToken ' + config.get_private_token()
+        )
+        self.__config = config
+
+    @adapter_logger
+    def create_test_run(self):
+        test_run_api = TestRunsApi(api_client=self.__api_client)
+
+        test_run_name = f'TestRun_{datetime.today().strftime("%Y-%m-%dT%H:%M:%S")}' if \
+            not self.__config.get_test_run_name() else self.__config.get_test_run_name()
+        model = Converter.test_run_to_test_run_short_model(
+            self.__config.get_project_id(),
+            test_run_name
+        )
+
+        response = test_run_api.create_empty(test_run_v2_post_short_model=model)
+
+        return Converter.get_id_from_create_test_run_response(response)
+
+    @adapter_logger
+    def set_test_run_id(self, test_run_id: str):
+        self.__config.set_test_run_id(test_run_id)
+
+    @adapter_logger
+    def get_autotests_by_test_run_id(self):
+        test_run_api = TestRunsApi(api_client=self.__api_client)
+
+        response = test_run_api.get_test_run_by_id(self.__config.get_test_run_id())
+
+        return Converter.get_resolved_autotests_from_get_test_run_response(
+            response,
+            self.__config.get_configuration_id())
+
+    @adapter_logger
+    def write_test(self, test_result: dict):
+        test_run_api = TestRunsApi(api_client=self.__api_client)
+        autotest_api = AutoTestsApi(api_client=self.__api_client)
+
+        autotest = autotest_api.get_all_auto_tests(project_id=self.__config.get_project_id(),
+                                                   external_id=test_result['externalID'])
+
+        if autotest:
+            logging.debug(f'Autotest "{test_result["autoTestName"]}" was found')
+
+            model = Converter.test_result_to_autotest_put_model(
+                test_result,
+                self.__config.get_project_id())
+
+            autotest_api.update_auto_test(auto_test_put_model=model)
+            autotest_global_id = autotest[0]['id']
+
+            logging.debug(f'Autotest "{test_result["autoTestName"]}" was updated')
+        else:
+            logging.debug(f'Autotest "{test_result["autoTestName"]}" was not found')
+
+            model = Converter.test_result_to_autotest_post_model(
+                test_result,
+                self.__config.get_project_id())
+
+            autotest_response = autotest_api.create_auto_test(auto_test_post_model=model)
+            autotest_global_id = autotest_response['id']
+
+            logging.debug(f'Autotest "{test_result["autoTestName"]}" was created')
+
+        if autotest_global_id:
+            for work_item_id in test_result['workItemsID']:
+                try:
+                    autotest_api.link_auto_test_to_work_item(
+                        autotest_global_id,
+                        work_item_id_model=WorkItemIdModel(id=work_item_id))
+
+                    logging.debug(f'Autotest "{test_result["autoTestName"]}" was linked with workItem "{work_item_id}"')
+                except Exception as exc:
+                    logging.error(f'Link with workItem "{work_item_id}" status: {exc.status}\n{exc.body}')
+
+        model = Converter.test_result_to_testrun_result_post_model(
+            test_result,
+            self.__config.get_configuration_id())
+
+        test_run_api.set_auto_test_results_for_test_run(
+            id=self.__config.get_test_run_id(),
+            auto_test_results_for_test_run_model=[model])
+
+        logging.debug(f'Result of the autotest "{test_result["autoTestName"]}" was set '
+                      f'in the test run "{self.__config.get_test_run_id()}"')
+
+    @adapter_logger
+    def load_attachments(self, attach_paths: list or tuple):
+        attachments_api = AttachmentsApi(api_client=self.__api_client)
+
+        attachments = []
+        for path in attach_paths:
+            if os.path.isfile(path):
+                try:
+                    attachment_response = attachments_api.api_v2_attachments_post(file=open(path, "rb"))
+
+                    attachments.append(AttachmentPutModel(attachment_response['id']))
+
+                    logging.debug(f'Attachment "{path}" was uploaded')
+                except Exception as exc:
+                    logging.error(f'Upload attachment "{path}" status: {exc.status}\n{exc.body}')
+            else:
+                logging.error(f'File "{path}" was not found!')
+        return attachments
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/client/converter.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/client/converter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-from testgear_api_client.models import (
-    AttachmentPutModelAutoTestStepResultsModel,
-    AutoTestPostModel,
-    AutoTestPutModel,
-    AutoTestResultsForTestRunModel,
-    AutoTestStepModel,
-    AvailableTestResultOutcome,
-    LinkPostModel,
-    LinkPutModel,
-    LinkType,
-    TestRunV2PostShortModel
-)
-
-from testgear_python_commons.services.logger import adapter_logger
-
-
-class Converter:
-    @classmethod
-    @adapter_logger
-    def test_run_to_test_run_short_model(cls, project_id, name):
-        return TestRunV2PostShortModel(
-            project_id=project_id,
-            name=name
-        )
-
-    @classmethod
-    @adapter_logger
-    def get_id_from_create_test_run_response(cls, response):
-        return response['id']
-
-    @classmethod
-    @adapter_logger
-    def get_resolved_autotests_from_get_test_run_response(cls, response, configuration: str):
-        autotests = response['_data_store']['test_results']
-
-        return cls.__get_resolved_autotests(autotests, configuration)
-
-    @staticmethod
-    @adapter_logger
-    def __get_resolved_autotests(autotests: list, configuration: str):
-        resolved_autotests = []
-
-        for autotest in autotests:
-            if configuration == autotest['_data_store']['configuration_id']:
-                resolved_autotests.append(autotest._data_store['auto_test']._data_store['external_id'])
-
-        return resolved_autotests
-
-    @classmethod
-    @adapter_logger
-    def test_result_to_autotest_post_model(
-            cls,
-            test_result: dict,
-            project_id: str):
-        return AutoTestPostModel(
-            test_result['externalID'],
-            project_id,
-            test_result['autoTestName'],
-            steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
-            setup=cls.step_results_to_autotest_steps_model(test_result['setUp']),
-            teardown=cls.step_results_to_autotest_steps_model(test_result['tearDown']),
-            namespace=test_result['namespace'],
-            classname=test_result['classname'],
-            title=test_result['title'],
-            description=test_result['description'],
-            links=cls.links_to_links_post_model(test_result['links']),
-            labels=test_result['labels'],
-            should_create_work_item=test_result['automaticCreationTestCases']
-        )
-
-    @classmethod
-    @adapter_logger
-    def test_result_to_autotest_put_model(
-            cls,
-            test_result: dict,
-            project_id: str):
-        if test_result['outcome'] == 'Passed':
-            return AutoTestPutModel(
-                test_result['externalID'],
-                project_id,
-                test_result['autoTestName'],
-                steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
-                setup=cls.step_results_to_autotest_steps_model(test_result['setUp']),
-                teardown=cls.step_results_to_autotest_steps_model(test_result['tearDown']),
-                namespace=test_result['namespace'],
-                classname=test_result['classname'],
-                title=test_result['title'],
-                description=test_result['description'],
-                links=cls.links_to_links_put_model(test_result['links']),
-                labels=test_result['labels']
-            )
-        else:
-            return AutoTestPutModel(
-                test_result['externalID'],
-                project_id,
-                test_result['autoTestName'],
-                steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
-                setup=cls.step_results_to_autotest_steps_model(test_result['setUp']),
-                teardown=cls.step_results_to_autotest_steps_model(test_result['tearDown']),
-                namespace=test_result['namespace'],
-                classname=test_result['classname'],
-                title=test_result['title'],
-                description=test_result['description'],
-                links=cls.links_to_links_put_model(test_result['links']),
-                labels=test_result['labels']
-            )
-
-    @classmethod
-    @adapter_logger
-    def test_result_to_testrun_result_post_model(
-            cls,
-            test_result: dict,
-            configuration_id: str):
-        return AutoTestResultsForTestRunModel(
-            configuration_id,
-            test_result['externalID'],
-            AvailableTestResultOutcome(test_result['outcome']),
-            step_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                test_result['stepResults']),
-            setup_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                test_result['setUpResults']),
-            teardown_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                test_result['tearDownResults']),
-            traces=test_result['traces'],
-            attachments=test_result['attachments'],
-            parameters=test_result['parameters'],
-            properties=test_result['properties'],
-            links=cls.links_to_links_post_model(test_result['resultLinks']),
-            duration=round(test_result['duration']),
-            message=test_result['message'],
-            started_on=test_result.get('started_on', None),
-            completed_on=test_result.get('completed_on', None)
-        )
-
-    @staticmethod
-    @adapter_logger
-    def link_to_link_post_model(
-            url: str,
-            title: str,
-            url_type: str,
-            description: str):
-        if url_type:
-            return LinkPostModel(
-                url,
-                title=title,
-                type=LinkType(value=url_type),
-                description=description
-            )
-        else:
-            return LinkPostModel(
-                url,
-                title=title,
-                description=description
-            )
-
-    @staticmethod
-    @adapter_logger
-    def link_to_link_put_model(
-            url: str,
-            title: str,
-            url_type: str,
-            description: str):
-        if url_type:
-            return LinkPutModel(
-                url,
-                title=title,
-                type=LinkType(value=url_type),
-                description=description
-            )
-        else:
-            return LinkPutModel(
-                url,
-                title=title,
-                description=description
-            )
-
-    @classmethod
-    @adapter_logger
-    def links_to_links_post_model(cls, links: list):
-        post_model_links = []
-
-        for link in links:
-            post_model_links.append(cls.link_to_link_post_model(
-                link['url'],
-                link.get('title', None),
-                link.get('type', None),
-                link.get('description', None)
-            ))
-
-        return post_model_links
-
-    @classmethod
-    @adapter_logger
-    def links_to_links_put_model(cls, links: list):
-        put_model_links = []
-
-        for link in links:
-            put_model_links.append(cls.link_to_link_put_model(
-                link['url'],
-                link.get('title', None),
-                link.get('type', None),
-                link.get('description', None)
-            ))
-
-        return put_model_links
-
-    @classmethod
-    @adapter_logger
-    def step_results_to_autotest_steps_model(cls, steps: list):
-        autotest_model_steps = []
-
-        for step in steps:
-            autotest_model_steps.append(
-                cls.step_result_to_autotest_step_model(
-                    step['title'],
-                    step['description'],
-                    cls.step_results_to_autotest_steps_model(
-                        step.get('steps', [])
-                    )
-                )
-            )
-
-        return autotest_model_steps
-
-    @staticmethod
-    @adapter_logger
-    def step_result_to_autotest_step_model(
-            title: str,
-            description: str = None,
-            steps: list = None):
-        return AutoTestStepModel(
-            title=title,
-            description=description,
-            steps=steps)
-
-    @classmethod
-    @adapter_logger
-    def step_results_to_attachment_put_model_autotest_step_results_model(cls, steps: list):
-        autotest_model_step_results = []
-
-        for step in steps:
-            autotest_model_step_results.append(
-                cls.step_result_to_attachment_put_model_autotest_step_results_model(
-                    step['title'],
-                    step['outcome'],
-                    step['description'],
-                    step['duration'],
-                    step['parameters'],
-                    step['attachments'],
-                    None,
-                    None,
-                    cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                        step.get('step_results', [])
-                    )
-                )
-            )
-
-        return autotest_model_step_results
-
-    @staticmethod
-    @adapter_logger
-    def step_result_to_attachment_put_model_autotest_step_results_model(
-            title: str,
-            outcome: str,
-            description: str = None,
-            duration: str = None,
-            parameters: list = None,
-            attachments: list = None,
-            started_on: str = None,
-            completed_on: str = None,
-            step_results: list = None):
-        return AttachmentPutModelAutoTestStepResultsModel(
-            title=title,
-            outcome=AvailableTestResultOutcome(outcome),
-            description=description,
-            duration=duration,
-            parameters=parameters,
-            attachments=attachments,
-            started_on=started_on,
-            completed_on=completed_on,
-            step_results=step_results
-        )
+from testgear_api_client.models import (
+    AttachmentPutModelAutoTestStepResultsModel,
+    AutoTestPostModel,
+    AutoTestPutModel,
+    AutoTestResultsForTestRunModel,
+    AutoTestStepModel,
+    AvailableTestResultOutcome,
+    LinkPostModel,
+    LinkPutModel,
+    LinkType,
+    TestRunV2PostShortModel
+)
+
+from testgear_python_commons.services.logger import adapter_logger
+
+
+class Converter:
+    @classmethod
+    @adapter_logger
+    def test_run_to_test_run_short_model(cls, project_id, name):
+        return TestRunV2PostShortModel(
+            project_id=project_id,
+            name=name
+        )
+
+    @classmethod
+    @adapter_logger
+    def get_id_from_create_test_run_response(cls, response):
+        return response['id']
+
+    @classmethod
+    @adapter_logger
+    def get_resolved_autotests_from_get_test_run_response(cls, response, configuration: str):
+        autotests = response['_data_store']['test_results']
+
+        return cls.__get_resolved_autotests(autotests, configuration)
+
+    @staticmethod
+    @adapter_logger
+    def __get_resolved_autotests(autotests: list, configuration: str):
+        resolved_autotests = []
+
+        for autotest in autotests:
+            if configuration == autotest['_data_store']['configuration_id']:
+                resolved_autotests.append(autotest._data_store['auto_test']._data_store['external_id'])
+
+        return resolved_autotests
+
+    @classmethod
+    @adapter_logger
+    def test_result_to_autotest_post_model(
+            cls,
+            test_result: dict,
+            project_id: str):
+        return AutoTestPostModel(
+            test_result['externalID'],
+            project_id,
+            test_result['autoTestName'],
+            steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
+            setup=cls.step_results_to_autotest_steps_model(test_result['setUp']),
+            teardown=cls.step_results_to_autotest_steps_model(test_result['tearDown']),
+            namespace=test_result['namespace'],
+            classname=test_result['classname'],
+            title=test_result['title'],
+            description=test_result['description'],
+            links=cls.links_to_links_post_model(test_result['links']),
+            labels=test_result['labels'],
+            should_create_work_item=test_result['automaticCreationTestCases']
+        )
+
+    @classmethod
+    @adapter_logger
+    def test_result_to_autotest_put_model(
+            cls,
+            test_result: dict,
+            project_id: str):
+        if test_result['outcome'] == 'Passed':
+            return AutoTestPutModel(
+                test_result['externalID'],
+                project_id,
+                test_result['autoTestName'],
+                steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
+                setup=cls.step_results_to_autotest_steps_model(test_result['setUp']),
+                teardown=cls.step_results_to_autotest_steps_model(test_result['tearDown']),
+                namespace=test_result['namespace'],
+                classname=test_result['classname'],
+                title=test_result['title'],
+                description=test_result['description'],
+                links=cls.links_to_links_put_model(test_result['links']),
+                labels=test_result['labels']
+            )
+        else:
+            return AutoTestPutModel(
+                test_result['externalID'],
+                project_id,
+                test_result['autoTestName'],
+                steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
+                setup=cls.step_results_to_autotest_steps_model(test_result['setUp']),
+                teardown=cls.step_results_to_autotest_steps_model(test_result['tearDown']),
+                namespace=test_result['namespace'],
+                classname=test_result['classname'],
+                title=test_result['title'],
+                description=test_result['description'],
+                links=cls.links_to_links_put_model(test_result['links']),
+                labels=test_result['labels']
+            )
+
+    @classmethod
+    @adapter_logger
+    def test_result_to_testrun_result_post_model(
+            cls,
+            test_result: dict,
+            configuration_id: str):
+        return AutoTestResultsForTestRunModel(
+            configuration_id,
+            test_result['externalID'],
+            AvailableTestResultOutcome(test_result['outcome']),
+            step_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                test_result['stepResults']),
+            setup_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                test_result['setUpResults']),
+            teardown_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                test_result['tearDownResults']),
+            traces=test_result['traces'],
+            attachments=test_result['attachments'],
+            parameters=test_result['parameters'],
+            properties=test_result['properties'],
+            links=cls.links_to_links_post_model(test_result['resultLinks']),
+            duration=round(test_result['duration']),
+            message=test_result['message'],
+            started_on=test_result.get('started_on', None),
+            completed_on=test_result.get('completed_on', None)
+        )
+
+    @staticmethod
+    @adapter_logger
+    def link_to_link_post_model(
+            url: str,
+            title: str,
+            url_type: str,
+            description: str):
+        if url_type:
+            return LinkPostModel(
+                url,
+                title=title,
+                type=LinkType(value=url_type),
+                description=description
+            )
+        else:
+            return LinkPostModel(
+                url,
+                title=title,
+                description=description
+            )
+
+    @staticmethod
+    @adapter_logger
+    def link_to_link_put_model(
+            url: str,
+            title: str,
+            url_type: str,
+            description: str):
+        if url_type:
+            return LinkPutModel(
+                url,
+                title=title,
+                type=LinkType(value=url_type),
+                description=description
+            )
+        else:
+            return LinkPutModel(
+                url,
+                title=title,
+                description=description
+            )
+
+    @classmethod
+    @adapter_logger
+    def links_to_links_post_model(cls, links: list):
+        post_model_links = []
+
+        for link in links:
+            post_model_links.append(cls.link_to_link_post_model(
+                link['url'],
+                link.get('title', None),
+                link.get('type', None),
+                link.get('description', None)
+            ))
+
+        return post_model_links
+
+    @classmethod
+    @adapter_logger
+    def links_to_links_put_model(cls, links: list):
+        put_model_links = []
+
+        for link in links:
+            put_model_links.append(cls.link_to_link_put_model(
+                link['url'],
+                link.get('title', None),
+                link.get('type', None),
+                link.get('description', None)
+            ))
+
+        return put_model_links
+
+    @classmethod
+    @adapter_logger
+    def step_results_to_autotest_steps_model(cls, steps: list):
+        autotest_model_steps = []
+
+        for step in steps:
+            autotest_model_steps.append(
+                cls.step_result_to_autotest_step_model(
+                    step['title'],
+                    step['description'],
+                    cls.step_results_to_autotest_steps_model(
+                        step.get('steps', [])
+                    )
+                )
+            )
+
+        return autotest_model_steps
+
+    @staticmethod
+    @adapter_logger
+    def step_result_to_autotest_step_model(
+            title: str,
+            description: str = None,
+            steps: list = None):
+        return AutoTestStepModel(
+            title=title,
+            description=description,
+            steps=steps)
+
+    @classmethod
+    @adapter_logger
+    def step_results_to_attachment_put_model_autotest_step_results_model(cls, steps: list):
+        autotest_model_step_results = []
+
+        for step in steps:
+            autotest_model_step_results.append(
+                cls.step_result_to_attachment_put_model_autotest_step_results_model(
+                    step['title'],
+                    step['outcome'],
+                    step['description'],
+                    step['duration'],
+                    step['parameters'],
+                    step['attachments'],
+                    None,
+                    None,
+                    cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                        step.get('step_results', [])
+                    )
+                )
+            )
+
+        return autotest_model_step_results
+
+    @staticmethod
+    @adapter_logger
+    def step_result_to_attachment_put_model_autotest_step_results_model(
+            title: str,
+            outcome: str,
+            description: str = None,
+            duration: str = None,
+            parameters: list = None,
+            attachments: list = None,
+            started_on: str = None,
+            completed_on: str = None,
+            step_results: list = None):
+        return AttachmentPutModelAutoTestStepResultsModel(
+            title=title,
+            outcome=AvailableTestResultOutcome(outcome),
+            description=description,
+            duration=duration,
+            parameters=parameters,
+            attachments=attachments,
+            started_on=started_on,
+            completed_on=completed_on,
+            step_results=step_results
+        )
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/decorators.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/decorators.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import logging
-import types
-from functools import wraps
-
-from testgear_python_commons.services.logger import adapter_logger
-from testgear_python_commons.services.utils import Utils
-
-
-def inner(function):
-    @wraps(function)
-    def wrapper(*args, **kwargs):
-        if not hasattr(function, 'test_properties') and kwargs:
-            function.test_properties = {}
-
-            for key, value in kwargs.items():
-                if hasattr(function,
-                           'callspec') and key not in function.callspec.params:
-                    function.test_properties[key] = str(value)
-        function(*args, **kwargs)
-
-    if isinstance(function, types.FunctionType):
-        return wrapper
-
-    return function
-
-
-@Utils.deprecated('Use "workItemIds" instead.')
-@adapter_logger
-def workItemID(*test_workitems_id: int or str):  # noqa: N802
-    def outer(function):
-        function.test_workitems_id = []
-        for test_workitem_id in test_workitems_id:
-            function.test_workitems_id.append(str(test_workitem_id))
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def workItemIds(*test_workitems_id: int or str):  # noqa: N802
-    def outer(function):  # noqa: N802
-        function.test_workitems_id = []
-        for test_workitem_id in test_workitems_id:
-            function.test_workitems_id.append(str(test_workitem_id))
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def displayName(test_displayname: str):  # noqa: N802
-    def outer(function):
-        function.test_displayname = test_displayname
-        return inner(function)
-
-    return outer
-
-
-def nameSpace(test_namespace: str):  # noqa: N802
-    def outer(function):
-        function.test_namespace = test_namespace
-        return inner(function)
-
-    return outer
-
-
-def className(test_classname: str):  # noqa: N802
-    def outer(function):
-        function.test_classname = test_classname
-        return inner(function)
-
-    return outer
-
-
-@Utils.deprecated('Use "externalId" instead.')
-@adapter_logger
-def externalID(test_external_id: str):  # noqa: N802
-    def outer(function):
-        function.test_external_id = test_external_id
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def externalId(test_external_id: str):  # noqa: N802
-    def outer(function):
-        function.test_external_id = test_external_id
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def title(test_title: str):
-    def outer(function):
-        function.test_title = test_title
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def description(test_description: str):
-    def outer(function):
-        function.test_description = test_description
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def labels(*test_labels: str):
-    def outer(function):
-        function.test_labels = test_labels
-        return inner(function)
-
-    return outer
-
-
-@Utils.deprecated('Use "links" instead.')
-@adapter_logger
-def link(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003
-    def outer(function):
-        if not hasattr(function, 'test_links'):
-            function.test_links = []
-        function.test_links.append({'url': url, 'title': title, 'type': type, 'description': description})
-        return inner(function)
-
-    return outer
-
-
-@adapter_logger
-def links(url: str = None, title: str = None, type: str = None,  # noqa: A002,VNE003
-          description: str = None, links: list or tuple = None):
-    def outer(function):
-        if not hasattr(function, 'test_links'):
-            function.test_links = []
-
-        if url:
-            function.test_links.append({'url': url, 'title': title, 'type': type, 'description': description})
-        elif links and (isinstance(links, list) or isinstance(links, tuple)):
-            for link in links:
-                if isinstance(link, dict) and 'url' in link:
-                    function.test_links.append(
-                        {'url': link['url'],
-                         'title': link['title'] if 'title' in link else None,
-                         'type': link['type'] if 'type' in link else None,
-                         'description': link['description'] if 'description' in link else None}
-                    )
-                else:
-                    logging.warning(f'Link ({link}) can\'t be processed!')
-        else:
-            logging.warning(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
-        return inner(function)
-
-    return outer
+import logging
+import types
+from functools import wraps
+
+from testgear_python_commons.services.logger import adapter_logger
+from testgear_python_commons.services.utils import Utils
+
+
+def inner(function):
+    @wraps(function)
+    def wrapper(*args, **kwargs):
+        if not hasattr(function, 'test_properties') and kwargs:
+            function.test_properties = {}
+
+            for key, value in kwargs.items():
+                if hasattr(function,
+                           'callspec') and key not in function.callspec.params:
+                    function.test_properties[key] = str(value)
+        function(*args, **kwargs)
+
+    if isinstance(function, types.FunctionType):
+        return wrapper
+
+    return function
+
+
+@Utils.deprecated('Use "workItemIds" instead.')
+@adapter_logger
+def workItemID(*test_workitems_id: int or str):  # noqa: N802
+    def outer(function):
+        function.test_workitems_id = []
+        for test_workitem_id in test_workitems_id:
+            function.test_workitems_id.append(str(test_workitem_id))
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def workItemIds(*test_workitems_id: int or str):  # noqa: N802
+    def outer(function):  # noqa: N802
+        function.test_workitems_id = []
+        for test_workitem_id in test_workitems_id:
+            function.test_workitems_id.append(str(test_workitem_id))
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def displayName(test_displayname: str):  # noqa: N802
+    def outer(function):
+        function.test_displayname = test_displayname
+        return inner(function)
+
+    return outer
+
+
+def nameSpace(test_namespace: str):  # noqa: N802
+    def outer(function):
+        function.test_namespace = test_namespace
+        return inner(function)
+
+    return outer
+
+
+def className(test_classname: str):  # noqa: N802
+    def outer(function):
+        function.test_classname = test_classname
+        return inner(function)
+
+    return outer
+
+
+@Utils.deprecated('Use "externalId" instead.')
+@adapter_logger
+def externalID(test_external_id: str):  # noqa: N802
+    def outer(function):
+        function.test_external_id = test_external_id
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def externalId(test_external_id: str):  # noqa: N802
+    def outer(function):
+        function.test_external_id = test_external_id
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def title(test_title: str):
+    def outer(function):
+        function.test_title = test_title
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def description(test_description: str):
+    def outer(function):
+        function.test_description = test_description
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def labels(*test_labels: str):
+    def outer(function):
+        function.test_labels = test_labels
+        return inner(function)
+
+    return outer
+
+
+@Utils.deprecated('Use "links" instead.')
+@adapter_logger
+def link(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003
+    def outer(function):
+        if not hasattr(function, 'test_links'):
+            function.test_links = []
+        function.test_links.append({'url': url, 'title': title, 'type': type, 'description': description})
+        return inner(function)
+
+    return outer
+
+
+@adapter_logger
+def links(url: str = None, title: str = None, type: str = None,  # noqa: A002,VNE003
+          description: str = None, links: list or tuple = None):
+    def outer(function):
+        if not hasattr(function, 'test_links'):
+            function.test_links = []
+
+        if url:
+            function.test_links.append({'url': url, 'title': title, 'type': type, 'description': description})
+        elif links and (isinstance(links, list) or isinstance(links, tuple)):
+            for link in links:
+                if isinstance(link, dict) and 'url' in link:
+                    function.test_links.append(
+                        {'url': link['url'],
+                         'title': link['title'] if 'title' in link else None,
+                         'type': link['type'] if 'type' in link else None,
+                         'description': link['description'] if 'description' in link else None}
+                    )
+                else:
+                    logging.warning(f'Link ({link}) can\'t be processed!')
+        else:
+            logging.warning(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
+        return inner(function)
+
+    return outer
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/dynamic_methods.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/dynamic_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,103 @@
-import logging
-
-from testgear_python_commons.services import TmsPluginManager
-from testgear_python_commons.services.logger import adapter_logger
-from testgear_python_commons.services.utils import Utils
-from testgear_python_commons.step import Step
-
-
-@Utils.deprecated('Use "addLinks" instead.')
-@adapter_logger
-def addLink(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003,N802
-    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
-        TmsPluginManager.get_plugin_manager().hook \
-            .add_link(
-            link={
-                "url": url,
-                "title": title,
-                "type": type,
-                "description": description
-            }
-        )
-
-
-@adapter_logger
-def addLinks(url: str = None, title: str = None, type: str = None, description: str = None,  # noqa: A002,VNE003,N802
-             links: list or tuple = None):
-    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
-        if url:
-            TmsPluginManager.get_plugin_manager().hook \
-                .add_link(
-                link={
-                    "url": url,
-                    "title": title,
-                    "type": type,
-                    "description": description
-                }
-            )
-        elif links and (isinstance(links, list) or isinstance(links, tuple)):
-            for link in links:
-                if isinstance(link, dict) and 'url' in link:
-                    TmsPluginManager.get_plugin_manager().hook \
-                        .add_link(link=link)
-                else:
-                    logging.warning(f'Link ({link}) can\'t be processed!')
-        else:
-            logging.warning("Links can't be processed!\nPlease, set 'url' or 'links'!")
-
-
-@Utils.deprecated('Use "addMessage" instead.')
-@adapter_logger
-def message(test_message: str):
-    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_message'):
-        TmsPluginManager.get_plugin_manager().hook \
-            .add_message(test_message=test_message)
-
-
-@adapter_logger
-def addMessage(test_message: str):   # noqa: N802
-    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_message'):
-        TmsPluginManager.get_plugin_manager().hook \
-            .add_message(test_message=test_message)
-
-
-@Utils.deprecated('Use "addAttachments" instead.')
-@adapter_logger
-def attachments(*attachments_paths):
-    if Step.step_is_active():
-        Step.add_attachments(attachments_paths)
-    else:
-        if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
-            TmsPluginManager.get_plugin_manager().hook \
-                .add_attachments(attach_paths=attachments_paths)
-
-
-@adapter_logger
-def addAttachments(data, is_text: bool = False, name: str = None):   # noqa: N802
-    if Step.step_is_active():
-        if is_text:
-            Step.create_attachment(
-                str(data),
-                name)
-        else:
-            if isinstance(data, str):
-                Step.add_attachments([data])
-            elif isinstance(data, tuple) or isinstance(data, list):
-                Step.add_attachments(data)
-            else:
-                logging.warning(f'File ({data}) not found!')
-    else:
-        if is_text and hasattr(TmsPluginManager.get_plugin_manager().hook, 'create_attachment'):
-            Step.create_attachment(str(data), name)
-            TmsPluginManager.get_plugin_manager().hook \
-                .create_attachment(
-                body=str(data),
-                name=name)
-        elif hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
-            if isinstance(data, str):
-                TmsPluginManager.get_plugin_manager().hook \
-                    .add_attachments(attach_paths=[data])
-            elif isinstance(data, tuple) or isinstance(data, list):
-                TmsPluginManager.get_plugin_manager().hook \
-                    .add_attachments(attach_paths=data)
-            else:
-                logging.warning(f'({data}) is not path!')
+import logging
+
+from testgear_python_commons.services import TmsPluginManager
+from testgear_python_commons.services.logger import adapter_logger
+from testgear_python_commons.services.utils import Utils
+from testgear_python_commons.step import Step
+
+
+@Utils.deprecated('Use "addLinks" instead.')
+@adapter_logger
+def addLink(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003,N802
+    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
+        TmsPluginManager.get_plugin_manager().hook \
+            .add_link(
+            link={
+                "url": url,
+                "title": title,
+                "type": type,
+                "description": description
+            }
+        )
+
+
+@adapter_logger
+def addLinks(url: str = None, title: str = None, type: str = None, description: str = None,  # noqa: A002,VNE003,N802
+             links: list or tuple = None):
+    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
+        if url:
+            TmsPluginManager.get_plugin_manager().hook \
+                .add_link(
+                link={
+                    "url": url,
+                    "title": title,
+                    "type": type,
+                    "description": description
+                }
+            )
+        elif links and (isinstance(links, list) or isinstance(links, tuple)):
+            for link in links:
+                if isinstance(link, dict) and 'url' in link:
+                    TmsPluginManager.get_plugin_manager().hook \
+                        .add_link(link=link)
+                else:
+                    logging.warning(f'Link ({link}) can\'t be processed!')
+        else:
+            logging.warning("Links can't be processed!\nPlease, set 'url' or 'links'!")
+
+
+@Utils.deprecated('Use "addMessage" instead.')
+@adapter_logger
+def message(test_message: str):
+    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_message'):
+        TmsPluginManager.get_plugin_manager().hook \
+            .add_message(test_message=test_message)
+
+
+@adapter_logger
+def addMessage(test_message: str):   # noqa: N802
+    if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_message'):
+        TmsPluginManager.get_plugin_manager().hook \
+            .add_message(test_message=test_message)
+
+
+@Utils.deprecated('Use "addAttachments" instead.')
+@adapter_logger
+def attachments(*attachments_paths):
+    if Step.step_is_active():
+        Step.add_attachments(attachments_paths)
+    else:
+        if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
+            TmsPluginManager.get_plugin_manager().hook \
+                .add_attachments(attach_paths=attachments_paths)
+
+
+@adapter_logger
+def addAttachments(data, is_text: bool = False, name: str = None):   # noqa: N802
+    if Step.step_is_active():
+        if is_text:
+            Step.create_attachment(
+                str(data),
+                name)
+        else:
+            if isinstance(data, str):
+                Step.add_attachments([data])
+            elif isinstance(data, tuple) or isinstance(data, list):
+                Step.add_attachments(data)
+            else:
+                logging.warning(f'File ({data}) not found!')
+    else:
+        if is_text and hasattr(TmsPluginManager.get_plugin_manager().hook, 'create_attachment'):
+            TmsPluginManager.get_plugin_manager().hook \
+                .create_attachment(
+                body=str(data),
+                name=name)
+        elif hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
+            if isinstance(data, str):
+                TmsPluginManager.get_plugin_manager().hook \
+                    .add_attachments(attach_paths=[data])
+            elif isinstance(data, tuple) or isinstance(data, list):
+                TmsPluginManager.get_plugin_manager().hook \
+                    .add_attachments(attach_paths=data)
+            else:
+                logging.warning(f'({data}) is not path!')
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/services/adapter_manager.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import os
-import uuid
-
-from testgear_python_commons.client.api_client import ApiClientWorker
-from testgear_python_commons.client.client_configuration import ClientConfiguration
-from testgear_python_commons.models.adapter_mode import AdapterMode
-from testgear_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
-from testgear_python_commons.services.logger import adapter_logger
-
-
-class AdapterManager:
-    def __init__(
-            self,
-            adapter_configuration: AdapterManagerConfiguration,
-            client_configuration: ClientConfiguration):
-        self.__config = adapter_configuration
-        self.__api_client = ApiClientWorker(client_configuration)
-
-    @adapter_logger
-    def set_test_run_id(self, test_run_id: str):
-        self.__config.set_test_run_id(test_run_id)
-        self.__api_client.set_test_run_id(test_run_id)
-
-    @adapter_logger
-    def get_test_run_id(self):
-        if self.__config.get_mode() != AdapterMode.NEW_TEST_RUN:
-            return self.__config.get_test_run_id()
-
-        return self.__api_client.create_test_run()
-
-    @adapter_logger
-    def get_autotests_for_launch(self):
-        if self.__config.get_mode() == AdapterMode.USE_FILTER:
-            return self.__api_client.get_autotests_by_test_run_id()
-
-        return
-
-    @adapter_logger
-    def write_test(self, test: dict):
-        test['automaticCreationTestCases'] = self.__config.should_automatic_creation_test_cases()
-        self.__api_client.write_test(test)
-
-    @adapter_logger
-    def load_attachments(self, attach_paths: list or tuple):
-        return self.__api_client.load_attachments(attach_paths)
-
-    @adapter_logger
-    def create_attachment(self, body: str, name: str):
-        if name is None:
-            name = str(uuid.uuid4()) + '-attachment.txt'
-
-        path = os.path.join(os.path.abspath(''), name)
-
-        with open(path, 'wb') as attached_file:
-            attached_file.write(body.encode('utf-8'))
-
-        attachment_id = self.__api_client.load_attachments((path,))
-
-        os.remove(path)
-
-        return attachment_id
+import os
+import uuid
+
+from testgear_python_commons.client.api_client import ApiClientWorker
+from testgear_python_commons.client.client_configuration import ClientConfiguration
+from testgear_python_commons.models.adapter_mode import AdapterMode
+from testgear_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
+from testgear_python_commons.services.logger import adapter_logger
+
+
+class AdapterManager:
+    def __init__(
+            self,
+            adapter_configuration: AdapterManagerConfiguration,
+            client_configuration: ClientConfiguration):
+        self.__config = adapter_configuration
+        self.__api_client = ApiClientWorker(client_configuration)
+
+    @adapter_logger
+    def set_test_run_id(self, test_run_id: str):
+        self.__config.set_test_run_id(test_run_id)
+        self.__api_client.set_test_run_id(test_run_id)
+
+    @adapter_logger
+    def get_test_run_id(self):
+        if self.__config.get_mode() != AdapterMode.NEW_TEST_RUN:
+            return self.__config.get_test_run_id()
+
+        return self.__api_client.create_test_run()
+
+    @adapter_logger
+    def get_autotests_for_launch(self):
+        if self.__config.get_mode() == AdapterMode.USE_FILTER:
+            return self.__api_client.get_autotests_by_test_run_id()
+
+        return
+
+    @adapter_logger
+    def write_test(self, test: dict):
+        test['automaticCreationTestCases'] = self.__config.should_automatic_creation_test_cases()
+        self.__api_client.write_test(test)
+
+    @adapter_logger
+    def load_attachments(self, attach_paths: list or tuple):
+        return self.__api_client.load_attachments(attach_paths)
+
+    @adapter_logger
+    def create_attachment(self, body: str, name: str):
+        if name is None:
+            name = str(uuid.uuid4()) + '-attachment.txt'
+
+        path = os.path.join(os.path.abspath(''), name)
+
+        with open(path, 'wb') as attached_file:
+            attached_file.write(body.encode('utf-8'))
+
+        attachment_id = self.__api_client.load_attachments((path,))
+
+        os.remove(path)
+
+        return attachment_id
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/services/adapter_manager_configuration.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/services/adapter_manager_configuration.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from testgear_python_commons.models.adapter_mode import AdapterMode
-from testgear_python_commons.services.logger import adapter_logger
-from testgear_python_commons.services.utils import Utils
-
-
-class AdapterManagerConfiguration:
-    __test_run_id = None
-
-    def __init__(self, app_properties: dict):
-        if app_properties.get('testrunid'):
-            self.__test_run_id = Utils.uuid_check(app_properties.get('testrunid'))
-
-        self.__adapter_mode = app_properties.get('adaptermode', AdapterMode.USE_FILTER)
-
-        __automatic_creation_test_cases = app_properties.get('automaticcreationtestcases')
-
-        if __automatic_creation_test_cases and __automatic_creation_test_cases == 'true':
-            self.__automatic_creation_test_cases = True
-        else:
-            self.__automatic_creation_test_cases = False
-
-    @adapter_logger
-    def get_test_run_id(self):
-        return self.__test_run_id
-
-    @adapter_logger
-    def set_test_run_id(self, test_run_id: str):
-        self.__test_run_id = test_run_id
-
-    @adapter_logger
-    def get_mode(self):
-        return self.__adapter_mode
-
-    @adapter_logger
-    def should_automatic_creation_test_cases(self):
-        return self.__automatic_creation_test_cases
+from testgear_python_commons.models.adapter_mode import AdapterMode
+from testgear_python_commons.services.logger import adapter_logger
+from testgear_python_commons.services.utils import Utils
+
+
+class AdapterManagerConfiguration:
+    __test_run_id = None
+
+    def __init__(self, app_properties: dict):
+        if app_properties.get('testrunid'):
+            self.__test_run_id = Utils.uuid_check(app_properties.get('testrunid'))
+
+        self.__adapter_mode = app_properties.get('adaptermode', AdapterMode.USE_FILTER)
+
+        __automatic_creation_test_cases = app_properties.get('automaticcreationtestcases')
+
+        if __automatic_creation_test_cases and __automatic_creation_test_cases == 'true':
+            self.__automatic_creation_test_cases = True
+        else:
+            self.__automatic_creation_test_cases = False
+
+    @adapter_logger
+    def get_test_run_id(self):
+        return self.__test_run_id
+
+    @adapter_logger
+    def set_test_run_id(self, test_run_id: str):
+        self.__test_run_id = test_run_id
+
+    @adapter_logger
+    def get_mode(self):
+        return self.__adapter_mode
+
+    @adapter_logger
+    def should_automatic_creation_test_cases(self):
+        return self.__automatic_creation_test_cases
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/services/logger.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/services/logger.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import inspect
-from functools import wraps
-
-from testgear_python_commons.services.plugin_manager import TmsPluginManager
-
-
-def adapter_logger(function):
-    @wraps(function)
-    def wrapper(*args, **kwargs):
-        logger = TmsPluginManager.get_logger()
-
-        parameters = get_function_parameters(function, *args, **kwargs)
-
-        message = f'Method "{function.__name__}" started'
-
-        if parameters:
-            message += f' with parameters: {parameters}'
-
-        logger.debug(message)
-
-        result = function(*args, **kwargs)
-
-        message = f'Method "{function.__name__}" finished'
-
-        if result:
-            message += f' with result: {result}'
-
-        logger.debug(message)
-
-        return result
-    return wrapper
-
-
-def get_function_parameters(function, *args, **kwargs):
-    parameters = {}
-    args_default_values = inspect.getfullargspec(function).defaults
-
-    if args or args_default_values:
-        all_keys = inspect.getfullargspec(function).args
-        all_args = list(args)
-
-        if args_default_values:
-            all_args += list(args_default_values[len(args) - (len(all_keys) - len(args_default_values)):])
-
-        method_args = [arg_name for arg_name in all_keys if arg_name not in list(kwargs)]
-
-        if len(method_args) == len(all_args):
-            for index in range(0, len(method_args)):
-                parameters[method_args[index]] = str(all_args[index])
-
-    if kwargs:
-        for key, parameter in kwargs.items():
-            parameters[key] = str(parameter)
-
-    return parameters
+import inspect
+from functools import wraps
+
+from testgear_python_commons.services.plugin_manager import TmsPluginManager
+
+
+def adapter_logger(function):
+    @wraps(function)
+    def wrapper(*args, **kwargs):
+        logger = TmsPluginManager.get_logger()
+
+        parameters = get_function_parameters(function, *args, **kwargs)
+
+        message = f'Method "{function.__name__}" started'
+
+        if parameters:
+            message += f' with parameters: {parameters}'
+
+        logger.debug(message)
+
+        result = function(*args, **kwargs)
+
+        message = f'Method "{function.__name__}" finished'
+
+        if result:
+            message += f' with result: {result}'
+
+        logger.debug(message)
+
+        return result
+    return wrapper
+
+
+def get_function_parameters(function, *args, **kwargs):
+    parameters = {}
+    args_default_values = inspect.getfullargspec(function).defaults
+
+    if args or args_default_values:
+        all_keys = inspect.getfullargspec(function).args
+        all_args = list(args)
+
+        if args_default_values:
+            all_args += list(args_default_values[len(args) - (len(all_keys) - len(args_default_values)):])
+
+        method_args = [arg_name for arg_name in all_keys if arg_name not in list(kwargs)]
+
+        if len(method_args) == len(all_args):
+            for index in range(0, len(method_args)):
+                parameters[method_args[index]] = str(all_args[index])
+
+    if kwargs:
+        for key, parameter in kwargs.items():
+            parameters[key] = str(parameter)
+
+    return parameters
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons/services/plugin_manager.py` & `testgear-python-commons-2.1.3/src/testgear_python_commons/services/plugin_manager.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import logging
-
-from pluggy import PluginManager
-
-from testgear_python_commons.app_properties import AppProperties
-
-
-class TmsPluginManager:
-    __plugin_manager = None
-    __adapter_manager = None
-    __logger = None
-
-    @classmethod
-    def get_plugin_manager(cls):
-        if cls.__plugin_manager is None:
-            cls.__plugin_manager = PluginManager('testgear')
-
-        return cls.__plugin_manager
-
-    @classmethod
-    def get_adapter_manager(cls, option=None):
-        if cls.__adapter_manager is None:
-            from testgear_python_commons.services.adapter_manager import AdapterManager
-            from testgear_python_commons.client.client_configuration import ClientConfiguration
-            from testgear_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
-
-            app_properties = AppProperties.load_properties(option)
-
-            cls.get_logger(app_properties.get('logs') == 'true')
-
-            client_configuration = ClientConfiguration(app_properties)
-            adapter_configuration = AdapterManagerConfiguration(app_properties)
-
-            cls.__adapter_manager = AdapterManager(adapter_configuration, client_configuration)
-
-        return cls.__adapter_manager
-
-    @classmethod
-    def get_logger(cls, debug: bool = False):
-        if cls.__logger is None:
-            if debug:
-                logging.basicConfig(format='\n%(levelname)s (%(asctime)s): %(message)s', level=logging.DEBUG)
-
-            cls.__logger = logging.getLogger('TmsLogger')
-
-        return cls.__logger
-
-    @classmethod
-    def __getattr__(cls, attribute):
-        return getattr(cls.get_plugin_manager(), attribute)
+import logging
+
+from pluggy import PluginManager
+
+from testgear_python_commons.app_properties import AppProperties
+
+
+class TmsPluginManager:
+    __plugin_manager = None
+    __adapter_manager = None
+    __logger = None
+
+    @classmethod
+    def get_plugin_manager(cls):
+        if cls.__plugin_manager is None:
+            cls.__plugin_manager = PluginManager('testgear')
+
+        return cls.__plugin_manager
+
+    @classmethod
+    def get_adapter_manager(cls, option=None):
+        if cls.__adapter_manager is None:
+            from testgear_python_commons.services.adapter_manager import AdapterManager
+            from testgear_python_commons.client.client_configuration import ClientConfiguration
+            from testgear_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
+
+            app_properties = AppProperties.load_properties(option)
+
+            cls.get_logger(app_properties.get('logs') == 'true')
+
+            client_configuration = ClientConfiguration(app_properties)
+            adapter_configuration = AdapterManagerConfiguration(app_properties)
+
+            cls.__adapter_manager = AdapterManager(adapter_configuration, client_configuration)
+
+        return cls.__adapter_manager
+
+    @classmethod
+    def get_logger(cls, debug: bool = False):
+        if cls.__logger is None:
+            if debug:
+                logging.basicConfig(format='\n%(levelname)s (%(asctime)s): %(message)s', level=logging.DEBUG)
+
+            cls.__logger = logging.getLogger('TmsLogger')
+
+        return cls.__logger
+
+    @classmethod
+    def __getattr__(cls, attribute):
+        return getattr(cls.get_plugin_manager(), attribute)
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/PKG-INFO` & `testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: testgear-python-commons
-Version: 2.1.2
-Summary: Python commons for Test Gear
-Home-page: https://github.com/testgear-tms/adapters-python/
-Author: Integration team
-Author-email: integrations@test-gear.io
-License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Metadata-Version: 2.1
+Name: testgear-python-commons
+Version: 2.1.3
+Summary: Python commons for Test Gear
+Home-page: https://github.com/testgear-tms/adapters-python/
+Author: Integration team
+Author-email: integrations@test-gear.io
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `testgear-python-commons-2.1.2/src/testgear_python_commons.egg-info/SOURCES.txt` & `testgear-python-commons-2.1.3/src/testgear_python_commons.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-requirements.txt
 setup.py
 src/testgear.py
 src/testgear_python_commons/__init__.py
 src/testgear_python_commons/app_properties.py
 src/testgear_python_commons/decorators.py
 src/testgear_python_commons/dynamic_methods.py
 src/testgear_python_commons/step.py
```


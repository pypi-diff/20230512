# Comparing `tmp/testit-adapter-pytest-2.1.7.tar.gz` & `tmp/testit-adapter-pytest-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-pytest-2.1.7.tar", last modified: Fri Apr 21 08:18:20 2023, max compression
+gzip compressed data, was "testit-adapter-pytest-2.1.8.tar", last modified: Fri May 12 08:34:58 2023, max compression
```

## Comparing `testit-adapter-pytest-2.1.7.tar` & `testit-adapter-pytest-2.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:20.525452 testit-adapter-pytest-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-21 08:18:20.521452 testit-adapter-pytest-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-21 08:17:56.000000 testit-adapter-pytest-2.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:18:20.525452 testit-adapter-pytest-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-21 08:17:56.000000 testit-adapter-pytest-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:20.521452 testit-adapter-pytest-2.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:20.521452 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-21 08:17:56.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-21 08:17:56.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:20.521452 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-21 08:18:20.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-21 08:18:20.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:18:20.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 08:18:20.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 08:18:20.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 08:18:20.000000 testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit-adapter-pytest-2.1.7/PKG-INFO` & `testit-adapter-pytest-2.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: testit-adapter-pytest
-Version: 2.1.7
-Summary: Pytest adapter for Test IT
-Home-page: https://github.com/testit-tms/adapters-python/
-Author: Integration team
-Author-email: integrations@testit.software
-License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
@@ -25,146 +10,60 @@
 pip install testit-adapter-pytest
 ```
 
 ## Usage
 
 ### Configuration
 
-#### File
-
-1. Create **connection_config.ini** file in the root directory of the project:
-    ```
-    [testit]
-    URL = <url>
-    privateToken = <token>
-    projectId = <id>
-    configurationId = <id>
-    testRunId = <optional id>
-    testRunName = <optional name>
-    adapterMode = <optional>
-    certValidation = <optional boolean>
-    automaticCreationTestCases = <optional boolean>
-    
-    # This section are optional. It enables debug mode.
-    [debug]
-    tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
-    ```
-
-2. Fill parameters with your configuration, where:
-    * `URL` - location of the TMS instance
-
-    * `privateToken` - API secret key
-        1. go to the https://{DOMAIN}/user-profile profile
-        2. copy the API secret key
-
-    * `projectId` - ID of project in TMS instance.
-
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request project, Preview tab, copy id field
-
-    * `configurationId` - ID of configuration in TMS instance.
-
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request configurations, Preview tab, copy id field
-
-    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
-      created automatically.
-
-    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
-      not provided, it is created automatically.
-
-    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
-
-        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
-          test run.
-        * 1 - in this mode, the adapter sends all results to the test run without filtering.
-        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-    
-    * `certValidation` - it enables/disables certificate validation. Default value - true.
-
-    * `automaticCreationTestCases` - mode of automatic creation test cases. Default value - false. The adapter supports following modes:
-        * true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest).
-        * false - in this mode, the adapter will not create a test case.
-
-    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-#### ENV
-
-You can use environment variables (environment variables take precedence over file variables):
-
-* `TMS_URL` - location of the TMS instance.
-
-* `TMS_PRIVATE_TOKEN` - API secret key.
-
-* `TMS_PROJECT_ID` - ID of a project in TMS instance.
-
-* `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
+| Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
+| Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
+| API secret key [How to getting API secret key?](https://github.com/testit-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                            | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
+| ID of project in TMS instance [How to getting project ID?](https://github.com/testit-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                    | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
+| ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testit-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                  | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
+| ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
+| Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
+| Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
+| It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
+| Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
+| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
 
-* `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
-
-* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
-  it is created automatically.
-
-* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
-  automatically.
-
-* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
-  default file name.
-
-* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. Default value - true.
-
-* `TMS_AUTOMATIC_CREATION_TEST_CASES` - mode of automatic creation test cases. Default value - false.
-
-#### Command line
-
-You also can CLI variables (CLI variables take precedence over environment variables):
-
-* `tmsUrl` - location of the TMS instance.
-
-* `tmsPrivateToken` - API secret key.
-
-* `tmsProjectId` - ID of a project in TMS instance.
-
-* `tmsConfigurationId` - ID of a configuration in TMS instance.
-
-* `tmsAdapterMode` - adapter mode. Default value - 0.
-
-* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
-  created automatically.
-
-* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
-  automatically.
-
-* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
-  default file name.
-
-* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-* `tmsCertValidation` - it enables/disables certificate validation. Default value - true.
+#### File
 
-* `tmsAutomaticCreationTestCases` - mode of automatic creation test cases. Default value - false.
+Create **connection_config.ini** file in the root directory of the project:
+```
+[testit]
+URL = URL
+privateToken = USER_PRIVATE_TOKEN
+projectId = PROJECT_ID
+configurationId = CONFIGURATION_ID
+testRunId = TEST_RUN_ID
+testRunName = TEST_RUN_NAME
+adapterMode = ADAPTER_MODE
+certValidation = CERT_VALIDATION
+automaticCreationTestCases = AUTOMATIC_CREATION_TEST_CASES
+
+# This section are optional. It enables debug mode.
+[debug]
+tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+```
 
 #### Examples
 
 Launch with a connection_config.ini file in the root directory of the project:
 
 ```
 $ pytest --testit
 ```
 
 Launch with command-line parameters:
 
 ```
-$ pytest --testit --tmsUrl=<url> --tmsPrivateToken=<token> --tmsProjectId=<id> --tmsConfigurationId=<id> --tmsTestRunId=<optional id> --tmsTestRunName=<optional name> --tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' --tmsCertValidation=<optional boolean> --tmsAutomaticCreationTestCases=<optional boolean>
+$ pytest --testit --tmsUrl=URL --tmsPrivateToken=USER_PRIVATE_TOKEN --tmsProjectId=PROJECT_ID --tmsConfigurationId=CONFIGURATION_ID --tmsTestRunId=TEST_RUN_ID --tmsTestRunName=TEST_RUN_NAME --tmsAdapterMode=ADAPTER_MODE --tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' --tmsCertValidation=CERT_VALIDATION --tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
 ```
 
 If you want to enable debug mode then
 see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Decorators
```

### Comparing `testit-adapter-pytest-2.1.7/README.md` & `testit-adapter-pytest-2.1.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: testit-adapter-pytest
+Version: 2.1.8
+Summary: Pytest adapter for Test IT
+Home-page: https://github.com/testit-tms/adapters-python/
+Author: Integration team
+Author-email: integrations@testit.software
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
@@ -10,146 +25,60 @@
 pip install testit-adapter-pytest
 ```
 
 ## Usage
 
 ### Configuration
 
-#### File
-
-1. Create **connection_config.ini** file in the root directory of the project:
-    ```
-    [testit]
-    URL = <url>
-    privateToken = <token>
-    projectId = <id>
-    configurationId = <id>
-    testRunId = <optional id>
-    testRunName = <optional name>
-    adapterMode = <optional>
-    certValidation = <optional boolean>
-    automaticCreationTestCases = <optional boolean>
-    
-    # This section are optional. It enables debug mode.
-    [debug]
-    tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
-    ```
-
-2. Fill parameters with your configuration, where:
-    * `URL` - location of the TMS instance
-
-    * `privateToken` - API secret key
-        1. go to the https://{DOMAIN}/user-profile profile
-        2. copy the API secret key
-
-    * `projectId` - ID of project in TMS instance.
-
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request project, Preview tab, copy id field
-
-    * `configurationId` - ID of configuration in TMS instance.
-
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request configurations, Preview tab, copy id field
-
-    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
-      created automatically.
-
-    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
-      not provided, it is created automatically.
-
-    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
-
-        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
-          test run.
-        * 1 - in this mode, the adapter sends all results to the test run without filtering.
-        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-    
-    * `certValidation` - it enables/disables certificate validation. Default value - true.
-
-    * `automaticCreationTestCases` - mode of automatic creation test cases. Default value - false. The adapter supports following modes:
-        * true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest).
-        * false - in this mode, the adapter will not create a test case.
-
-    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-#### ENV
-
-You can use environment variables (environment variables take precedence over file variables):
-
-* `TMS_URL` - location of the TMS instance.
-
-* `TMS_PRIVATE_TOKEN` - API secret key.
-
-* `TMS_PROJECT_ID` - ID of a project in TMS instance.
-
-* `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
+| Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
+| Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
+| API secret key [How to getting API secret key?](https://github.com/testit-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                            | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
+| ID of project in TMS instance [How to getting project ID?](https://github.com/testit-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                    | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
+| ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testit-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                  | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
+| ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
+| Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
+| Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
+| It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
+| Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
+| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
 
-* `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
-
-* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
-  it is created automatically.
-
-* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
-  automatically.
-
-* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
-  default file name.
-
-* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. Default value - true.
-
-* `TMS_AUTOMATIC_CREATION_TEST_CASES` - mode of automatic creation test cases. Default value - false.
-
-#### Command line
-
-You also can CLI variables (CLI variables take precedence over environment variables):
-
-* `tmsUrl` - location of the TMS instance.
-
-* `tmsPrivateToken` - API secret key.
-
-* `tmsProjectId` - ID of a project in TMS instance.
-
-* `tmsConfigurationId` - ID of a configuration in TMS instance.
-
-* `tmsAdapterMode` - adapter mode. Default value - 0.
-
-* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
-  created automatically.
-
-* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
-  automatically.
-
-* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
-  default file name.
-
-* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-* `tmsCertValidation` - it enables/disables certificate validation. Default value - true.
+#### File
 
-* `tmsAutomaticCreationTestCases` - mode of automatic creation test cases. Default value - false.
+Create **connection_config.ini** file in the root directory of the project:
+```
+[testit]
+URL = URL
+privateToken = USER_PRIVATE_TOKEN
+projectId = PROJECT_ID
+configurationId = CONFIGURATION_ID
+testRunId = TEST_RUN_ID
+testRunName = TEST_RUN_NAME
+adapterMode = ADAPTER_MODE
+certValidation = CERT_VALIDATION
+automaticCreationTestCases = AUTOMATIC_CREATION_TEST_CASES
+
+# This section are optional. It enables debug mode.
+[debug]
+tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+```
 
 #### Examples
 
 Launch with a connection_config.ini file in the root directory of the project:
 
 ```
 $ pytest --testit
 ```
 
 Launch with command-line parameters:
 
 ```
-$ pytest --testit --tmsUrl=<url> --tmsPrivateToken=<token> --tmsProjectId=<id> --tmsConfigurationId=<id> --tmsTestRunId=<optional id> --tmsTestRunName=<optional name> --tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' --tmsCertValidation=<optional boolean> --tmsAutomaticCreationTestCases=<optional boolean>
+$ pytest --testit --tmsUrl=URL --tmsPrivateToken=USER_PRIVATE_TOKEN --tmsProjectId=PROJECT_ID --tmsConfigurationId=CONFIGURATION_ID --tmsTestRunId=TEST_RUN_ID --tmsTestRunName=TEST_RUN_NAME --tmsAdapterMode=ADAPTER_MODE --tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' --tmsCertValidation=CERT_VALIDATION --tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
 ```
 
 If you want to enable debug mode then
 see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Decorators
```

### Comparing `testit-adapter-pytest-2.1.7/setup.py` & `testit-adapter-pytest-2.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='2.1.7',
+    version='2.1.8',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,10 +16,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.1.7'],
+    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.1.8'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit-adapter-pytest-2.1.7/src/testit_adapter_pytest/listener.py` & `testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/listener.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.1.7/src/testit_adapter_pytest/plugin.py` & `testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.1.7/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.1.7
+Version: 2.1.8
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -25,146 +25,60 @@
 pip install testit-adapter-pytest
 ```
 
 ## Usage
 
 ### Configuration
 
-#### File
-
-1. Create **connection_config.ini** file in the root directory of the project:
-    ```
-    [testit]
-    URL = <url>
-    privateToken = <token>
-    projectId = <id>
-    configurationId = <id>
-    testRunId = <optional id>
-    testRunName = <optional name>
-    adapterMode = <optional>
-    certValidation = <optional boolean>
-    automaticCreationTestCases = <optional boolean>
-    
-    # This section are optional. It enables debug mode.
-    [debug]
-    tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
-    ```
-
-2. Fill parameters with your configuration, where:
-    * `URL` - location of the TMS instance
-
-    * `privateToken` - API secret key
-        1. go to the https://{DOMAIN}/user-profile profile
-        2. copy the API secret key
-
-    * `projectId` - ID of project in TMS instance.
-
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request project, Preview tab, copy id field
-
-    * `configurationId` - ID of configuration in TMS instance.
-
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request configurations, Preview tab, copy id field
-
-    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
-      created automatically.
-
-    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
-      not provided, it is created automatically.
-
-    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
-
-        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
-          test run.
-        * 1 - in this mode, the adapter sends all results to the test run without filtering.
-        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-    
-    * `certValidation` - it enables/disables certificate validation. Default value - true.
-
-    * `automaticCreationTestCases` - mode of automatic creation test cases. Default value - false. The adapter supports following modes:
-        * true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest).
-        * false - in this mode, the adapter will not create a test case.
-
-    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-#### ENV
-
-You can use environment variables (environment variables take precedence over file variables):
-
-* `TMS_URL` - location of the TMS instance.
-
-* `TMS_PRIVATE_TOKEN` - API secret key.
-
-* `TMS_PROJECT_ID` - ID of a project in TMS instance.
-
-* `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
-
-* `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
+| Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
+| Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
+| API secret key [How to getting API secret key?](https://github.com/testit-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                            | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
+| ID of project in TMS instance [How to getting project ID?](https://github.com/testit-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                    | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
+| ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testit-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                  | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
+| ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
+| Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
+| Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
+| It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
+| Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
+| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
 
-* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
-  it is created automatically.
-
-* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
-  automatically.
-
-* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
-  default file name.
-
-* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. Default value - true.
-
-* `TMS_AUTOMATIC_CREATION_TEST_CASES` - mode of automatic creation test cases. Default value - false.
-
-#### Command line
-
-You also can CLI variables (CLI variables take precedence over environment variables):
-
-* `tmsUrl` - location of the TMS instance.
-
-* `tmsPrivateToken` - API secret key.
-
-* `tmsProjectId` - ID of a project in TMS instance.
-
-* `tmsConfigurationId` - ID of a configuration in TMS instance.
-
-* `tmsAdapterMode` - adapter mode. Default value - 0.
-
-* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
-  created automatically.
-
-* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
-  automatically.
-
-* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
-  default file name.
-
-* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-* `tmsCertValidation` - it enables/disables certificate validation. Default value - true.
+#### File
 
-* `tmsAutomaticCreationTestCases` - mode of automatic creation test cases. Default value - false.
+Create **connection_config.ini** file in the root directory of the project:
+```
+[testit]
+URL = URL
+privateToken = USER_PRIVATE_TOKEN
+projectId = PROJECT_ID
+configurationId = CONFIGURATION_ID
+testRunId = TEST_RUN_ID
+testRunName = TEST_RUN_NAME
+adapterMode = ADAPTER_MODE
+certValidation = CERT_VALIDATION
+automaticCreationTestCases = AUTOMATIC_CREATION_TEST_CASES
+
+# This section are optional. It enables debug mode.
+[debug]
+tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+```
 
 #### Examples
 
 Launch with a connection_config.ini file in the root directory of the project:
 
 ```
 $ pytest --testit
 ```
 
 Launch with command-line parameters:
 
 ```
-$ pytest --testit --tmsUrl=<url> --tmsPrivateToken=<token> --tmsProjectId=<id> --tmsConfigurationId=<id> --tmsTestRunId=<optional id> --tmsTestRunName=<optional name> --tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' --tmsCertValidation=<optional boolean> --tmsAutomaticCreationTestCases=<optional boolean>
+$ pytest --testit --tmsUrl=URL --tmsPrivateToken=USER_PRIVATE_TOKEN --tmsProjectId=PROJECT_ID --tmsConfigurationId=CONFIGURATION_ID --tmsTestRunId=TEST_RUN_ID --tmsTestRunName=TEST_RUN_NAME --tmsAdapterMode=ADAPTER_MODE --tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' --tmsCertValidation=CERT_VALIDATION --tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
 ```
 
 If you want to enable debug mode then
 see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Decorators
```


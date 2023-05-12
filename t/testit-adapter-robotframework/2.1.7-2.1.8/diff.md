# Comparing `tmp/testit-adapter-robotframework-2.1.7.tar.gz` & `tmp/testit-adapter-robotframework-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-robotframework-2.1.7.tar", last modified: Fri Apr 21 08:18:26 2023, max compression
+gzip compressed data, was "testit-adapter-robotframework-2.1.8.tar", last modified: Fri May 12 08:35:01 2023, max compression
```

## Comparing `testit-adapter-robotframework-2.1.7.tar` & `testit-adapter-robotframework-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.937446 testit-adapter-robotframework-2.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-21 08:17:56.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:26.941446 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 08:18:26.000000 testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.698252 testit-adapter-robotframework-2.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit-adapter-robotframework-2.1.7/PKG-INFO` & `testit-adapter-robotframework-2.1.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,67 @@
-Metadata-Version: 2.1
-Name: testit-adapter-robotframework
-Version: 2.1.7
-Summary: Robot Framework adapter for Test IT
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
 # Test IT TMS adapter for Robot Framework
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
 ```
 pip install testit-adapter-robotframework
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
-$ robot -v testit <test directory>
+$ robot -v testit TEST_DIRECTORY
 ```
 
 Launch with command-line parameters (parameters are case-insensitive):
 
 ```
-$ robot -v testit -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> -v tmsAutomaticCreationTestCases:<optional boolean> <test directory>
+$ robot -v testit -v tmsUrl:URL -v tmsPrivateToken:USER_PRIVATE_TOKEN -v tmsProjectId:PROJECT_ID -v tmsConfigurationId:CONFIGURATION_ID -v tmsTestRunId:TEST_RUN_ID -v tmsTestRunName:TEST_RUN_NAME -v tmsAdapterMode:ADAPTER_MODE -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:CERT_VALIDATION -v tmsAutomaticCreationTestCases:AUTOMATIC_CREATION_TEST_CASES TEST_DIRECTORY
 ```
 
 If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Tags
 
 Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
```

### Comparing `testit-adapter-robotframework-2.1.7/README.md` & `testit-adapter-robotframework-2.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,82 @@
+Metadata-Version: 2.1
+Name: testit-adapter-robotframework
+Version: 2.1.8
+Summary: Robot Framework adapter for Test IT
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
 # Test IT TMS adapter for Robot Framework
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
 ```
 pip install testit-adapter-robotframework
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
-$ robot -v testit <test directory>
+$ robot -v testit TEST_DIRECTORY
 ```
 
 Launch with command-line parameters (parameters are case-insensitive):
 
 ```
-$ robot -v testit -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> -v tmsAutomaticCreationTestCases:<optional boolean> <test directory>
+$ robot -v testit -v tmsUrl:URL -v tmsPrivateToken:USER_PRIVATE_TOKEN -v tmsProjectId:PROJECT_ID -v tmsConfigurationId:CONFIGURATION_ID -v tmsTestRunId:TEST_RUN_ID -v tmsTestRunName:TEST_RUN_NAME -v tmsAdapterMode:ADAPTER_MODE -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:CERT_VALIDATION -v tmsAutomaticCreationTestCases:AUTOMATIC_CREATION_TEST_CASES TEST_DIRECTORY
 ```
 
 If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Tags
 
 Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
```

### Comparing `testit-adapter-robotframework-2.1.7/setup.py` & `testit-adapter-robotframework-2.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='2.1.7',
+    version='2.1.8',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,9 +16,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.7']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.8']
 )
```

### Comparing `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/TMSLibrary.py` & `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/listeners.py` & `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/listeners.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework/models.py` & `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,18 @@
                         logger.error(f"[TestIt] Link Error: {e}")
                 elif attr == 'labels':
                     value = ast.literal_eval(value)
                     if isinstance(value, (str, int)):
                         self.labels.append(Label(value))
                     elif isinstance(value, list):
                         self.labels.extend([Label(item) for item in value if isinstance(item, (str, int))])
+                elif attr == 'namespace':
+                    self.namespace = str(value).replace("'", "").replace('"', '')
+                elif attr == 'classname':
+                    self.classname = str(value).replace("'", "").replace('"', '')
                 else:
                     logger.error(f"[TestIt] Unknown attribute: {attr}")
         if not self.externalID:
             self.externalID = Utils.get_hash(attrs['longname'].split('.', 1)[-1])
 
     def add_step(self, step_type, title, description, parameters):
         if len(self.step_depth) == 0:
```

### Comparing `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.7
+Version: 2.1.8
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -23,146 +23,60 @@
 pip install testit-adapter-robotframework
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
-$ robot -v testit <test directory>
+$ robot -v testit TEST_DIRECTORY
 ```
 
 Launch with command-line parameters (parameters are case-insensitive):
 
 ```
-$ robot -v testit -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> -v tmsAutomaticCreationTestCases:<optional boolean> <test directory>
+$ robot -v testit -v tmsUrl:URL -v tmsPrivateToken:USER_PRIVATE_TOKEN -v tmsProjectId:PROJECT_ID -v tmsConfigurationId:CONFIGURATION_ID -v tmsTestRunId:TEST_RUN_ID -v tmsTestRunName:TEST_RUN_NAME -v tmsAdapterMode:ADAPTER_MODE -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:CERT_VALIDATION -v tmsAutomaticCreationTestCases:AUTOMATIC_CREATION_TEST_CASES TEST_DIRECTORY
 ```
 
 If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Tags
 
 Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
```

### Comparing `testit-adapter-robotframework-2.1.7/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*


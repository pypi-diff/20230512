# Comparing `tmp/testit-adapter-behave-2.1.7.tar.gz` & `tmp/testit-adapter-behave-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-behave-2.1.7.tar", last modified: Fri Apr 21 08:18:07 2023, max compression
+gzip compressed data, was "testit-adapter-behave-2.1.8.tar", last modified: Fri May 12 08:35:04 2023, max compression
```

## Comparing `testit-adapter-behave-2.1.7.tar` & `testit-adapter-behave-2.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:07.673460 testit-adapter-behave-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-21 08:18:07.673460 testit-adapter-behave-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:18:07.673460 testit-adapter-behave-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:07.669460 testit-adapter-behave-2.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:07.669460 testit-adapter-behave-2.1.7/src/testit_adapter_behave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:07.669460 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/option.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/test_result_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/models/url_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/scenario_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/tags_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-21 08:17:56.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:07.669460 testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-21 08:18:07.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 08:18:07.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:18:07.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 08:18:07.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 08:18:07.000000 testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.762863 testit-adapter-behave-2.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/src/testit_adapter_behave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/url_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/scenario_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/tags_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/top_level.txt
```

### Comparing `testit-adapter-behave-2.1.7/PKG-INFO` & `testit-adapter-behave-2.1.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: testit-adapter-behave
-Version: 2.1.7
-Summary: Behave adapter for Test IT
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
 # Test IT TMS adapter for Behave
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
@@ -25,149 +10,63 @@
 pip install testit-adapter-behave
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
 $ behave -f testit_adapter_behave.formatter:AdapterFormatter
 ```
 
 Launch with command-line parameters:
 
 ```
-$ behave -f testit_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
-tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
-tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
-tmsCertValidation=<optional boolean> -D tmsAutomaticCreationTestCases=<optional boolean>
+$ behave -f testit_adapter_behave.formatter:AdapterFormatter -D tmsUrl=URL -D tmsPrivateToken=USER_PRIVATE_TOKEN -D
+tmsProjectId=PROJECT_ID -D tmsConfigurationId=CONFIGURATION_ID -D tmsTestRunId=TEST_RUN_ID -D tmsAdapterMode=ADAPTER_MODE -D
+tmsTestRunName=TEST_RUN_NAME -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
+tmsCertValidation=CERT_VALIDATION -D tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
 ```
 
 If you want to enable debug mode then
 see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Tags
```

### Comparing `testit-adapter-behave-2.1.7/README.md` & `testit-adapter-behave-2.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: testit-adapter-behave
+Version: 2.1.8
+Summary: Behave adapter for Test IT
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
 # Test IT TMS adapter for Behave
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
@@ -10,149 +25,63 @@
 pip install testit-adapter-behave
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
 $ behave -f testit_adapter_behave.formatter:AdapterFormatter
 ```
 
 Launch with command-line parameters:
 
 ```
-$ behave -f testit_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
-tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
-tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
-tmsCertValidation=<optional boolean> -D tmsAutomaticCreationTestCases=<optional boolean>
+$ behave -f testit_adapter_behave.formatter:AdapterFormatter -D tmsUrl=URL -D tmsPrivateToken=USER_PRIVATE_TOKEN -D
+tmsProjectId=PROJECT_ID -D tmsConfigurationId=CONFIGURATION_ID -D tmsTestRunId=TEST_RUN_ID -D tmsAdapterMode=ADAPTER_MODE -D
+tmsTestRunName=TEST_RUN_NAME -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
+tmsCertValidation=CERT_VALIDATION -D tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
 ```
 
 If you want to enable debug mode then
 see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Tags
```

### Comparing `testit-adapter-behave-2.1.7/setup.py` & `testit-adapter-behave-2.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-behave',
-    version='2.1.7',
+    version='2.1.8',
     description='Behave adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_behave'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'behave',
-        'testit-python-commons==2.1.7',
+        'testit-python-commons==2.1.8',
         'attrs'],
 )
```

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave/formatter.py` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave/formatter.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave/listener.py` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave/listener.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave/scenario_parser.py` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave/scenario_parser.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave/tags_parser.py` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave/tags_parser.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave/utils.py` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/PKG-INFO` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.7
+Version: 2.1.8
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -25,149 +25,63 @@
 pip install testit-adapter-behave
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
 $ behave -f testit_adapter_behave.formatter:AdapterFormatter
 ```
 
 Launch with command-line parameters:
 
 ```
-$ behave -f testit_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
-tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
-tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
-tmsCertValidation=<optional boolean> -D tmsAutomaticCreationTestCases=<optional boolean>
+$ behave -f testit_adapter_behave.formatter:AdapterFormatter -D tmsUrl=URL -D tmsPrivateToken=USER_PRIVATE_TOKEN -D
+tmsProjectId=PROJECT_ID -D tmsConfigurationId=CONFIGURATION_ID -D tmsTestRunId=TEST_RUN_ID -D tmsAdapterMode=ADAPTER_MODE -D
+tmsTestRunName=TEST_RUN_NAME -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
+tmsCertValidation=CERT_VALIDATION -D tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
 ```
 
 If you want to enable debug mode then
 see [How to enable debug logging?](https://github.com/testit-tms/adapters-python/tree/main/testit-python-commons)
 
 ### Tags
```

### Comparing `testit-adapter-behave-2.1.7/src/testit_adapter_behave.egg-info/SOURCES.txt` & `testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*


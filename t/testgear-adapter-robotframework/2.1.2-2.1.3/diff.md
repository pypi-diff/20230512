# Comparing `tmp/testgear-adapter-robotframework-2.1.2.tar.gz` & `tmp/testgear-adapter-robotframework-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-robotframework-2.1.2.tar", last modified: Fri Apr 21 14:55:07 2023, max compression
+gzip compressed data, was "testgear-adapter-robotframework-2.1.3.tar", last modified: Fri May 12 09:41:17 2023, max compression
```

## Comparing `testgear-adapter-robotframework-2.1.2.tar` & `testgear-adapter-robotframework-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/
--rw-rw-rw-   0        0        0    11211 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10640 2023-03-31 06:28:55.000000 testgear-adapter-robotframework-2.1.2/README.md
--rw-rw-rw-   0        0        0       21 2023-01-19 07:55:39.000000 testgear-adapter-robotframework-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-04-21 14:03:38.000000 testgear-adapter-robotframework-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.239820 testgear-adapter-robotframework-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/
--rw-rw-rw-   0        0        0     4343 2023-04-21 13:55:56.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/TMSLibrary.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/__init__.py
--rw-rw-rw-   0        0        0     4210 2023-04-21 13:55:13.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/listeners.py
--rw-rw-rw-   0        0        0     8974 2023-04-21 13:55:56.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/models.py
--rw-rw-rw-   0        0        0      297 2023-04-21 13:47:37.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/
--rw-rw-rw-   0        0        0    11211 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-21 14:55:07.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:17.091574 testgear-adapter-robotframework-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-05-12 09:41:17.091574 testgear-adapter-robotframework-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:41:17.091574 testgear-adapter-robotframework-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:17.087574 testgear-adapter-robotframework-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:17.087574 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 09:41:00.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:17.091574 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-05-12 09:41:17.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-12 09:41:17.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:41:17.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 09:41:17.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 09:41:17.000000 testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testgear-adapter-robotframework-2.1.2/PKG-INFO` & `testgear-adapter-robotframework-2.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,297 +1,227 @@
-Metadata-Version: 2.1
-Name: testgear-adapter-robotframework
-Version: 2.1.2
-Summary: Robot Framework adapter for Test Gear
-Home-page: https://github.com/testgear-tms/adapters-python/
-Author: Integration team
-Author-email: integrations@test-gear.io
-License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
-# Test Gear TMS adapter for Robot Framework
-![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-
-## Getting Started
-
-### Installation
-```
-pip install testgear-adapter-robotframework
-```
-
-## Usage
-
-### Configuration
-
-#### File
-
-1. Create **connection_config.ini** file in the root directory of the project:
-    ```
-    [testgear]
-    URL = <url>
-    privateToken = <token>
-    projectId = <id>
-    configurationId = <id>
-    testRunId = <optional id>
-    testRunName = <optional name>
-    adapterMode = <optional>
-    certValidation = <optional boolean>
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
-    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
-      
-    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
-    
-    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
-        
-        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
-        * 1 - in this mode, the adapter sends all results to the test run without filtering.
-        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-   
-    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-    
-    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-    
-3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
-  
-* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
-  
-* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
-  
-* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
-
-* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-
-#### Command line
-
-You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
-* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
-  
-* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
-  
-* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
-
-* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-* `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
-
-#### Examples
-
-Launch with a connection_config.ini file in the root directory of the project:
-
-```
-$ robot -v testgear <test directory>
-```
-
-Launch with command-line parameters (parameters are case-insensitive):
-
-```
-$ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
-```
-
-If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-
-### Tags
-
-Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
-
-Description of tags:
-- `testgear.workItemsId` - linking an autotest to a test case
-- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
-- `testgear.externalId` - ID of the autotest within the project in the TMS System
-- `testgear.title` - title in the autotest card (default - name of test)
-- `testgear.description` - description in the autotest card (default - documentation of test)
-- `testgear.links` - links in the autotest card
-- `testgear.labels` - labels in the autotest card
-- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
-- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
-
-Description of methods:
-- `Add Links` - links in the autotest result
-- `Add Link` - add one link in the autotest result
-- `Add Attachments` - uploading files in the autotest result
-- `Add Attachment` - upload given content with given filename in the autotest result
-- `Add Message` - information about autotest in the autotest result
-
-### Parallel execution
-
-You can also run your test in parallel with [Pabot](https://pabot.org/).
-
-```
-$ pabot --pabotlib -v testgear <test directory>
-```
-
-All other settings are the same as for standard execution.
-
-### Examples
-
-```robotframework
-*** Settings ***
-Documentation      Main Suite with examples
-Library            testgear_adapter_robotframework.TMSLibrary
-
-*** Variables ***
-&{SIMPLE_LINK}             url=http://google.com
-&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
-
-@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
-
-
-*** Test Cases ***
-Simple Test
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with link as variable
-    [Tags]   testgear.links:${SIMPLE_LINK}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with link as dict
-    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with WorkitemId as string
-    [Tags]   testgear.workitemsID:123
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with WorkitemId as list
-    [Tags]   testgear.workitemsID:${{[123, '456']}}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with Title or Description or DisplayName with simple formatting
-    [Documentation]  Tags are space sensitive, use only one space between words
-    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
-    ...    testgear.description:"This works too"
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Test With All Params
-    [Documentation]  It's better to use this kind of formatting for different data types in tags
-    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
-    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
-    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
-    [Setup]  Setup
-    Log    Something
-    Log    Another
-    [Teardown]  Teardown
-
-Test With Add Link
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Add Links    @{LINKS}
-#    You can also add one link (default type is Defect)
-    Add Link    http://ya.ru
-    Add Link    http://ya.ru    type=Issue
-    Add Link    ${SIMPLE_LINK}[url]
-    [Teardown]  Teardown
-
-Test With Add Attachment
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    ${V}   Get Variables
-    Add Attachment    '${V}'    file.txt
-    Add Attachments    images/banner.png     images/icon.png
-    [Teardown]  Teardown
-
-Test With Add Message
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Add Message    Wow, it's my error message!
-    Fail
-    [Teardown]  Teardown
-```
-
-# Contributing
-
-You can help to develop the project. Any contributions are **greatly appreciated**.
-
-* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-* Please make sure you check your spelling and grammar.
-* Create individual PR for each suggestion.
-* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-
-# License
-
-Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
-
+Metadata-Version: 2.1
+Name: testgear-adapter-robotframework
+Version: 2.1.3
+Summary: Robot Framework adapter for Test Gear
+Home-page: https://github.com/testgear-tms/adapters-python/
+Author: Integration team
+Author-email: integrations@test-gear.io
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# Test Gear TMS adapter for Robot Framework
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+```
+pip install testgear-adapter-robotframework
+```
+
+## Usage
+
+### Configuration
+
+| Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
+| Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
+| API secret key [How to getting API secret key?](https://github.com/testgear-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                          | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
+| ID of project in TMS instance [How to getting project ID?](https://github.com/testgear-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                  | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
+| ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testgear-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
+| ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
+| Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
+| Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
+| It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
+| Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
+| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
+
+#### File
+
+Create **connection_config.ini** file in the root directory of the project:
+```
+[testgear]
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
+
+#### Examples
+
+Launch with a connection_config.ini file in the root directory of the project:
+
+```
+$ robot -v testgear TEST_DIRECTORY
+```
+
+Launch with command-line parameters (parameters are case-insensitive):
+
+```
+$ robot -v testgear -v tmsUrl:URL -v tmsPrivateToken:USER_PRIVATE_TOKEN -v tmsProjectId:PROJECT_ID -v tmsConfigurationId:CONFIGURATION_ID -v tmsTestRunId:TEST_RUN_ID -v tmsTestRunName:TEST_RUN_NAME -v tmsAdapterMode:ADAPTER_MODE -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:CONFIG_FILE_NAME -v tmsCertValidation:CERT_VALIDATION -v tmsAutomaticCreationTestCases:AUTOMATIC_CREATION_TEST_CASES TEST_DIRECTORY
+```
+
+If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
+
+Description of tags:
+- `testgear.workItemsId` - linking an autotest to a test case
+- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
+- `testgear.externalId` - ID of the autotest within the project in the TMS System
+- `testgear.title` - title in the autotest card (default - name of test)
+- `testgear.description` - description in the autotest card (default - documentation of test)
+- `testgear.links` - links in the autotest card
+- `testgear.labels` - labels in the autotest card
+- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
+- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+- `Add Links` - links in the autotest result
+- `Add Link` - add one link in the autotest result
+- `Add Attachments` - uploading files in the autotest result
+- `Add Attachment` - upload given content with given filename in the autotest result
+- `Add Message` - information about autotest in the autotest result
+
+### Parallel execution
+
+You can also run your test in parallel with [Pabot](https://pabot.org/).
+
+```
+$ pabot --pabotlib -v testgear <test directory>
+```
+
+All other settings are the same as for standard execution.
+
+### Examples
+
+```robotframework
+*** Settings ***
+Documentation      Main Suite with examples
+Library            testgear_adapter_robotframework.TMSLibrary
+
+*** Variables ***
+&{SIMPLE_LINK}             url=http://google.com
+&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
+
+@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
+
+
+*** Test Cases ***
+Simple Test
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as variable
+    [Tags]   testgear.links:${SIMPLE_LINK}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as dict
+    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as string
+    [Tags]   testgear.workitemsID:123
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as list
+    [Tags]   testgear.workitemsID:${{[123, '456']}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with Title or Description or DisplayName with simple formatting
+    [Documentation]  Tags are space sensitive, use only one space between words
+    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
+    ...    testgear.description:"This works too"
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Test With All Params
+    [Documentation]  It's better to use this kind of formatting for different data types in tags
+    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
+    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
+    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
+    [Setup]  Setup
+    Log    Something
+    Log    Another
+    [Teardown]  Teardown
+
+Test With Add Link
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Links    @{LINKS}
+#    You can also add one link (default type is Defect)
+    Add Link    http://ya.ru
+    Add Link    http://ya.ru    type=Issue
+    Add Link    ${SIMPLE_LINK}[url]
+    [Teardown]  Teardown
+
+Test With Add Attachment
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    ${V}   Get Variables
+    Add Attachment    '${V}'    file.txt
+    Add Attachments    images/banner.png     images/icon.png
+    [Teardown]  Teardown
+
+Test With Add Message
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Message    Wow, it's my error message!
+    Fail
+    [Teardown]  Teardown
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-robotframework-2.1.2/README.md` & `testgear-adapter-robotframework-2.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,282 +1,212 @@
-# Test Gear TMS adapter for Robot Framework
-![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-
-## Getting Started
-
-### Installation
-```
-pip install testgear-adapter-robotframework
-```
-
-## Usage
-
-### Configuration
-
-#### File
-
-1. Create **connection_config.ini** file in the root directory of the project:
-    ```
-    [testgear]
-    URL = <url>
-    privateToken = <token>
-    projectId = <id>
-    configurationId = <id>
-    testRunId = <optional id>
-    testRunName = <optional name>
-    adapterMode = <optional>
-    certValidation = <optional boolean>
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
-    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
-      
-    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
-    
-    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
-        
-        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
-        * 1 - in this mode, the adapter sends all results to the test run without filtering.
-        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-   
-    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-    
-    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-    
-3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
-  
-* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
-  
-* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
-  
-* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
-
-* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-
-#### Command line
-
-You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
-* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
-  
-* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
-  
-* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
-
-* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-* `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
-
-#### Examples
-
-Launch with a connection_config.ini file in the root directory of the project:
-
-```
-$ robot -v testgear <test directory>
-```
-
-Launch with command-line parameters (parameters are case-insensitive):
-
-```
-$ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
-```
-
-If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-
-### Tags
-
-Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
-
-Description of tags:
-- `testgear.workItemsId` - linking an autotest to a test case
-- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
-- `testgear.externalId` - ID of the autotest within the project in the TMS System
-- `testgear.title` - title in the autotest card (default - name of test)
-- `testgear.description` - description in the autotest card (default - documentation of test)
-- `testgear.links` - links in the autotest card
-- `testgear.labels` - labels in the autotest card
-- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
-- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
-
-Description of methods:
-- `Add Links` - links in the autotest result
-- `Add Link` - add one link in the autotest result
-- `Add Attachments` - uploading files in the autotest result
-- `Add Attachment` - upload given content with given filename in the autotest result
-- `Add Message` - information about autotest in the autotest result
-
-### Parallel execution
-
-You can also run your test in parallel with [Pabot](https://pabot.org/).
-
-```
-$ pabot --pabotlib -v testgear <test directory>
-```
-
-All other settings are the same as for standard execution.
-
-### Examples
-
-```robotframework
-*** Settings ***
-Documentation      Main Suite with examples
-Library            testgear_adapter_robotframework.TMSLibrary
-
-*** Variables ***
-&{SIMPLE_LINK}             url=http://google.com
-&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
-
-@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
-
-
-*** Test Cases ***
-Simple Test
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with link as variable
-    [Tags]   testgear.links:${SIMPLE_LINK}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with link as dict
-    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with WorkitemId as string
-    [Tags]   testgear.workitemsID:123
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with WorkitemId as list
-    [Tags]   testgear.workitemsID:${{[123, '456']}}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with Title or Description or DisplayName with simple formatting
-    [Documentation]  Tags are space sensitive, use only one space between words
-    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
-    ...    testgear.description:"This works too"
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Test With All Params
-    [Documentation]  It's better to use this kind of formatting for different data types in tags
-    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
-    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
-    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
-    [Setup]  Setup
-    Log    Something
-    Log    Another
-    [Teardown]  Teardown
-
-Test With Add Link
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Add Links    @{LINKS}
-#    You can also add one link (default type is Defect)
-    Add Link    http://ya.ru
-    Add Link    http://ya.ru    type=Issue
-    Add Link    ${SIMPLE_LINK}[url]
-    [Teardown]  Teardown
-
-Test With Add Attachment
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    ${V}   Get Variables
-    Add Attachment    '${V}'    file.txt
-    Add Attachments    images/banner.png     images/icon.png
-    [Teardown]  Teardown
-
-Test With Add Message
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Add Message    Wow, it's my error message!
-    Fail
-    [Teardown]  Teardown
-```
-
-# Contributing
-
-You can help to develop the project. Any contributions are **greatly appreciated**.
-
-* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-* Please make sure you check your spelling and grammar.
-* Create individual PR for each suggestion.
-* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-
-# License
-
-Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
-
+# Test Gear TMS adapter for Robot Framework
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+```
+pip install testgear-adapter-robotframework
+```
+
+## Usage
+
+### Configuration
+
+| Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
+| Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
+| API secret key [How to getting API secret key?](https://github.com/testgear-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                          | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
+| ID of project in TMS instance [How to getting project ID?](https://github.com/testgear-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                  | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
+| ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testgear-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
+| ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
+| Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
+| Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
+| It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
+| Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
+| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
+
+#### File
+
+Create **connection_config.ini** file in the root directory of the project:
+```
+[testgear]
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
+
+#### Examples
+
+Launch with a connection_config.ini file in the root directory of the project:
+
+```
+$ robot -v testgear TEST_DIRECTORY
+```
+
+Launch with command-line parameters (parameters are case-insensitive):
+
+```
+$ robot -v testgear -v tmsUrl:URL -v tmsPrivateToken:USER_PRIVATE_TOKEN -v tmsProjectId:PROJECT_ID -v tmsConfigurationId:CONFIGURATION_ID -v tmsTestRunId:TEST_RUN_ID -v tmsTestRunName:TEST_RUN_NAME -v tmsAdapterMode:ADAPTER_MODE -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:CONFIG_FILE_NAME -v tmsCertValidation:CERT_VALIDATION -v tmsAutomaticCreationTestCases:AUTOMATIC_CREATION_TEST_CASES TEST_DIRECTORY
+```
+
+If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
+
+Description of tags:
+- `testgear.workItemsId` - linking an autotest to a test case
+- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
+- `testgear.externalId` - ID of the autotest within the project in the TMS System
+- `testgear.title` - title in the autotest card (default - name of test)
+- `testgear.description` - description in the autotest card (default - documentation of test)
+- `testgear.links` - links in the autotest card
+- `testgear.labels` - labels in the autotest card
+- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
+- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+- `Add Links` - links in the autotest result
+- `Add Link` - add one link in the autotest result
+- `Add Attachments` - uploading files in the autotest result
+- `Add Attachment` - upload given content with given filename in the autotest result
+- `Add Message` - information about autotest in the autotest result
+
+### Parallel execution
+
+You can also run your test in parallel with [Pabot](https://pabot.org/).
+
+```
+$ pabot --pabotlib -v testgear <test directory>
+```
+
+All other settings are the same as for standard execution.
+
+### Examples
+
+```robotframework
+*** Settings ***
+Documentation      Main Suite with examples
+Library            testgear_adapter_robotframework.TMSLibrary
+
+*** Variables ***
+&{SIMPLE_LINK}             url=http://google.com
+&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
+
+@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
+
+
+*** Test Cases ***
+Simple Test
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as variable
+    [Tags]   testgear.links:${SIMPLE_LINK}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as dict
+    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as string
+    [Tags]   testgear.workitemsID:123
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as list
+    [Tags]   testgear.workitemsID:${{[123, '456']}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with Title or Description or DisplayName with simple formatting
+    [Documentation]  Tags are space sensitive, use only one space between words
+    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
+    ...    testgear.description:"This works too"
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Test With All Params
+    [Documentation]  It's better to use this kind of formatting for different data types in tags
+    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
+    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
+    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
+    [Setup]  Setup
+    Log    Something
+    Log    Another
+    [Teardown]  Teardown
+
+Test With Add Link
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Links    @{LINKS}
+#    You can also add one link (default type is Defect)
+    Add Link    http://ya.ru
+    Add Link    http://ya.ru    type=Issue
+    Add Link    ${SIMPLE_LINK}[url]
+    [Teardown]  Teardown
+
+Test With Add Attachment
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    ${V}   Get Variables
+    Add Attachment    '${V}'    file.txt
+    Add Attachments    images/banner.png     images/icon.png
+    [Teardown]  Teardown
+
+Test With Add Message
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Message    Wow, it's my error message!
+    Fail
+    [Teardown]  Teardown
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/TMSLibrary.py` & `testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/TMSLibrary.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-from robot.libraries.BuiltIn import BuiltIn
-
-from testgear_python_commons.services import TmsPluginManager
-
-from .listeners import AutotestAdapter, TestRunAdapter
-from .models import Link, Option
-
-
-def enabled(func):
-    def wrapped(self, *args, **kwargs):
-        if self.enabled:
-            return func(self, *args, **kwargs)
-        else:
-            raise ImportError("TestGear module should be enabled. Use '-v testgear' CLI option")
-
-    return wrapped
-
-
-class TMSLibrary:
-    """Library for exporting result to TestGear.
-
-        = Table of contents =
-
-        %TOC%
-
-        = Usage =
-
-        This library has several keyword, for example `Add Link`, adding links to result of test in TestGear
-
-        = Examples =
-
-        | `Add Message`      | My message    |                |               |
-        | `Add Link`         | http://ya.ru  |                |               |
-        | `Add Attachments`  | image.png     | log.txt        | video.gif     |
-        """
-    ROBOT_LIBRARY_SCOPE = 'GLOBAL'
-    ROBOT_LIBRARY_VERSION = '1.0'
-
-    def __init__(self):
-        built_in = BuiltIn()
-        self.enabled = built_in.get_variable_value("${testgear}", None) is not None
-        if self.enabled:
-            cli_params = ["tmsUrl", "tmsPrivateToken", "tmsProjectId",
-                          "tmsConfigurationId", "tmsTestRunId", "tmsTestRunName",
-                          "tmsAdapterMode", "tmsConfigFile", "tmsCertValidation", "tmsAutomaticCreationTestCases"]
-            option = Option(**{param: built_in.get_variable_value(f'${{{param}}}', None) for param in cli_params})
-            self.adapter_manager = TmsPluginManager.get_adapter_manager(option)
-            pabot_index = built_in.get_variable_value('${PABOTQUEUEINDEX}', None)
-            if pabot_index is not None:
-                try:
-                    from pabot import PabotLib
-                    pabot = PabotLib()
-                    if int(pabot_index) == 0:
-                        test_run_id = self.adapter_manager.get_test_run_id()
-                        pabot.set_parallel_value_for_key('test_run_id', test_run_id)
-                    else:
-                        while True:
-                            test_run_id = pabot.get_parallel_value_for_key('test_run_id')
-                            if test_run_id:
-                                break
-                    self.adapter_manager.set_test_run_id(test_run_id)
-                except RuntimeError:
-                    raise SystemExit
-            else:
-                self.adapter_manager.set_test_run_id(self.adapter_manager.get_test_run_id())
-            self.ROBOT_LIBRARY_LISTENER = [AutotestAdapter(self.adapter_manager), TestRunAdapter(self.adapter_manager)]
-
-    @enabled
-    def add_link(self, url, type='Defect', title=None, description=None):  # noqa: A002,VNE003
-        """
-        Adds link to current test.
-
-        Valid link types are ``Defect``, ``Issue``, ``Related``, ``BlockedBy``, ``Requirement``, ``Repository``.
-
-        """
-        link = Link(url=url, type=type, title=title, description=description)
-        self.ROBOT_LIBRARY_LISTENER[0].active_test.resultLinks.append(link)
-
-    @enabled
-    def add_links(self, *links):
-        """
-        Adds several links to current test.
-
-        Every link should be a dict with ``url`` key. See `Add Link` keyword for more information.
-
-        """
-        for link in links:
-            if isinstance(link, dict):
-                self.add_link(**link)
-
-    @enabled
-    def add_attachments(self, *paths):
-        """
-        Adds several attachments to current test.
-
-        """
-        attachments = self.adapter_manager.load_attachments(paths)
-        self.ROBOT_LIBRARY_LISTENER[0].active_test.attachments.extend(attachments)
-
-    @enabled
-    def add_attachment(self, text, filename=None):
-        """
-        Adds attachment to current test
-
-        """
-        attachment = self.adapter_manager.create_attachment(text, filename)
-        self.ROBOT_LIBRARY_LISTENER[0].active_test.attachments.extend(attachment)
-
-    @enabled
-    def add_message(self, message):
-        """
-        Adds error message to current test
-        """
-        self.ROBOT_LIBRARY_LISTENER[0].active_test.message = message
+from robot.libraries.BuiltIn import BuiltIn
+
+from testgear_python_commons.services import TmsPluginManager
+
+from .listeners import AutotestAdapter, TestRunAdapter
+from .models import Link, Option
+
+
+def enabled(func):
+    def wrapped(self, *args, **kwargs):
+        if self.enabled:
+            return func(self, *args, **kwargs)
+        else:
+            raise ImportError("TestGear module should be enabled. Use '-v testgear' CLI option")
+
+    return wrapped
+
+
+class TMSLibrary:
+    """Library for exporting result to TestGear.
+
+        = Table of contents =
+
+        %TOC%
+
+        = Usage =
+
+        This library has several keyword, for example `Add Link`, adding links to result of test in TestGear
+
+        = Examples =
+
+        | `Add Message`      | My message    |                |               |
+        | `Add Link`         | http://ya.ru  |                |               |
+        | `Add Attachments`  | image.png     | log.txt        | video.gif     |
+        """
+    ROBOT_LIBRARY_SCOPE = 'GLOBAL'
+    ROBOT_LIBRARY_VERSION = '1.0'
+
+    def __init__(self):
+        built_in = BuiltIn()
+        self.enabled = built_in.get_variable_value("${testgear}", None) is not None
+        if self.enabled:
+            cli_params = ["tmsUrl", "tmsPrivateToken", "tmsProjectId",
+                          "tmsConfigurationId", "tmsTestRunId", "tmsTestRunName",
+                          "tmsAdapterMode", "tmsConfigFile", "tmsCertValidation", "tmsAutomaticCreationTestCases"]
+            option = Option(**{param: built_in.get_variable_value(f'${{{param}}}', None) for param in cli_params})
+            self.adapter_manager = TmsPluginManager.get_adapter_manager(option)
+            pabot_index = built_in.get_variable_value('${PABOTQUEUEINDEX}', None)
+            if pabot_index is not None:
+                try:
+                    from pabot import PabotLib
+                    pabot = PabotLib()
+                    if int(pabot_index) == 0:
+                        test_run_id = self.adapter_manager.get_test_run_id()
+                        pabot.set_parallel_value_for_key('test_run_id', test_run_id)
+                    else:
+                        while True:
+                            test_run_id = pabot.get_parallel_value_for_key('test_run_id')
+                            if test_run_id:
+                                break
+                    self.adapter_manager.set_test_run_id(test_run_id)
+                except RuntimeError:
+                    raise SystemExit
+            else:
+                self.adapter_manager.set_test_run_id(self.adapter_manager.get_test_run_id())
+            self.ROBOT_LIBRARY_LISTENER = [AutotestAdapter(self.adapter_manager), TestRunAdapter(self.adapter_manager)]
+
+    @enabled
+    def add_link(self, url, type='Defect', title=None, description=None):  # noqa: A002,VNE003
+        """
+        Adds link to current test.
+
+        Valid link types are ``Defect``, ``Issue``, ``Related``, ``BlockedBy``, ``Requirement``, ``Repository``.
+
+        """
+        link = Link(url=url, type=type, title=title, description=description)
+        self.ROBOT_LIBRARY_LISTENER[0].active_test.resultLinks.append(link)
+
+    @enabled
+    def add_links(self, *links):
+        """
+        Adds several links to current test.
+
+        Every link should be a dict with ``url`` key. See `Add Link` keyword for more information.
+
+        """
+        for link in links:
+            if isinstance(link, dict):
+                self.add_link(**link)
+
+    @enabled
+    def add_attachments(self, *paths):
+        """
+        Adds several attachments to current test.
+
+        """
+        attachments = self.adapter_manager.load_attachments(paths)
+        self.ROBOT_LIBRARY_LISTENER[0].active_test.attachments.extend(attachments)
+
+    @enabled
+    def add_attachment(self, text, filename=None):
+        """
+        Adds attachment to current test
+
+        """
+        attachment = self.adapter_manager.create_attachment(text, filename)
+        self.ROBOT_LIBRARY_LISTENER[0].active_test.attachments.extend(attachment)
+
+    @enabled
+    def add_message(self, message):
+        """
+        Adds error message to current test
+        """
+        self.ROBOT_LIBRARY_LISTENER[0].active_test.message = message
```

### Comparing `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/models.py` & `testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,209 +1,213 @@
-import ast
-import re
-
-from attr import Factory, asdict, attrib, s
-
-from robot.api import logger
-
-from testgear_python_commons.services import Utils
-
-LinkTypes = ['Related', 'BlockedBy', 'Defect', 'Issue', 'Requirement', 'Repository']
-
-
-def link_type_check(self, attribute, value):
-    if value.title() not in LinkTypes:
-        raise ValueError(f"Incorrect Link type: {value}")
-
-
-def url_check(self, attribute, value):
-    if not bool(re.match(
-            r"(https?|ftp)://"
-            r"(\w+(-\w+)*\.)?"
-            r"((\w+(-\w+)*)\.(\w+))"
-            r"(\.\w+)*"
-            r"([\w\-._~/]*)*(?<!\.)",
-            value)):
-        raise ValueError(f"Incorrect URL: {value}")
-
-
-class Default:
-
-    def order(self):
-        return asdict(self)
-
-
-@s
-class StepResult(Default):
-    title = attrib(default='')
-    description = attrib(default='')
-    started_on = attrib(default=None)
-    completed_on = attrib(default=None)
-    duration = attrib(default=None)
-    outcome = attrib(default=None)
-    step_results = attrib(default=Factory(list))
-    attachments = attrib(default=Factory(list))
-    parameters = attrib(default=Factory(dict))
-
-
-@s
-class Step(Default):
-    title = attrib()
-    description = attrib()
-    steps = attrib(default=Factory(list))
-
-
-@s(kw_only=True)
-class Link:
-    url = attrib(validator=[url_check])
-    type = attrib(default='Defect', validator=[link_type_check])  # noqa: A003,VNE003
-    title = attrib(default='')
-    description = attrib(default='')
-
-    def __attrs_post_init__(self):
-        self.type = self.type.title()
-
-
-@s
-class Label:
-    name = attrib()
-
-
-@s(kw_only=True)
-class Autotest(Default):
-    externalID = attrib(default=None)  # noqa: N815
-    autoTestName = attrib()  # noqa: N815
-    steps = attrib(default=Factory(list))
-    stepResults = attrib(default=Factory(list))  # noqa: N815
-    setUp = attrib(default=Factory(list))  # noqa: N815
-    setUpResults = attrib(default=Factory(list))  # noqa: N815
-    tearDown = attrib(default=Factory(list))  # noqa: N815
-    tearDownResults = attrib(default=Factory(list))  # noqa: N815
-    resultLinks = attrib(default=Factory(list))  # noqa: N815
-    duration = attrib(default=None)
-    failureReasonNames = attrib(default=Factory(list))  # noqa: N815
-    traces = attrib(default=None)
-    outcome = attrib(default=None)
-    namespace = attrib(default=None)
-    attachments = attrib(default=Factory(list))
-    parameters = attrib(default=Factory(dict))
-    properties = attrib(default=Factory(dict))
-    classname = attrib(default=None)
-    title = attrib(default=None)
-    description = attrib(default=None)
-    links = attrib(default=Factory(list))
-    labels = attrib(default=Factory(list))
-    workItemsID = attrib(default=Factory(list))  # noqa: N815
-    message = attrib(default="")
-    started_on = attrib(default=None)
-    completed_on = attrib(default=None)
-
-    step_depth = attrib(default=Factory(list))
-    result_depth = attrib(default=Factory(list))
-
-    def add_attributes(self, attrs):
-        self.title = attrs['originalname']
-        self.autoTestName = attrs['originalname']
-        self.description = attrs['doc']
-        self.template = attrs['template']
-        self.classname = attrs['longname'].split('.')[-2]
-        for tag in attrs['tags']:
-            if tag.lower().startswith('testgear.'):
-                attr = re.findall(r'(?<=\.).*?(?=:)', tag)[0].strip().lower()
-                value = tag.split(':', 1)[-1].strip()
-                if attr == 'externalid':
-                    self.externalID = str(value).replace("'", "").replace('"', '')
-                elif attr == 'displayname':
-                    self.autoTestName = str(value).replace("'", "").replace('"', '')
-                elif attr == 'title':
-                    self.title = str(value).replace("'", "").replace('"', '')
-                elif attr == 'description':
-                    self.description = str(value).replace("'", "").replace('"', '')
-                elif attr == 'workitemsid' or attr == 'workitemsids':
-                    value = ast.literal_eval(value)
-                    if isinstance(value, (str, int)):
-                        self.workItemsID.append(str(value))
-                    elif isinstance(value, list):
-                        self.workItemsID.extend([str(i) for i in value])
-                    else:
-                        logger.error(f"[TestGear] Wrong workitem format: {value}")
-                elif attr == 'links':
-                    value = ast.literal_eval(value)
-                    try:
-                        if isinstance(value, dict):
-                            self.links.append(Link(**value))
-                        elif isinstance(value, list):
-                            self.links.extend([Link(**link) for link in value if isinstance(link, dict)])
-                    except ValueError as e:
-                        logger.error(f"[TestGear] Link Error: {e}")
-                elif attr == 'labels':
-                    value = ast.literal_eval(value)
-                    if isinstance(value, (str, int)):
-                        self.labels.append(Label(value))
-                    elif isinstance(value, list):
-                        self.labels.extend([Label(item) for item in value if isinstance(item, (str, int))])
-                else:
-                    logger.error(f"[TestGear] Unknown attribute: {attr}")
-        if not self.externalID:
-            self.externalID = Utils.get_hash(attrs['longname'].split('.', 1)[-1])
-
-    def add_step(self, step_type, title, description, parameters):
-        if len(self.step_depth) == 0:
-            if step_type.lower() == 'setup':
-                self.setUp.append(Step(title, description))
-                self.step_depth.append(self.setUp[-1])
-                self.setUpResults.append(StepResult(title, description, parameters=parameters))
-                self.result_depth.append(self.setUpResults[-1])
-            elif step_type.lower() == 'teardown':
-                self.tearDown.append(Step(title, description))
-                self.step_depth.append(self.tearDown[-1])
-                self.tearDownResults.append(StepResult(title, description, parameters=parameters))
-                self.result_depth.append(self.tearDownResults[-1])
-            else:
-                self.steps.append(Step(title, description))
-                self.step_depth.append(self.steps[-1])
-                self.stepResults.append(StepResult(title, description, parameters=parameters))
-                self.result_depth.append(self.stepResults[-1])
-        elif 1 <= len(self.step_depth) < 14:
-            self.step_depth[-1].steps.append(Step(title, description))
-            self.step_depth.append(self.step_depth[-1].steps[-1])
-            self.result_depth[-1].step_results.append(StepResult(title, description, parameters=parameters))
-            self.result_depth.append(self.result_depth[-1].step_results[-1])
-
-    def add_step_result(self, title, start, complete, duration, outcome):
-        if self.result_depth:
-            if self.result_depth[-1].title == title:
-                step = self.result_depth.pop()
-                step.started_on = start
-                step.completed_on = complete
-                step.duration = duration
-                step.outcome = outcome
-        if self.step_depth:
-            if self.step_depth[-1].title == title:
-                self.step_depth.pop()
-
-
-class Option:
-
-    def __init__(self, **kwargs):
-        if kwargs.get('tmsUrl', None):
-            self.set_url = kwargs.get('tmsUrl', None)
-        if kwargs.get('tmsPrivateToken', None):
-            self.set_private_token = kwargs.get('tmsPrivateToken', None)
-        if kwargs.get('tmsProjectId', None):
-            self.set_project_id = kwargs.get('tmsProjectId', None)
-        if kwargs.get('tmsConfigurationId', None):
-            self.set_configuration_id = kwargs.get('tmsConfigurationId', None)
-        if kwargs.get('tmsTestRunId', None):
-            self.set_test_run_id = kwargs.get('tmsTestRunId', None)
-        if kwargs.get('tmsTestRunId', None):
-            self.set_tms_proxy = kwargs.get('tmsTestRunId', None)
-        if kwargs.get('tmsTestRunName', None):
-            self.set_test_run_name = kwargs.get('tmsTestRunName', None)
-        if kwargs.get('tmsAdapterMode', None):
-            self.set_adapter_mode = kwargs.get('tmsAdapterMode', None)
-        if kwargs.get('tmsConfigFile', None):
-            self.set_config_file = kwargs.get('tmsConfigFile', None)
-        if kwargs.get('tmsCertValidation', None):
-            self.set_cert_validation = kwargs.get('tmsCertValidation', None)
-        if kwargs.get('tmsAutomaticCreationTestCases', None):
-            self.set_automatic_creation_test_cases = kwargs.get('tmsAutomaticCreationTestCases', None)
+import ast
+import re
+
+from attr import Factory, asdict, attrib, s
+
+from robot.api import logger
+
+from testgear_python_commons.services import Utils
+
+LinkTypes = ['Related', 'BlockedBy', 'Defect', 'Issue', 'Requirement', 'Repository']
+
+
+def link_type_check(self, attribute, value):
+    if value.title() not in LinkTypes:
+        raise ValueError(f"Incorrect Link type: {value}")
+
+
+def url_check(self, attribute, value):
+    if not bool(re.match(
+            r"(https?|ftp)://"
+            r"(\w+(-\w+)*\.)?"
+            r"((\w+(-\w+)*)\.(\w+))"
+            r"(\.\w+)*"
+            r"([\w\-._~/]*)*(?<!\.)",
+            value)):
+        raise ValueError(f"Incorrect URL: {value}")
+
+
+class Default:
+
+    def order(self):
+        return asdict(self)
+
+
+@s
+class StepResult(Default):
+    title = attrib(default='')
+    description = attrib(default='')
+    started_on = attrib(default=None)
+    completed_on = attrib(default=None)
+    duration = attrib(default=None)
+    outcome = attrib(default=None)
+    step_results = attrib(default=Factory(list))
+    attachments = attrib(default=Factory(list))
+    parameters = attrib(default=Factory(dict))
+
+
+@s
+class Step(Default):
+    title = attrib()
+    description = attrib()
+    steps = attrib(default=Factory(list))
+
+
+@s(kw_only=True)
+class Link:
+    url = attrib(validator=[url_check])
+    type = attrib(default='Defect', validator=[link_type_check])  # noqa: A003,VNE003
+    title = attrib(default='')
+    description = attrib(default='')
+
+    def __attrs_post_init__(self):
+        self.type = self.type.title()
+
+
+@s
+class Label:
+    name = attrib()
+
+
+@s(kw_only=True)
+class Autotest(Default):
+    externalID = attrib(default=None)  # noqa: N815
+    autoTestName = attrib()  # noqa: N815
+    steps = attrib(default=Factory(list))
+    stepResults = attrib(default=Factory(list))  # noqa: N815
+    setUp = attrib(default=Factory(list))  # noqa: N815
+    setUpResults = attrib(default=Factory(list))  # noqa: N815
+    tearDown = attrib(default=Factory(list))  # noqa: N815
+    tearDownResults = attrib(default=Factory(list))  # noqa: N815
+    resultLinks = attrib(default=Factory(list))  # noqa: N815
+    duration = attrib(default=None)
+    failureReasonNames = attrib(default=Factory(list))  # noqa: N815
+    traces = attrib(default=None)
+    outcome = attrib(default=None)
+    namespace = attrib(default=None)
+    attachments = attrib(default=Factory(list))
+    parameters = attrib(default=Factory(dict))
+    properties = attrib(default=Factory(dict))
+    classname = attrib(default=None)
+    title = attrib(default=None)
+    description = attrib(default=None)
+    links = attrib(default=Factory(list))
+    labels = attrib(default=Factory(list))
+    workItemsID = attrib(default=Factory(list))  # noqa: N815
+    message = attrib(default="")
+    started_on = attrib(default=None)
+    completed_on = attrib(default=None)
+
+    step_depth = attrib(default=Factory(list))
+    result_depth = attrib(default=Factory(list))
+
+    def add_attributes(self, attrs):
+        self.title = attrs['originalname']
+        self.autoTestName = attrs['originalname']
+        self.description = attrs['doc']
+        self.template = attrs['template']
+        self.classname = attrs['longname'].split('.')[-2]
+        for tag in attrs['tags']:
+            if tag.lower().startswith('testgear.'):
+                attr = re.findall(r'(?<=\.).*?(?=:)', tag)[0].strip().lower()
+                value = tag.split(':', 1)[-1].strip()
+                if attr == 'externalid':
+                    self.externalID = str(value).replace("'", "").replace('"', '')
+                elif attr == 'displayname':
+                    self.autoTestName = str(value).replace("'", "").replace('"', '')
+                elif attr == 'title':
+                    self.title = str(value).replace("'", "").replace('"', '')
+                elif attr == 'description':
+                    self.description = str(value).replace("'", "").replace('"', '')
+                elif attr == 'workitemsid' or attr == 'workitemsids':
+                    value = ast.literal_eval(value)
+                    if isinstance(value, (str, int)):
+                        self.workItemsID.append(str(value))
+                    elif isinstance(value, list):
+                        self.workItemsID.extend([str(i) for i in value])
+                    else:
+                        logger.error(f"[TestGear] Wrong workitem format: {value}")
+                elif attr == 'links':
+                    value = ast.literal_eval(value)
+                    try:
+                        if isinstance(value, dict):
+                            self.links.append(Link(**value))
+                        elif isinstance(value, list):
+                            self.links.extend([Link(**link) for link in value if isinstance(link, dict)])
+                    except ValueError as e:
+                        logger.error(f"[TestGear] Link Error: {e}")
+                elif attr == 'labels':
+                    value = ast.literal_eval(value)
+                    if isinstance(value, (str, int)):
+                        self.labels.append(Label(value))
+                    elif isinstance(value, list):
+                        self.labels.extend([Label(item) for item in value if isinstance(item, (str, int))])
+                elif attr == 'namespace':
+                    self.namespace = str(value).replace("'", "").replace('"', '')
+                elif attr == 'classname':
+                    self.classname = str(value).replace("'", "").replace('"', '')
+                else:
+                    logger.error(f"[TestGear] Unknown attribute: {attr}")
+        if not self.externalID:
+            self.externalID = Utils.get_hash(attrs['longname'].split('.', 1)[-1])
+
+    def add_step(self, step_type, title, description, parameters):
+        if len(self.step_depth) == 0:
+            if step_type.lower() == 'setup':
+                self.setUp.append(Step(title, description))
+                self.step_depth.append(self.setUp[-1])
+                self.setUpResults.append(StepResult(title, description, parameters=parameters))
+                self.result_depth.append(self.setUpResults[-1])
+            elif step_type.lower() == 'teardown':
+                self.tearDown.append(Step(title, description))
+                self.step_depth.append(self.tearDown[-1])
+                self.tearDownResults.append(StepResult(title, description, parameters=parameters))
+                self.result_depth.append(self.tearDownResults[-1])
+            else:
+                self.steps.append(Step(title, description))
+                self.step_depth.append(self.steps[-1])
+                self.stepResults.append(StepResult(title, description, parameters=parameters))
+                self.result_depth.append(self.stepResults[-1])
+        elif 1 <= len(self.step_depth) < 14:
+            self.step_depth[-1].steps.append(Step(title, description))
+            self.step_depth.append(self.step_depth[-1].steps[-1])
+            self.result_depth[-1].step_results.append(StepResult(title, description, parameters=parameters))
+            self.result_depth.append(self.result_depth[-1].step_results[-1])
+
+    def add_step_result(self, title, start, complete, duration, outcome):
+        if self.result_depth:
+            if self.result_depth[-1].title == title:
+                step = self.result_depth.pop()
+                step.started_on = start
+                step.completed_on = complete
+                step.duration = duration
+                step.outcome = outcome
+        if self.step_depth:
+            if self.step_depth[-1].title == title:
+                self.step_depth.pop()
+
+
+class Option:
+
+    def __init__(self, **kwargs):
+        if kwargs.get('tmsUrl', None):
+            self.set_url = kwargs.get('tmsUrl', None)
+        if kwargs.get('tmsPrivateToken', None):
+            self.set_private_token = kwargs.get('tmsPrivateToken', None)
+        if kwargs.get('tmsProjectId', None):
+            self.set_project_id = kwargs.get('tmsProjectId', None)
+        if kwargs.get('tmsConfigurationId', None):
+            self.set_configuration_id = kwargs.get('tmsConfigurationId', None)
+        if kwargs.get('tmsTestRunId', None):
+            self.set_test_run_id = kwargs.get('tmsTestRunId', None)
+        if kwargs.get('tmsTestRunId', None):
+            self.set_tms_proxy = kwargs.get('tmsTestRunId', None)
+        if kwargs.get('tmsTestRunName', None):
+            self.set_test_run_name = kwargs.get('tmsTestRunName', None)
+        if kwargs.get('tmsAdapterMode', None):
+            self.set_adapter_mode = kwargs.get('tmsAdapterMode', None)
+        if kwargs.get('tmsConfigFile', None):
+            self.set_config_file = kwargs.get('tmsConfigFile', None)
+        if kwargs.get('tmsCertValidation', None):
+            self.set_cert_validation = kwargs.get('tmsCertValidation', None)
+        if kwargs.get('tmsAutomaticCreationTestCases', None):
+            self.set_automatic_creation_test_cases = kwargs.get('tmsAutomaticCreationTestCases', None)
```

### Comparing `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/PKG-INFO` & `testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,297 +1,227 @@
-Metadata-Version: 2.1
-Name: testgear-adapter-robotframework
-Version: 2.1.2
-Summary: Robot Framework adapter for Test Gear
-Home-page: https://github.com/testgear-tms/adapters-python/
-Author: Integration team
-Author-email: integrations@test-gear.io
-License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
-# Test Gear TMS adapter for Robot Framework
-![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-
-## Getting Started
-
-### Installation
-```
-pip install testgear-adapter-robotframework
-```
-
-## Usage
-
-### Configuration
-
-#### File
-
-1. Create **connection_config.ini** file in the root directory of the project:
-    ```
-    [testgear]
-    URL = <url>
-    privateToken = <token>
-    projectId = <id>
-    configurationId = <id>
-    testRunId = <optional id>
-    testRunName = <optional name>
-    adapterMode = <optional>
-    certValidation = <optional boolean>
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
-    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
-      
-    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
-    
-    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
-        
-        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
-        * 1 - in this mode, the adapter sends all results to the test run without filtering.
-        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-   
-    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-    
-    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-    
-3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
-  
-* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
-  
-* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
-  
-* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
-
-* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-
-#### Command line
-
-You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
-* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
-  
-* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
-  
-* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
-
-* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-
-* `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
-
-#### Examples
-
-Launch with a connection_config.ini file in the root directory of the project:
-
-```
-$ robot -v testgear <test directory>
-```
-
-Launch with command-line parameters (parameters are case-insensitive):
-
-```
-$ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
-```
-
-If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-
-### Tags
-
-Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
-
-Description of tags:
-- `testgear.workItemsId` - linking an autotest to a test case
-- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
-- `testgear.externalId` - ID of the autotest within the project in the TMS System
-- `testgear.title` - title in the autotest card (default - name of test)
-- `testgear.description` - description in the autotest card (default - documentation of test)
-- `testgear.links` - links in the autotest card
-- `testgear.labels` - labels in the autotest card
-- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
-- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
-
-Description of methods:
-- `Add Links` - links in the autotest result
-- `Add Link` - add one link in the autotest result
-- `Add Attachments` - uploading files in the autotest result
-- `Add Attachment` - upload given content with given filename in the autotest result
-- `Add Message` - information about autotest in the autotest result
-
-### Parallel execution
-
-You can also run your test in parallel with [Pabot](https://pabot.org/).
-
-```
-$ pabot --pabotlib -v testgear <test directory>
-```
-
-All other settings are the same as for standard execution.
-
-### Examples
-
-```robotframework
-*** Settings ***
-Documentation      Main Suite with examples
-Library            testgear_adapter_robotframework.TMSLibrary
-
-*** Variables ***
-&{SIMPLE_LINK}             url=http://google.com
-&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
-
-@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
-
-
-*** Test Cases ***
-Simple Test
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with link as variable
-    [Tags]   testgear.links:${SIMPLE_LINK}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with link as dict
-    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with WorkitemId as string
-    [Tags]   testgear.workitemsID:123
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with WorkitemId as list
-    [Tags]   testgear.workitemsID:${{[123, '456']}}
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Simple Test with Title or Description or DisplayName with simple formatting
-    [Documentation]  Tags are space sensitive, use only one space between words
-    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
-    ...    testgear.description:"This works too"
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Log  I'am a step
-    [Teardown]  Teardown
-
-Test With All Params
-    [Documentation]  It's better to use this kind of formatting for different data types in tags
-    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
-    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
-    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
-    [Setup]  Setup
-    Log    Something
-    Log    Another
-    [Teardown]  Teardown
-
-Test With Add Link
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Add Links    @{LINKS}
-#    You can also add one link (default type is Defect)
-    Add Link    http://ya.ru
-    Add Link    http://ya.ru    type=Issue
-    Add Link    ${SIMPLE_LINK}[url]
-    [Teardown]  Teardown
-
-Test With Add Attachment
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    ${V}   Get Variables
-    Add Attachment    '${V}'    file.txt
-    Add Attachments    images/banner.png     images/icon.png
-    [Teardown]  Teardown
-
-Test With Add Message
-    [Setup]  Setup
-    Do Something
-    Do Another Thing
-    Add Message    Wow, it's my error message!
-    Fail
-    [Teardown]  Teardown
-```
-
-# Contributing
-
-You can help to develop the project. Any contributions are **greatly appreciated**.
-
-* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-* Please make sure you check your spelling and grammar.
-* Create individual PR for each suggestion.
-* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-
-# License
-
-Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
-
+Metadata-Version: 2.1
+Name: testgear-adapter-robotframework
+Version: 2.1.3
+Summary: Robot Framework adapter for Test Gear
+Home-page: https://github.com/testgear-tms/adapters-python/
+Author: Integration team
+Author-email: integrations@test-gear.io
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# Test Gear TMS adapter for Robot Framework
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+```
+pip install testgear-adapter-robotframework
+```
+
+## Usage
+
+### Configuration
+
+| Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
+| Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
+| API secret key [How to getting API secret key?](https://github.com/testgear-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                          | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
+| ID of project in TMS instance [How to getting project ID?](https://github.com/testgear-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                  | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
+| ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testgear-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
+| ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
+| Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
+| Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
+| It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
+| Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
+| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
+
+#### File
+
+Create **connection_config.ini** file in the root directory of the project:
+```
+[testgear]
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
+
+#### Examples
+
+Launch with a connection_config.ini file in the root directory of the project:
+
+```
+$ robot -v testgear TEST_DIRECTORY
+```
+
+Launch with command-line parameters (parameters are case-insensitive):
+
+```
+$ robot -v testgear -v tmsUrl:URL -v tmsPrivateToken:USER_PRIVATE_TOKEN -v tmsProjectId:PROJECT_ID -v tmsConfigurationId:CONFIGURATION_ID -v tmsTestRunId:TEST_RUN_ID -v tmsTestRunName:TEST_RUN_NAME -v tmsAdapterMode:ADAPTER_MODE -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:CONFIG_FILE_NAME -v tmsCertValidation:CERT_VALIDATION -v tmsAutomaticCreationTestCases:AUTOMATIC_CREATION_TEST_CASES TEST_DIRECTORY
+```
+
+If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
+
+Description of tags:
+- `testgear.workItemsId` - linking an autotest to a test case
+- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
+- `testgear.externalId` - ID of the autotest within the project in the TMS System
+- `testgear.title` - title in the autotest card (default - name of test)
+- `testgear.description` - description in the autotest card (default - documentation of test)
+- `testgear.links` - links in the autotest card
+- `testgear.labels` - labels in the autotest card
+- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
+- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+- `Add Links` - links in the autotest result
+- `Add Link` - add one link in the autotest result
+- `Add Attachments` - uploading files in the autotest result
+- `Add Attachment` - upload given content with given filename in the autotest result
+- `Add Message` - information about autotest in the autotest result
+
+### Parallel execution
+
+You can also run your test in parallel with [Pabot](https://pabot.org/).
+
+```
+$ pabot --pabotlib -v testgear <test directory>
+```
+
+All other settings are the same as for standard execution.
+
+### Examples
+
+```robotframework
+*** Settings ***
+Documentation      Main Suite with examples
+Library            testgear_adapter_robotframework.TMSLibrary
+
+*** Variables ***
+&{SIMPLE_LINK}             url=http://google.com
+&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
+
+@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
+
+
+*** Test Cases ***
+Simple Test
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as variable
+    [Tags]   testgear.links:${SIMPLE_LINK}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as dict
+    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as string
+    [Tags]   testgear.workitemsID:123
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as list
+    [Tags]   testgear.workitemsID:${{[123, '456']}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with Title or Description or DisplayName with simple formatting
+    [Documentation]  Tags are space sensitive, use only one space between words
+    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
+    ...    testgear.description:"This works too"
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Test With All Params
+    [Documentation]  It's better to use this kind of formatting for different data types in tags
+    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
+    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
+    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
+    [Setup]  Setup
+    Log    Something
+    Log    Another
+    [Teardown]  Teardown
+
+Test With Add Link
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Links    @{LINKS}
+#    You can also add one link (default type is Defect)
+    Add Link    http://ya.ru
+    Add Link    http://ya.ru    type=Issue
+    Add Link    ${SIMPLE_LINK}[url]
+    [Teardown]  Teardown
+
+Test With Add Attachment
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    ${V}   Get Variables
+    Add Attachment    '${V}'    file.txt
+    Add Attachments    images/banner.png     images/icon.png
+    [Teardown]  Teardown
+
+Test With Add Message
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Message    Wow, it's my error message!
+    Fail
+    [Teardown]  Teardown
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/SOURCES.txt` & `testgear-adapter-robotframework-2.1.3/src/testgear_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-requirements.txt
 setup.py
 src/testgear_adapter_robotframework/TMSLibrary.py
 src/testgear_adapter_robotframework/__init__.py
 src/testgear_adapter_robotframework/listeners.py
 src/testgear_adapter_robotframework/models.py
 src/testgear_adapter_robotframework/utils.py
 src/testgear_adapter_robotframework.egg-info/PKG-INFO
```


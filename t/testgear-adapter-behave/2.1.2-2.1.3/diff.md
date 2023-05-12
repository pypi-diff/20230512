# Comparing `tmp/testgear-adapter-behave-2.1.2.tar.gz` & `tmp/testgear-adapter-behave-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-behave-2.1.2.tar", last modified: Fri Apr 21 14:57:11 2023, max compression
+gzip compressed data, was "testgear-adapter-behave-2.1.3.tar", last modified: Fri May 12 09:41:20 2023, max compression
```

## Comparing `testgear-adapter-behave-2.1.2.tar` & `testgear-adapter-behave-2.1.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/
--rw-rw-rw-   0        0        0     9537 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8983 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.2/README.md
--rw-rw-rw-   0        0        0       48 2023-04-21 13:48:08.000000 testgear-adapter-behave-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-21 14:02:35.000000 testgear-adapter-behave-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.484461 testgear-adapter-behave-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-04-21 14:01:40.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/formatter.py
--rw-rw-rw-   0        0        0     4152 2023-04-21 14:01:40.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/listener.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/__init__.py
--rw-rw-rw-   0        0        0      131 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/label.py
--rw-rw-rw-   0        0        0      513 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/option.py
--rw-rw-rw-   0        0        0      282 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/tags.py
--rw-rw-rw-   0        0        0      393 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/test_result_step.py
--rw-rw-rw-   0        0        0      269 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/url_link.py
--rw-rw-rw-   0        0        0     4323 2023-04-21 14:01:40.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/scenario_parser.py
--rw-rw-rw-   0        0        0     2314 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/tags_parser.py
--rw-rw-rw-   0        0        0     2695 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/
--rw-rw-rw-   0        0        0     9537 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:20.850715 testgear-adapter-behave-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-05-12 09:41:20.850715 testgear-adapter-behave-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:41:20.850715 testgear-adapter-behave-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:20.846715 testgear-adapter-behave-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:20.850715 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:20.850715 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/models/url_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/scenario_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/tags_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-12 09:41:04.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:20.850715 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-05-12 09:41:20.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-12 09:41:20.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:41:20.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 09:41:20.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 09:41:20.000000 testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/top_level.txt
```

### Comparing `testgear-adapter-behave-2.1.2/PKG-INFO` & `testgear-adapter-behave-2.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,297 +1,207 @@
-Metadata-Version: 2.1
-Name: testgear-adapter-behave
-Version: 2.1.2
-Summary: Behave adapter for Test Gear
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
-# Test Gear TMS adapter for Behave
-
-![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-
-## Getting Started
-
-### Installation
-
-```
-pip install testgear-adapter-behave
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
-    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
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
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
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
-* `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
-
-#### Examples
-
-Launch with a connection_config.ini file in the root directory of the project:
-
-```
-$ behave -f testgear_adapter_behave.formatter:AdapterFormatter
-```
-
-Launch with command-line parameters:
-
-```
-$ behave -f testgear_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
-tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
-tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D tmsCertValidation=<optional boolean>
-```
-
-If you want to enable debug mode then
-see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-
-### Tags
-
-Use tags to specify information about autotest.
-
-Description of tags:
-
-- `WorkItemIds` - linking an autotest to a test case.
-- `DisplayName` - name of the autotest in TMS.
-- `ExternalId` - ID of the autotest within the project in TMS.
-- `Title` - title in the autotest card.
-- `Description` - description in the autotest card.
-- `Labels` - tags in the autotest card.
-- `Links` - links in the autotest card.
-- `NameSpace` - directory in the TMS system (default - file's name of test)
-- `ClassName` - subdirectory in the TMS system (default - class's name of test)
-
-Description of methods:
-
-- `testgear.addLinks` - links in the autotest result
-- `testgear.addAttachments` - uploading files in the autotest result
-- `testgear.addMessage` - information about autotest in the autotest result
-- `testgear.step` - usage in the "with" construct to designation a step in the body of the test
-
-### Examples
-
-#### Simple Test
-
-```py
-import testgear
-from behave import given
-from behave import then
-from behave import when
-
-
-@given("I authorize on the portal")
-def authorization(context):
-    with testgear.step("I set login"):
-        pass
-    with testgear.step("I set password"):
-        pass
-
-
-@when("I create a project")
-def create_project(context):
-    pass
-
-
-@when("I open the project")
-def enter_project(context):
-    pass
-
-
-@when("I create a section")
-def create_section(context):
-    testgear.addLinks(
-        title='component_dump.dmp',
-        type=testgear.LinkType.RELATED,
-        url='https://dumps.example.com/module/some_module_dump',
-        description='Description'
-    )
-
-
-@then("I create a test case")
-def create_test_case(context):
-    testgear.addAttachments('pictures/picture.jpg')
-```
-
-```buildoutcfg
-Feature: Sample
-
-  Background:
-    Given I authorize on the portal
-
-  @ExternalId=failed_with_all_annotations
-  @DisplayName=Failed_test_with_all_annotations
-  @WorkItemIds=123
-  @Title=Title_in_the_autotest_card
-  @Description=Test_with_all_annotations
-  @Labels=Tag1,Tag2
-  @Links={"url":"https://dumps.example.com/module/repository","title":"Repository","description":"Example_of_repository","type":"Repository"}
-  Scenario: Create new project, section and test case
-    When I create a project
-    And I open the project
-    And I create a section
-    Then I create a test case
-```
-
-#### Parameterized test
-
-```py
-from behave import when
-from behave import then
-
-
-@when("Summing {left:d}+{right:d}")
-def step_impl(context, left, right):
-    context.sum = left + right
-
-
-@then("Result is {result:d}")
-def step_impl(context, result):
-    assert context.sum == result
-
-```
-
-```buildoutcfg
-Feature: Rule
-  Tests that use Rule
-
-  Scenario Outline: Summing
-    When Summing <left>+<right>
-    Then Result is <result>
-
-    Examples:
-      | left | right | result |
-      | 1    | 1     | 3      |
-      | 9    | 9     | 18     |
-```
-
-# Contributing
-
-You can help to develop the project. Any contributions are **greatly appreciated**.
-
-* If you have suggestions for adding or removing projects, feel free
-  to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull
-  request after you edit the *README.md* file with necessary changes.
-* Please make sure you check your spelling and grammar.
-* Create individual PR for each suggestion.
-* Please also read through
-  the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting
-  your first idea as well.
-
-# License
-
-Distributed under the Apache-2.0 License.
-See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
-
+# Test Gear TMS adapter for Behave
+
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+
+```
+pip install testgear-adapter-behave
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
+$ behave -f testgear_adapter_behave.formatter:AdapterFormatter
+```
+
+Launch with command-line parameters:
+
+```
+$ behave -f testgear_adapter_behave.formatter:AdapterFormatter -D tmsUrl=URL -D tmsPrivateToken=USER_PRIVATE_TOKEN -D
+tmsProjectId=PROJECT_ID -D tmsConfigurationId=CONFIGURATION_ID -D tmsTestRunId=TEST_RUN_ID -D tmsAdapterMode=ADAPTER_MODE -D
+tmsTestRunName=TEST_RUN_NAME -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D
+tmsCertValidation=CERT_VALIDATION -D tmsAutomaticCreationTestCases=AUTOMATIC_CREATION_TEST_CASES
+```
+
+If you want to enable debug mode then
+see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Use tags to specify information about autotest.
+
+Description of tags:
+
+- `WorkItemIds` - linking an autotest to a test case.
+- `DisplayName` - name of the autotest in TMS.
+- `ExternalId` - ID of the autotest within the project in TMS.
+- `Title` - title in the autotest card.
+- `Description` - description in the autotest card.
+- `Labels` - tags in the autotest card.
+- `Links` - links in the autotest card.
+- `NameSpace` - directory in the TMS system (default - file's name of test)
+- `ClassName` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+
+- `testgear.addLinks` - links in the autotest result
+- `testgear.addAttachments` - uploading files in the autotest result
+- `testgear.addMessage` - information about autotest in the autotest result
+- `testgear.step` - usage in the "with" construct to designation a step in the body of the test
+
+### Examples
+
+#### Simple Test
+
+```py
+import testgear
+from behave import given
+from behave import then
+from behave import when
+
+
+@given("I authorize on the portal")
+def authorization(context):
+    with testgear.step("I set login"):
+        pass
+    with testgear.step("I set password"):
+        pass
+
+
+@when("I create a project")
+def create_project(context):
+    pass
+
+
+@when("I open the project")
+def enter_project(context):
+    pass
+
+
+@when("I create a section")
+def create_section(context):
+    testgear.addLinks(
+        title='component_dump.dmp',
+        type=testgear.LinkType.RELATED,
+        url='https://dumps.example.com/module/some_module_dump',
+        description='Description'
+    )
+
+
+@then("I create a test case")
+def create_test_case(context):
+    testgear.addAttachments('pictures/picture.jpg')
+```
+
+```buildoutcfg
+Feature: Sample
+
+  Background:
+    Given I authorize on the portal
+
+  @ExternalId=failed_with_all_annotations
+  @DisplayName=Failed_test_with_all_annotations
+  @WorkItemIds=123
+  @Title=Title_in_the_autotest_card
+  @Description=Test_with_all_annotations
+  @Labels=Tag1,Tag2
+  @Links={"url":"https://dumps.example.com/module/repository","title":"Repository","description":"Example_of_repository","type":"Repository"}
+  Scenario: Create new project, section and test case
+    When I create a project
+    And I open the project
+    And I create a section
+    Then I create a test case
+```
+
+#### Parameterized test
+
+```py
+from behave import when
+from behave import then
+
+
+@when("Summing {left:d}+{right:d}")
+def step_impl(context, left, right):
+    context.sum = left + right
+
+
+@then("Result is {result:d}")
+def step_impl(context, result):
+    assert context.sum == result
+
+```
+
+```buildoutcfg
+Feature: Rule
+  Tests that use Rule
+
+  Scenario Outline: Summing
+    When Summing <left>+<right>
+    Then Result is <result>
+
+    Examples:
+      | left | right | result |
+      | 1    | 1     | 3      |
+      | 9    | 9     | 18     |
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free
+  to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull
+  request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through
+  the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting
+  your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License.
+See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-behave-2.1.2/setup.py` & `testgear-adapter-behave-2.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import find_packages, setup
-
-setup(
-    name='testgear-adapter-behave',
-    version='2.1.2',
-    description='Behave adapter for Test Gear',
-    long_description=open('README.md', "r").read(),
-    long_description_content_type="text/markdown",
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
-    ],
-    py_modules=['testgear_adapter_behave'],
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
-    install_requires=[
-        'behave',
-        'testgear-python-commons==2.1.2',
-        'attrs'],
-)
+from setuptools import find_packages, setup
+
+setup(
+    name='testgear-adapter-behave',
+    version='2.1.3',
+    description='Behave adapter for Test Gear',
+    long_description=open('README.md', "r").read(),
+    long_description_content_type="text/markdown",
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
+    ],
+    py_modules=['testgear_adapter_behave'],
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
+    install_requires=[
+        'behave',
+        'testgear-python-commons==2.1.3',
+        'attrs'],
+)
```

### Comparing `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/formatter.py` & `testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/formatter.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from behave.formatter.base import Formatter
-
-from testgear_python_commons.services import TmsPluginManager
-
-from .listener import AdapterListener
-from .utils import filter_out_scenarios, parse_userdata
-
-
-class AdapterFormatter(Formatter):
-    __adapter_launch_is_started = False
-    __tests_for_launch = None
-
-    def __init__(self, stream_opener, config):
-        super(AdapterFormatter, self).__init__(stream_opener, config)
-
-        option = parse_userdata(config.userdata)
-
-        self.__listener = AdapterListener(
-            TmsPluginManager.get_adapter_manager(option))
-
-        TmsPluginManager.get_plugin_manager().register(self.__listener)
-
-    def start_adapter_launch(self):
-        self.__listener.start_launch()
-
-        self.__tests_for_launch = self.__listener.get_tests_for_launch()
-        self.__adapter_launch_is_started = True
-
-    def uri(self, uri):
-        if not self.__adapter_launch_is_started:
-            self.start_adapter_launch()
-
-    def feature(self, feature):
-        feature.scenarios = filter_out_scenarios(
-            self.__tests_for_launch,
-            feature.scenarios)
-
-    def scenario(self, scenario):
-        self.__listener.get_scenario(scenario)
-
-    def match(self, match):
-        self.__listener.get_step_parameters(match)
-
-    def result(self, step):
-        self.__listener.get_step_result(step)
+from behave.formatter.base import Formatter
+
+from testgear_python_commons.services import TmsPluginManager
+
+from .listener import AdapterListener
+from .utils import filter_out_scenarios, parse_userdata
+
+
+class AdapterFormatter(Formatter):
+    __adapter_launch_is_started = False
+    __tests_for_launch = None
+
+    def __init__(self, stream_opener, config):
+        super(AdapterFormatter, self).__init__(stream_opener, config)
+
+        option = parse_userdata(config.userdata)
+
+        self.__listener = AdapterListener(
+            TmsPluginManager.get_adapter_manager(option))
+
+        TmsPluginManager.get_plugin_manager().register(self.__listener)
+
+    def start_adapter_launch(self):
+        self.__listener.start_launch()
+
+        self.__tests_for_launch = self.__listener.get_tests_for_launch()
+        self.__adapter_launch_is_started = True
+
+    def uri(self, uri):
+        if not self.__adapter_launch_is_started:
+            self.start_adapter_launch()
+
+    def feature(self, feature):
+        feature.scenarios = filter_out_scenarios(
+            self.__tests_for_launch,
+            feature.scenarios)
+
+    def scenario(self, scenario):
+        self.__listener.get_scenario(scenario)
+
+    def match(self, match):
+        self.__listener.get_step_parameters(match)
+
+    def result(self, step):
+        self.__listener.get_step_result(step)
```

### Comparing `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/listener.py` & `testgear-adapter-behave-2.1.3/src/testgear_adapter_behave/listener.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import testgear_python_commons.services as adapter
-from testgear_python_commons.models.outcome_type import OutcomeType
-from testgear_python_commons.services import AdapterManager
-from testgear_python_commons.step import Step
-
-from .models.test_result_step import get_test_result_step_model
-from .scenario_parser import (
-    parse_scenario,
-    parse_status)
-from .utils import (
-    convert_step_to_step,
-    convert_step_to_step_result)
-
-
-class AdapterListener(object):
-    __executable_test = None
-    __background_steps_count = 0
-    __steps_count = 0
-
-    def __init__(self, adapter_manager: AdapterManager):
-        self.__adapter_manager = adapter_manager
-
-    def start_launch(self):
-        test_run_id = self.__adapter_manager.get_test_run_id()
-
-        self.__adapter_manager.set_test_run_id(test_run_id)
-
-    def get_tests_for_launch(self):
-        return self.__adapter_manager.get_autotests_for_launch()
-
-    def get_scenario(self, scenario):
-        self.__executable_test = parse_scenario(scenario)
-        self.__background_steps_count = len(scenario.background_steps)
-        self.__steps_count = len(scenario.steps)
-
-    def set_scenario(self):
-        self.__adapter_manager.write_test(self.__executable_test)
-
-    def get_step_parameters(self, match):
-        scope = self.get_scope()
-
-        executable_step = get_test_result_step_model()
-
-        for argument in match.arguments:
-            name = argument.name if argument.name else 'param' + str(match.arguments.index(argument))
-            executable_step['description'] += f'{name} = {argument.original} '
-            executable_step['parameters'][name] = argument.original
-
-        self.__executable_test[scope].append(executable_step)
-
-    def get_step_result(self, result):
-        scope = self.get_scope()
-        outcome = parse_status(result.status)
-
-        self.__executable_test[scope][-1]['title'] = result.name
-        self.__executable_test[scope][-1]['outcome'] = outcome
-        self.__executable_test[scope][-1]['duration'] = round(result.duration * 1000)
-        self.__executable_test['duration'] += result.duration * 1000
-
-        # TODO: Add to python-commons
-        nested_steps, nested_step_results = Step.get_steps_data()
-        executable_step = self.__executable_test[scope][-1]
-        # TODO: Fix in python-commons
-        result_scope = f'{scope}Results' if scope == 'setUp' else 'stepResults'
-        self.__executable_test[scope][-1] = convert_step_to_step(
-            executable_step,
-            nested_steps)
-        self.__executable_test[result_scope].append(
-            convert_step_to_step_result(
-                executable_step,
-                nested_step_results))
-
-        if outcome != OutcomeType.PASSED:
-            self.__executable_test['traces'] = result.error_message
-            self.__executable_test['outcome'] = outcome
-            self.set_scenario()
-            return
-
-        if scope == 'setUp':
-            self.__background_steps_count -= 1
-            return
-
-        self.__steps_count -= 1
-
-        if self.__steps_count == 0:
-            self.__executable_test['outcome'] = outcome
-            self.set_scenario()
-
-    def get_scope(self):
-        if self.__background_steps_count != 0:
-            return 'setUp'
-
-        return 'steps'
-
-    @adapter.hookimpl
-    def add_link(self, link):
-        if self.__executable_test:
-            self.__executable_test['resultLinks'].append(link)
-
-    @adapter.hookimpl
-    def add_message(self, test_message):
-        if self.__executable_test:
-            self.__executable_test['message'] = str(test_message)
-
-    @adapter.hookimpl
-    def add_attachments(self, attach_paths: list or tuple):
-        if self.__executable_test:
-            self.__executable_test['attachments'] += self.__adapter_manager.load_attachments(attach_paths)
-
-    @adapter.hookimpl
-    def create_attachment(self, body, name: str):
-        if self.__executable_test:
-            self.__executable_test['attachments'] += self.__adapter_manager.create_attachment(body, name)
+import testgear_python_commons.services as adapter
+from testgear_python_commons.models.outcome_type import OutcomeType
+from testgear_python_commons.services import AdapterManager
+from testgear_python_commons.step import Step
+
+from .models.test_result_step import get_test_result_step_model
+from .scenario_parser import (
+    parse_scenario,
+    parse_status)
+from .utils import (
+    convert_step_to_step,
+    convert_step_to_step_result)
+
+
+class AdapterListener(object):
+    __executable_test = None
+    __background_steps_count = 0
+    __steps_count = 0
+
+    def __init__(self, adapter_manager: AdapterManager):
+        self.__adapter_manager = adapter_manager
+
+    def start_launch(self):
+        test_run_id = self.__adapter_manager.get_test_run_id()
+
+        self.__adapter_manager.set_test_run_id(test_run_id)
+
+    def get_tests_for_launch(self):
+        return self.__adapter_manager.get_autotests_for_launch()
+
+    def get_scenario(self, scenario):
+        self.__executable_test = parse_scenario(scenario)
+        self.__background_steps_count = len(scenario.background_steps)
+        self.__steps_count = len(scenario.steps)
+
+    def set_scenario(self):
+        self.__adapter_manager.write_test(self.__executable_test)
+
+    def get_step_parameters(self, match):
+        scope = self.get_scope()
+
+        executable_step = get_test_result_step_model()
+
+        for argument in match.arguments:
+            name = argument.name if argument.name else 'param' + str(match.arguments.index(argument))
+            executable_step['description'] += f'{name} = {argument.original} '
+            executable_step['parameters'][name] = argument.original
+
+        self.__executable_test[scope].append(executable_step)
+
+    def get_step_result(self, result):
+        scope = self.get_scope()
+        outcome = parse_status(result.status)
+
+        self.__executable_test[scope][-1]['title'] = result.name
+        self.__executable_test[scope][-1]['outcome'] = outcome
+        self.__executable_test[scope][-1]['duration'] = round(result.duration * 1000)
+        self.__executable_test['duration'] += result.duration * 1000
+
+        # TODO: Add to python-commons
+        nested_steps, nested_step_results = Step.get_steps_data()
+        executable_step = self.__executable_test[scope][-1]
+        # TODO: Fix in python-commons
+        result_scope = f'{scope}Results' if scope == 'setUp' else 'stepResults'
+        self.__executable_test[scope][-1] = convert_step_to_step(
+            executable_step,
+            nested_steps)
+        self.__executable_test[result_scope].append(
+            convert_step_to_step_result(
+                executable_step,
+                nested_step_results))
+
+        if outcome != OutcomeType.PASSED:
+            self.__executable_test['traces'] = result.error_message
+            self.__executable_test['outcome'] = outcome
+            self.set_scenario()
+            return
+
+        if scope == 'setUp':
+            self.__background_steps_count -= 1
+            return
+
+        self.__steps_count -= 1
+
+        if self.__steps_count == 0:
+            self.__executable_test['outcome'] = outcome
+            self.set_scenario()
+
+    def get_scope(self):
+        if self.__background_steps_count != 0:
+            return 'setUp'
+
+        return 'steps'
+
+    @adapter.hookimpl
+    def add_link(self, link):
+        if self.__executable_test:
+            self.__executable_test['resultLinks'].append(link)
+
+    @adapter.hookimpl
+    def add_message(self, test_message):
+        if self.__executable_test:
+            self.__executable_test['message'] = str(test_message)
+
+    @adapter.hookimpl
+    def add_attachments(self, attach_paths: list or tuple):
+        if self.__executable_test:
+            self.__executable_test['attachments'] += self.__adapter_manager.load_attachments(attach_paths)
+
+    @adapter.hookimpl
+    def create_attachment(self, body, name: str):
+        if self.__executable_test:
+            self.__executable_test['attachments'] += self.__adapter_manager.create_attachment(body, name)
```

### Comparing `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/SOURCES.txt` & `testgear-adapter-behave-2.1.3/src/testgear_adapter_behave.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-requirements.txt
 setup.py
 src/testgear_adapter_behave/__init__.py
 src/testgear_adapter_behave/formatter.py
 src/testgear_adapter_behave/listener.py
 src/testgear_adapter_behave/scenario_parser.py
 src/testgear_adapter_behave/tags_parser.py
 src/testgear_adapter_behave/utils.py
```


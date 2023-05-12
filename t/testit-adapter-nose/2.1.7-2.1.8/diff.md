# Comparing `tmp/testit-adapter-nose-2.1.7.tar.gz` & `tmp/testit-adapter-nose-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-nose-2.1.7.tar", last modified: Fri Apr 21 08:18:14 2023, max compression
+gzip compressed data, was "testit-adapter-nose-2.1.8.tar", last modified: Fri May 12 08:34:55 2023, max compression
```

## Comparing `testit-adapter-nose-2.1.7.tar` & `testit-adapter-nose-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:14.109457 testit-adapter-nose-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-21 08:18:14.109457 testit-adapter-nose-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-21 08:17:56.000000 testit-adapter-nose-2.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:18:14.109457 testit-adapter-nose-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 08:17:56.000000 testit-adapter-nose-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:14.109457 testit-adapter-nose-2.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:14.109457 testit-adapter-nose-2.1.7/src/testit_adapter_nose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:56.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 08:17:56.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-21 08:17:56.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-21 08:17:56.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:18:14.109457 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-21 08:18:14.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-21 08:18:14.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:18:14.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 08:18:14.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:18:14.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 08:18:14.000000 testit-adapter-nose-2.1.7/src/testit_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.148847 testit-adapter-nose-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-12 08:34:55.144847 testit-adapter-nose-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:34:55.148847 testit-adapter-nose-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.140847 testit-adapter-nose-2.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.144847 testit-adapter-nose-2.1.8/src/testit_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.144847 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/top_level.txt
```

### Comparing `testit-adapter-nose-2.1.7/PKG-INFO` & `testit-adapter-nose-2.1.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: testit-adapter-nose
-Version: 2.1.7
-Summary: Nose adapter for Test IT
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
 # Test IT TMS adapter for Nose
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 ## Getting Started
 
 ### Installation
@@ -25,104 +10,47 @@
 pip install testit-adapter-nose
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
-* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. Default value - true.
+#### File
 
-* `TMS_AUTOMATIC_CREATION_TEST_CASES` - mode of automatic creation test cases. Default value - false.
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
 $ nose2 --testit
```

### Comparing `testit-adapter-nose-2.1.7/setup.py` & `testit-adapter-nose-2.1.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testit-adapter-nose',
-    version='2.1.7',
+    version='2.1.8',
     description='Nose adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,14 +16,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.7'],
+    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.8'],
     entry_points={
             'nose.plugins.0.10': [
                 'testit_adapter_nose = testit_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testit-adapter-nose-2.1.7/src/testit_adapter_nose/plugin.py` & `testit-adapter-nose-2.1.8/src/testit_adapter_nose/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.7/src/testit_adapter_nose/utils.py` & `testit-adapter-nose-2.1.8/src/testit_adapter_nose/utils.py`

 * *Files identical despite different names*


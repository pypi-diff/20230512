# Comparing `tmp/pysafeguard-1.0.2.tar.gz` & `tmp/pysafeguard-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysafeguard-1.0.2.tar", max compression
+gzip compressed data, was "pysafeguard-7.3.0.tar", max compression
```

## Comparing `pysafeguard-1.0.2.tar` & `pysafeguard-7.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11357 2022-10-04 18:47:06.892912 pysafeguard-1.0.2/LICENSE
--rw-r--r--   0        0        0    11343 2022-10-04 18:47:50.768725 pysafeguard-1.0.2/README.md
--rw-r--r--   0        0        0     1032 2022-10-04 18:47:44.768276 pysafeguard-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    11340 2022-10-04 18:47:06.892912 pysafeguard-1.0.2/src/pysafeguard.py
--rw-r--r--   0        0        0    12563 1970-01-01 00:00:00.000000 pysafeguard-1.0.2/setup.py
--rw-r--r--   0        0        0    12419 1970-01-01 00:00:00.000000 pysafeguard-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 21:41:42.777650 pysafeguard-7.3.0/LICENSE
+-rw-r--r--   0        0        0    11343 2023-05-12 21:42:02.933882 pysafeguard-7.3.0/README.md
+-rw-r--r--   0        0        0      986 2023-05-12 21:42:01.345866 pysafeguard-7.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11368 2023-05-12 21:41:42.781650 pysafeguard-7.3.0/src/pysafeguard.py
+-rw-r--r--   0        0        0    12473 1970-01-01 00:00:00.000000 pysafeguard-7.3.0/PKG-INFO
```

### Comparing `pysafeguard-1.0.2/LICENSE` & `pysafeguard-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysafeguard-1.0.2/README.md` & `pysafeguard-7.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PySafeguard
 One Identity Safeguard Python SDK
 
 -----------
 
 <p align="center">
-<i>Check out our <a href='https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples'>sample projects</a> to get started with your own custom integration to Safeguard!</i>
+<i>Check out our <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples'>sample projects</a> to get started with your own custom integration to Safeguard!</i>
 </p>
 
 -----------
 
 ## Support
 
 One Identity open source projects are supported through [One Identity GitHub issues](https://github.com/OneIdentity/PySafeguard/issues) and the [One Identity Community](https://www.oneidentity.com/community/). This includes all scripts, plugins, SDKs, modules, code snippets or other solutions. For assistance with any One Identity GitHub project, please raise a new Issue on the [One Identity GitHub project](https://github.com/OneIdentity/PySafeguard/issues) page. You may also visit the [One Identity Community](https://www.oneidentity.com/community/) to ask questions.  Requests for assistance made through official One Identity Support will be referred back to GitHub and the One Identity Community forums where those requests can benefit all users.
@@ -94,15 +94,15 @@
 connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
 connection.connect_password('Admin','Admin123')
 me = connection.invoke(HttpMethods.GET, Services.CORE, 'Me', query=dict(fields='DisplayName'))
 print('Connected to Safeguard as %s' % me.json()['DisplayName'])
 ```
 
 Password authentication to an external provider is as follows:
-(Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/PasswordExternalExample.py'>here</a>.)
+(Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/PasswordExternalExample.py'>here</a>.)
 
 ```Python
 from pysafeguard import *
 
 connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
 connection.connect_password('Admin','Admin123', 'myexternalprovider')
 ```
@@ -201,27 +201,27 @@
 ### Examples
 
 Most functionality is in the core service as mentioned above.  The notification service
 provides read-only information for status, etc.
 
 #### Anonymous Call for Safeguard Status
 
-Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/AnonymousExample.py'>here</a>.
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/AnonymousExample.py'>here</a>.
 
 ```Python
 from pysafeguard import *
 
 connection = PySafeguardConnection('safeguard.sample.corp', False)
 result = connection.invoke(HttpMethods.GET, Services.NOTIFICATION, 'Status')
 print(json.dumps(result.json(),indent=2,sort_keys=True))
 ```
 
 #### Get remaining access token lifetime
 
-Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/PasswordExample.py'>here</a>.
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/PasswordExample.py'>here</a>.
 
 ```Python
 from pysafeguard import *
 
 connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
 connection.connect_password('username', 'password')
 minutes_left = connection.get_remaining_token_lifetime()
@@ -232,15 +232,15 @@
 
 To use the SignalR functionality, you will need to install the python SignalR Core client module
 
 ```Bash
 > pip install signalrcore
 ```
 
-Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/SignalRExample.py'>here</a>.
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/SignalRExample.py'>here</a>.
 
 ```Python
 from pysafeguard import *
 
 connection = PySafeguardConnection(hostName, caFile)
 
 # SignalR callback function to handle the signalR messages
@@ -254,15 +254,15 @@
 connection.register_signalr_certificate(connection, signalrcallback, userCertFile, userKeyFile)
 ```
 > **Note**  
 > Password protected certificates are not currently supported in PySafeguard.
 
 #### Create a New User and Set the Password
 
-Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/NewUserExample.py'>here</a>.
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/NewUserExample.py'>here</a>.
 
 ```Python
 from pysafeguard import *
 import json
 
 user = {
     'PrimaryAuthenticationProvider': { 'Id': -1 },
```

### Comparing `pysafeguard-1.0.2/pyproject.toml` & `pysafeguard-7.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 #https://python-poetry.org/docs/pyproject
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pysafeguard"
 description = "One Identity Safeguard Python Package"
-version = "1.0.2"
+version = "7.3.0"
 readme = "README.md"
 keywords = ["safeguard","oneidentity"]
 repository = "https://github.com/OneIdentity/PySafeguard"
 authors = [
     "Tania Engel <Tania.Engel@oneidentity.com>",
 ]
 maintainers = [
-    "Rich Gagliano <Rich.Gagliano@oneidentity.com>",
-    "Edward Mun <Edward.Mun@oneidentity.com>",
+    "Stephanie Zinn <Stephanie.Zinn@oneidentity.com>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pysafeguard-1.0.2/src/pysafeguard.py` & `pysafeguard-7.3.0/src/pysafeguard.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     POST = requests.post
     PUT = requests.put
     DELETE = requests.delete
 
 class A2ATypes:
     PASSWORD = "password"
     PRIVATEKEY = "privatekey"
+    APIKEYSECRET = "apikey"
 
 class SshKeyFormats:
     OPENSSH = "openssh"
     SSH2 = "ssh2"
     PUTTY = "putty"
 
 class WebRequestError(Exception):
```

### Comparing `pysafeguard-1.0.2/setup.py` & `pysafeguard-7.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,305 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pysafeguard
+Version: 7.3.0
+Summary: One Identity Safeguard Python Package
+Home-page: https://github.com/OneIdentity/PySafeguard
+Keywords: safeguard,oneidentity
+Author: Tania Engel
+Author-email: Tania.Engel@oneidentity.com
+Maintainer: Stephanie Zinn
+Maintainer-email: Stephanie.Zinn@oneidentity.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Provides-Extra: signalr
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: signalrcore (>=0.9.5,<0.10.0) ; extra == "signalr"
+Project-URL: Bug Tracker, https://github.com/OneIdentity/PySafeguard/issues
+Project-URL: Repository, https://github.com/OneIdentity/PySafeguard
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# PySafeguard
+One Identity Safeguard Python SDK
 
-modules = \
-['pysafeguard']
-install_requires = \
-['requests>=2.28.1,<3.0.0']
-
-extras_require = \
-{'signalr': ['signalrcore>=0.9.5,<0.10.0']}
-
-setup_kwargs = {
-    'name': 'pysafeguard',
-    'version': '1.0.2',
-    'description': 'One Identity Safeguard Python Package',
-    'long_description': '# PySafeguard\nOne Identity Safeguard Python SDK\n\n-----------\n\n<p align="center">\n<i>Check out our <a href=\'https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples\'>sample projects</a> to get started with your own custom integration to Safeguard!</i>\n</p>\n\n-----------\n\n## Support\n\nOne Identity open source projects are supported through [One Identity GitHub issues](https://github.com/OneIdentity/PySafeguard/issues) and the [One Identity Community](https://www.oneidentity.com/community/). This includes all scripts, plugins, SDKs, modules, code snippets or other solutions. For assistance with any One Identity GitHub project, please raise a new Issue on the [One Identity GitHub project](https://github.com/OneIdentity/PySafeguard/issues) page. You may also visit the [One Identity Community](https://www.oneidentity.com/community/) to ask questions.  Requests for assistance made through official One Identity Support will be referred back to GitHub and the One Identity Community forums where those requests can benefit all users.\n\n## Introduction\n\nAll functionality in Safeguard is available via the Safeguard API. There is\nnothing that can be done in the Safeguard UI that cannot also be performed\nusing the Safeguard API programmatically.\n\nPySafeguard is provided to facilitate calling the Safeguard API from Python.\nIt is meant to remove the complexity of dealing with authentication via\nSafeguard\'s embedded secure token service (STS). The basic usage is to call\none of the `connect_*()` methods to establish a connection to Safeguard, then\nyou can call `invoke()` multiple times using the same authenticated connection.\n\nPySafeguard also provides an easy way to call Safeguard A2A from Python. The A2A service requires client certificate authentication for retrieving passwords for application integration. When Safeguard A2A is properly configured, specified passwords can be retrieved with a single method call without requiring access request workflow approvals. Safeguard A2A is protected by API keys and IP restrictions in addition to client certificate authentication.\n\nPySafeguard includes an SDK for listening to Safeguard\'s powerful, real-time event notification system. Safeguard provides role-based event notifications via SignalR to subscribed clients. If a Safeguard user is an Asset Administrator events related to the creation, modification, or deletion of Assets and Asset Accounts will be sent to that user. When used with a certificate user, this provides an opportunity for reacting programmatically to any data modification in Safeguard. Events are also supported for access request workflow and for A2A password changes.\n\n## Installation\n\nThis Python module is published to the [PyPi registry](https://pypi.org/project/pysafeguard) to make it as easy as possible to install.\n\n```Bash\n> pip install pysafeguard\n```\n\n## Dependencies\npysafeguard uses the python requests module, which will need to be installed prior to using pysafeguard\n\n```Bash\n> pip install requests\n```\nIn addition if you will be using the SignalR functionality you will need to install SignalR Core client module.  SignalR Core client is only required if using the SignalR functionality\n\n```Bash\n> pip install signalrcore\n```\n\n### Communicating securely with Safeguard using the SDK\n\nWhen using the SDK to communicate with Safeguard, all communication will\nbe done using HTTPS.  To keep the communication secure, all certificates\nused to secure Safeguard\'s API should be configured on the system where\nthe SDK is used.  How this is accomplished varies on each system,\nhowever, here are some tips that can help get started.\n\nIf the system is already properly configured, the SDK should work\nwithout any errors.  If there are errors, consider using one of the\nfollowing methods to establish trust.\n\n- Environment variable providing path to certificates</li>\n\n  In Bourne Shell:\n  ```Bash\n  $ export WEBSOCKET_CLIENT_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt\n  $ export REQUESTS_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt\n  ```\n  \n  In PowerShell:\n  ```Powershell\n  > $env:WEBSOCKET_CLIENT_CA_BUNDLE="c:\\ssl\\certs\\ca-certificates.crt"\n  > $env:REQUESTS_CA_BUNDLE="c:ssl\\certs\\ca-certificates.crt"\n  ```\n  \n- Use the `verify` option when creating the `PySafeguardConnection`</li>\n\n  See examples below for utilizing this method.  While `verify` can be\n  used to disable security checking this is not recommended.\n\n> **Note**  \n> The WEBSOCKET_CLIENT_CA_BUNDLE environment variable is only necessary\n> when working with SignalR.\n\n## Getting Started\n\nA simple code example for calling the Safeguard API with username and password authentication through the local Safeguard STS:\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_password(\'Admin\',\'Admin123\')\nme = connection.invoke(HttpMethods.GET, Services.CORE, \'Me\', query=dict(fields=\'DisplayName\'))\nprint(\'Connected to Safeguard as %s\' % me.json()[\'DisplayName\'])\n```\n\nPassword authentication to an external provider is as follows:\n(Sample can be found <a href=\'https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/PasswordExternalExample.py\'>here</a>.)\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_password(\'Admin\',\'Admin123\', \'myexternalprovider\')\n```\n\n\nClient certificate authentication is also available. This can be done using PEM and KEY file.\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_certificate(\'ssl/pathtocertuser.pem\', \'ssl/pathtocertuser.key\')\n```\n\n> **Note**  \n> Password protected certificates are not currently supported in PySafeguard.\n\nClient certificate authentication to an external provider is also available. This can be done using PEM and KEY file.\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_certificate(\'ssl/pathtocertuser.pem\', \'ssl/pathtocertuser.key\', \'myexternalprovider\')\n```\n\n\nA connection can also be made anonymously and without verifying the appliance certificate.\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', False)\nsystem_time = connection.invoke(HttpMethods.GET, Services.APPLIANCE, \'SystemTime\')\n```\n\nAuthentication is also possible using an existing Safeguard API token:\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_token(myApiToken)\n```\n> **Note**  \n> Two-factor authentication is not currently supported in PySafeguard.\n\n## Getting Started With A2A\n\nOnce you have configured your A2A registration in Safeguard you can retrieve an A2A password or private key using a certificate and api key.\n\nTo retrieve a password via A2A:\n\n```Python\nfrom pysafeguard import *\n\npassword = PySafeguardConnection.a2a_get_credential(\'safeguard.sample.corp\', \'myapikey\', \'ssl/pathtocertuser.pem\', \'ssl/pathtocertuser.key\', \'ssl/pathtoca.pem\')\n```\n\nTo retrieve a private key in OpenSSH format via A2A:\n\n```Python\nfrom pysafeguard import *\n\nprivatekey = PySafeguardConnection.a2a_get_credential(\'safeguard.sample.corp\', \'myapikey\', \'ssl/pathtocertuser.pem\', \'ssl/pathtocertuser.key\', \'ssl/pathtoca.pem\', A2ATypes.PRIVATEKEY)\n```\n\n## About the Safeguard API\n\nThe Safeguard API is a REST-based Web API. Safeguard API endpoints are called\nusing HTTP operators and JSON (or XML) requests and responses. The Safeguard API\nis documented using Swagger. You may use Swagger UI to call the API directly or\nto read the documentation about URLs, parameters, and payloads.\n\nTo access the Swagger UI use a browser to navigate to:\n`https://<address>/service/<service>/swagger`\n\n- `<address>` = Safeguard network address\n- `<service>` = Safeguard service to use\n\nThe Safeguard API is made up of multiple services: core, appliance, notification,\nand a2a.\n\n|Service|Description|\n|-|-|\n|core|Most product functionality is found here. All cluster-wide operations: access request workflow, asset management, policy management, etc.|\n|appliance|Appliance specific operations, such as setting IP address, maintenance, backups, support bundles, appliance management|\n|notification|Anonymous, unauthenticated operations. This service is available even when the appliance isn\'t fully online|\n|a2a|Application integration specific operations. Fetching passwords, making access requests on behalf of users, etc.|\n\nEach of these services provides a separate Swagger endpoint.\n\nYou may use the `Authorize` button at the top of the screen to get an API token\nto call the Safeguard API directly using Swagger.\n\n### Examples\n\nMost functionality is in the core service as mentioned above.  The notification service\nprovides read-only information for status, etc.\n\n#### Anonymous Call for Safeguard Status\n\nSample can be found <a href=\'https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/AnonymousExample.py\'>here</a>.\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', False)\nresult = connection.invoke(HttpMethods.GET, Services.NOTIFICATION, \'Status\')\nprint(json.dumps(result.json(),indent=2,sort_keys=True))\n```\n\n#### Get remaining access token lifetime\n\nSample can be found <a href=\'https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/PasswordExample.py\'>here</a>.\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_password(\'username\', \'password\')\nminutes_left = connection.get_remaining_token_lifetime()\nprint(minutes_left)\n```\n\n#### Register for SignalR events\n\nTo use the SignalR functionality, you will need to install the python SignalR Core client module\n\n```Bash\n> pip install signalrcore\n```\n\nSample can be found <a href=\'https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/SignalRExample.py\'>here</a>.\n\n```Python\nfrom pysafeguard import *\n\nconnection = PySafeguardConnection(hostName, caFile)\n\n# SignalR callback function to handle the signalR messages\ndef signalrcallback(results):\n    print("Received SignalR event: {0}".format(results[0][\'Message\']))\n\nprint("Connecting to SignalR via username/password")\nconnection.register_signalr_username(connection, signalrcallback, userName, password)\n\nprint("Connecting to SignalR via certifacte")\nconnection.register_signalr_certificate(connection, signalrcallback, userCertFile, userKeyFile)\n```\n> **Note**  \n> Password protected certificates are not currently supported in PySafeguard.\n\n#### Create a New User and Set the Password\n\nSample can be found <a href=\'https://github.com/OneIdentity/PySafeguard/blob/1.0.2/samples/NewUserExample.py\'>here</a>.\n\n```Python\nfrom pysafeguard import *\nimport json\n\nuser = {\n    \'PrimaryAuthenticationProvider\': { \'Id\': -1 },\n    \'Name\': \'MyNewUser\'\n}\npassword = \'MyNewUser123\'\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/pathtoca.pem\')\nconnection.connect_password(\'username\', \'password\')\nresult = connection.invoke(HttpMethods.POST, Services.CORE, \'Users\', body=user).json()\nuserId = result.get(\'Id\')\nconnection.invoke(HttpMethods.PUT, Services.CORE, f\'Users/{userId}/Password\', body=password)\n```\n',
-    'author': 'Tania Engel',
-    'author_email': 'Tania.Engel@oneidentity.com',
-    'maintainer': 'Rich Gagliano',
-    'maintainer_email': 'Rich.Gagliano@oneidentity.com',
-    'url': 'https://github.com/OneIdentity/PySafeguard',
-    'package_dir': package_dir,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+-----------
+
+<p align="center">
+<i>Check out our <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples'>sample projects</a> to get started with your own custom integration to Safeguard!</i>
+</p>
+
+-----------
+
+## Support
+
+One Identity open source projects are supported through [One Identity GitHub issues](https://github.com/OneIdentity/PySafeguard/issues) and the [One Identity Community](https://www.oneidentity.com/community/). This includes all scripts, plugins, SDKs, modules, code snippets or other solutions. For assistance with any One Identity GitHub project, please raise a new Issue on the [One Identity GitHub project](https://github.com/OneIdentity/PySafeguard/issues) page. You may also visit the [One Identity Community](https://www.oneidentity.com/community/) to ask questions.  Requests for assistance made through official One Identity Support will be referred back to GitHub and the One Identity Community forums where those requests can benefit all users.
+
+## Introduction
+
+All functionality in Safeguard is available via the Safeguard API. There is
+nothing that can be done in the Safeguard UI that cannot also be performed
+using the Safeguard API programmatically.
+
+PySafeguard is provided to facilitate calling the Safeguard API from Python.
+It is meant to remove the complexity of dealing with authentication via
+Safeguard's embedded secure token service (STS). The basic usage is to call
+one of the `connect_*()` methods to establish a connection to Safeguard, then
+you can call `invoke()` multiple times using the same authenticated connection.
+
+PySafeguard also provides an easy way to call Safeguard A2A from Python. The A2A service requires client certificate authentication for retrieving passwords for application integration. When Safeguard A2A is properly configured, specified passwords can be retrieved with a single method call without requiring access request workflow approvals. Safeguard A2A is protected by API keys and IP restrictions in addition to client certificate authentication.
+
+PySafeguard includes an SDK for listening to Safeguard's powerful, real-time event notification system. Safeguard provides role-based event notifications via SignalR to subscribed clients. If a Safeguard user is an Asset Administrator events related to the creation, modification, or deletion of Assets and Asset Accounts will be sent to that user. When used with a certificate user, this provides an opportunity for reacting programmatically to any data modification in Safeguard. Events are also supported for access request workflow and for A2A password changes.
+
+## Installation
+
+This Python module is published to the [PyPi registry](https://pypi.org/project/pysafeguard) to make it as easy as possible to install.
+
+```Bash
+> pip install pysafeguard
+```
+
+## Dependencies
+pysafeguard uses the python requests module, which will need to be installed prior to using pysafeguard
+
+```Bash
+> pip install requests
+```
+In addition if you will be using the SignalR functionality you will need to install SignalR Core client module.  SignalR Core client is only required if using the SignalR functionality
+
+```Bash
+> pip install signalrcore
+```
+
+### Communicating securely with Safeguard using the SDK
+
+When using the SDK to communicate with Safeguard, all communication will
+be done using HTTPS.  To keep the communication secure, all certificates
+used to secure Safeguard's API should be configured on the system where
+the SDK is used.  How this is accomplished varies on each system,
+however, here are some tips that can help get started.
+
+If the system is already properly configured, the SDK should work
+without any errors.  If there are errors, consider using one of the
+following methods to establish trust.
+
+- Environment variable providing path to certificates</li>
+
+  In Bourne Shell:
+  ```Bash
+  $ export WEBSOCKET_CLIENT_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
+  $ export REQUESTS_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
+  ```
+  
+  In PowerShell:
+  ```Powershell
+  > $env:WEBSOCKET_CLIENT_CA_BUNDLE="c:\ssl\certs\ca-certificates.crt"
+  > $env:REQUESTS_CA_BUNDLE="c:ssl\certs\ca-certificates.crt"
+  ```
+  
+- Use the `verify` option when creating the `PySafeguardConnection`</li>
+
+  See examples below for utilizing this method.  While `verify` can be
+  used to disable security checking this is not recommended.
+
+> **Note**  
+> The WEBSOCKET_CLIENT_CA_BUNDLE environment variable is only necessary
+> when working with SignalR.
+
+## Getting Started
+
+A simple code example for calling the Safeguard API with username and password authentication through the local Safeguard STS:
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_password('Admin','Admin123')
+me = connection.invoke(HttpMethods.GET, Services.CORE, 'Me', query=dict(fields='DisplayName'))
+print('Connected to Safeguard as %s' % me.json()['DisplayName'])
+```
+
+Password authentication to an external provider is as follows:
+(Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/PasswordExternalExample.py'>here</a>.)
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_password('Admin','Admin123', 'myexternalprovider')
+```
+
+
+Client certificate authentication is also available. This can be done using PEM and KEY file.
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_certificate('ssl/pathtocertuser.pem', 'ssl/pathtocertuser.key')
+```
+
+> **Note**  
+> Password protected certificates are not currently supported in PySafeguard.
+
+Client certificate authentication to an external provider is also available. This can be done using PEM and KEY file.
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_certificate('ssl/pathtocertuser.pem', 'ssl/pathtocertuser.key', 'myexternalprovider')
+```
+
+
+A connection can also be made anonymously and without verifying the appliance certificate.
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', False)
+system_time = connection.invoke(HttpMethods.GET, Services.APPLIANCE, 'SystemTime')
+```
 
+Authentication is also possible using an existing Safeguard API token:
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_token(myApiToken)
+```
+> **Note**  
+> Two-factor authentication is not currently supported in PySafeguard.
+
+## Getting Started With A2A
+
+Once you have configured your A2A registration in Safeguard you can retrieve an A2A password or private key using a certificate and api key.
+
+To retrieve a password via A2A:
+
+```Python
+from pysafeguard import *
+
+password = PySafeguardConnection.a2a_get_credential('safeguard.sample.corp', 'myapikey', 'ssl/pathtocertuser.pem', 'ssl/pathtocertuser.key', 'ssl/pathtoca.pem')
+```
+
+To retrieve a private key in OpenSSH format via A2A:
+
+```Python
+from pysafeguard import *
+
+privatekey = PySafeguardConnection.a2a_get_credential('safeguard.sample.corp', 'myapikey', 'ssl/pathtocertuser.pem', 'ssl/pathtocertuser.key', 'ssl/pathtoca.pem', A2ATypes.PRIVATEKEY)
+```
+
+## About the Safeguard API
+
+The Safeguard API is a REST-based Web API. Safeguard API endpoints are called
+using HTTP operators and JSON (or XML) requests and responses. The Safeguard API
+is documented using Swagger. You may use Swagger UI to call the API directly or
+to read the documentation about URLs, parameters, and payloads.
+
+To access the Swagger UI use a browser to navigate to:
+`https://<address>/service/<service>/swagger`
+
+- `<address>` = Safeguard network address
+- `<service>` = Safeguard service to use
+
+The Safeguard API is made up of multiple services: core, appliance, notification,
+and a2a.
+
+|Service|Description|
+|-|-|
+|core|Most product functionality is found here. All cluster-wide operations: access request workflow, asset management, policy management, etc.|
+|appliance|Appliance specific operations, such as setting IP address, maintenance, backups, support bundles, appliance management|
+|notification|Anonymous, unauthenticated operations. This service is available even when the appliance isn't fully online|
+|a2a|Application integration specific operations. Fetching passwords, making access requests on behalf of users, etc.|
+
+Each of these services provides a separate Swagger endpoint.
+
+You may use the `Authorize` button at the top of the screen to get an API token
+to call the Safeguard API directly using Swagger.
+
+### Examples
+
+Most functionality is in the core service as mentioned above.  The notification service
+provides read-only information for status, etc.
+
+#### Anonymous Call for Safeguard Status
+
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/AnonymousExample.py'>here</a>.
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', False)
+result = connection.invoke(HttpMethods.GET, Services.NOTIFICATION, 'Status')
+print(json.dumps(result.json(),indent=2,sort_keys=True))
+```
+
+#### Get remaining access token lifetime
+
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/PasswordExample.py'>here</a>.
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_password('username', 'password')
+minutes_left = connection.get_remaining_token_lifetime()
+print(minutes_left)
+```
+
+#### Register for SignalR events
+
+To use the SignalR functionality, you will need to install the python SignalR Core client module
+
+```Bash
+> pip install signalrcore
+```
+
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/SignalRExample.py'>here</a>.
+
+```Python
+from pysafeguard import *
+
+connection = PySafeguardConnection(hostName, caFile)
+
+# SignalR callback function to handle the signalR messages
+def signalrcallback(results):
+    print("Received SignalR event: {0}".format(results[0]['Message']))
+
+print("Connecting to SignalR via username/password")
+connection.register_signalr_username(connection, signalrcallback, userName, password)
+
+print("Connecting to SignalR via certifacte")
+connection.register_signalr_certificate(connection, signalrcallback, userCertFile, userKeyFile)
+```
+> **Note**  
+> Password protected certificates are not currently supported in PySafeguard.
+
+#### Create a New User and Set the Password
+
+Sample can be found <a href='https://github.com/OneIdentity/PySafeguard/blob/7.3.0/samples/NewUserExample.py'>here</a>.
+
+```Python
+from pysafeguard import *
+import json
+
+user = {
+    'PrimaryAuthenticationProvider': { 'Id': -1 },
+    'Name': 'MyNewUser'
+}
+password = 'MyNewUser123'
+connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_password('username', 'password')
+result = connection.invoke(HttpMethods.POST, Services.CORE, 'Users', body=user).json()
+userId = result.get('Id')
+connection.invoke(HttpMethods.PUT, Services.CORE, f'Users/{userId}/Password', body=password)
+```
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,115 +1,118 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} modules = \ ['pysafeguard'] install_requires = \
-['requests>=2.28.1,<3.0.0'] extras_require = \ {'signalr':
-['signalrcore>=0.9.5,<0.10.0']} setup_kwargs = { 'name': 'pysafeguard',
-'version': '1.0.2', 'description': 'One Identity Safeguard Python Package',
-'long_description': '# PySafeguard\nOne Identity Safeguard Python SDK\n\n------
------\n\n
-\nCheck out our sample_projects to get started with your own custom integration
-                                to Safeguard!\n
-\n\n-----------\n\n## Support\n\nOne Identity open source projects are
-supported through [One Identity GitHub issues](https://github.com/OneIdentity/
-PySafeguard/issues) and the [One Identity Community](https://
-www.oneidentity.com/community/). This includes all scripts, plugins, SDKs,
-modules, code snippets or other solutions. For assistance with any One Identity
-GitHub project, please raise a new Issue on the [One Identity GitHub project]
-(https://github.com/OneIdentity/PySafeguard/issues) page. You may also visit
-the [One Identity Community](https://www.oneidentity.com/community/) to ask
-questions. Requests for assistance made through official One Identity Support
-will be referred back to GitHub and the One Identity Community forums where
-those requests can benefit all users.\n\n## Introduction\n\nAll functionality
-in Safeguard is available via the Safeguard API. There is\nnothing that can be
-done in the Safeguard UI that cannot also be performed\nusing the Safeguard API
-programmatically.\n\nPySafeguard is provided to facilitate calling the
-Safeguard API from Python.\nIt is meant to remove the complexity of dealing
-with authentication via\nSafeguard\'s embedded secure token service (STS). The
-basic usage is to call\none of the `connect_*()` methods to establish a
-connection to Safeguard, then\nyou can call `invoke()` multiple times using the
-same authenticated connection.\n\nPySafeguard also provides an easy way to call
-Safeguard A2A from Python. The A2A service requires client certificate
-authentication for retrieving passwords for application integration. When
-Safeguard A2A is properly configured, specified passwords can be retrieved with
-a single method call without requiring access request workflow approvals.
-Safeguard A2A is protected by API keys and IP restrictions in addition to
-client certificate authentication.\n\nPySafeguard includes an SDK for listening
-to Safeguard\'s powerful, real-time event notification system. Safeguard
-provides role-based event notifications via SignalR to subscribed clients. If a
-Safeguard user is an Asset Administrator events related to the creation,
-modification, or deletion of Assets and Asset Accounts will be sent to that
-user. When used with a certificate user, this provides an opportunity for
-reacting programmatically to any data modification in Safeguard. Events are
-also supported for access request workflow and for A2A password changes.\n\n##
-Installation\n\nThis Python module is published to the [PyPi registry](https://
-pypi.org/project/pysafeguard) to make it as easy as possible to
-install.\n\n```Bash\n> pip install pysafeguard\n```\n\n##
-Dependencies\npysafeguard uses the python requests module, which will need to
-be installed prior to using pysafeguard\n\n```Bash\n> pip install
-requests\n```\nIn addition if you will be using the SignalR functionality you
-will need to install SignalR Core client module. SignalR Core client is only
-required if using the SignalR functionality\n\n```Bash\n> pip install
-signalrcore\n```\n\n### Communicating securely with Safeguard using the
-SDK\n\nWhen using the SDK to communicate with Safeguard, all communication
-will\nbe done using HTTPS. To keep the communication secure, all
-certificates\nused to secure Safeguard\'s API should be configured on the
-system where\nthe SDK is used. How this is accomplished varies on each
-system,\nhowever, here are some tips that can help get started.\n\nIf the
-system is already properly configured, the SDK should work\nwithout any errors.
-If there are errors, consider using one of the\nfollowing methods to establish
-trust.\n\n- Environment variable providing path to certificates
-\n\n In Bourne Shell:\n ```Bash\n $ export WEBSOCKET_CLIENT_CA_BUNDLE=/etc/ssl/
-certs/ca-certificates.crt\n $ export REQUESTS_CA_BUNDLE=/etc/ssl/certs/ca-
-certificates.crt\n ```\n \n In PowerShell:\n ```Powershell\n > $env:
-WEBSOCKET_CLIENT_CA_BUNDLE="c:\\ssl\\certs\\ca-certificates.crt"\n > $env:
-REQUESTS_CA_BUNDLE="c:ssl\\certs\\ca-certificates.crt"\n ```\n \n- Use the
-`verify` option when creating the `PySafeguardConnection`
-\n\n See examples below for utilizing this method. While `verify` can be\n used
-to disable security checking this is not recommended.\n\n> **Note** \n> The
-WEBSOCKET_CLIENT_CA_BUNDLE environment variable is only necessary\n> when
-working with SignalR.\n\n## Getting Started\n\nA simple code example for
-calling the Safeguard API with username and password authentication through the
-local Safeguard STS:\n\n```Python\nfrom pysafeguard import *\n\nconnection =
-PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/
-pathtoca.pem\')\nconnection.connect_password(\'Admin\',\'Admin123\')\nme =
-connection.invoke(HttpMethods.GET, Services.CORE, \'Me\', query=dict
-(fields=\'DisplayName\'))\nprint(\'Connected to Safeguard as %s\' % me.json()
-[\'DisplayName\'])\n```\n\nPassword authentication to an external provider is
-as follows:\n(Sample can be found here.)\n\n```Python\nfrom pysafeguard import
-*\n\nconnection = PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/
-pathtoca.pem\')\nconnection.connect_password(\'Admin\',\'Admin123\',
-\'myexternalprovider\')\n```\n\n\nClient certificate authentication is also
-available. This can be done using PEM and KEY file.\n\n```Python\nfrom
-pysafeguard import *\n\nconnection = PySafeguardConnection
-(\'safeguard.sample.corp\', \'ssl/
-pathtoca.pem\')\nconnection.connect_certificate(\'ssl/pathtocertuser.pem\',
-\'ssl/pathtocertuser.key\')\n```\n\n> **Note** \n> Password protected
-certificates are not currently supported in PySafeguard.\n\nClient certificate
-authentication to an external provider is also available. This can be done
-using PEM and KEY file.\n\n```Python\nfrom pysafeguard import *\n\nconnection =
-PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/
-pathtoca.pem\')\nconnection.connect_certificate(\'ssl/pathtocertuser.pem\',
-\'ssl/pathtocertuser.key\', \'myexternalprovider\')\n```\n\n\nA connection can
-also be made anonymously and without verifying the appliance
-certificate.\n\n```Python\nfrom pysafeguard import *\n\nconnection =
-PySafeguardConnection(\'safeguard.sample.corp\', False)\nsystem_time =
-connection.invoke(HttpMethods.GET, Services.APPLIANCE,
-\'SystemTime\')\n```\n\nAuthentication is also possible using an existing
-Safeguard API token:\n\n```Python\nfrom pysafeguard import *\n\nconnection =
-PySafeguardConnection(\'safeguard.sample.corp\', \'ssl/
-pathtoca.pem\')\nconnection.connect_token(myApiToken)\n```\n> **Note** \n> Two-
-factor authentication is not currently supported in PySafeguard.\n\n## Getting
-Started With A2A\n\nOnce you have configured your A2A registration in Safeguard
-you can retrieve an A2A password or private key using a certificate and api
-key.\n\nTo retrieve a password via A2A:\n\n```Python\nfrom pysafeguard import
-*\n\npassword = PySafeguardConnection.a2a_get_credential
-(\'safeguard.sample.corp\', \'myapikey\', \'ssl/pathtocertuser.pem\', \'ssl/
-pathtocertuser.key\', \'ssl/pathtoca.pem\')\n```\n\nTo retrieve a private key
-in OpenSSH format via A2A:\n\n```Python\nfrom pysafeguard import
-*\n\nprivatekey = PySafeguardConnection.a2a_get_credential
-(\'safeguard.sample.corp\', \'myapikey\', \'ssl/pathtocertuser.pem\', \'ssl/
-pathtocertuser.key\', \'ssl/pathtoca.pem\', A2ATypes.PRIVATEKEY)\n```\n\n##
-About the Safeguard API\n\nThe Safeguard API is a REST-based Web API. Safeguard
-API endpoints are called\nusing HTTP operators and JSON (or XML) requests and
-responses. The Safeguard API\nis documented using Swagger. You may use Swagger
-UI to call the API directly or\nto read the documentation about URLs,
-parameters, and payloads.\n\nTo access the Swagger UI use a browser to navigate
-to:\n`https://
+Metadata-Version: 2.1 Name: pysafeguard Version: 7.3.0 Summary: One Identity
+Safeguard Python Package Home-page: https://github.com/OneIdentity/PySafeguard
+Keywords: safeguard,oneidentity Author: Tania Engel Author-email:
+Tania.Engel@oneidentity.com Maintainer: Stephanie Zinn Maintainer-email:
+Stephanie.Zinn@oneidentity.com Requires-Python: >=3.7,<4.0 Classifier: License
+:: OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 Provides-Extra:
+signalr Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: signalrcore
+(>=0.9.5,<0.10.0) ; extra == "signalr" Project-URL: Bug Tracker, https://
+github.com/OneIdentity/PySafeguard/issues Project-URL: Repository, https://
+github.com/OneIdentity/PySafeguard Description-Content-Type: text/markdown #
+PySafeguard One Identity Safeguard Python SDK -----------
+ Check out our sample_projects to get started with your own custom integration
+                                 to Safeguard!
+----------- ## Support One Identity open source projects are supported through
+[One Identity GitHub issues](https://github.com/OneIdentity/PySafeguard/issues)
+and the [One Identity Community](https://www.oneidentity.com/community/). This
+includes all scripts, plugins, SDKs, modules, code snippets or other solutions.
+For assistance with any One Identity GitHub project, please raise a new Issue
+on the [One Identity GitHub project](https://github.com/OneIdentity/
+PySafeguard/issues) page. You may also visit the [One Identity Community]
+(https://www.oneidentity.com/community/) to ask questions. Requests for
+assistance made through official One Identity Support will be referred back to
+GitHub and the One Identity Community forums where those requests can benefit
+all users. ## Introduction All functionality in Safeguard is available via the
+Safeguard API. There is nothing that can be done in the Safeguard UI that
+cannot also be performed using the Safeguard API programmatically. PySafeguard
+is provided to facilitate calling the Safeguard API from Python. It is meant to
+remove the complexity of dealing with authentication via Safeguard's embedded
+secure token service (STS). The basic usage is to call one of the `connect_*()`
+methods to establish a connection to Safeguard, then you can call `invoke()`
+multiple times using the same authenticated connection. PySafeguard also
+provides an easy way to call Safeguard A2A from Python. The A2A service
+requires client certificate authentication for retrieving passwords for
+application integration. When Safeguard A2A is properly configured, specified
+passwords can be retrieved with a single method call without requiring access
+request workflow approvals. Safeguard A2A is protected by API keys and IP
+restrictions in addition to client certificate authentication. PySafeguard
+includes an SDK for listening to Safeguard's powerful, real-time event
+notification system. Safeguard provides role-based event notifications via
+SignalR to subscribed clients. If a Safeguard user is an Asset Administrator
+events related to the creation, modification, or deletion of Assets and Asset
+Accounts will be sent to that user. When used with a certificate user, this
+provides an opportunity for reacting programmatically to any data modification
+in Safeguard. Events are also supported for access request workflow and for A2A
+password changes. ## Installation This Python module is published to the [PyPi
+registry](https://pypi.org/project/pysafeguard) to make it as easy as possible
+to install. ```Bash > pip install pysafeguard ``` ## Dependencies pysafeguard
+uses the python requests module, which will need to be installed prior to using
+pysafeguard ```Bash > pip install requests ``` In addition if you will be using
+the SignalR functionality you will need to install SignalR Core client module.
+SignalR Core client is only required if using the SignalR functionality ```Bash
+> pip install signalrcore ``` ### Communicating securely with Safeguard using
+the SDK When using the SDK to communicate with Safeguard, all communication
+will be done using HTTPS. To keep the communication secure, all certificates
+used to secure Safeguard's API should be configured on the system where the SDK
+is used. How this is accomplished varies on each system, however, here are some
+tips that can help get started. If the system is already properly configured,
+the SDK should work without any errors. If there are errors, consider using one
+of the following methods to establish trust. - Environment variable providing
+path to certificates
+In Bourne Shell: ```Bash $ export WEBSOCKET_CLIENT_CA_BUNDLE=/etc/ssl/certs/ca-
+certificates.crt $ export REQUESTS_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
+``` In PowerShell: ```Powershell > $env:WEBSOCKET_CLIENT_CA_BUNDLE="c:
+\ssl\certs\ca-certificates.crt" > $env:REQUESTS_CA_BUNDLE="c:ssl\certs\ca-
+certificates.crt" ``` - Use the `verify` option when creating the
+`PySafeguardConnection`
+See examples below for utilizing this method. While `verify` can be used to
+disable security checking this is not recommended. > **Note** > The
+WEBSOCKET_CLIENT_CA_BUNDLE environment variable is only necessary > when
+working with SignalR. ## Getting Started A simple code example for calling the
+Safeguard API with username and password authentication through the local
+Safeguard STS: ```Python from pysafeguard import * connection =
+PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_password('Admin','Admin123') me = connection.invoke
+(HttpMethods.GET, Services.CORE, 'Me', query=dict(fields='DisplayName')) print
+('Connected to Safeguard as %s' % me.json()['DisplayName']) ``` Password
+authentication to an external provider is as follows: (Sample can be found
+here.) ```Python from pysafeguard import * connection = PySafeguardConnection
+('safeguard.sample.corp', 'ssl/pathtoca.pem') connection.connect_password
+('Admin','Admin123', 'myexternalprovider') ``` Client certificate
+authentication is also available. This can be done using PEM and KEY file.
+```Python from pysafeguard import * connection = PySafeguardConnection
+('safeguard.sample.corp', 'ssl/pathtoca.pem') connection.connect_certificate
+('ssl/pathtocertuser.pem', 'ssl/pathtocertuser.key') ``` > **Note** > Password
+protected certificates are not currently supported in PySafeguard. Client
+certificate authentication to an external provider is also available. This can
+be done using PEM and KEY file. ```Python from pysafeguard import * connection
+= PySafeguardConnection('safeguard.sample.corp', 'ssl/pathtoca.pem')
+connection.connect_certificate('ssl/pathtocertuser.pem', 'ssl/
+pathtocertuser.key', 'myexternalprovider') ``` A connection can also be made
+anonymously and without verifying the appliance certificate. ```Python from
+pysafeguard import * connection = PySafeguardConnection
+('safeguard.sample.corp', False) system_time = connection.invoke
+(HttpMethods.GET, Services.APPLIANCE, 'SystemTime') ``` Authentication is also
+possible using an existing Safeguard API token: ```Python from pysafeguard
+import * connection = PySafeguardConnection('safeguard.sample.corp', 'ssl/
+pathtoca.pem') connection.connect_token(myApiToken) ``` > **Note** > Two-factor
+authentication is not currently supported in PySafeguard. ## Getting Started
+With A2A Once you have configured your A2A registration in Safeguard you can
+retrieve an A2A password or private key using a certificate and api key. To
+retrieve a password via A2A: ```Python from pysafeguard import * password =
+PySafeguardConnection.a2a_get_credential('safeguard.sample.corp', 'myapikey',
+'ssl/pathtocertuser.pem', 'ssl/pathtocertuser.key', 'ssl/pathtoca.pem') ``` To
+retrieve a private key in OpenSSH format via A2A: ```Python from pysafeguard
+import * privatekey = PySafeguardConnection.a2a_get_credential
+('safeguard.sample.corp', 'myapikey', 'ssl/pathtocertuser.pem', 'ssl/
+pathtocertuser.key', 'ssl/pathtoca.pem', A2ATypes.PRIVATEKEY) ``` ## About the
+Safeguard API The Safeguard API is a REST-based Web API. Safeguard API
+endpoints are called using HTTP operators and JSON (or XML) requests and
+responses. The Safeguard API is documented using Swagger. You may use Swagger
+UI to call the API directly or to read the documentation about URLs,
+parameters, and payloads. To access the Swagger UI use a browser to navigate
+to: `https://
```


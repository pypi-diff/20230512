# Comparing `tmp/peachpayments_partner_marshmallow-0.2.9.tar.gz` & `tmp/peachpayments_partner_marshmallow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachpayments_partner_marshmallow-0.2.9.tar", max compression
+gzip compressed data, was "peachpayments_partner_marshmallow-1.1.0.tar", max compression
```

## Comparing `peachpayments_partner_marshmallow-0.2.9.tar` & `peachpayments_partner_marshmallow-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-01-02 12:25:49.591357 peachpayments_partner_marshmallow-0.2.9/LICENSE.txt
--rw-r--r--   0        0        0     1893 2023-01-02 12:25:49.595357 peachpayments_partner_marshmallow-0.2.9/README.md
--rw-r--r--   0        0        0       22 2023-01-02 13:08:42.362010 peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/__init__.py
--rw-r--r--   0        0        0    17664 2023-01-02 12:25:49.595357 peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/fields.py
--rw-r--r--   0        0        0     6705 2023-01-02 12:25:49.595357 peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/schemas.py
--rw-r--r--   0        0        0     1682 2023-01-02 12:25:49.595357 peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/validate.py
--rw-r--r--   0        0        0     5835 2023-01-02 12:25:49.595357 peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/validator.py
--rw-r--r--   0        0        0     1320 2023-01-02 13:08:42.362010 peachpayments_partner_marshmallow-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 peachpayments_partner_marshmallow-0.2.9/setup.py
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 peachpayments_partner_marshmallow-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-12 07:11:05.778365 peachpayments_partner_marshmallow-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1893 2023-05-12 07:11:05.778365 peachpayments_partner_marshmallow-1.1.0/README.md
+-rw-r--r--   0        0        0       36 2023-05-12 07:11:05.778365 peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/__init__.py
+-rw-r--r--   0        0        0    17664 2023-05-12 07:11:05.782365 peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/fields.py
+-rw-r--r--   0        0        0     6673 2023-05-12 07:11:05.782365 peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/schemas.py
+-rw-r--r--   0        0        0     1682 2023-05-12 07:11:05.782365 peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/validate.py
+-rw-r--r--   0        0        0     5835 2023-05-12 07:11:05.782365 peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/validator.py
+-rw-r--r--   0        0        0     1320 2023-05-12 14:20:36.670906 peachpayments_partner_marshmallow-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 peachpayments_partner_marshmallow-1.1.0/PKG-INFO
```

### Comparing `peachpayments_partner_marshmallow-0.2.9/LICENSE.txt` & `peachpayments_partner_marshmallow-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_marshmallow-0.2.9/README.md` & `peachpayments_partner_marshmallow-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/fields.py` & `peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/fields.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/schemas.py` & `peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     paymentType = PaymentType(required=True, validate=validate.Equal(comparable=PAYMENT_TYPE_DEBIT))
     customer = Nested(Customer)
     customParameters = CustomParameters()
     # example: "Shopping Merchant"
     merchantName = String(validate=Regexp(regex=r"^[\s\S]{1,255}$"), required=True)
     merchantTransactionId = MerchantTransactionId()
     # "20170630-4072-00"
-    merchantInvoiceId = String(validate=Regexp(regex=r"^[\w~!@#$%\^&*()+\-,./:?\][\\\{}`;|\"']{8,255}$"))
+    merchantInvoiceId = String(validate=Regexp(regex=r"^[\s\S]{8,255}$"))
     clearingInstituteSessionId = ClearingInstituteSessionId()
     notificationUrl = Url(required=True)
     # This will only be used to redirect back to Peach
     # example: "https://peachredirect.com/v1/redirect/paymentBrand"
     shopperResultUrl = Url(required=True)
     card = Nested(DebitRequestCard)
     billing = Nested(Data)
```

### Comparing `peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/validate.py` & `peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/validate.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_marshmallow-0.2.9/peachpayments_partner_marshmallow/validator.py` & `peachpayments_partner_marshmallow-1.1.0/peachpayments_partner_marshmallow/validator.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_marshmallow-0.2.9/pyproject.toml` & `peachpayments_partner_marshmallow-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peachpayments-partner-marshmallow"
-version = "0.2.9"
+version = "1.1.0"
 description = "PeachPayments Partner Marshmallow library contains Marshmallow schemas to help integrate PeachPayments with their partners."
 readme = "README.md"
 license = "MIT"
 authors = ["PeachPayments <support@peachpayments.com>"]
 repository = "https://gitlab.com/peachpayments/peachpayments-partner-marshmallow/"
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `peachpayments_partner_marshmallow-0.2.9/setup.py` & `peachpayments_partner_marshmallow-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,81 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: peachpayments-partner-marshmallow
+Version: 1.1.0
+Summary: PeachPayments Partner Marshmallow library contains Marshmallow schemas to help integrate PeachPayments with their partners.
+Home-page: https://gitlab.com/peachpayments/peachpayments-partner-marshmallow/
+License: MIT
+Author: PeachPayments
+Author-email: support@peachpayments.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: iso4217 (>=1.6.20180829,<2.0.0)
+Requires-Dist: marshmallow (==3.13.0)
+Requires-Dist: peachpayments-partner (>=0.1.11,<0.2.0)
+Project-URL: Repository, https://gitlab.com/peachpayments/peachpayments-partner-marshmallow/
+Description-Content-Type: text/markdown
+
+# PeachPayments Partner Marshmallow Library
+
+## Overview
+
+**PeachPayments Partner Marshmallow Library** is a platform-agnostic Python package to help Payment Service Providers in integrating with PeachPayments. This library provides functionality to validate request and response data using Marshmallow Python library.
+
+**Source Code**: https://gitlab.com/peachpayments/peach-partner-marshmallow/
+
+---
+### Key terms
+|   Term	                    |   Definition	|
+|---------------------------- |--------------	|
+|   Partner API		            |   A service provided by Peach Payments to enable Payment Service Providers to become available on the Peach Platform |
+|   Payment Service Provider	|   A payment service provider who integrates with the Partner API	|
+|   Outbound API call	        |   API calls sent from Partner API to the Payment Service Provider  |
+|   Inbound API call		      |   API calls sent from Payment Service Provider to Partner API    |
+
+## Usage
+Package requires Python 3.9+
+
+### Installation
+```sh
+# pip
+$ pip3 install peachpayments-partner-marshmallow
+```
+```sh
+# poetry
+$ poetry add peachpayments-partner-marshmallow
+```
+
+### Field validation
+
+Payment Service Provider receives a debit request from PeachPayments.
+
+```python
+# ... imports
+from peachpayments_partner_marshmallow.validator import validate_debit_request, validate_debit_response
+
+
+def debit(db: Session, data: dict):
+    request_validation = validate_debit_request(data)
+    if not request_validation["valid"]:
+        raise HttpJSONError(request_validation["response"])
+
+    # Store a transaction in a database
+    # Prepare the response to PeachPayments in the `response_fields` dictionary
+
+    response_validation = validate_debit_response(response_fields)
+    if not response_validation["valid"]:
+        raise Exception("Badly formatted response fields")
 
-packages = \
-['peachpayments_partner_marshmallow']
+    return HttpResponse(response_fields)
+```
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['iso4217>=1.6.20180829,<2.0.0',
- 'marshmallow==3.13.0',
- 'peachpayments-partner>=0.1.11,<0.2.0']
-
-setup_kwargs = {
-    'name': 'peachpayments-partner-marshmallow',
-    'version': '0.2.9',
-    'description': 'PeachPayments Partner Marshmallow library contains Marshmallow schemas to help integrate PeachPayments with their partners.',
-    'long_description': '# PeachPayments Partner Marshmallow Library\n\n## Overview\n\n**PeachPayments Partner Marshmallow Library** is a platform-agnostic Python package to help Payment Service Providers in integrating with PeachPayments. This library provides functionality to validate request and response data using Marshmallow Python library.\n\n**Source Code**: https://gitlab.com/peachpayments/peach-partner-marshmallow/\n\n---\n### Key terms\n|   Term\t                    |   Definition\t|\n|---------------------------- |--------------\t|\n|   Partner API\t\t            |   A service provided by Peach Payments to enable Payment Service Providers to become available on the Peach Platform |\n|   Payment Service Provider\t|   A payment service provider who integrates with the Partner API\t|\n|   Outbound API call\t        |   API calls sent from Partner API to the Payment Service Provider  |\n|   Inbound API call\t\t      |   API calls sent from Payment Service Provider to Partner API    |\n\n## Usage\nPackage requires Python 3.9+\n\n### Installation\n```sh\n# pip\n$ pip3 install peachpayments-partner-marshmallow\n```\n```sh\n# poetry\n$ poetry add peachpayments-partner-marshmallow\n```\n\n### Field validation\n\nPayment Service Provider receives a debit request from PeachPayments.\n\n```python\n# ... imports\nfrom peachpayments_partner_marshmallow.validator import validate_debit_request, validate_debit_response\n\n\ndef debit(db: Session, data: dict):\n    request_validation = validate_debit_request(data)\n    if not request_validation["valid"]:\n        raise HttpJSONError(request_validation["response"])\n\n    # Store a transaction in a database\n    # Prepare the response to PeachPayments in the `response_fields` dictionary\n\n    response_validation = validate_debit_response(response_fields)\n    if not response_validation["valid"]:\n        raise Exception("Badly formatted response fields")\n\n    return HttpResponse(response_fields)\n```\n',
-    'author': 'PeachPayments',
-    'author_email': 'support@peachpayments.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/peachpayments/peachpayments-partner-marshmallow/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```


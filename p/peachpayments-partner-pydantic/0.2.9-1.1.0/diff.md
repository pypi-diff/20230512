# Comparing `tmp/peachpayments_partner_pydantic-0.2.9.tar.gz` & `tmp/peachpayments_partner_pydantic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachpayments_partner_pydantic-0.2.9.tar", max compression
+gzip compressed data, was "peachpayments_partner_pydantic-1.1.0.tar", max compression
```

## Comparing `peachpayments_partner_pydantic-0.2.9.tar` & `peachpayments_partner_pydantic-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1088 2022-12-22 13:19:11.471278 peachpayments_partner_pydantic-0.2.9/LICENSE.txt
--rw-r--r--   0        0        0     3087 2022-12-22 13:19:11.471278 peachpayments_partner_pydantic-0.2.9/README.md
--rw-r--r--   0        0        0       22 2023-01-02 13:19:29.468483 peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/__init__.py
--rw-r--r--   0        0        0     3277 2022-12-22 13:19:11.471278 peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/exception_handlers.py
--rw-r--r--   0        0        0     2793 2022-12-22 13:19:11.471278 peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/helpers.py
--rw-r--r--   0        0        0     7973 2022-12-22 13:19:11.471278 peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/inbound_schemas.py
--rw-r--r--   0        0        0    22072 2022-12-23 13:12:35.548014 peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/outbound_schemas.py
--rw-r--r--   0        0        0     7762 2022-12-22 13:19:11.471278 peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/schemas.py
--rw-r--r--   0        0        0     1507 2023-01-02 13:19:29.468483 peachpayments_partner_pydantic-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 peachpayments_partner_pydantic-0.2.9/setup.py
--rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 peachpayments_partner_pydantic-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3087 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/README.md
+-rw-r--r--   0        0        0       36 2023-05-12 07:07:24.502190 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/__init__.py
+-rw-r--r--   0        0        0     3277 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/exception_handlers.py
+-rw-r--r--   0        0        0     2793 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/helpers.py
+-rw-r--r--   0        0        0     7973 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/inbound_schemas.py
+-rw-r--r--   0        0        0    22033 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/outbound_schemas.py
+-rw-r--r--   0        0        0     7762 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/schemas.py
+-rw-r--r--   0        0        0     1507 2023-05-12 13:13:40.533687 peachpayments_partner_pydantic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 peachpayments_partner_pydantic-1.1.0/PKG-INFO
```

### Comparing `peachpayments_partner_pydantic-0.2.9/LICENSE.txt` & `peachpayments_partner_pydantic-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-0.2.9/README.md` & `peachpayments_partner_pydantic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/exception_handlers.py` & `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/helpers.py` & `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/helpers.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/inbound_schemas.py` & `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/inbound_schemas.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/outbound_schemas.py` & `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/outbound_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,15 +591,15 @@
     merchantName: str = Field(
         ..., description="The merchant's name.", example="Shopping Merchant", regex="^[\\s\\S]{1,255}$"
     )
     merchantInvoiceId: Optional[str] = Field(
         None,
         description="The merchant's invoice ID.",
         example="20170630-4072-00",
-        regex="^[\\w~!@#$%\\^&*()+\\-,./:?\\][\\\\\\{}`;|\\\"']{8,255}$",
+        regex="^[\\s\\S]{8,255}$",
     )
     notificationUrl: NotificationUrl
     clearingInstituteSessionId: Optional[ClearingInstituteSessionId] = None
     shopperResultUrl: AnyUrl = Field(
         ...,
         description="The Payment Service Provider must redirect the user to this URL after processing the payment request.",
         example="https://peachredirect.com/v1/redirect/paymentBrand",
```

### Comparing `peachpayments_partner_pydantic-0.2.9/peachpayments_partner_pydantic/schemas.py` & `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/schemas.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-0.2.9/pyproject.toml` & `peachpayments_partner_pydantic-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peachpayments-partner-pydantic"
-version = "0.2.9"
+version = "1.1.0"
 description = "PeachPayments Partner Pydantic library contains Pydantic schemas to help integrate PeachPayments with their partners."
 readme = "README.md"
 license = "MIT"
 authors = ["PeachPayments <support@peachpayments.com>"]
 repository = "https://gitlab.com/peachpayments/peachpayments-partner-pydantic/"
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `peachpayments_partner_pydantic-0.2.9/setup.py` & `peachpayments_partner_pydantic-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,116 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: peachpayments-partner-pydantic
+Version: 1.1.0
+Summary: PeachPayments Partner Pydantic library contains Pydantic schemas to help integrate PeachPayments with their partners.
+Home-page: https://gitlab.com/peachpayments/peachpayments-partner-pydantic/
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
+Requires-Dist: email-validator (>=1.2.1,<2.0.0)
+Requires-Dist: ipaddress (>=1.0.23,<2.0.0)
+Requires-Dist: iso4217 (>=1.9.20220401,<2.0.0)
+Requires-Dist: peachpayments-partner (>=0.1.11,<0.2.0)
+Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Project-URL: Repository, https://gitlab.com/peachpayments/peachpayments-partner-pydantic/
+Description-Content-Type: text/markdown
+
+# PeachPayments Partner Pydantic Library
+
+## Overview
+
+**PeachPayments Partner Pydantic Library** is a platform-agnostic Python package to help Payment Service Providers in integrating with PeachPayments. This library provides functionality to validate request and response data using Pydantic Python library.
+
+**Source Code**: <https://gitlab.com/peachpayments/peach-partner-pydantic/>
+
+* * *
+
+### Key terms
+
+| Term                     | Definition                                                                                                         |
+| ------------------------ | ------------------------------------------------------------------------------------------------------------------ |
+| Partner API              | A service provided by Peach Payments to enable Payment Service Providers to become available on the Peach Platform |
+| Payment Service Provider | A payment service provider who integrates with the Partner API                                                     |
+| Outbound API call        | API calls sent from Partner API to the Payment Service Provider                                                    |
+| Inbound API call         | API calls sent from Payment Service Provider to Partner API                                                        |
+
+## Usage
+
+Package requires Python 3.9+
+
+### Installation
+
+```sh
+# pip
+$ pip3 install peachpayments-partner-pydantic
+```
+
+```sh
+# poetry
+$ poetry add peachpayments-partner-pydantic
+```
+
+### Field validation
+
+**Scenario:** Payment Service Provider written in FastAPI receives a debit request from PeachPayments.
+
+```python
+# ... imports
+from peachpayments_partner_pydantic.schemas import DebitRequest, DebitResponse
+
+@router.post(
+    "/v1/debit",
+    response_model=schemas.DebitResponse,
+)
+def debit_request(
+    *, debit_in: schemas.DebitRequest
+) -> Any:
+    # Store the transaction
+    transaction = Transaction.create_from_debit(debit_in)
+    # Validate the debit response
+    debit_response = DebitResponse(**transaction.to_debit_response_fields())
+    return debit_response.dict()
+```
+
+### Translating exception to PeachPayments error response
+
+**Scenario:** Payment Service Provider written in FastAPI receives a request with a validation error from PeachPayments.
+
+#### 1. Write validation exception handler
+
+```python
+# app/exception_handlers.py
+from fastapi import Request, status
+from fastapi.exceptions import RequestValidationError
+from fastapi.responses import JSONResponse
+from peachpayments_partner_pydantic.exception_handlers import exception_to_response
+
+async def validation_exception_handler(request: Request, exc: RequestValidationError) -> JSONResponse:
+    return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=exception_to_response(exc))
+```
+
+#### 2. Connect it to the application
+
+```python
+# app/main.py
+from fastapi import FastAPI
+from fastapi.exceptions import RequestValidationError
+from app.exception_handlers import validation_exception_handler
+
+application = FastAPI(
+    exception_handlers={RequestValidationError: validation_exception_handler},
+)
+```
 
-packages = \
-['peachpayments_partner_pydantic']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['email-validator>=1.2.1,<2.0.0',
- 'ipaddress>=1.0.23,<2.0.0',
- 'iso4217>=1.9.20220401,<2.0.0',
- 'peachpayments-partner>=0.1.11,<0.2.0',
- 'pydantic>=1.9.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'peachpayments-partner-pydantic',
-    'version': '0.2.9',
-    'description': 'PeachPayments Partner Pydantic library contains Pydantic schemas to help integrate PeachPayments with their partners.',
-    'long_description': '# PeachPayments Partner Pydantic Library\n\n## Overview\n\n**PeachPayments Partner Pydantic Library** is a platform-agnostic Python package to help Payment Service Providers in integrating with PeachPayments. This library provides functionality to validate request and response data using Pydantic Python library.\n\n**Source Code**: <https://gitlab.com/peachpayments/peach-partner-pydantic/>\n\n* * *\n\n### Key terms\n\n| Term                     | Definition                                                                                                         |\n| ------------------------ | ------------------------------------------------------------------------------------------------------------------ |\n| Partner API              | A service provided by Peach Payments to enable Payment Service Providers to become available on the Peach Platform |\n| Payment Service Provider | A payment service provider who integrates with the Partner API                                                     |\n| Outbound API call        | API calls sent from Partner API to the Payment Service Provider                                                    |\n| Inbound API call         | API calls sent from Payment Service Provider to Partner API                                                        |\n\n## Usage\n\nPackage requires Python 3.9+\n\n### Installation\n\n```sh\n# pip\n$ pip3 install peachpayments-partner-pydantic\n```\n\n```sh\n# poetry\n$ poetry add peachpayments-partner-pydantic\n```\n\n### Field validation\n\n**Scenario:** Payment Service Provider written in FastAPI receives a debit request from PeachPayments.\n\n```python\n# ... imports\nfrom peachpayments_partner_pydantic.schemas import DebitRequest, DebitResponse\n\n@router.post(\n    "/v1/debit",\n    response_model=schemas.DebitResponse,\n)\ndef debit_request(\n    *, debit_in: schemas.DebitRequest\n) -> Any:\n    # Store the transaction\n    transaction = Transaction.create_from_debit(debit_in)\n    # Validate the debit response\n    debit_response = DebitResponse(**transaction.to_debit_response_fields())\n    return debit_response.dict()\n```\n\n### Translating exception to PeachPayments error response\n\n**Scenario:** Payment Service Provider written in FastAPI receives a request with a validation error from PeachPayments.\n\n#### 1. Write validation exception handler\n\n```python\n# app/exception_handlers.py\nfrom fastapi import Request, status\nfrom fastapi.exceptions import RequestValidationError\nfrom fastapi.responses import JSONResponse\nfrom peachpayments_partner_pydantic.exception_handlers import exception_to_response\n\nasync def validation_exception_handler(request: Request, exc: RequestValidationError) -> JSONResponse:\n    return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=exception_to_response(exc))\n```\n\n#### 2. Connect it to the application\n\n```python\n# app/main.py\nfrom fastapi import FastAPI\nfrom fastapi.exceptions import RequestValidationError\nfrom app.exception_handlers import validation_exception_handler\n\napplication = FastAPI(\n    exception_handlers={RequestValidationError: validation_exception_handler},\n)\n```\n',
-    'author': 'PeachPayments',
-    'author_email': 'support@peachpayments.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/peachpayments/peachpayments-partner-pydantic/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```


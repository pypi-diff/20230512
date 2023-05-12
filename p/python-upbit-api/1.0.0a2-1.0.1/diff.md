# Comparing `tmp/python-upbit-api-1.0.0a2.tar.gz` & `tmp/python-upbit-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-upbit-api-1.0.0a2.tar", last modified: Mon May  1 08:37:07 2023, max compression
+gzip compressed data, was "/Users/jihye/PycharmProjects/python-upbit-api/dist/.tmp-iwjerw9v/python-upbit-api-1.0.1.tar", last modified: Fri May 12 04:52:31 2023, max compression
```

## Comparing `python-upbit-api-1.0.0a2.tar` & `python-upbit-api-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.600436 python-upbit-api-1.0.0a2/
--rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.0.0a2/LICENSE
--rw-r--r--   0 jihye      (501) staff       (20)      928 2023-05-01 08:37:07.600218 python-upbit-api-1.0.0a2/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)       47 2023-04-28 04:46:27.000000 python-upbit-api-1.0.0a2/README.md
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.597771 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/
--rw-r--r--   0 jihye      (501) staff       (20)      928 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)      349 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/SOURCES.txt
--rw-r--r--   0 jihye      (501) staff       (20)        1 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/dependency_links.txt
--rw-r--r--   0 jihye      (501) staff       (20)       44 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/requires.txt
--rw-r--r--   0 jihye      (501) staff       (20)       12 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/top_level.txt
--rw-r--r--   0 jihye      (501) staff       (20)       38 2023-05-01 08:37:07.600499 python-upbit-api-1.0.0a2/setup.cfg
--rw-r--r--   0 jihye      (501) staff       (20)     1599 2023-05-01 08:36:54.000000 python-upbit-api-1.0.0a2/setup.py
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.598430 python-upbit-api-1.0.0a2/tests/
--rw-r--r--   0 jihye      (501) staff       (20)        0 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a2/tests/__init__.py
--rw-r--r--   0 jihye      (501) staff       (20)      548 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a2/tests/test_exceptions.py
--rw-r--r--   0 jihye      (501) staff       (20)      947 2023-05-01 04:26:36.000000 python-upbit-api-1.0.0a2/tests/test_remaining_req.py
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.599345 python-upbit-api-1.0.0a2/upbit/
--rw-r--r--   0 jihye      (501) staff       (20)      753 2023-05-01 03:34:38.000000 python-upbit-api-1.0.0a2/upbit/__init__.py
--rw-r--r--   0 jihye      (501) staff       (20)     3375 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a2/upbit/exceptions.py
--rw-r--r--   0 jihye      (501) staff       (20)    50349 2023-05-01 02:20:15.000000 python-upbit-api-1.0.0a2/upbit/upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.479816 python-upbit-api-1.0.1/
+-rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.0.1/LICENSE
+-rw-r--r--   0 jihye      (501) staff       (20)     8052 2023-05-12 04:52:31.479642 python-upbit-api-1.0.1/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)     5762 2023-05-11 14:40:27.000000 python-upbit-api-1.0.1/README.md
+-rw-r--r--   0 jihye      (501) staff       (20)     1492 2023-05-12 04:52:09.000000 python-upbit-api-1.0.1/pyproject.toml
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.477464 python-upbit-api-1.0.1/python_upbit_api.egg-info/
+-rw-r--r--   0 jihye      (501) staff       (20)     8052 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)      348 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        1 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       44 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/requires.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        6 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/top_level.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       38 2023-05-12 04:52:31.479869 python-upbit-api-1.0.1/setup.cfg
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.477881 python-upbit-api-1.0.1/tests/
+-rw-r--r--   0 jihye      (501) staff       (20)     1248 2023-05-11 03:13:33.000000 python-upbit-api-1.0.1/tests/test_remaining_req.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3174 2023-05-12 04:51:11.000000 python-upbit-api-1.0.1/tests/test_upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.478977 python-upbit-api-1.0.1/upbit/
+-rw-r--r--   0 jihye      (501) staff       (20)      726 2023-05-10 04:44:07.000000 python-upbit-api-1.0.1/upbit/__init__.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3469 2023-05-11 03:13:33.000000 python-upbit-api-1.0.1/upbit/exceptions.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3524 2023-05-10 05:00:31.000000 python-upbit-api-1.0.1/upbit/models.py
+-rw-r--r--   0 jihye      (501) staff       (20)    66010 2023-05-12 04:51:11.000000 python-upbit-api-1.0.1/upbit/upbit.py
```

### Comparing `python-upbit-api-1.0.0a2/LICENSE` & `python-upbit-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.0a2/setup.py` & `python-upbit-api-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-from setuptools import setup, find_packages
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-# Should be one of:
-# 'Development Status :: 3 - Alpha'
-# 'Development Status :: 4 - Beta'
-# 'Development Status :: 5 - Production/Stable'
-release_status = "Development Status :: 3 - Alpha"
-version = '1.0.0-alpha.2'
+[tool.setuptools.packages.find]
+#where = ["src"]  # ["."] by default
+include = ["upbit*"]  # ["*"] by default
+#exclude = ["tests*"]  # empty by default
+#namespaces = true  # true by default
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-
-install_requires = []
-with open("requirements.txt", "r") as reqs:
-    for install in reqs:
-        if install.startswith("#"):
-            continue
-        install_requires.append(install.strip())
-
-setup(
-    name='python-upbit-api',
-    version=version,
-    description='Python Upbit API Wrapper',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url='https://github.com/designmeme/python-upbit-api',
-    project_urls={
-        'Source': 'https://github.com/designmeme/python-upbit-api',
-        'Tracker': 'https://github.com/designmeme/python-upbit-api/issues',
-    },
-    author='이지혜 Lee Jihye',
-    author_email='ghe.lee19@gmail.com',
-    python_requires='>=3.8',
-    packages=find_packages(),
-    install_requires=install_requires,
+[project]
+name = "python-upbit-api"
+version = "1.0.1"
+authors = [
+    {name = "이지혜 Lee Jihye", email = "ghe.lee19@gmail.com"},
+]
+maintainers = [
+    {name = "이지혜 Lee Jihye", email = "ghe.lee19@gmail.com"},
+]
+description = "Python Upbit API Wrapper"
+readme = "README.md"
+requires-python = ">=3.8"
+#keywords = ["one", "two"]
+license = {file = "LICENSE"}
+classifiers = [
     # 참고: https://pypi.org/classifiers/
-    classifiers=[
-        release_status,
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-)
+    "Development Status :: 3 - Alpha",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "requests >= 2.0.0",
+    "urllib3 >= 1.0.0",
+    "pyjwt >= 2.0.0",
+]
+#dynamic = ["version"]
+
+[project.urls]
+homepage = "https://github.com/designmeme/python-upbit-api"
+repository = "https://github.com/designmeme/python-upbit-api.git"
+changelog = "https://github.com/designmeme/python-upbit-api/blob/main/CHANGELOG.md"
+issues = "https://github.com/designmeme/python-upbit-api/issues"
```

### Comparing `python-upbit-api-1.0.0a2/upbit/__init__.py` & `python-upbit-api-1.0.1/upbit/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Copyright 2023
 # 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 """A library that provides a Python interface to the Upbit API"""
 
 __all__ = [
 ]
 
-from .upbit import Upbit, RemainingReq, RequestGroup
+from .upbit import Upbit
 
 from .exceptions import (
-    UpbitError,
+    UpbitHTTPError,
     UpbitClientError,
     UpbitServerError,
     TooManyRequests,
     CreateAskError,
     CreateBidError,
     InsufficientFundsAsk,
     InsufficientFundsBid,
@@ -25,9 +25,9 @@
     InvalidQueryPayload,
     JwtVerification,
     ExpiredAccessKey,
     NonceUsed,
     NoAuthorizationIP,
     OutOfScope,
     ApiKeyError,
-    RemainingReqValueError,
+    InvalidRemainingReq,
 )
```

### Comparing `python-upbit-api-1.0.0a2/upbit/exceptions.py` & `python-upbit-api-1.0.1/upbit/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 upbit.exceptions
 
-요청 수 제한 (429)
-https://docs.upbit.com/docs/user-request-guide
-
-API 주요 에러 코드 목록 (400, 401)
-https://docs.upbit.com/docs/api-%EC%A3%BC%EC%9A%94-%EC%97%90%EB%9F%AC-%EC%BD%94%EB%93%9C-%EB%AA%A9%EB%A1%9D
-
-에러 발생시 JSON body 구조
-{
-  "error": {
-    "message": "<오류에 대한 설명>",
-    "name": "<오류 코드>"
-  }
-}
+Upbit API Error 공식 페이지 참고
+- 요청 수 제한 (429)
+    https://docs.upbit.com/docs/user-request-guide
+
+- API 주요 에러 코드 목록 (400, 401)
+    https://docs.upbit.com/docs/api-%EC%A3%BC%EC%9A%94-%EC%97%90%EB%9F%AC-%EC%BD%94%EB%93%9C-%EB%AA%A9%EB%A1%9D
+
+    에러 발생시 JSON body 구조
+    {
+      "error": {
+        "name": "<오류 코드>"
+        "message": "<오류에 대한 설명>",
+      }
+    }
 """
 
 from requests import HTTPError
 
 
-class UpbitError(HTTPError):
+class UpbitHTTPError(HTTPError):
     def __init__(self, msg: str, ex: HTTPError):
         # Invoke the super class's __init__
-        super(UpbitError, self).__init__(msg, response=ex.response)
+        super(UpbitHTTPError, self).__init__(msg, response=ex.response)
 
 
-class UpbitClientError(UpbitError):
+class UpbitClientError(UpbitHTTPError):
     """기타 업비트 클라이언트 에러 발생"""
 
 
-class UpbitServerError(UpbitError):
+class UpbitServerError(UpbitHTTPError):
     """기타 업비트 서버 에러 발생"""
 
 
 class TooManyRequests(UpbitClientError):
     """429 요청 수 제한 초과 에러 발생"""
 
 
@@ -94,23 +95,21 @@
 
 
 class OutOfScope(UpbitClientError):
     """401 허용되지 않은 기능 에러 발생"""
 
 
 class ApiKeyError(Exception):
-    """access_key 혹은 secret_key 가 필요한 경우 에러 발생"""
+    """access_key 혹은 secret_key 누락 에러 발생"""
 
 
-class RemainingReqValueError(Exception):
-    """Remaining-Req 헤더값이 규격에 맞지 않는 경우 에러 발생"""
+class InvalidRemainingReq(Exception):
+    """규격에 맞지 않는 Remaining-Req 헤더값 에러 발생"""
 
 
-# key: error.name (오류 코드)
-# value: 오류 코드에 맞는 Exception
 _ERROR_EXCEPTION_DICT = {
     "create_ask_error": CreateAskError,
     "create_bid_error": CreateBidError,
     "insufficient_funds_ask": InsufficientFundsAsk,
     "insufficient_funds_bid": InsufficientFundsBid,
     "under_min_total_ask": UnderMinTotalAsk,
     "under_min_total_bid": UnderMinTotalBid,
@@ -120,7 +119,8 @@
     "invalid_query_payload": InvalidQueryPayload,
     "jwt_verification": JwtVerification,
     "expired_access_key": ExpiredAccessKey,
     "nonce_used": NonceUsed,
     "no_authorization_i_p": NoAuthorizationIP,
     "out_of_scope": OutOfScope,
 }
+"""Upbit API 오류 코드와 1:1로 맞춘 UpbitHTTPError 예외 클래스를 담은 딕셔너리"""
```

### Comparing `python-upbit-api-1.0.0a2/upbit/upbit.py` & `python-upbit-api-1.0.1/upbit/upbit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,110 @@
 from __future__ import annotations
 
-import datetime
 import functools
 import hashlib
 import logging
-import re
-import uuid
+import uuid as _uuid
 from typing import Any, Optional, Literal, Dict, Callable, Tuple
 from urllib.parse import urlencode, unquote
 
 import jwt
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter
-from urllib3.util import Retry
 
-from upbit.exceptions import (
+from .exceptions import (
     _ERROR_EXCEPTION_DICT,
     TooManyRequests,
     UpbitServerError,
-    UpbitError,
     UpbitClientError,
     ApiKeyError,
-    RemainingReqValueError,
+    InvalidRemainingReq,
+)
+from .models import (
+    OrderBy,
+    OrderState,
+    OrderSide,
+    OrderType,
+    TransactionStatus,
+    TwoFactorType,
+    TransactionType,
+    MinuteUnit,
+    RequestGroup,
+    RemainingReq,
 )
-
-# 잔여 요청 그룹
-RequestGroup = Literal[
-    # Exchange API
-    'default',  # 주문요청 외
-    'order',
-    # Quotation API
-    'market', 'candles', 'ticker', 'crix-trades', 'orderbook',
-]
-
-
-class RemainingReq:
-    """
-    잔여 요청수 클래스
-    참고) https://docs.upbit.com/docs/user-request-guide
-
-    group: RequestGroup 잔여 요청 그룹명
-    minute: 그룹별 분당 남은 요청수.
-    second: 그룹별 초당 남은 요청수.
-    updated: 요청수 응답을 저장한 일시.
-    """
-
-    def __init__(self, remaining_req: str):
-        self._remaining_req = remaining_req
-
-        pattern = re.compile(r"group=([a-z\-]+); min=([0-9]+); sec=([0-9]+)")
-        matched = pattern.search(remaining_req)
-
-        self.group: RequestGroup = matched.group(1)
-        self.minute: int = int(matched.group(2))
-        self.second: int = int(matched.group(3))
-        self.updated: datetime.datetime = datetime.datetime.now()
-
-    def __str__(self):
-        return f"RemainingReq group={self.group!r}; min={self.minute!r}; sec={self.second!r}; updated={self.updated!r}"
-
-    def __repr__(self):
-        return f"RemainingReq(${self._remaining_req!r})"
 
 
 class Upbit:
     def __init__(self,
                  access_key: str | None = None,
                  secret_key: str | None = None,
-                 *,
-                 timeout: float | Tuple[float, float] | None = (6, 30),
+                 http_adapter: HTTPAdapter | None = None,
+                 timeout: float | Tuple[float, float] | Tuple[float, None] | None = None,
                  ):
         """
-
         :param access_key: 업비트 API Access Key
-            Quotation API만 사용한다면 설정하지 않아도 됩니다.
-            Exchange API를 사용하려면 필수로 설정해야 합니다.
-            설정하지 않고 관련 메소드를 요청하면 ApiKeyError 예외가 발생합니다.
-
         :param secret_key: 업비트 API Secret Key
-            Quotation API만 사용한다면 설정하지 않아도 됩니다.
-            Exchange API를 사용하려면 필수로 설정해야 합니다.
-            설정하지 않고 관련 메소드를 요청하면 ApiKeyError 예외가 발생합니다.
-
-        :param timeout: 업비트 API request 의 기본 timeout 설정값. (connect, read)
-            예) connect, read timeout 함께 설정시 timeout=5
-            예) connect, read timeout 따로 설정시 timeout=(6, 12)
-            예) None 인 경우 무한 대기
-            업비트 서버 점검시 연결 되지 않으며 커넥션이 무한 대기 상태가 됩니다. 이를 방지를 위해 적절한 timout 값을 설정하길 권장합니다.
-            참고: https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
+        :param http_adapter: 업비트 API 호출용 `requests.Session` 에 설정 할 HTTPAdapter
+        :param timeout: 업비트 API 호출시 `requests.Session.request` 의 기본 timeout 설정값 (connect, read)
+
+        .. note::
+            - Quotation API만 사용한다면 access_key, secret_key를 설정하지 않아도 됩니다.
+            - Exchange API를 사용하려면 access_key, secret_key를 필수로 설정해야 합니다.
+            - 업비트 서버 점검시 연결 되지 않으며 커넥션이 무한 대기 상태가 됩니다. 이를 방지를 위해 적절한 timout 값을 설정하길 권장합니다. `Requests Timeouts 참고 <https://requests.readthedocs.io/en/latest/user/advanced/#timeouts>`_
         """
 
         self._endpoint = "https://api.upbit.com/v1"
 
         self._access_key = access_key
         self._secret_key = secret_key
 
         # 요청 그룹별 잔여 요청수를 저장할 딕셔너리
         # - 키: group 명 / 값: RemainingReq 인스턴스
         self._remaining_reqs: Dict[RequestGroup, RemainingReq] = {}
 
-        # 서버에러시 자동으로 재시도하도록 max_retries 설정
+        # Requests Session 인스턴스 사용하여 모든 요청을 처리함.
         self._session = requests.Session()
-        # https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
-        retry = Retry(
-            total=None,
-            # 각자 설정해야 Retry 발생시 로그에서 어떤 요인인지 쉽게 알 수 있음.
-            redirect=5,
-            status=5,
-            connect=0,
-            read=0,
-            other=0,
-            backoff_factor=1,
-            # 기본값에 post 추가
-            allowed_methods=frozenset({'DELETE', 'GET', 'HEAD', 'OPTIONS', 'PUT', 'TRACE', 'POST'}),
-            # 서버 에러 - todo check 429 추가?
-            status_forcelist=tuple(range(500, 512)),
-            raise_on_status=True,
-        )
-        self._session.mount(self._endpoint, HTTPAdapter(max_retries=retry))
+
+        if http_adapter and isinstance(http_adapter, HTTPAdapter):
+            self._session.mount(self._endpoint, http_adapter)
+
         self._session.request = functools.partial(self._session.request, timeout=timeout)
 
         self._logger = logging.getLogger(__name__)
 
-    def _request_wrapper(func: Callable):
+    def _request_wrapper(func: Callable) -> Callable:
         """
         업비트 API 요청 래퍼
 
         1) 잔여 요청수 처리
         2) HTTPError를 UpbitError로 변환
+
+        :raises upbit.exceptions.TooManyRequests: 상태 코드가 423인 경우 발생
+        :raises upbit.exceptions.CreateAskError: 상태 코드가 400이고 인 오류 코드가 'create_ask_error' 인 경우 발생
+        :raises upbit.exceptions.CreateBidError: 상태 코드가 400이고 인 오류 코드가 'create_bid_error' 인 경우 발생
+        :raises upbit.exceptions.InsufficientFundsAsk: 상태 코드가 400이고 인 오류 코드가 'insufficient_funds_ask' 인 경우 발생
+        :raises upbit.exceptions.InsufficientFundsBid: 상태 코드가 400이고 인 오류 코드가 'insufficient_funds_bid' 인 경우 발생
+        :raises upbit.exceptions.UnderMinTotalAsk: 상태 코드가 400이고 인 오류 코드가 'under_min_total_ask' 인 경우 발생
+        :raises upbit.exceptions.UnderMinTotalAsk: 상태 코드가 400이고 인 오류 코드가 'under_min_total_ask' 인 경우 발생
+        :raises upbit.exceptions.UnderMinTotalBid: 상태 코드가 400이고 인 오류 코드가 'under_min_total_bid' 인 경우 발생
+        :raises upbit.exceptions.WithdrawAddressNotRegistered: 상태 코드가 400이고 인 오류 코드가 'withdraw_address_not_registerd' 인 경우 발생
+        :raises upbit.exceptions.InvalidParameterError: 상태 코드가 400이고 인 오류 코드가 'invalid_parameter' 인 경우 발생
+        :raises upbit.exceptions.ValidationError: 상태 코드가 400이고 인 오류 코드가 'validation_error' 인 경우 발생
+        :raises upbit.exceptions.InvalidQueryPayload: 상태 코드가 401이고 인 오류 코드가 'invalid_query_payload' 인 경우 발생
+        :raises upbit.exceptions.JwtVerification: 상태 코드가 401이고 인 오류 코드가 'jwt_verification' 인 경우 발생
+        :raises upbit.exceptions.ExpiredAccessKey: 상태 코드가 401이고 인 오류 코드가 'expired_access_key' 인 경우 발생
+        :raises upbit.exceptions.NonceUsed: 상태 코드가 401이고 인 오류 코드가 'nonce_used' 인 경우 발생
+        :raises upbit.exceptions.NoAuthorizationIP: 상태 코드가 401이고 인 오류 코드가 'no_authorization_i_p' 인 경우 발생
+        :raises upbit.exceptions.OutOfScope: 상태 코드가 401이고 인 오류 코드가 'out_of_scope' 인 경우 발생
+        :raises upbit.exceptions.UpbitClientError: 이 외에 상태 코드가 400 이상, 500 미만인 경우 발생
+        :raises upbit.exceptions.UpbitServerError: 상태 코드가 500 이상, 600 미만인 경우 발생
         """
 
+        @functools.wraps(func)
         def wrapper(self, *args: Any, **kwargs: Dict[str, Any]) -> Response:
             remaining_req: Optional[RemainingReq] = None
 
             try:
                 response: Response = func(self, *args, **kwargs)
 
                 # 잔여 요청수 기록
@@ -142,133 +112,153 @@
 
                 # status code가 400~600 일 때 예외 발생시키기
                 response.raise_for_status()
 
                 return response
             except requests.HTTPError as e:
                 status_code = e.response.status_code
+                reason = e.response.reason
+                url = e.response.url
+                error_msg = f"{status_code} Client Error: {reason} for url: {url}"
 
                 # TooManyRequests 에러 처리
-                if status_code == requests.codes.too_many_requests:
+                if status_code == 429:
                     # 이 에러는 규격화된 Upbit 에러 JSON 바디를 갖지 않음.
-                    raise TooManyRequests(f"Upbit TooManyRequests Error {status_code} Remaining-Req={remaining_req}", e)
+                    raise TooManyRequests(error_msg, e)
 
                 # Upbit API 주요 에러 코드 목록에 명시된 에러 처리
                 elif status_code in [400, 401]:
                     try:
                         # 에러 코드와 맞는 예외를 찾아 발생시킨다.
                         error_body = e.response.json()["error"]
                         error_code = error_body.get("name")
                         error_msg = error_body.get("message")
                         error_exception = _ERROR_EXCEPTION_DICT.get(error_code)
+
+                        reason = error_msg
                         if error_exception:
-                            raise error_exception(f"Upbit Client Error {status_code} {error_code=!r} {error_msg=!r}", e)
+                            raise error_exception(error_msg, e)
+                        else:
+                            # 명시되지 않은 에러가 발생한 경우
+                            raise UpbitClientError(error_msg, e)
+                    # body 내용이 json 형태가 아닌 경우
                     except requests.JSONDecodeError:
-                        raise UpbitClientError(f'Upbit Client Error {status_code} {e.response.reason}', e)
+                        raise UpbitClientError(error_msg, e)
 
                 # 기타 Upbit Client error 처리
                 elif 400 <= status_code < 500:
-                    raise UpbitClientError(f'Upbit Client Error {status_code} {e.response.reason}', e)
+                    raise UpbitClientError(error_msg, e)
 
                 # Upbit Server error 처리
-                elif 500 <= self.status_code < 600:
-                    raise UpbitServerError(f'Upbit Server Error {status_code} {e.response.reason}', e)
-
-                # 방어적 에러 작성 - 발생하지 않아야 함.
-                raise UpbitError(f'Upbit Error {status_code} {e.response.reason}', e)
+                elif 500 <= status_code < 600:
+                    raise UpbitServerError(f"{status_code} Server Error: {reason} for url: {url}", e)
 
         return wrapper
 
     @_request_wrapper
-    def _request_get(self, url: str, **kwargs) -> Response:
-        return self._session.get(url, **kwargs)
-
-    @_request_wrapper
-    def _request_put(self, url: str, **kwargs) -> Response:
-        return self._session.put(url, **kwargs)
-
-    @_request_wrapper
-    def _request_post(self, url: str, **kwargs) -> Response:
-        return self._session.post(url, **kwargs)
-
-    @_request_wrapper
-    def _request_delete(self, url: str, **kwargs) -> Response:
-        return self._session.delete(url, **kwargs)
+    def _request(self, method: str, url: str, **kwargs) -> Response:
+        return self._session.request(method, url, **kwargs)
 
     def _process_remaining_req(self, remaining_req: str) -> Optional[RemainingReq]:
-        """
-        Remaining-Req 응답 헤더를 캐시하고 RemainingReq 인스턴스로 변환하여 반환한다.
+        """Remaining-Req 응답 헤더를 캐시하고 RemainingReq 인스턴스로 변환하여 반환한다.
 
         :param remaining_req: Remaining-Req 응답 헤더값
+
         :return: RemainingReq 인스턴스
         """
         try:
             rr = RemainingReq(remaining_req)
             self._remaining_reqs[rr.group] = rr
             self._logger.debug(f"Upbit API 잔여 요청수 {rr}")
             return rr
-        except RemainingReqValueError as e:
-            self._logger.warning(f"Upbit API 잔여 요청수 처리 RemainingReqValueError. {e!r}")
+        except InvalidRemainingReq as e:
+            self._logger.warning(f"Upbit API 잔여 요청수 처리 InvalidRemainingReq. {e!r}")
             pass
         except Exception as e:
             self._logger.warning(f"Upbit API 잔여 요청수 처리 에러. {remaining_req=!r} {e!r}")
             pass
 
-    def _auth_guard(func: Callable):
-        """인증이 필요한 메서드 호출시 API 키가 셋팅되어 있는지 확인하는 가드"""
+    def _get_request_headers(self, query: Dict = None, headers: Dict | None = None) -> Dict:
+        """인증 헤더를 만들어 반환한다.
 
-        def wrapper(self, *args, **kwargs) -> Callable:
-            if not self._access_key or not self._secret_key:
-                raise ApiKeyError(f'{func.__name__} 메서드는 API Key 가 필요해요. '
-                                  f'Upbit 인스턴스 생성시 access_key, secret_key 값을 인자로 넣어주세요.')
+        :param query: 요청 바디
+        :param headers: 기존 요청 헤더
+        :return: 기존 요청 헤더에 인증 헤더를 추가해서 반환
 
-            return func(self, *args, **kwargs)
+        :raises upbit.exceptions.ApiKeyError: 인증 키 정보가 없을 때 발생
+        """
 
-        return wrapper
+        if not self._access_key or not self._secret_key:
+            raise ApiKeyError(f'인증 정보가 필요합니다.')
 
-    def _get_request_headers(self, query: Dict = None) -> Dict:
         payload = {
             "access_key": self._access_key,
-            "nonce": str(uuid.uuid4())
+            "nonce": str(_uuid.uuid4())
         }
 
         if query is not None:
             query = {k: v for k, v in query.items() if v is not None}
             query_string = unquote(urlencode(query, doseq=True)).encode("utf-8")
             m = hashlib.sha512()
             m.update(query_string)
             query_hash = m.hexdigest()
             payload['query_hash'] = query_hash
             payload['query_hash_alg'] = "SHA512"
 
         jwt_token = jwt.encode(payload, self._secret_key)
         authorization_token = 'Bearer {}'.format(jwt_token)
-        headers = {"Authorization": authorization_token}
+
+        if headers is None:
+            headers = {}
+        headers['Authorization'] = authorization_token
         return headers
 
     def get_remaining_reqs(self, group: RequestGroup) -> Optional[RemainingReq]:
-        """
-        그룹의 잔여 요청수 정보 반환
+        """그룹의 잔여 요청수 정보 반환
 
         :param group: RequestGroup 잔여 요청 그룹
+
         :return: RemainingReq 잔여 요청 정보. 이전 응답 헤더에서 얻은 정보를 저장해 놓은 가장 최신 정보.
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_candles_day('KRW-BTC')
+            rr = upbit.get_remaining_reqs('candles')
+
         """
         return self._remaining_reqs.get(group)
 
     # --------------------------------------------------------------------------
     # Exchange API > 자산
     # --------------------------------------------------------------------------
 
-    @_auth_guard
-    def get_accounts(self, **kwargs) -> Response:
-        """
-        전체 계좌 조회
-        https://docs.upbit.com/reference/%EC%A0%84%EC%B2%B4-%EA%B3%84%EC%A2%8C-%EC%A1%B0%ED%9A%8C
-        :return:
-            data example:
+    def get_accounts(self,
+                     **kwargs) -> Response:
+        """전체 계좌 조회
+
+        내가 보유한 자산 리스트를 보여줍니다.
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A0%84%EC%B2%B4-%EA%B3%84%EC%A2%8C-%EC%A1%B0%ED%9A%8C>`_
+
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_accounts()
+            print(res.json())
+
             [{
                 'currency': 'KRW',
                 'balance': '628906.97823303',
                 'locked': '0',
                 'avg_buy_price': '0',
                 'avg_buy_price_modified': True,
                 'unit_currency': 'KRW'
@@ -278,30 +268,45 @@
                 'locked': '0',
                 'avg_buy_price': '292.6613',
                 'avg_buy_price_modified': False,
                 'unit_currency': 'KRW'
             }, ...]
         """
         url = self._endpoint + "/accounts"
-        headers = self._get_request_headers()
+        headers = self._get_request_headers(headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, **kwargs)
+        return self._request('get', url, headers=headers, **kwargs)
 
     # --------------------------------------------------------------------------
     # Exchange API > 주문
     # --------------------------------------------------------------------------
 
-    @_auth_guard
-    def get_order_chance(self, market: str = "KRW-BTC", **kwargs) -> Response:
-        """
-        주문 가능 정보 조회
-        https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EA%B0%80%EB%8A%A5-%EC%A0%95%EB%B3%B4
+    def get_order_chance(self,
+                         market: str,
+                         **kwargs) -> Response:
+        """주문 가능 정보 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EA%B0%80%EB%8A%A5-%EC%A0%95%EB%B3%B4>`_
+
         :param market: 마켓 코드 (ex. KRW-BTC)
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_order_chance('KRW-BTC')
+            print(res.json())
+
             {'ask_account': {'avg_buy_price': '28560783.8337',
                              'avg_buy_price_modified': False,
                              'balance': '0',
                              'currency': 'BTC',
                              'locked': '0',
                              'unit_currency': 'KRW'},
              'ask_fee': '0.0005',
@@ -325,27 +330,45 @@
                         'order_types': ['limit'],
                         'state': 'active'}}
         """
         url = self._endpoint + "/orders/chance"
         params = {
             "market": market,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
 
-    @_auth_guard
-    def get_order(self, order_uuid: str = None, identifier: str = None, **kwargs) -> Response:
-        """
-        개별 주문 조회
-        https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C
-        :param order_uuid: 주문 UUID
+    def get_order(self,
+                  uuid: Optional[str] = None,
+                  identifier: Optional[str] = None,
+                  **kwargs) -> Response:
+        """개별 주문 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C>`_
+
+        .. note:: uuid 혹은 identifier 둘 중 하나의 값이 반드시 포함되어야 합니다.
+
+        :param uuid: 주문 UUID
         :param identifier: 조회용 사용자 지정 값
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_order('d7c96420-a9ab-4ae8-a461-3db412427fb3')
+            print(res.json())
+
             {
                 'created_at': '2023-02-06T11:00:45+09:00',
                 'executed_volume': '132.99843443',
                 'locked': '0',
                 'market': 'KRW-STRAX',
                 'ord_type': 'market',
                 'paid_fee': '50.738902735045',
@@ -365,38 +388,58 @@
                 'trades_count': 1,
                 'uuid': 'd7c96420-a9ab-4ae8-a461-3db412427fb3',
                 'volume': '132.99843443'
             }
         """
         url = self._endpoint + "/order"
         params = {
-            "uuid": order_uuid,
+            "uuid": uuid,
             "identifier": identifier,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
+
+        return self._request('get', url, headers=headers, params=params, **kwargs)
+
+    def get_orders(self,
+                   market: Optional[str] = None,
+                   uuids: Optional[list[str]] = None,
+                   identifiers: Optional[list[str]] = None,
+                   state: OrderState = 'wait',
+                   states: Optional[list[OrderState]] = None,
+                   page: int = 1,
+                   limit: int = 100,
+                   order_by: OrderBy = 'desc',
+                   **kwargs) -> Response:
+        """주문 리스트 조회
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C>`_
+
+        :param market: 마켓 코드 (ex. KRW-BTC)
+        :param uuids: 주문 UUID 리스트
+        :param identifiers: 주문 identifier 리스트
+        :param state: 주문 상태
+        :param states: 주문 상태 리스트
+        :param page: 페이지 수
+        :param limit: 요청 개수
+        :param order_by: 정렬 방식
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_orders(market='KRW-ELF', state='done')
+            print(res.json())
 
-    @_auth_guard
-    def get_orders(self, market: str = None, uuids: [str] = None, identifiers: [str] = None,
-                   state: str = 'wait', states: [str] = None, page: int = 1, limit: int = 100,
-                   order_by: str = 'desc', **kwargs) -> Response:
-        """
-        주문 리스트 조회
-        https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C
-        :param market: 마켓 아이디
-        :param uuids: 주문 UUID의 목록
-        :param identifiers: 주문 identifier의 목록
-        :param state: 주문 상태 wait, watch, done, cancel
-        :param states: 주문 상태의 목록
-        :param page: 페이지 수, default: 1
-        :param limit: 요청 개수, default: 100
-        :param order_by: 정렬 방식 asc, desc(default)
-        :return:
-            data example:
             [{
                 'created_at': '2023-02-15T08:00:40+09:00',
                 'executed_volume': '380.4181703',
                 'locked': '0',
                 'market': 'KRW-ELF',
                 'ord_type': 'market',
                 'paid_fee': '56.6823073747',
@@ -417,27 +460,45 @@
             "identifiers[]": identifiers,
             "state": state,
             "states[]": states,
             "page": page,
             "limit": limit,
             "order_by": order_by,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
 
-    @_auth_guard
-    def delete_order(self, order_uuid: str = None, identifier: str = None, **kwargs) -> Response:
-        """
-        주문 취소 접수
-        https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EC%B7%A8%EC%86%8C
-        :param order_uuid: 주문 UUID
+    def delete_order(self,
+                     uuid: Optional[str] = None,
+                     identifier: Optional[str] = None,
+                     **kwargs) -> Response:
+        """주문 취소 접수
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EC%B7%A8%EC%86%8C>`_
+
+        .. note:: uuid 혹은 identifier 둘 중 하나의 값이 반드시 포함되어야 합니다.
+
+        :param uuid: 주문 UUID
         :param identifier: 조회용 사용자 지정 값
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.delete_order('cdd92199-2897-4e14-9448-f923320408ad')
+            print(res.json())
+
             {
                 "uuid": "cdd92199-2897-4e14-9448-f923320408ad",
                 "side": "bid",
                 "ord_type": "limit",
                 "price": "100.0",
                 "state": "wait",
                 "market": "KRW-BTC",
@@ -450,36 +511,54 @@
                 "locked": "1.0015",
                 "executed_volume": "0.0",
                 "trades_count": 0
             }
         """
         url = self._endpoint + "/order"
         params = {
-            "uuid": order_uuid,
+            "uuid": uuid,
             "identifier": identifier,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
+
+        return self._request('delete', url, headers=headers, params=params, **kwargs)
 
-        return self._request_delete(url, headers=headers, params=params, **kwargs)
+    def create_order(self,
+                     market: str, 
+                     side: OrderSide, 
+                     ord_type: OrderType,
+                     volume: Optional[str] = None,
+                     price: Optional[str] = None,
+                     identifier: Optional[str] = None,
+                     **kwargs) -> Response:
+        """주문하기
 
-    @_auth_guard
-    def create_order(self, market: str, side: str, ord_type: str,
-                     volume: str = None, price: str = None,
-                     identifier: str = None, **kwargs) -> Response:
-        """
-        주문하기
-        https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8%ED%95%98%EA%B8%B0
-        :param market: 마켓 ID (필수)
-        :param side: 주문 종류 (필수) - bid(매수), ask(매도)
-        :param ord_type: 주문 타입 (필수) - limit(지정가), price(시장가 매수), market(시장가 매도)
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8%ED%95%98%EA%B8%B0>`_
+
+        :param market: 마켓 코드 (ex. KRW-BTC)
+        :param side: 주문 종류 - bid(매수), ask(매도)
+        :param ord_type: 주문 타입 - limit(지정가), price(시장가 매수), market(시장가 매도)
         :param volume: 주문량 (지정가, 시장가 매도 시 필수)
-        :param price: 주문 가격. (지정가, 시장가 매수 시 필수)
-        :param identifier: 조회용 사용자 지정 값 (선택)
-        :return:
-            data example:
+        :param price: 주문 가격 (지정가, 시장가 매수 시 필수)
+        :param identifier: 조회용 사용자 지정 값
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.create_order(market='KRW-BTC', side='bid', ord_type='limit', price='100', volume='0.01')
+            print(res.json())
+
             {
                 "uuid": "cdd92199-2897-4e14-9448-f923320408ad",
                 "side": "bid",
                 "ord_type": "limit",
                 "price": "100.0",
                 "avg_price": "0.0",
                 "state": "wait",
@@ -500,37 +579,57 @@
             "market": market,
             "side": side,
             "volume": volume,
             "price": price,
             "ord_type": ord_type,
             "identifier": identifier,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_post(url, headers=headers, params=params, **kwargs)
+        return self._request('post', url, headers=headers, params=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Exchange API > 출금
     # --------------------------------------------------------------------------
 
-    @_auth_guard
-    def get_withdraws(self, currency: str = None, state: str = None, uuids: [str] = None, txids: [str] = None,
-                      page: int = 1, limit: int = 100, order_by: str = 'desc', **kwargs) -> Response:
-        """
-        출금 리스트 조회
-        https://docs.upbit.com/reference/%EC%A0%84%EC%B2%B4-%EC%B6%9C%EA%B8%88-%EC%A1%B0%ED%9A%8C
+    def get_withdraws(self,
+                      currency: Optional[str] = None,
+                      state: Optional[TransactionStatus] = None,
+                      uuids: Optional[list[str]] = None,
+                      txids: Optional[list[str]] = None,
+                      page: int = 1,
+                      limit: int = 100,
+                      order_by: OrderBy = 'desc',
+                      **kwargs) -> Response:
+        """출금 리스트 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A0%84%EC%B2%B4-%EC%B6%9C%EA%B8%88-%EC%A1%B0%ED%9A%8C>`_
+
         :param currency: Currency 코드
-        :param state: 출금 상태 WAITING, PROCESSING, DONE, FAILED, CANCELLED, REJECTED
-        :param uuids: 출금 UUID의 목록
-        :param txids: 출금 TXID의 목록
-        :param page: 페이지 수, default: 1
+        :param state: 출금 상태
+        :param uuids: 출금 UUID 리스트
+        :param txids: 출금 TXID 리스트
+        :param page: 페이지 수
         :param limit: 개수 제한 (default: 100, max: 100)
-        :param order_by: 정렬 방식 asc, desc(default)
-        :return:
-            data example:
+        :param order_by: 정렬 방식
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_withdraws(currency='XRP', state='DONE')
+            print(res.json())
+
             [{
                 "type": "withdraw",
                 "uuid": "35a4f1dc-1db5-4d6b-89b5-7ec137875956",
                 "currency": "XRP",
                 "txid": "98c15999f0bdc4ae0e8a-ed35868bb0c204fe6ec29e4058a3451e-88636d1040f4baddf943274ce37cf9cc",
                 "state": "DONE",
                 "created_at": "2019-02-28T15:17:51+09:00",
@@ -546,28 +645,45 @@
             "state": state,
             "uuids[]": uuids,
             "txids[]": txids,
             "page": page,
             "limit": limit,
             "order_by": order_by,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
 
-    @_auth_guard
-    def get_withdraw(self, data_uuid: str = None, txid: str = None, currency: str = None, **kwargs) -> Response:
-        """
-        개별 출금 조회
-        https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%B6%9C%EA%B8%88-%EC%A1%B0%ED%9A%8C
-        :param data_uuid: 출금 UUID
+    def get_withdraw(self,
+                     uuid: Optional[str] = None,
+                     txid: Optional[str] = None,
+                     currency: Optional[str] = None,
+                     **kwargs) -> Response:
+        """개별 출금 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%B6%9C%EA%B8%88-%EC%A1%B0%ED%9A%8C>`_
+
+        :param uuid: 출금 UUID
         :param txid: 출금 TXID
         :param currency: Currency 코드
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_withdraw('9f432943-54e0-40b7-825f-b6fec8b42b79')
+            print(res.json())
+
             {
                 "type": "withdraw",
                 "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
                 "currency": "BTC",
                 "txid": null,
                 "state": "processing",
                 "created_at": "2018-04-13T11:24:01+09:00",
@@ -575,30 +691,45 @@
                 "amount": "0.01",
                 "fee": "0.0",
                 "transaction_type": "default"
             }
         """
         url = self._endpoint + "/withdraw"
         params = {
-            "uuid": data_uuid,
+            "uuid": uuid,
             "txid": txid,
             "currency": currency,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
+
+    def get_withdraw_chance(self,
+                            currency: str,
+                            **kwargs) -> Response:
+        """출금 가능 정보 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%B6%9C%EA%B8%88-%EA%B0%80%EB%8A%A5-%EC%A0%95%EB%B3%B4>`_
 
-    @_auth_guard
-    def get_withdraw_chance(self, currency: str, **kwargs) -> Response:
-        """
-        출금 가능 정보 조회
-        https://docs.upbit.com/reference/%EC%B6%9C%EA%B8%88-%EA%B0%80%EB%8A%A5-%EC%A0%95%EB%B3%B4
         :param currency: Currency 코드
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_withdraw_chance('BTC')
+            print(res.json())
+
             {
                 "member_level": {
                     "security_level": 3,
                     "fee_level": 0,
                     "email_verified": true,
                     "identity_auth_verified": true,
                     "bank_account_verified": true,
@@ -636,32 +767,49 @@
                 }
             }
         """
         url = self._endpoint + "/withdraws/chance"
         params = {
             "currency": currency,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
 
-    @_auth_guard
-    def create_withdraw_coin(self, currency: str, amount: float, address: str,
-                             secondary_address: str = None, transaction_type: str = 'default',
+    def create_withdraw_coin(self,
+                             currency: str,
+                             amount: str,
+                             address: str,
+                             secondary_address: Optional[str] = None,
+                             transaction_type: TransactionType = 'default',
                              **kwargs) -> Response:
-        """
-        코인 출금하기
-        https://docs.upbit.com/reference/%EC%BD%94%EC%9D%B8-%EC%B6%9C%EA%B8%88%ED%95%98%EA%B8%B0
+        """코인 출금하기
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%BD%94%EC%9D%B8-%EC%B6%9C%EA%B8%88%ED%95%98%EA%B8%B0>`_
+
         :param currency: Currency 코드
         :param amount: 출금 수량
         :param address: 출금 가능 주소에 등록된 출금 주소
         :param secondary_address: 2차 출금 주소 (필요한 코인에 한해서)
-        :param transaction_type: 출금 유형 - default : 일반출금, internal : 바로출금
-        :return:
-            data example:
+        :param transaction_type: 출금 유형. default: 일반출금, internal: 바로출금
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.create_withdraw_coin('BTC', '0.01', '1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa')
+            print(res.json())
+
             {
                 "type": "withdraw",
                 "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
                 "currency": "BTC",
                 "txid": "ebe6937b-130e-4066-8ac6-4b0e67f28adc",
                 "state": "processing",
                 "created_at": "2018-04-13T11:24:01+09:00",
@@ -676,27 +824,43 @@
         params = {
             "currency": currency,
             "amount": amount,
             "address": address,
             "secondary_address": secondary_address,
             "transaction_type": transaction_type,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_post(url, headers=headers, json=params, **kwargs)
+        return self._request('post', url, headers=headers, json=params, **kwargs)
+
+    def create_withdraw_krw(self,
+                            amount: str,
+                            two_factor_type: TwoFactorType = 'kakao_pay',
+                            **kwargs) -> Response:
+        """원화 출금하기
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9B%90%ED%99%94-%EC%B6%9C%EA%B8%88%ED%95%98%EA%B8%B0>`_
+
+        :param amount: 출금액
+        :param two_factor_type: 2차 인증 수단
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.create_withdraw_krw('10000')
+            print(res.json())
 
-    @_auth_guard
-    def create_withdraw_krw(self, amount: float, two_factor_type: str = 'kakao_pay', **kwargs) -> Response:
-        """
-        원화 출금하기
-        https://docs.upbit.com/reference/%EC%9B%90%ED%99%94-%EC%B6%9C%EA%B8%88%ED%95%98%EA%B8%B0
-        :param amount: 출금 수량
-        :param two_factor_type: 2차 인증 수단 - kakao_pay : 카카오페이 인증(default), naver : 네이버 인증
-        :return:
-            data example:
             {
                 "type": "withdraw",
                 "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
                 "currency": "KRW",
                 "txid": "ebe6937b-130e-4066-8ac6-4b0e67f28adc",
                 "state": "processing",
                 "created_at": "2018-04-13T11:24:01+09:00",
@@ -707,37 +871,57 @@
             }
         """
         url = self._endpoint + "/withdraws/krw"
         params = {
             "amount": amount,
             "two_factor_type": two_factor_type,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_post(url, headers=headers, json=params, **kwargs)
+        return self._request('post', url, headers=headers, json=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Exchange API > 입금
     # --------------------------------------------------------------------------
 
-    @_auth_guard
-    def get_deposits(self, currency: str = None, state: str = None, uuids: [str] = None, txids: [str] = None,
-                     page: int = 1, limit: int = 100, order_by: str = 'desc', **kwargs) -> Response:
-        """
-        입금 리스트 조회
-        https://docs.upbit.com/reference/%EC%9E%85%EA%B8%88-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C
+    def get_deposits(self,
+                     currency: Optional[str] = None,
+                     state: Optional[TransactionStatus] = None,
+                     uuids: Optional[list[str]] = None,
+                     txids: Optional[list[str]] = None,
+                     page: int = 1,
+                     limit: int = 100,
+                     order_by: OrderBy = 'desc',
+                     **kwargs) -> Response:
+        """입금 리스트 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9E%85%EA%B8%88-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C>`_
+
         :param currency: Currency 코드
-        :param state: 출금 상태 WAITING, PROCESSING, DONE, FAILED, CANCELLED, REJECTED
-        :param uuids: 출금 UUID의 목록
-        :param txids: 출금 TXID의 목록
-        :param page: 페이지 수, default: 1
+        :param state: 출금 상태
+        :param uuids: 출금 UUID 리스트
+        :param txids: 출금 TXID 리스트
+        :param page: 페이지 수
         :param limit: 개수 제한 (default: 100, max: 100)
-        :param order_by: 정렬 방식 asc, desc(default)
-        :return:
-            data example:
+        :param order_by: 정렬 방식
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_deposits(currency='KRW')
+            print(res.json())
+
             [{
                 "type": "deposit",
                 "uuid": "94332e99-3a87-4a35-ad98-28b0c969f830",
                 "currency": "KRW",
                 "txid": "9e37c537-6849-4c8b-a134-57313f5dfc5a",
                 "state": "ACCEPTED",
                 "created_at": "2017-12-08T15:38:02+09:00",
@@ -753,28 +937,45 @@
             "state": state,
             "uuids[]": uuids,
             "txids[]": txids,
             "page": page,
             "limit": limit,
             "order_by": order_by,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
 
-    @_auth_guard
-    def get_deposit(self, data_uuid: str = None, txid: str = None, currency: str = None, **kwargs) -> Response:
-        """
-        개별 입금 조회
-        https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%9E%85%EA%B8%88-%EC%A1%B0%ED%9A%8C
-        :param data_uuid: 출금 UUID
+    def get_deposit(self,
+                    uuid: Optional[str] = None,
+                    txid: Optional[str] = None,
+                    currency: Optional[str] = None,
+                    **kwargs) -> Response:
+        """개별 입금 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%9E%85%EA%B8%88-%EC%A1%B0%ED%9A%8C>`_
+
+        :param uuid: 출금 UUID
         :param txid: 출금 TXID
         :param currency: Currency 코드
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_deposit('94332e99-3a87-4a35-ad98-28b0c969f830')
+            print(res.json())
+
             {
                 "type": "deposit",
                 "uuid": "94332e99-3a87-4a35-ad98-28b0c969f830",
                 "currency": "KRW",
                 "txid": "9e37c537-6849-4c8b-a134-57313f5dfc5a",
                 "state": "ACCEPTED",
                 "created_at": "2017-12-08T15:38:02+09:00",
@@ -782,193 +983,310 @@
                 "amount": "100000.0",
                 "fee": "0.0",
                 "transaction_type": "default"
             }
         """
         url = self._endpoint + "/deposit"
         params = {
-            "uuid": data_uuid,
+            "uuid": uuid,
             "txid": txid,
             "currency": currency,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
+
+    def create_coin_address(self,
+                            currency: str,
+                            **kwargs) -> Response:
+        """입금 주소 생성 요청
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%83%9D%EC%84%B1-%EC%9A%94%EC%B2%AD>`_
+
+        :param currency: Currency 코드
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.create_coin_address('BTC')
+            print(res.json())
 
-    @_auth_guard
-    def create_deposit_krw(self, amount: float, two_factor_type: str = 'kakao_pay', **kwargs) -> Response:
-        """
-        원화 입금하기
-        https://docs.upbit.com/reference/%EC%9B%90%ED%99%94-%EC%9E%85%EA%B8%88%ED%95%98%EA%B8%B0
-        :param amount: 출금 수량
-        :param two_factor_type: 2차 인증 수단 - kakao_pay : 카카오페이 인증(default), naver : 네이버 인증
-        :return:
-            data example:
             {
-                "type": "deposit",
-                "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
-                "currency": "KRW",
-                "txid": "ebe6937b-130e-4066-8ac6-4b0e67f28adc",
-                "state": "processing",
-                "created_at": "2018-04-13T11:24:01+09:00",
-                "done_at": null,
-                "amount": "10000",
-                "fee": "0.0",
-                "transaction_type": "default"
+              "success": true,
+              "message": "BTC 입금주소를 생성중입니다."
             }
         """
-        url = self._endpoint + "/deposits/krw"
+        url = self._endpoint + "/deposits/generate_coin_address"
         params = {
-            "amount": amount,
-            "two_factor_type": two_factor_type,
+            "currency": currency,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_post(url, headers=headers, json=params, **kwargs)
+        return self._request('post', url, headers=headers, json=params, **kwargs)
+
+    def get_coin_addresses(self,
+                           **kwargs) -> Response:
+        """전체 입금 주소 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A0%84%EC%B2%B4-%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%A1%B0%ED%9A%8C>`_
+
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_coin_addresses()
+            print(res.json())
 
-    @_auth_guard
-    def get_coin_addresses(self, **kwargs) -> Response:
-        """
-        전체 입금 주소 조회
-        https://docs.upbit.com/reference/%EC%A0%84%EC%B2%B4-%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%A1%B0%ED%9A%8C
-        :return:
-            data example:
             [{
                 "currency": "BTC",
                 "deposit_address": "3EusRwybuZUhVDeHL7gh3HSLmbhLcy7NqD",
                 "secondary_address": null
             }, ...]
         """
         url = self._endpoint + "/deposits/coin_addresses"
-        headers = self._get_request_headers()
+        headers = self._get_request_headers(headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, **kwargs)
+        return self._request('get', url, headers=headers, **kwargs)
+
+    def get_coin_address(self,
+                         currency: str,
+                         **kwargs) -> Response:
+        """개별 입금 주소 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%A1%B0%ED%9A%8C>`_
 
-    @_auth_guard
-    def get_coin_address(self, currency: str = None, **kwargs) -> Response:
-        """
-        개별 입금 주소 조회
-        https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%A1%B0%ED%9A%8C
         :param currency: Currency 코드
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_coin_address('BTC')
+            print(res.json())
+
             {
                 "currency": "BTC",
                 "deposit_address": "3EusRwybuZUhVDeHL7gh3HSLmbhLcy7NqD",
                 "secondary_address": null
             }
         """
         url = self._endpoint + "/deposits/coin_address"
         params = {
             "currency": currency,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, params=params, **kwargs)
+        return self._request('get', url, headers=headers, params=params, **kwargs)
+
+    def create_deposit_krw(self,
+                           amount: str,
+                           two_factor_type: TwoFactorType = 'kakao_pay',
+                           **kwargs) -> Response:
+        """원화 입금하기
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9B%90%ED%99%94-%EC%9E%85%EA%B8%88%ED%95%98%EA%B8%B0>`_
+
+        :param amount: 입금액
+        :param two_factor_type: 2차 인증 수단
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.create_deposit_krw('10000')
+            print(res.json())
 
-    @_auth_guard
-    def create_coin_address(self, currency: str, **kwargs) -> Response:
-        """
-        입금 주소 생성하기
-        https://docs.upbit.com/reference/%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%83%9D%EC%84%B1-%EC%9A%94%EC%B2%AD
-        :param currency: Currency 코드
-        :return:
-            data example:
             {
-              "success": true,
-              "message": "BTC 입금주소를 생성중입니다."
+                "type": "deposit",
+                "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
+                "currency": "KRW",
+                "txid": "ebe6937b-130e-4066-8ac6-4b0e67f28adc",
+                "state": "processing",
+                "created_at": "2018-04-13T11:24:01+09:00",
+                "done_at": null,
+                "amount": "10000",
+                "fee": "0.0",
+                "transaction_type": "default"
             }
         """
-        url = self._endpoint + "/deposits/generate_coin_address"
+        url = self._endpoint + "/deposits/krw"
         params = {
-            "currency": currency,
+            "amount": amount,
+            "two_factor_type": two_factor_type,
         }
-        headers = self._get_request_headers(params)
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
-        return self._request_post(url, headers=headers, json=params, **kwargs)
+        return self._request('post', url, headers=headers, json=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Exchange API > 서비스 정보
     # --------------------------------------------------------------------------
 
-    @_auth_guard
-    def get_wallet_status(self, **kwargs) -> Response:
-        """
-        입출금 현황 조회 (전체)
-        https://docs.upbit.com/reference/%EC%9E%85%EC%B6%9C%EA%B8%88-%ED%98%84%ED%99%A9
-        :return:
-            data example:
+    def get_wallet_status(self,
+                          **kwargs) -> Response:
+        """입출금 현황 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9E%85%EC%B6%9C%EA%B8%88-%ED%98%84%ED%99%A9>`_
+
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_wallet_status()
+            print(res.json())
+
             [{
                 'currency': 'BTC',
                 'wallet_state': 'working',
                 'block_state': 'normal',
                 'block_height': 776512,
                 'block_updated_at': '2023-02-14T13:37:39.806+00:00',
                 'block_elapsed_minutes': 12
             }, ...]
         """
         url = self._endpoint + "/status/wallet"
-        headers = self._get_request_headers()
+        headers = self._get_request_headers(headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, **kwargs)
+        return self._request('get', url, headers=headers, **kwargs)
 
-    @_auth_guard
-    def get_api_keys(self, **kwargs) -> Response:
-        """
-        API 키 리스트 조회
-        https://docs.upbit.com/reference/open-api-%ED%82%A4-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C
-        :return:
-            data example:
-            [{'access_key': 'xxxxxxxxxxxxxxxxxxxxxxxx', 'expire_at': '2024-02-13T13:57:59+09:00'}, ...]
+    def get_api_keys(self,
+                     **kwargs) -> Response:
+        """API 키 리스트 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/open-api-%ED%82%A4-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C>`_
+
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_api_keys()
+            print(res.json())
+
+            [{
+                'access_key': 'xxxxxxxxxxxxxxxxxxxxxxxx',
+                'expire_at': '2021-03-09T12:39:39+00:00'
+             }, ...]
         """
         url = self._endpoint + "/api_keys"
-        headers = self._get_request_headers()
+        headers = self._get_request_headers(headers=kwargs.pop('headers', None))
 
-        return self._request_get(url, headers=headers, **kwargs)
+        return self._request('get', url, headers=headers, **kwargs)
 
     # --------------------------------------------------------------------------
     # Quotation API > 시세 종목 조회
     # --------------------------------------------------------------------------
 
-    def get_markets(self, is_detail: bool = None, **kwargs) -> Response:
-        """
-        거래 가능한 마켓 목록 조회
-        https://docs.upbit.com/reference/%EB%A7%88%EC%BC%93-%EC%BD%94%EB%93%9C-%EC%A1%B0%ED%9A%8C
-        :param is_detail: 유의 종목(market_warning) 정보 포함 여부
-        :return:
-            data example:
+    def get_markets(self,
+                    is_detail: bool = False,
+                    **kwargs) -> Response:
+        """거래 가능한 마켓 목록 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EB%A7%88%EC%BC%93-%EC%BD%94%EB%93%9C-%EC%A1%B0%ED%9A%8C>`_
+
+        :param is_detail: 유의종목 필드과 같은 상세 정보 노출 여부
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_markets(True)
+            print(res.json())
+
             [{
                 'market_warning': 'NONE',
                 'market': 'KRW-BTC',
                 'korean_name': '비트코인',
                 'english_name': 'Bitcoin'
             }, ...]
         """
         url = self._endpoint + "/market/all"
         params = {
             "isDetails": is_detail,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Quotation API > 시세 캔들 조회
     # --------------------------------------------------------------------------
 
-    def get_candles_minute(self, unit: int = 1, market: str = "KRW-BTC",
-                           to: str = None, count: int = None, **kwargs) -> Response:
-        """
-        분(Minute) 캔들 조회
-        https://docs.upbit.com/reference/%EB%B6%84minute-%EC%BA%94%EB%93%A4-1
-        :param unit: 분 단위. 가능한 값 : 1, 3, 5, 15, 10, 30, 60, 240
+    def get_candles_minute(self,
+                           unit: MinuteUnit,
+                           market: str,
+                           to: Optional[str] = None,
+                           count: Optional[int] = None,
+                           **kwargs) -> Response:
+        """분(Minute) 캔들 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EB%B6%84minute-%EC%BA%94%EB%93%A4-1>`_
+
+        :param unit: 분 단위.
         :param market: 마켓 코드 (ex. KRW-BTC)
         :param to: 마지막 캔들 시각 (exclusive). 포맷 : yyyy-MM-dd'T'HH:mm:ss'Z' or yyyy-MM-dd HH:mm:ss. 비워서 요청시 가장 최근 캔들
-        :param count: 캔들 개수(최대 200개까지 요청 가능) - 200개 초과로 요청해도 200개만 응답함
-        :return:
-            data example:
+        :param count: 캔들 개수. 최대 200
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_candles_minute(1, 'KRW-BTC')
+            print(res.json())
+
             [{
                 'market': 'KRW-BTC',
                 'candle_date_time_utc': '2023-02-14T09:43:00',
                 'candle_date_time_kst': '2023-02-14T18:43:00',
                 'opening_price': 28087000.0,
                 'high_price': 28090000.0,
                 'low_price': 28080000.0,
@@ -982,27 +1300,41 @@
         url = self._endpoint + "/candles/minutes/" + str(unit)
         params = {
             "market": market,
             "to": to,
             "count": count,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
+
+    def get_candles_day(self,
+                        market: str,
+                        to: Optional[str] = None,
+                        count: Optional[int] = None,
+                        converting_price_unit: Optional[str] = None,
+                        **kwargs) -> Response:
+        """일(Day) 캔들 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9D%BCday-%EC%BA%94%EB%93%A4-1>`_
 
-    def get_candles_day(self, market: str = "KRW-BTC", to: str = None, count: int = None,
-                        converting_price_unit: str = None, **kwargs) -> Response:
-        """
-        일(Day) 캔들 조회
-        https://docs.upbit.com/reference/%EC%9D%BCday-%EC%BA%94%EB%93%A4-1
         :param market: 마켓 코드 (ex. KRW-BTC)
         :param to: 마지막 캔들 시각 (exclusive). 포맷 : yyyy-MM-dd'T'HH:mm:ss'Z' or yyyy-MM-dd HH:mm:ss. 비워서 요청시 가장 최근 캔들
-        :param count: 캔들 개수(최대 200개까지 요청 가능) - 200개 초과로 요청해도 200개만 응답함
-        :param converting_price_unit: 원화 마켓이 아닌 다른 마켓(ex. BTC, ETH)의 일봉 요청시, 종가 환산 화폐 단위 (예, KRW)
-        :return:
-            data example:
+        :param count: 캔들 개수. 최대 200
+        :param converting_price_unit: 원화 마켓이 아닌 다른 마켓(ex. BTC, USDT)의 일봉 요청시, 종가 환산 화폐 단위 (예, KRW)
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_candles_day('USDT-BTC', converting_price_unit='KRW')
+            print(res.json())
+
             [{
                 'market': 'USDT-BTC',
                 'candle_date_time_utc': '2023-02-14T00:00:00',
                 'candle_date_time_kst': '2023-02-14T09:00:00',
                 'opening_price': 21366.66292861,
                 'high_price': 21977.99979999,
                 'low_price': 21121.0004,
@@ -1020,25 +1352,39 @@
         params = {
             "market": market,
             "to": to,
             "count": count,
             "convertingPriceUnit": converting_price_unit,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
+
+    def get_candles_week(self,
+                         market: str,
+                         to: Optional[str] = None,
+                         count: Optional[int] = None,
+                         **kwargs) -> Response:
+        """주(Week) 캔들 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BCweek-%EC%BA%94%EB%93%A4-1>`_
 
-    def get_candles_week(self, market: str = "KRW-BTC", to: str = None, count: int = None, **kwargs) -> Response:
-        """
-        주(Week) 캔들 조회
-        https://docs.upbit.com/reference/%EC%A3%BCweek-%EC%BA%94%EB%93%A4-1
         :param market: 마켓 코드 (ex. KRW-BTC)
         :param to: 마지막 캔들 시각 (exclusive). 포맷 : yyyy-MM-dd'T'HH:mm:ss'Z' or yyyy-MM-dd HH:mm:ss. 비워서 요청시 가장 최근 캔들
-        :param count: 캔들 개수(최대 200개까지 요청 가능) - 200개 초과로 요청해도 200개만 응답함
-        :return:
-            data example:
+        :param count: 캔들 개수. 최대 200
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_candles_week('KRW-BTC')
+            print(res.json())
+
             [{
                 'market': 'KRW-BTC',
                 'candle_date_time_utc': '2023-02-14T09:43:00',
                 'candle_date_time_kst': '2023-02-14T18:43:00',
                 'opening_price': 28087000.0,
                 'high_price': 28090000.0,
                 'low_price': 28080000.0,
@@ -1052,25 +1398,39 @@
         url = self._endpoint + "/candles/weeks"
         params = {
             "market": market,
             "to": to,
             "count": count,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
+
+    def get_candles_month(self,
+                          market: str,
+                          to: Optional[str] = None,
+                          count: Optional[int] = None,
+                          **kwargs) -> Response:
+        """월(Month) 캔들 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%9B%94month-%EC%BA%94%EB%93%A4-1>`_
 
-    def get_candles_month(self, market: str = "KRW-BTC", to: str = None, count: int = None, **kwargs) -> Response:
-        """
-        월(Month) 캔들 조회
-        https://docs.upbit.com/reference/%EC%9B%94month-%EC%BA%94%EB%93%A4-1
         :param market: 마켓 코드 (ex. KRW-BTC)
         :param to: 마지막 캔들 시각 (exclusive). 포맷 : yyyy-MM-dd'T'HH:mm:ss'Z' or yyyy-MM-dd HH:mm:ss. 비워서 요청시 가장 최근 캔들
-        :param count: 캔들 개수(최대 200개까지 요청 가능) - 200개 초과로 요청해도 200개만 응답함
-        :return:
-            data example:
+        :param count: 캔들 개수. 최대 200
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_candles_month('KRW-BTC')
+            print(res.json())
+
             [{
                 'market': 'KRW-BTC',
                 'candle_date_time_utc': '2023-02-14T09:43:00',
                 'candle_date_time_kst': '2023-02-14T18:43:00',
                 'opening_price': 28087000.0,
                 'high_price': 28090000.0,
                 'low_price': 28080000.0,
@@ -1084,32 +1444,47 @@
         url = self._endpoint + "/candles/months"
         params = {
             "market": market,
             "to": to,
             "count": count,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Quotation API > 시세 체결 조회
     # --------------------------------------------------------------------------
 
-    def get_trades_ticks(self, market: str = "KRW-BTC", to: str = None, count: int = None,
-                         cursor: str = None, days_ago: int = None, **kwargs) -> Response:
-        """
-        최근 체결 내역 조회
-        https://docs.upbit.com/reference/%EC%B5%9C%EA%B7%BC-%EC%B2%B4%EA%B2%B0-%EB%82%B4%EC%97%AD
+    def get_trades_ticks(self,
+                         market: str,
+                         to: Optional[str] = None,
+                         count: Optional[int] = None,
+                         cursor: Optional[str] = None,
+                         days_ago: Optional[Literal[1, 2, 3, 4, 5, 6, 7]] = None,
+                         **kwargs) -> Response:
+        """최근 체결 내역 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%B5%9C%EA%B7%BC-%EC%B2%B4%EA%B2%B0-%EB%82%B4%EC%97%AD>`_
+
         :param market: 마켓 코드 (ex. KRW-BTC)
         :param to: 마지막 체결 시각. 형식 : [HHmmss 또는 HH:mm:ss]. 비워서 요청시 가장 최근 데이터
         :param count: 체결 개수. 최대 500개
         :param cursor: 페이지네이션 커서 (sequentialId)
-        :param days_ago: 최근 체결 날짜 기준 7일 이내의 이전 데이터 조회 가능. 비워서 요청 시 가장 최근 체결 날짜 반환. (범위: 1 ~ 7))
-        :return:
-            data example:
+        :param days_ago: 최근 체결 날짜 기준 7일 이내의 이전 데이터 조회 가능. 비워서 요청 시 가장 최근 체결 날짜 반환. 범위: 1~7
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_trades_ticks('KRW-BTC')
+            print(res.json())
+
             [{
                 'market': 'KRW-BTC',
                 'trade_date_utc': '2023-02-14',
                 'trade_time_utc': '12:52:42',
                 'timestamp': 1676379162028,
                 'trade_price': 28250000.0,
                 'trade_volume': 0.00353982,
@@ -1124,27 +1499,39 @@
             "market": market,
             "to": to,
             "count": count,
             "cursor": cursor,
             "daysAgo": days_ago,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Quotation API > 시세 현재가 조회
     # --------------------------------------------------------------------------
 
-    def get_ticker(self, markets: [str] = None, **kwargs) -> Response:
-        """
-        현재가 정보 조회
-        https://docs.upbit.com/reference/ticker%ED%98%84%EC%9E%AC%EA%B0%80-%EC%A0%95%EB%B3%B4
+    def get_ticker(self,
+                   markets: list[str],
+                   **kwargs) -> Response:
+        """현재가 정보 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/ticker%ED%98%84%EC%9E%AC%EA%B0%80-%EC%A0%95%EB%B3%B4>`_
+
         :param markets: 마켓 코드 리스트 (ex. ["KRW-BTC"])
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_ticker(['KRW-BTC'])
+            print(res.json())
+
             [{
                 'market': 'KRW-BTC',
                 'trade_date': '20230214',
                 'trade_time': '130155',
                 'trade_date_kst': '20230214',
                 'trade_time_kst': '220155',
                 'trade_timestamp': 1676379715095,
@@ -1166,35 +1553,44 @@
                 'highest_52_week_price': 57678000.0,
                 'highest_52_week_date': '2022-03-28',
                 'lowest_52_week_price': 20700000.0,
                 'lowest_52_week_date': '2022-12-30',
                 'timestamp': 1676379715138
             }, ...]
         """
-        if markets is None:
-            markets = ["KRW-BTC"]
-
         url = self._endpoint + "/ticker"
         params = {
             "markets": markets,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Quotation API > 시세 호가 조회
     # --------------------------------------------------------------------------
 
-    def get_orderbook(self, markets: [str] = None, **kwargs) -> Response:
-        """
-        호가 정보 조회
-        https://docs.upbit.com/reference/%ED%98%B8%EA%B0%80-%EC%A0%95%EB%B3%B4-%EC%A1%B0%ED%9A%8C
+    def get_orderbook(self,
+                      markets: [str],
+                      **kwargs) -> Response:
+        """호가 정보 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%ED%98%B8%EA%B0%80-%EC%A0%95%EB%B3%B4-%EC%A1%B0%ED%9A%8C>`_
+
         :param markets: 마켓 코드 리스트 (ex. ["KRW-BTC"])
-        :return:
-            data example:
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :return: API 서버 응답
+
+        Usage::
+
+            upbit = Upbit()
+            res = upbit.get_orderbook(['KRW-BTC'])
+            print(res.json())
+
             [{
                 'market': 'KRW-BTC',
                 'timestamp': 1676380537532,
                 'total_ask_size': 5.71529774,
                 'total_bid_size': 3.5650408600000008,
                 'orderbook_units':
                     [{'ask_price': 28252000.0, 'bid_price': 28242000.0, 'ask_size': 0.22130992, 'bid_size': 0.69372092},
@@ -1210,16 +1606,13 @@
                     {'ask_price': 28268000.0, 'bid_price': 28227000.0, 'ask_size': 0.01, 'bid_size': 0.02220865},
                     {'ask_price': 28269000.0, 'bid_price': 28225000.0, 'ask_size': 0.0169, 'bid_size': 0.00035429},
                     {'ask_price': 28270000.0, 'bid_price': 28223000.0, 'ask_size': 0.02017691, 'bid_size': 0.02408774},
                     {'ask_price': 28271000.0, 'bid_price': 28222000.0, 'ask_size': 0.17979996, 'bid_size': 0.08573207},
                     {'ask_price': 28272000.0, 'bid_price': 28221000.0, 'ask_size': 1.81017689, 'bid_size': 0.11078135}
             }, ...]
         """
-        if markets is None:
-            markets = ["KRW-BTC"]
-
         url = self._endpoint + "/orderbook"
         params = {
             "markets": markets,
         }
 
-        return self._request_get(url, params=params, **kwargs)
+        return self._request('get', url, params=params, **kwargs)
```


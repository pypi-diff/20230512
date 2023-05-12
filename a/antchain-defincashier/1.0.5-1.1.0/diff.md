# Comparing `tmp/antchain_defincashier-1.0.5.tar.gz` & `tmp/antchain_defincashier-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_defincashier-1.0.5.tar", last modified: Thu Oct 27 02:05:01 2022, max compression
+gzip compressed data, was "dist/antchain_defincashier-1.1.0.tar", last modified: Fri May 12 08:23:50 2023, max compression
```

## Comparing `antchain_defincashier-1.0.5.tar` & `antchain_defincashier-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      600 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2216 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1017 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_defincashier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2216 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_defincashier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_defincashier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_defincashier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_defincashier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_defincashier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/antchain_sdk_defincashier/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/antchain_sdk_defincashier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36607 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/antchain_sdk_defincashier/client.py
--rw-r--r--   0 root         (0) root         (0)    69212 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/antchain_sdk_defincashier/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-27 02:05:01.000000 antchain_defincashier-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2533 2022-10-27 02:05:00.000000 antchain_defincashier-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_defincashier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39521 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/client.py
+-rw-r--r--   0 root         (0) root         (0)    76117 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/antchain_sdk_defincashier/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-05-12 08:23:50.000000 antchain_defincashier-1.1.0/setup.py
```

### Comparing `antchain_defincashier-1.0.5/LICENSE` & `antchain_defincashier-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.0.5/PKG-INFO` & `antchain_defincashier-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_defincashier
-Version: 1.0.5
+Version: 1.1.0
 Summary: Ant Chain DEFINCASHIER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_defincashier-1.0.5/README-CN.md` & `antchain_defincashier-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.0.5/README.md` & `antchain_defincashier-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.0.5/antchain_defincashier.egg-info/PKG-INFO` & `antchain_defincashier-1.1.0/antchain_defincashier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-defincashier
-Version: 1.0.5
+Version: 1.1.0
 Summary: Ant Chain DEFINCASHIER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_defincashier-1.0.5/antchain_sdk_defincashier/client.py` & `antchain_defincashier-1.1.0/antchain_sdk_defincashier/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,27 +94,27 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 账号
+            # 金额
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.1.0',
                     '_prod_code': 'DEFINCASHIER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -198,27 +198,27 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 账号
+            # 金额
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.1.0',
                     '_prod_code': 'DEFINCASHIER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -774,7 +774,63 @@
         Summary: B2B资金服务机构信息查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             defincashier_models.QuerySaasInstResponse(),
             await self.do_request_async('1.0', 'antchain.defincashier.saas.inst.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def apply_saas_share(
+        self,
+        request: defincashier_models.ApplySaasShareRequest,
+    ) -> defincashier_models.ApplySaasShareResponse:
+        """
+        Description: 基于已完成支付或收款的交易单，进行一付多收的分账申请。每次分账请求金额需小于等于原交易单金额，单次最多支持10个分账接收方，一个交易单支持多次分账。
+        Summary: B2B资金服务交易分账
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.apply_saas_share_ex(request, headers, runtime)
+
+    async def apply_saas_share_async(
+        self,
+        request: defincashier_models.ApplySaasShareRequest,
+    ) -> defincashier_models.ApplySaasShareResponse:
+        """
+        Description: 基于已完成支付或收款的交易单，进行一付多收的分账申请。每次分账请求金额需小于等于原交易单金额，单次最多支持10个分账接收方，一个交易单支持多次分账。
+        Summary: B2B资金服务交易分账
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.apply_saas_share_ex_async(request, headers, runtime)
+
+    def apply_saas_share_ex(
+        self,
+        request: defincashier_models.ApplySaasShareRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> defincashier_models.ApplySaasShareResponse:
+        """
+        Description: 基于已完成支付或收款的交易单，进行一付多收的分账申请。每次分账请求金额需小于等于原交易单金额，单次最多支持10个分账接收方，一个交易单支持多次分账。
+        Summary: B2B资金服务交易分账
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            defincashier_models.ApplySaasShareResponse(),
+            self.do_request('1.0', 'antchain.defincashier.saas.share.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def apply_saas_share_ex_async(
+        self,
+        request: defincashier_models.ApplySaasShareRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> defincashier_models.ApplySaasShareResponse:
+        """
+        Description: 基于已完成支付或收款的交易单，进行一付多收的分账申请。每次分账请求金额需小于等于原交易单金额，单次最多支持10个分账接收方，一个交易单支持多次分账。
+        Summary: B2B资金服务交易分账
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            defincashier_models.ApplySaasShareResponse(),
+            await self.do_request_async('1.0', 'antchain.defincashier.saas.share.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_defincashier-1.0.5/antchain_sdk_defincashier/models.py` & `antchain_defincashier-1.1.0/antchain_sdk_defincashier/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,53 +150,70 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
-class AccountVO(TeaModel):
+class AmountItem(TeaModel):
+    def __init__(
+        self,
+        balance_amount: str = None,
+        currency: str = None,
+    ):
+        # 余额，单位元
+        self.balance_amount = balance_amount
+        # 币种，CNY-人民币
+        self.currency = currency
+
+    def validate(self):
+        self.validate_required(self.balance_amount, 'balance_amount')
+        self.validate_required(self.currency, 'currency')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.balance_amount is not None:
+            result['balance_amount'] = self.balance_amount
+        if self.currency is not None:
+            result['currency'] = self.currency
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('balance_amount') is not None:
+            self.balance_amount = m.get('balance_amount')
+        if m.get('currency') is not None:
+            self.currency = m.get('currency')
+        return self
+
+
+class AccountDTO(TeaModel):
     def __init__(
         self,
         account_no: str = None,
         account_name: str = None,
         offical_name: str = None,
         offical_number: str = None,
-        status: str = None,
-        category: List[str] = None,
-        last_pay_fail: bool = None,
-        pay_method: List[str] = None,
-        type: str = None,
     ):
         # 账号
         self.account_no = account_no
         # 户名
         self.account_name = account_name
         # 开户网点
         self.offical_name = offical_name
         # 联行号
         self.offical_number = offical_number
-        # 账号状态
-        # 
-        self.status = status
-        # 分类 BUYER付款账户； SELLER收款账户
-        self.category = category
-        # 上次支付是否失败
-        self.last_pay_fail = last_pay_fail
-        # 支付方式 BALANCE余额账户；BILL票据账户
-        self.pay_method = pay_method
-        # 账户类型 MAIN 对公账户；ECOLLECTION e收宝
-        self.type = type
 
     def validate(self):
         self.validate_required(self.account_no, 'account_no')
         self.validate_required(self.account_name, 'account_name')
-        self.validate_required(self.offical_name, 'offical_name')
-        self.validate_required(self.offical_number, 'offical_number')
-        self.validate_required(self.status, 'status')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -204,69 +221,76 @@
             result['account_no'] = self.account_no
         if self.account_name is not None:
             result['account_name'] = self.account_name
         if self.offical_name is not None:
             result['offical_name'] = self.offical_name
         if self.offical_number is not None:
             result['offical_number'] = self.offical_number
-        if self.status is not None:
-            result['status'] = self.status
-        if self.category is not None:
-            result['category'] = self.category
-        if self.last_pay_fail is not None:
-            result['last_pay_fail'] = self.last_pay_fail
-        if self.pay_method is not None:
-            result['pay_method'] = self.pay_method
-        if self.type is not None:
-            result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('account_no') is not None:
             self.account_no = m.get('account_no')
         if m.get('account_name') is not None:
             self.account_name = m.get('account_name')
         if m.get('offical_name') is not None:
             self.offical_name = m.get('offical_name')
         if m.get('offical_number') is not None:
             self.offical_number = m.get('offical_number')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('last_pay_fail') is not None:
-            self.last_pay_fail = m.get('last_pay_fail')
-        if m.get('pay_method') is not None:
-            self.pay_method = m.get('pay_method')
-        if m.get('type') is not None:
-            self.type = m.get('type')
         return self
 
 
-class AccountDTO(TeaModel):
+class AccountVO(TeaModel):
     def __init__(
         self,
         account_no: str = None,
         account_name: str = None,
         offical_name: str = None,
         offical_number: str = None,
+        status: str = None,
+        category: List[str] = None,
+        last_pay_fail: bool = None,
+        pay_method: List[str] = None,
+        type: str = None,
+        principal: str = None,
+        amount_item: AmountItem = None,
     ):
         # 账号
         self.account_no = account_no
         # 户名
         self.account_name = account_name
         # 开户网点
         self.offical_name = offical_name
         # 联行号
         self.offical_number = offical_number
+        # 账号状态
+        # 
+        self.status = status
+        # 分类 BUYER付款账户； SELLER收款账户
+        self.category = category
+        # 上次支付是否失败
+        self.last_pay_fail = last_pay_fail
+        # 支付方式 BALANCE余额账户；BILL票据账户
+        self.pay_method = pay_method
+        # 账户类型 MAIN 银行账户；ECOLLECTION e收宝
+        self.type = type
+        # 主体：I-个人；E-企业
+        self.principal = principal
+        # 金额明细
+        self.amount_item = amount_item
 
     def validate(self):
         self.validate_required(self.account_no, 'account_no')
         self.validate_required(self.account_name, 'account_name')
+        self.validate_required(self.offical_name, 'offical_name')
+        self.validate_required(self.offical_number, 'offical_number')
+        self.validate_required(self.status, 'status')
+        if self.amount_item:
+            self.amount_item.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -274,26 +298,55 @@
             result['account_no'] = self.account_no
         if self.account_name is not None:
             result['account_name'] = self.account_name
         if self.offical_name is not None:
             result['offical_name'] = self.offical_name
         if self.offical_number is not None:
             result['offical_number'] = self.offical_number
+        if self.status is not None:
+            result['status'] = self.status
+        if self.category is not None:
+            result['category'] = self.category
+        if self.last_pay_fail is not None:
+            result['last_pay_fail'] = self.last_pay_fail
+        if self.pay_method is not None:
+            result['pay_method'] = self.pay_method
+        if self.type is not None:
+            result['type'] = self.type
+        if self.principal is not None:
+            result['principal'] = self.principal
+        if self.amount_item is not None:
+            result['amount_item'] = self.amount_item.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('account_no') is not None:
             self.account_no = m.get('account_no')
         if m.get('account_name') is not None:
             self.account_name = m.get('account_name')
         if m.get('offical_name') is not None:
             self.offical_name = m.get('offical_name')
         if m.get('offical_number') is not None:
             self.offical_number = m.get('offical_number')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('last_pay_fail') is not None:
+            self.last_pay_fail = m.get('last_pay_fail')
+        if m.get('pay_method') is not None:
+            self.pay_method = m.get('pay_method')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('principal') is not None:
+            self.principal = m.get('principal')
+        if m.get('amount_item') is not None:
+            temp_model = AmountItem()
+            self.amount_item = temp_model.from_map(m['amount_item'])
         return self
 
 
 class AccountQueryResult(TeaModel):
     def __init__(
         self,
         out_member_id: str = None,
@@ -433,14 +486,143 @@
         if m.get('sub_code') is not None:
             self.sub_code = m.get('sub_code')
         if m.get('sub_msg') is not None:
             self.sub_msg = m.get('sub_msg')
         return self
 
 
+class FundItemQueryResult(TeaModel):
+    def __init__(
+        self,
+        platform_member_id: str = None,
+        out_order_id: str = None,
+        out_request_id: str = None,
+        fund_type: str = None,
+        state: str = None,
+        request_amount: int = None,
+        request_currency: str = None,
+        sub_code: str = None,
+        sub_msg: str = None,
+    ):
+        # 会员所属业务平台在智能科技的会员ID
+        self.platform_member_id = platform_member_id
+        # 外部业务平台原始交易号
+        self.out_order_id = out_order_id
+        # 外部请求ID
+        # 
+        self.out_request_id = out_request_id
+        # 资金操作类型。CAPTURE(请款);CANCEL(撤销/退款);WITHDRAW(提现);
+        self.fund_type = fund_type
+        # 资金操作状态。PROCESSING(处理中);SUCCESS(成功);FAIL(失败);
+        self.state = state
+        # 本次请求金额，单位为元。
+        self.request_amount = request_amount
+        # 支付币种三位字母编码。（编码规则遵循https://zh.wikipedia.org/wiki/ISO_4217）
+        self.request_currency = request_currency
+        # 业务错误码(为空表示成功，否则为业务错误码)
+        self.sub_code = sub_code
+        # 业务错误描述
+        self.sub_msg = sub_msg
+
+    def validate(self):
+        self.validate_required(self.platform_member_id, 'platform_member_id')
+        self.validate_required(self.out_order_id, 'out_order_id')
+        self.validate_required(self.fund_type, 'fund_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.platform_member_id is not None:
+            result['platform_member_id'] = self.platform_member_id
+        if self.out_order_id is not None:
+            result['out_order_id'] = self.out_order_id
+        if self.out_request_id is not None:
+            result['out_request_id'] = self.out_request_id
+        if self.fund_type is not None:
+            result['fund_type'] = self.fund_type
+        if self.state is not None:
+            result['state'] = self.state
+        if self.request_amount is not None:
+            result['request_amount'] = self.request_amount
+        if self.request_currency is not None:
+            result['request_currency'] = self.request_currency
+        if self.sub_code is not None:
+            result['sub_code'] = self.sub_code
+        if self.sub_msg is not None:
+            result['sub_msg'] = self.sub_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('platform_member_id') is not None:
+            self.platform_member_id = m.get('platform_member_id')
+        if m.get('out_order_id') is not None:
+            self.out_order_id = m.get('out_order_id')
+        if m.get('out_request_id') is not None:
+            self.out_request_id = m.get('out_request_id')
+        if m.get('fund_type') is not None:
+            self.fund_type = m.get('fund_type')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        if m.get('request_amount') is not None:
+            self.request_amount = m.get('request_amount')
+        if m.get('request_currency') is not None:
+            self.request_currency = m.get('request_currency')
+        if m.get('sub_code') is not None:
+            self.sub_code = m.get('sub_code')
+        if m.get('sub_msg') is not None:
+            self.sub_msg = m.get('sub_msg')
+        return self
+
+
+class PaymentCreateCheckResult(TeaModel):
+    def __init__(
+        self,
+        result: str = None,
+        sub_code: str = None,
+        sub_msg: str = None,
+    ):
+        # 检查是否通过。PASS(检查通过);NOT_PASS(检查不通过)
+        self.result = result
+        # 业务错误码(为空表示成功，否则为业务错误码)
+        self.sub_code = sub_code
+        # 业务错误描述
+        self.sub_msg = sub_msg
+
+    def validate(self):
+        self.validate_required(self.result, 'result')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        if self.sub_code is not None:
+            result['sub_code'] = self.sub_code
+        if self.sub_msg is not None:
+            result['sub_msg'] = self.sub_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('sub_code') is not None:
+            self.sub_code = m.get('sub_code')
+        if m.get('sub_msg') is not None:
+            self.sub_msg = m.get('sub_msg')
+        return self
+
+
 class InstCodeResult(TeaModel):
     def __init__(
         self,
         channel_member_code: str = None,
         channel_official_number: str = None,
         sub_code: str = None,
         sub_msg: str = None,
@@ -496,14 +678,15 @@
         out_payee_id: str = None,
         out_order_id: str = None,
         order_state: str = None,
         fund_mode: str = None,
         payee_account: AccountDTO = None,
         sub_code: str = None,
         sub_msg: str = None,
+        trade_id: str = None,
     ):
         # 
         # 会员所属业务平台在智能科技的会员ID
         self.platform_member_id = platform_member_id
         # 付款方在外部业务平台的用户ID
         self.out_payer_id = out_payer_id
         # 收款方外部业务平台会员ID，收单场景表示卖家，纯资金场景表示收款方
@@ -516,21 +699,24 @@
         self.fund_mode = fund_mode
         # 收款方账号
         self.payee_account = payee_account
         # 业务错误码(为空表示成功，否则为业务错误码)
         self.sub_code = sub_code
         # 业务错误描述
         self.sub_msg = sub_msg
+        # 蚂蚁交易单ID
+        self.trade_id = trade_id
 
     def validate(self):
         self.validate_required(self.platform_member_id, 'platform_member_id')
         self.validate_required(self.out_payer_id, 'out_payer_id')
         self.validate_required(self.out_order_id, 'out_order_id')
         if self.payee_account:
             self.payee_account.validate()
+        self.validate_required(self.trade_id, 'trade_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -548,14 +734,16 @@
             result['fund_mode'] = self.fund_mode
         if self.payee_account is not None:
             result['payee_account'] = self.payee_account.to_map()
         if self.sub_code is not None:
             result['sub_code'] = self.sub_code
         if self.sub_msg is not None:
             result['sub_msg'] = self.sub_msg
+        if self.trade_id is not None:
+            result['trade_id'] = self.trade_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('platform_member_id') is not None:
             self.platform_member_id = m.get('platform_member_id')
         if m.get('out_payer_id') is not None:
@@ -571,14 +759,16 @@
         if m.get('payee_account') is not None:
             temp_model = AccountDTO()
             self.payee_account = temp_model.from_map(m['payee_account'])
         if m.get('sub_code') is not None:
             self.sub_code = m.get('sub_code')
         if m.get('sub_msg') is not None:
             self.sub_msg = m.get('sub_msg')
+        if m.get('trade_id') is not None:
+            self.trade_id = m.get('trade_id')
         return self
 
 
 class PaymentQueryResult(TeaModel):
     def __init__(
         self,
         platform_member_id: str = None,
@@ -667,14 +857,59 @@
         if m.get('sub_code') is not None:
             self.sub_code = m.get('sub_code')
         if m.get('sub_msg') is not None:
             self.sub_msg = m.get('sub_msg')
         return self
 
 
+class PaymentShareAcceptanceResult(TeaModel):
+    def __init__(
+        self,
+        out_order_id: str = None,
+        out_request_id: str = None,
+        state: str = None,
+    ):
+        # 外部业务平台原始交易号
+        self.out_order_id = out_order_id
+        # 外部请求ID，幂等字段
+        # 
+        self.out_request_id = out_request_id
+        # 分账单状态
+        self.state = state
+
+    def validate(self):
+        self.validate_required(self.out_order_id, 'out_order_id')
+        self.validate_required(self.out_request_id, 'out_request_id')
+        self.validate_required(self.state, 'state')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.out_order_id is not None:
+            result['out_order_id'] = self.out_order_id
+        if self.out_request_id is not None:
+            result['out_request_id'] = self.out_request_id
+        if self.state is not None:
+            result['state'] = self.state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('out_order_id') is not None:
+            self.out_order_id = m.get('out_order_id')
+        if m.get('out_request_id') is not None:
+            self.out_request_id = m.get('out_request_id')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        return self
+
+
 class AgreementQueryResult(TeaModel):
     def __init__(
         self,
         platform_member_id: str = None,
         out_member_id: str = None,
         product_code: str = None,
         product_name: str = None,
@@ -762,101 +997,14 @@
         if m.get('sub_code') is not None:
             self.sub_code = m.get('sub_code')
         if m.get('sub_msg') is not None:
             self.sub_msg = m.get('sub_msg')
         return self
 
 
-class FundItemQueryResult(TeaModel):
-    def __init__(
-        self,
-        platform_member_id: str = None,
-        out_order_id: str = None,
-        out_request_id: str = None,
-        fund_type: str = None,
-        state: str = None,
-        request_amount: int = None,
-        request_currency: str = None,
-        sub_code: str = None,
-        sub_msg: str = None,
-    ):
-        # 会员所属业务平台在智能科技的会员ID
-        self.platform_member_id = platform_member_id
-        # 外部业务平台原始交易号
-        self.out_order_id = out_order_id
-        # 外部请求ID
-        # 
-        self.out_request_id = out_request_id
-        # 资金操作类型。CAPTURE(请款);CANCEL(撤销/退款);
-        self.fund_type = fund_type
-        # 资金操作状态。PROCESSING(处理中);SUCCESS(成功);FAIL(失败);
-        self.state = state
-        # 本次请求金额，单位为元。
-        self.request_amount = request_amount
-        # 支付币种三位字母编码。（编码规则遵循https://zh.wikipedia.org/wiki/ISO_4217）
-        self.request_currency = request_currency
-        # 业务错误码(为空表示成功，否则为业务错误码)
-        self.sub_code = sub_code
-        # 业务错误描述
-        self.sub_msg = sub_msg
-
-    def validate(self):
-        self.validate_required(self.platform_member_id, 'platform_member_id')
-        self.validate_required(self.out_order_id, 'out_order_id')
-        self.validate_required(self.fund_type, 'fund_type')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.platform_member_id is not None:
-            result['platform_member_id'] = self.platform_member_id
-        if self.out_order_id is not None:
-            result['out_order_id'] = self.out_order_id
-        if self.out_request_id is not None:
-            result['out_request_id'] = self.out_request_id
-        if self.fund_type is not None:
-            result['fund_type'] = self.fund_type
-        if self.state is not None:
-            result['state'] = self.state
-        if self.request_amount is not None:
-            result['request_amount'] = self.request_amount
-        if self.request_currency is not None:
-            result['request_currency'] = self.request_currency
-        if self.sub_code is not None:
-            result['sub_code'] = self.sub_code
-        if self.sub_msg is not None:
-            result['sub_msg'] = self.sub_msg
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('platform_member_id') is not None:
-            self.platform_member_id = m.get('platform_member_id')
-        if m.get('out_order_id') is not None:
-            self.out_order_id = m.get('out_order_id')
-        if m.get('out_request_id') is not None:
-            self.out_request_id = m.get('out_request_id')
-        if m.get('fund_type') is not None:
-            self.fund_type = m.get('fund_type')
-        if m.get('state') is not None:
-            self.state = m.get('state')
-        if m.get('request_amount') is not None:
-            self.request_amount = m.get('request_amount')
-        if m.get('request_currency') is not None:
-            self.request_currency = m.get('request_currency')
-        if m.get('sub_code') is not None:
-            self.sub_code = m.get('sub_code')
-        if m.get('sub_msg') is not None:
-            self.sub_msg = m.get('sub_msg')
-        return self
-
-
 class PaymentCancelResult(TeaModel):
     def __init__(
         self,
         out_order_id: str = None,
         fund_mode: str = None,
         order_state: str = None,
         available_amount: int = None,
@@ -935,56 +1083,14 @@
         if m.get('sub_code') is not None:
             self.sub_code = m.get('sub_code')
         if m.get('sub_msg') is not None:
             self.sub_msg = m.get('sub_msg')
         return self
 
 
-class PaymentCreateCheckResult(TeaModel):
-    def __init__(
-        self,
-        result: str = None,
-        sub_code: str = None,
-        sub_msg: str = None,
-    ):
-        # 检查是否通过。PASS(检查通过);NOT_PASS(检查不通过)
-        self.result = result
-        # 业务错误码(为空表示成功，否则为业务错误码)
-        self.sub_code = sub_code
-        # 业务错误描述
-        self.sub_msg = sub_msg
-
-    def validate(self):
-        self.validate_required(self.result, 'result')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.result is not None:
-            result['result'] = self.result
-        if self.sub_code is not None:
-            result['sub_code'] = self.sub_code
-        if self.sub_msg is not None:
-            result['sub_msg'] = self.sub_msg
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('result') is not None:
-            self.result = m.get('result')
-        if m.get('sub_code') is not None:
-            self.sub_code = m.get('sub_code')
-        if m.get('sub_msg') is not None:
-            self.sub_msg = m.get('sub_msg')
-        return self
-
-
 class QuerySaasPaymentRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_content: str = None,
         service_version: str = None,
@@ -1880,7 +1986,107 @@
             self.result_msg = m.get('result_msg')
         if m.get('data') is not None:
             temp_model = InstCodeResult()
             self.data = temp_model.from_map(m['data'])
         return self
 
 
+class ApplySaasShareRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_content: str = None,
+        service_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # JSON请求参数
+        self.biz_content = biz_content
+        # 版本号
+        self.service_version = service_version
+
+    def validate(self):
+        self.validate_required(self.biz_content, 'biz_content')
+        self.validate_required(self.service_version, 'service_version')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_content is not None:
+            result['biz_content'] = self.biz_content
+        if self.service_version is not None:
+            result['service_version'] = self.service_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_content') is not None:
+            self.biz_content = m.get('biz_content')
+        if m.get('service_version') is not None:
+            self.service_version = m.get('service_version')
+        return self
+
+
+class ApplySaasShareResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: PaymentShareAcceptanceResult = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 分账受理结果
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('data') is not None:
+            temp_model = PaymentShareAcceptanceResult()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
```

### Comparing `antchain_defincashier-1.0.5/setup.py` & `antchain_defincashier-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_defincashier.
 
-Created on 27/10/2022
+Created on 12/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_defincashier"
 NAME = "antchain_defincashier" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DEFINCASHIER SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```


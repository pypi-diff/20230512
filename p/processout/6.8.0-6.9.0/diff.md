# Comparing `tmp/processout-6.8.0.tar.gz` & `tmp/processout-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/processout-6.8.0.tar", last modified: Mon Jun  4 16:22:14 2018, max compression
+gzip compressed data, was "dist/processout-6.9.0.tar", last modified: Fri Aug 31 13:40:53 2018, max compression
```

## Comparing `processout-6.8.0.tar` & `processout-6.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-06-04 16:22:14.000000 processout-6.8.0/
--rw-r--r--   0 manuel     (501) staff       (20)      364 2018-06-04 16:22:14.000000 processout-6.8.0/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)      478 2018-06-04 16:20:46.000000 processout-6.8.0/setup.py
--rw-r--r--   0 manuel     (501) staff       (20)       39 2018-06-04 16:20:46.000000 processout-6.8.0/setup.cfg
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-06-04 16:22:14.000000 processout-6.8.0/processout/
--rwxr-xr-x   0 manuel     (501) staff       (20)    11557 2018-06-04 16:20:46.000000 processout-6.8.0/processout/addon.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     2186 2018-06-04 16:20:46.000000 processout-6.8.0/processout/paymentdatathreedsrequest.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     4067 2018-06-04 16:20:46.000000 processout-6.8.0/processout/cardinformation.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     8374 2018-06-04 16:20:46.000000 processout-6.8.0/processout/apirequest.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    10195 2018-06-04 16:20:46.000000 processout-6.8.0/processout/plan.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     1411 2018-06-04 16:20:46.000000 processout-6.8.0/processout/customeraction.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     6232 2018-06-04 16:20:46.000000 processout-6.8.0/processout/payoutitem.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     5660 2018-06-04 16:20:46.000000 processout-6.8.0/processout/event.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     6068 2018-06-04 16:20:46.000000 processout-6.8.0/processout/gateway.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     9714 2018-06-04 16:20:46.000000 processout-6.8.0/processout/token.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    27826 2018-06-04 16:20:46.000000 processout-6.8.0/processout/subscription.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     7134 2018-06-04 16:20:46.000000 processout-6.8.0/processout/webhook.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    11592 2018-06-04 16:20:46.000000 processout-6.8.0/processout/transactionoperation.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    21131 2018-06-04 16:20:46.000000 processout-6.8.0/processout/transaction.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-06-04 16:22:14.000000 processout-6.8.0/processout/networking/
--rw-r--r--   0 manuel     (501) staff       (20)     3579 2018-06-04 16:20:46.000000 processout-6.8.0/processout/networking/request.py
--rw-r--r--   0 manuel     (501) staff       (20)        0 2018-06-04 16:20:46.000000 processout-6.8.0/processout/networking/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     2429 2018-06-04 16:20:46.000000 processout-6.8.0/processout/networking/response.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     1530 2018-06-04 16:20:46.000000 processout-6.8.0/processout/dunningaction.py
--rw-r--r--   0 manuel     (501) staff       (20)     8440 2018-06-04 16:20:46.000000 processout-6.8.0/processout/client.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     9923 2018-06-04 16:20:46.000000 processout-6.8.0/processout/coupon.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     1903 2018-06-04 16:20:46.000000 processout-6.8.0/processout/apiversion.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    11288 2018-06-04 16:20:46.000000 processout-6.8.0/processout/payout.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     5050 2018-06-04 16:20:46.000000 processout-6.8.0/processout/activity.py
--rw-r--r--   0 manuel     (501) staff       (20)     2024 2018-06-04 16:20:46.000000 processout-6.8.0/processout/__init__.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     2574 2018-06-04 16:20:46.000000 processout-6.8.0/processout/invoicedetail.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    12718 2018-06-04 16:20:46.000000 processout-6.8.0/processout/card.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    10257 2018-06-04 16:20:46.000000 processout-6.8.0/processout/discount.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     9870 2018-06-04 16:20:46.000000 processout-6.8.0/processout/product.py
--rw-r--r--   0 manuel     (501) staff       (20)     1009 2018-06-04 16:20:46.000000 processout-6.8.0/processout/gatewayrequest.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    21357 2018-06-04 16:20:46.000000 processout-6.8.0/processout/customer.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     1065 2018-06-04 16:20:46.000000 processout-6.8.0/processout/paymentdatanetworkauthentication.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     3736 2018-06-04 16:20:46.000000 processout-6.8.0/processout/webhookendpoint.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-06-04 16:22:14.000000 processout-6.8.0/processout/errors/
--rw-r--r--   0 manuel     (501) staff       (20)      127 2018-06-04 16:20:46.000000 processout-6.8.0/processout/errors/notfounderror.py
--rw-r--r--   0 manuel     (501) staff       (20)      126 2018-06-04 16:20:46.000000 processout-6.8.0/processout/errors/genericerror.py
--rw-r--r--   0 manuel     (501) staff       (20)      127 2018-06-04 16:20:46.000000 processout-6.8.0/processout/errors/internalerror.py
--rw-r--r--   0 manuel     (501) staff       (20)      133 2018-06-04 16:20:46.000000 processout-6.8.0/processout/errors/authenticationerror.py
--rw-r--r--   0 manuel     (501) staff       (20)        0 2018-06-04 16:20:46.000000 processout-6.8.0/processout/errors/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)      129 2018-06-04 16:20:46.000000 processout-6.8.0/processout/errors/validationerror.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     1053 2018-06-04 16:20:46.000000 processout-6.8.0/processout/paymentdatathreedsauthentication.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    10641 2018-06-04 16:20:46.000000 processout-6.8.0/processout/gatewayconfiguration.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     9769 2018-06-04 16:20:46.000000 processout-6.8.0/processout/authorizationrequest.py
--rwxr-xr-x   0 manuel     (501) staff       (20)     7378 2018-06-04 16:20:46.000000 processout-6.8.0/processout/refund.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    10735 2018-06-04 16:20:46.000000 processout-6.8.0/processout/project.py
--rwxr-xr-x   0 manuel     (501) staff       (20)    22065 2018-06-04 16:20:46.000000 processout-6.8.0/processout/invoice.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-08-31 13:40:53.000000 processout-6.9.0/
+-rw-r--r--   0 manuel     (501) staff       (20)      364 2018-08-31 13:40:53.000000 processout-6.9.0/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)      478 2018-08-31 13:17:43.000000 processout-6.9.0/setup.py
+-rw-r--r--   0 manuel     (501) staff       (20)       39 2018-08-31 13:17:43.000000 processout-6.9.0/setup.cfg
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-08-31 13:40:53.000000 processout-6.9.0/processout/
+-rwxr-xr-x   0 manuel     (501) staff       (20)    11557 2018-08-31 13:17:43.000000 processout-6.9.0/processout/addon.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     2186 2018-08-31 13:17:43.000000 processout-6.9.0/processout/paymentdatathreedsrequest.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     4067 2018-08-31 13:17:43.000000 processout-6.9.0/processout/cardinformation.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     8374 2018-08-31 13:17:43.000000 processout-6.9.0/processout/apirequest.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    10195 2018-08-31 13:17:43.000000 processout-6.9.0/processout/plan.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     1411 2018-08-31 13:17:43.000000 processout-6.9.0/processout/customeraction.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     6232 2018-08-31 13:17:43.000000 processout-6.9.0/processout/payoutitem.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     5660 2018-08-31 13:17:43.000000 processout-6.9.0/processout/event.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     6068 2018-08-31 13:17:43.000000 processout-6.9.0/processout/gateway.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     9714 2018-08-31 13:17:43.000000 processout-6.9.0/processout/token.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    27826 2018-08-31 13:17:43.000000 processout-6.9.0/processout/subscription.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     7134 2018-08-31 13:17:43.000000 processout-6.9.0/processout/webhook.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    11592 2018-08-31 13:17:43.000000 processout-6.9.0/processout/transactionoperation.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    21131 2018-08-31 13:17:43.000000 processout-6.9.0/processout/transaction.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-08-31 13:40:53.000000 processout-6.9.0/processout/networking/
+-rw-r--r--   0 manuel     (501) staff       (20)     3646 2018-08-31 13:17:43.000000 processout-6.9.0/processout/networking/request.py
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2018-08-31 13:17:43.000000 processout-6.9.0/processout/networking/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2429 2018-08-31 13:17:43.000000 processout-6.9.0/processout/networking/response.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     1530 2018-08-31 13:17:43.000000 processout-6.9.0/processout/dunningaction.py
+-rw-r--r--   0 manuel     (501) staff       (20)     8440 2018-08-31 13:17:43.000000 processout-6.9.0/processout/client.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     9923 2018-08-31 13:17:43.000000 processout-6.9.0/processout/coupon.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     1903 2018-08-31 13:17:43.000000 processout-6.9.0/processout/apiversion.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    11288 2018-08-31 13:17:43.000000 processout-6.9.0/processout/payout.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     5050 2018-08-31 13:17:43.000000 processout-6.9.0/processout/activity.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2024 2018-08-31 13:17:43.000000 processout-6.9.0/processout/__init__.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     2574 2018-08-31 13:17:43.000000 processout-6.9.0/processout/invoicedetail.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    12718 2018-08-31 13:17:43.000000 processout-6.9.0/processout/card.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    10257 2018-08-31 13:17:43.000000 processout-6.9.0/processout/discount.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     9870 2018-08-31 13:17:43.000000 processout-6.9.0/processout/product.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1009 2018-08-31 13:17:43.000000 processout-6.9.0/processout/gatewayrequest.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    21357 2018-08-31 13:17:43.000000 processout-6.9.0/processout/customer.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     1065 2018-08-31 13:17:43.000000 processout-6.9.0/processout/paymentdatanetworkauthentication.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     3736 2018-08-31 13:17:43.000000 processout-6.9.0/processout/webhookendpoint.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2018-08-31 13:40:53.000000 processout-6.9.0/processout/errors/
+-rw-r--r--   0 manuel     (501) staff       (20)      127 2018-08-31 13:17:43.000000 processout-6.9.0/processout/errors/notfounderror.py
+-rw-r--r--   0 manuel     (501) staff       (20)      126 2018-08-31 13:17:43.000000 processout-6.9.0/processout/errors/genericerror.py
+-rw-r--r--   0 manuel     (501) staff       (20)      127 2018-08-31 13:17:43.000000 processout-6.9.0/processout/errors/internalerror.py
+-rw-r--r--   0 manuel     (501) staff       (20)      133 2018-08-31 13:17:43.000000 processout-6.9.0/processout/errors/authenticationerror.py
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2018-08-31 13:17:43.000000 processout-6.9.0/processout/errors/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)      129 2018-08-31 13:17:43.000000 processout-6.9.0/processout/errors/validationerror.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     1053 2018-08-31 13:17:43.000000 processout-6.9.0/processout/paymentdatathreedsauthentication.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    10641 2018-08-31 13:17:43.000000 processout-6.9.0/processout/gatewayconfiguration.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     9769 2018-08-31 13:17:43.000000 processout-6.9.0/processout/authorizationrequest.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)     7378 2018-08-31 13:17:43.000000 processout-6.9.0/processout/refund.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    10714 2018-08-31 13:17:43.000000 processout-6.9.0/processout/project.py
+-rwxr-xr-x   0 manuel     (501) staff       (20)    22131 2018-08-31 13:17:43.000000 processout-6.9.0/processout/invoice.py
```

### Comparing `processout-6.8.0/processout/addon.py` & `processout-6.9.0/processout/addon.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/paymentdatathreedsrequest.py` & `processout-6.9.0/processout/paymentdatathreedsrequest.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/cardinformation.py` & `processout-6.9.0/processout/cardinformation.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/apirequest.py` & `processout-6.9.0/processout/apirequest.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/plan.py` & `processout-6.9.0/processout/plan.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/customeraction.py` & `processout-6.9.0/processout/customeraction.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/payoutitem.py` & `processout-6.9.0/processout/payoutitem.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/event.py` & `processout-6.9.0/processout/event.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/gateway.py` & `processout-6.9.0/processout/gateway.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/token.py` & `processout-6.9.0/processout/token.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/subscription.py` & `processout-6.9.0/processout/subscription.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/webhook.py` & `processout-6.9.0/processout/webhook.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/transactionoperation.py` & `processout-6.9.0/processout/transactionoperation.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/transaction.py` & `processout-6.9.0/processout/transaction.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/networking/request.py` & `processout-6.9.0/processout/networking/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         password = self._client.project_secret
         return (username, password)
 
     def _get_headers(self, options):
         """Return the headers sent with the request"""
         headers = {}
         headers["API-Version"] = "1.4.0.0"
+        headers["User-Agent"] = "ProcessOut Python-Bindings/6.9.0"
 
         if options is None:
             return headers
 
         if "idempotency_key" in options:
             headers["Idempotency-Key"] = options["idempotency_key"]
         if "disable_logging" in options:
```

### Comparing `processout-6.8.0/processout/networking/response.py` & `processout-6.9.0/processout/networking/response.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/dunningaction.py` & `processout-6.9.0/processout/dunningaction.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/client.py` & `processout-6.9.0/processout/client.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/coupon.py` & `processout-6.9.0/processout/coupon.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/apiversion.py` & `processout-6.9.0/processout/apiversion.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/payout.py` & `processout-6.9.0/processout/payout.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/activity.py` & `processout-6.9.0/processout/activity.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/__init__.py` & `processout-6.9.0/processout/__init__.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/invoicedetail.py` & `processout-6.9.0/processout/invoicedetail.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/card.py` & `processout-6.9.0/processout/card.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/discount.py` & `processout-6.9.0/processout/discount.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/product.py` & `processout-6.9.0/processout/product.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/gatewayrequest.py` & `processout-6.9.0/processout/gatewayrequest.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/customer.py` & `processout-6.9.0/processout/customer.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/paymentdatanetworkauthentication.py` & `processout-6.9.0/processout/paymentdatanetworkauthentication.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/webhookendpoint.py` & `processout-6.9.0/processout/webhookendpoint.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/paymentdatathreedsauthentication.py` & `processout-6.9.0/processout/paymentdatathreedsauthentication.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/gatewayconfiguration.py` & `processout-6.9.0/processout/gatewayconfiguration.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/authorizationrequest.py` & `processout-6.9.0/processout/authorizationrequest.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/refund.py` & `processout-6.9.0/processout/refund.py`

 * *Files identical despite different names*

### Comparing `processout-6.8.0/processout/project.py` & `processout-6.9.0/processout/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,110 +228,110 @@
         if "dunning_configuration" in data.keys():
             self.dunning_configuration = data["dunning_configuration"]
         if "created_at" in data.keys():
             self.created_at = data["created_at"]
         
         return self
 
-    def fetch(self, options = {}):
-        """Fetch the current project information.
+    def regenerate_private_key(self, options = {}):
+        """Regenerate the project private key. Make sure to store the new private key and use it in any future request.
         Keyword argument:
         
         options -- Options for the request"""
         self.fill_with_data(options)
 
         request = Request(self._client)
-        path    = "/projects/" + quote_plus(self.id) + ""
+        path    = "/private-keys"
         data    = {
 
         }
 
-        response = Response(request.get(path, data, options))
+        response = Response(request.post(path, data, options))
         return_values = []
         
         body = response.body
         body = body["project"]
                 
                 
-        return_values.append(self.fill_with_data(body))
+        obj = processout.Project(self._client)
+        return_values.append(obj.fill_with_data(body))
                 
 
         
         return return_values[0]
 
-    def save(self, options = {}):
-        """Save the updated project's attributes.
+    def fetch(self, options = {}):
+        """Fetch the current project information.
         Keyword argument:
         
         options -- Options for the request"""
         self.fill_with_data(options)
 
         request = Request(self._client)
         path    = "/projects/" + quote_plus(self.id) + ""
         data    = {
 
         }
 
-        response = Response(request.put(path, data, options))
+        response = Response(request.get(path, data, options))
         return_values = []
         
         body = response.body
         body = body["project"]
                 
                 
         return_values.append(self.fill_with_data(body))
                 
 
         
         return return_values[0]
 
-    def delete(self, options = {}):
-        """Delete the project. Be careful! Executing this request will prevent any further interaction with the API that uses this project.
+    def save(self, options = {}):
+        """Save the updated project's attributes.
         Keyword argument:
         
         options -- Options for the request"""
         self.fill_with_data(options)
 
         request = Request(self._client)
-        path    = "/projects/{project_id}"
+        path    = "/projects/" + quote_plus(self.id) + ""
         data    = {
 
         }
 
-        response = Response(request.delete(path, data, options))
+        response = Response(request.put(path, data, options))
         return_values = []
         
-        return_values.append(response.success)
+        body = response.body
+        body = body["project"]
+                
+                
+        return_values.append(self.fill_with_data(body))
+                
 
         
         return return_values[0]
 
-    def regenerate_private_key(self, options = {}):
-        """Regenerate the project private key. Make sure to store the new private key and use it in any future request.
+    def delete(self, options = {}):
+        """Delete the project. Be careful! Executing this request will prevent any further interaction with the API that uses this project.
         Keyword argument:
         
         options -- Options for the request"""
         self.fill_with_data(options)
 
         request = Request(self._client)
-        path    = "/projects/{project_id}/private-key"
+        path    = "/projects/{project_id}"
         data    = {
 
         }
 
-        response = Response(request.post(path, data, options))
+        response = Response(request.delete(path, data, options))
         return_values = []
         
-        body = response.body
-        body = body["project"]
-                
-                
-        obj = processout.Project(self._client)
-        return_values.append(obj.fill_with_data(body))
-                
+        return_values.append(response.success)
 
         
         return return_values[0]
 
     def fetch_supervised(self, options = {}):
         """Get all the supervised projects.
         Keyword argument:
```

### Comparing `processout-6.8.0/processout/invoice.py` & `processout-6.9.0/processout/invoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -506,15 +506,15 @@
         options -- Options for the request"""
         self.fill_with_data(options)
 
         request = Request(self._client)
         path    = "/invoices/" + quote_plus(self.id) + "/authorize"
         data    = {
             'synchronous': options.get("synchronous"), 
-            'prioritized_gateway_configuration_id': options.get("prioritized_gateway_configuration_id"), 
+            'retry_drop_liability_shift': options.get("retry_drop_liability_shift"), 
             'source': source
         }
 
         response = Response(request.post(path, data, options))
         return_values = []
         
         body = response.body
@@ -533,14 +533,15 @@
         self.fill_with_data(options)
 
         request = Request(self._client)
         path    = "/invoices/" + quote_plus(self.id) + "/capture"
         data    = {
             'authorize_only': options.get("authorize_only"), 
             'synchronous': options.get("synchronous"), 
+            'retry_drop_liability_shift': options.get("retry_drop_liability_shift"), 
             'source': source
         }
 
         response = Response(request.post(path, data, options))
         return_values = []
         
         body = response.body
```


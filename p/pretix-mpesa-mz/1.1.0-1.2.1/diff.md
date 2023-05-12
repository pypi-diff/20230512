# Comparing `tmp/pretix-mpesa-mz-1.1.0.tar.gz` & `tmp/pretix-mpesa-mz-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.1.0.tar", last modified: Thu May 11 15:04:08 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.2.1.tar", last modified: Fri May 12 13:59:59 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.1.0.tar` & `pretix-mpesa-mz-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.626879 pretix-mpesa-mz-1.1.0/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1686 2023-05-11 15:04:08.627883 pretix-mpesa-mz-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.444893 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1686 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-05-11 15:04:08.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.487881 pretix-mpesa-mz-1.1.0/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-05-11 15:01:48.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.361879 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.359879 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.506914 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.519884 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.540881 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0    11909 2023-05-11 14:52:54.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.367877 pretix-mpesa-mz-1.1.0/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.550880 pretix-mpesa-mz-1.1.0/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.372883 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.612882 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      380 2023-05-11 14:14:56.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      236 2023-05-11 14:34:44.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0      452 2023-05-11 14:57:44.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      903 2023-05-11 15:04:08.630881 pretix-mpesa-mz-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.619879 pretix-mpesa-mz-1.1.0/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.697905 pretix-mpesa-mz-1.2.1/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1844 2023-05-12 13:59:59.698906 pretix-mpesa-mz-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.581909 pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1844 2023-05-12 13:59:59.000000 pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1096 2023-05-12 13:59:59.000000 pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 13:59:59.000000 pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-12 13:59:59.000000 pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 13:59:59.000000 pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.609903 pretix-mpesa-mz-1.2.1/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-05-12 13:59:13.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.514906 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.512910 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.619903 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.625911 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.635904 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     7658 2023-05-11 17:22:13.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/mpesa_api.py
+-rw-rw-rw-   0        0        0    11912 2023-05-11 17:23:29.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.519909 pretix-mpesa-mz-1.2.1/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.641905 pretix-mpesa-mz-1.2.1/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.522904 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.685903 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      377 2023-05-11 17:08:48.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0      452 2023-05-11 14:57:44.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      903 2023-05-12 13:59:59.701906 pretix-mpesa-mz-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:59:59.691906 pretix-mpesa-mz-1.2.1/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.2.1/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.1.0/LICENSE` & `pretix-mpesa-mz-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.1.0/PKG-INFO` & `pretix-mpesa-mz-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.1.0
+Version: 1.2.1
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
 
 MPesaMZ
 ==========================
 
 This is a plugin for `pretix`_. 
 
 A plugin to allow payments through the M-Pesa mobile payment platform
 
+Dependencies (mpesa-sdk)
+------------------------
+certifi==2018.1.18
+chardet==5.1.*
+idna==2.6
+pycryptodome==3.6
+requests==2.28.1
+urllib3==1.26.12
+
+
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository.
```

### Comparing `pretix-mpesa-mz-1.1.0/README.rst` & `pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,34 @@
+Metadata-Version: 2.1
+Name: pretix-mpesa-mz
+Version: 1.2.1
+Summary: A plugin to allow payments through the M-Pesa mobile payment platform
+Home-page: https://github.com/ivanruby/pretix-mpesa-mz
+Author: Ivan Ruby
+Author-email: ivanrubyds@gmail.com
+License: Apache
+License-File: LICENSE
+
 MPesaMZ
 ==========================
 
 This is a plugin for `pretix`_. 
 
 A plugin to allow payments through the M-Pesa mobile payment platform
 
+Dependencies (mpesa-sdk)
+------------------------
+certifi==2018.1.18
+chardet==5.1.*
+idna==2.6
+pycryptodome==3.6
+requests==2.28.1
+urllib3==1.26.12
+
+
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository.
```

### Comparing `pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.2.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: pretix-mpesa-mz
-Version: 1.1.0
-Summary: A plugin to allow payments through the M-Pesa mobile payment platform
-Home-page: https://github.com/ivanruby/pretix-mpesa-mz
-Author: Ivan Ruby
-Author-email: ivanrubyds@gmail.com
-License: Apache
-License-File: LICENSE
-
 MPesaMZ
 ==========================
 
 This is a plugin for `pretix`_. 
 
 A plugin to allow payments through the M-Pesa mobile payment platform
 
+Dependencies (mpesa-sdk)
+------------------------
+certifi==2018.1.18
+chardet==5.1.*
+idna==2.6
+pycryptodome==3.6
+requests==2.28.1
+urllib3==1.26.12
+
+
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository.
```

### Comparing `pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.2.1/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pretix_mpesa_mz.egg-info/PKG-INFO
 pretix_mpesa_mz.egg-info/SOURCES.txt
 pretix_mpesa_mz.egg-info/dependency_links.txt
 pretix_mpesa_mz.egg-info/entry_points.txt
 pretix_mpesa_mz.egg-info/top_level.txt
 pretix_mpesamz/__init__.py
 pretix_mpesamz/apps.py
+pretix_mpesamz/mpesa_api.py
 pretix_mpesamz/payment.py
 pretix_mpesamz/signals.py
 pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
 pretix_mpesamz/locale/de/LC_MESSAGES/django.po
 pretix_mpesamz/locale/de_Informal/.gitkeep
 pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
 pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
```

### Comparing `pretix-mpesa-mz-1.1.0/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.2.1/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.1.0/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.2.1/pretix_mpesamz/payment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
+from pprint import pprint
 from collections import OrderedDict
 
 from i18nfield.fields import I18nFormField, I18nTextarea
 from i18nfield.strings import LazyI18nString
 
 from pretix.base.models import OrderPayment
 from pretix.base.payment import BasePaymentProvider, PaymentException
 from pretix.base.templatetags.rich_text import rich_text
 from django.utils.translation import ugettext_lazy as _
 from django.template.loader import get_template
 from django import forms
 
-from paymentsds.mpesa import Client
 from random import randint
+from pretix_mpesamz.mpesa_api import execute_mpesa_c2b
 
 
 class MpesaPayment(BasePaymentProvider):
     identifier = 'mpesa'
 
     ########################################################
     #                   General Settings
@@ -123,14 +124,15 @@
                                 'invalid': 'Por favor, introduza um número 84 ou 85 válido'}
                         ))
         return OrderedDict([
             msisdn_field,
         ])
 
     def payment_form_render(self, request):
+
         form = self.payment_form(request)
         template = get_template('pretix_mpesamz/checkout_payment_form.html')
         ctx = {
             'request': request,
             'form': form,
             'information_text': self.information_text,
         }
@@ -140,137 +142,137 @@
         template = get_template('pretix_mpesamz/order.html')
         ctx = {
             'information_text': self.information_text,
             'msisdn': request.session.get('payment_%s_msisdn' % self.identifier)
         }
         return template.render(ctx)
 
-    def execute_mpesa_payment(self, payload):
-        client = Client(
-            api_key=self.settings.get('api_key'),
-            public_key=self.settings.get('public_key'),
-            service_provider_code=self.settings.get('service_provider_code')
-        )
-
-        return client.receive(payload)
-
     def execute_payment(self, request, payment):
         msisdn = request.session.get('payment_%s_msisdn' % self.identifier, '')
 
         try:
+            config = {
+                'api_key': self.settings.get('api_key'),
+                'public_key': self.settings.get('public_key')
+            }
+
             payment_data = {
-                'from': "258" + str(msisdn),
-                'reference': payment.order.code,
-                'transaction': 'TEST' + str(randint(0, 1000)),
-                'amount': str(int(float(payment.amount)))
+                'msisdn': "258" + str(msisdn),
+                'reference': 'TKT' + str(randint(0, 10000)),
+                'third_party_reference': payment.order.code,
+                'amount': str(int(float(payment.amount))),
+                'service_provider_code': self.settings.get('service_provider_code')
             }
 
-            result = self.execute_mpesa_payment(payment_data)
-            print(vars(result))
+            result = execute_mpesa_c2b(config, payment_data)
+            # pprint(result)
 
-            if result.success:
+            if result['output_ResponseCode'] == 'INS-0':
                 success_payload = json.dumps({
                     'success': True,
-                    'code': result.status.code,
+                    'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
-                    'conversation': result.data['conversation'],
-                    'description': result.status.description
+                    'conversation': result['output_ConversationID'],
+                    'description': result['output_ResponseDesc'],
+                    'transaction': result['output_TransactionID']
                 })
                 # Displayed in control panel but not on API order response
                 payment.info = success_payload
 
-                # Add success payload to a field returned on Order Endpoint
-                payment.order.meta_info = success_payload
-                payment.order.save(update_fields=['meta_info'])
-
                 payment.save(update_fields=['info'])
                 payment.confirm()
             else:
                 error_payload = json.dumps({
                     'success': False,
+                    'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
-                    'code': result.status.code,
-                    'conversation': result.data['conversation'],
-                    'description': result.status.description
+                    'conversation': result['output_ConversationID'],
+                    'description': result['output_ResponseDesc'],
+                    'transaction': result['output_TransactionID']
                 })
 
                 # Displayed in control panel but not on API order response
                 payment.info = error_payload
 
                 payment.save(update_fields=['info'])
                 payment.fail()
 
             return
         except Exception as e:
             print(repr(e))
 
     def payment_prepare(self, request, payment):
-        msisdn = request.session.get(
-            'payment_%s_msisdn' % self.identifier, '')
+        msisdn = request.session.get('payment_%s_msisdn' % self.identifier, '')
 
         try:
+            config = {
+                'api_key': self.settings.get('api_key'),
+                'public_key': self.settings.get('public_key')
+            }
+
             payment_data = {
-                'from': "258" + str(msisdn),
-                'reference': payment.order.code + str(randint(0, 10)),
-                'transaction': 'TEST' + str(randint(0, 1000)),
-                'amount': str(int(float(payment.amount)))
+                'msisdn': "258" + str(msisdn),
+                'reference': 'TKT' + str(randint(0, 10000)),
+                'third_party_reference': payment.order.code + str(randint(1, 10)),
+                'amount': str(int(float(payment.amount))),
+                'service_provider_code': self.settings.get('service_provider_code')
             }
 
-            result = self.execute_mpesa_payment(payment_data)
-            print(vars(result))
+            result = execute_mpesa_c2b(config, payment_data)
+            # pprint(result)
 
-            if result.success:
+            if result['output_ResponseCode'] == 'INS-0':
                 success_payload = json.dumps({
                     'success': True,
-                    'code': result.status.code,
+                    'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
-                    'conversation': result.data['conversation'],
-                    'description': result.status.description
+                    'conversation': result['output_ConversationID'],
+                    'description': result['output_ResponseDesc'],
+                    'transaction': result['output_TransactionID']
                 })
                 # Displayed in control panel but not on API order response
                 payment.info = success_payload
 
-                # Add success payload to a field returned on Order Endpoint
-                payment.order.meta_info = success_payload
-                payment.order.save(update_fields=['meta_info'])
-
                 payment.save(update_fields=['info'])
                 payment.confirm()
             else:
                 error_payload = json.dumps({
                     'success': False,
+                    'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
-                    'code': result.status.code,
-                    'conversation': result.data['conversation'],
-                    'description': result.status.description
+                    'conversation': result['output_ConversationID'],
+                    'description': result['output_ResponseDesc'],
+                    'transaction': result['output_TransactionID']
                 })
 
                 # Displayed in control panel but not on API order response
                 payment.info = error_payload
 
                 payment.save(update_fields=['info'])
                 payment.fail()
 
             return
         except Exception as e:
             print(repr(e))
 
     def payment_pending_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/payment_pending.html')
-        if payment.info:
+        if payment.info is not None and 'conversation' in payment.info:
             payment_info = json.loads(payment.info)
         else:
             return _("No payment information available.")
 
         if payment_info['code'] == "INS-6":
             reason = "PIN incorreto"
         elif payment_info['code'] == "INS-9":
             reason = "demora na comunicação entre a aplicação e o M-Pesa"
         elif payment_info['code'] == "INS-10":
             reason = "transação duplicada"
+        else:
+            reason = payment_info['description']
 
         ctx = {
             'reason': reason,
             'msisdn': request.session.get('payment_%s_msisdn' % self.identifier, '')
         }
         return template.render(ctx)
 
@@ -291,25 +293,18 @@
     #                   info in Control Panel
     ########################################################
     def payment_control_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/control.html')
 
         if payment.info is not None and 'conversation' in payment.info:
             payment_info = json.loads(payment.info)
-            if payment_info['success']:
-                ctx = {
-                    'conversationID': payment_info['conversation'],
-                    'msisdn': payment_info['msisdn'],
-                    'description': payment_info['description'],
-                    'code': payment_info['code']
-                }
-            else:
-                ctx = {
-                    'conversationID': payment_info['conversation'],
-                    'msisdn': payment_info['msisdn'],
-                    'code': payment_info['code'],
-                    'description': payment_info['description'],
-                }
         else:
             return _("Pagamento via M-Pesa sem sucesso.")
 
+        ctx = {
+            'conversationID': payment_info['conversation'],
+            'msisdn': payment_info['msisdn'],
+            'description': payment_info['description'],
+            'code': payment_info['code'],
+            'transaction': payment_info['transaction']
+        }
         return template.render(ctx)
```

### Comparing `pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.2.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.1.0/setup.cfg` & `pretix-mpesa-mz-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.1.0/setup.py` & `pretix-mpesa-mz-1.2.1/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/oking_oz-3.2.31.tar.gz` & `tmp/oking_oz-3.2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oking_oz-3.2.31.tar", last modified: Fri May 12 18:34:24 2023, max compression
+gzip compressed data, was "oking_oz-3.2.32.tar", last modified: Fri May 12 18:45:02 2023, max compression
```

## Comparing `oking_oz-3.2.31.tar` & `oking_oz-3.2.32.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.689138 oking_oz-3.2.31/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/LICENSE
--rw-rw-rw-   0        0        0       29 2022-06-03 11:48:57.000000 oking_oz-3.2.31/MANIFEST.in
--rw-rw-rw-   0        0        0      935 2023-05-12 18:34:24.689138 oking_oz-3.2.31/PKG-INFO
--rw-rw-rw-   0        0        0     1187 2022-06-03 12:55:44.000000 oking_oz-3.2.31/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.634742 oking_oz-3.2.31/oking_oz.egg-info/
--rw-rw-rw-   0        0        0      935 2023-05-12 18:34:24.000000 oking_oz-3.2.31/oking_oz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2023-05-12 18:34:24.000000 oking_oz-3.2.31/oking_oz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 18:34:24.000000 oking_oz-3.2.31/oking_oz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-12 18:34:24.000000 oking_oz-3.2.31/oking_oz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-12 18:34:24.000000 oking_oz-3.2.31/oking_oz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-12 18:34:24.000000 oking_oz-3.2.31/oking_oz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-06-03 11:48:57.000000 oking_oz-3.2.31/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 18:34:24.689138 oking_oz-3.2.31/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-05-12 18:34:21.000000 oking_oz-3.2.31/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.634742 oking_oz-3.2.31/src/
--rw-rw-rw-   0        0        0     2979 2022-08-23 11:22:25.000000 oking_oz-3.2.31/src/__init__.py
--rw-rw-rw-   0        0        0    25475 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.634742 oking_oz-3.2.31/src/api/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.650380 oking_oz-3.2.31/src/api/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/api/entities/__init__.py
--rw-rw-rw-   0        0        0     5097 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/api/entities/cliente.py
--rw-rw-rw-   0        0        0     4496 2022-12-23 14:47:52.000000 oking_oz-3.2.31/src/api/entities/cliente_aprovado.py
--rw-rw-rw-   0        0        0      249 2022-12-19 18:06:20.000000 oking_oz-3.2.31/src/api/entities/cliente_erp_code.py
--rw-rw-rw-   0        0        0      932 2022-10-03 17:41:50.000000 oking_oz-3.2.31/src/api/entities/imposto_produto.py
--rw-rw-rw-   0        0        0     1171 2022-10-03 17:41:50.000000 oking_oz-3.2.31/src/api/entities/lista_preco.py
--rw-rw-rw-   0        0        0      390 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/api/entities/plano_pagamento_cliente.py
--rw-rw-rw-   0        0        0      934 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/api/entities/representante.py
--rw-rw-rw-   0        0        0      739 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/api/oking.py
--rw-rw-rw-   0        0        0    20636 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/api/okvendas.py
--rw-rw-rw-   0        0        0      886 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/api/slack.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.650380 oking_oz-3.2.31/src/database/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/database/__init__.py
--rw-rw-rw-   0        0        0     2488 2022-08-23 11:22:25.000000 oking_oz-3.2.31/src/database/connection.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.666002 oking_oz-3.2.31/src/database/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/database/entities/__init__.py
--rw-rw-rw-   0        0        0     1616 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/database/entities/client.py
--rw-rw-rw-   0        0        0      253 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/database/entities/client_payment_plan.py
--rw-rw-rw-   0        0        0     1077 2022-10-03 17:41:50.000000 oking_oz-3.2.31/src/database/entities/price_list.py
--rw-rw-rw-   0        0        0      801 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/database/entities/product_tax.py
--rw-rw-rw-   0        0        0      639 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/database/entities/representative.py
--rw-rw-rw-   0        0        0    49121 2023-05-12 18:30:53.000000 oking_oz-3.2.31/src/database/queries.py
--rw-rw-rw-   0        0        0      327 2022-07-04 16:40:47.000000 oking_oz-3.2.31/src/database/sqlserver_db.py
--rw-rw-rw-   0        0        0     1106 2022-07-04 16:40:47.000000 oking_oz-3.2.31/src/database/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.681626 oking_oz-3.2.31/src/entities/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/entities/__init__.py
--rw-rw-rw-   0        0        0      628 2022-07-29 17:49:42.000000 oking_oz-3.2.31/src/entities/invoice.py
--rw-rw-rw-   0        0        0      288 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/entities/log.py
--rw-rw-rw-   0        0        0     6798 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/entities/order.py
--rw-rw-rw-   0        0        0    16869 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/entities/orderb2b.py
--rw-rw-rw-   0        0        0     6823 2023-05-12 18:30:53.000000 oking_oz-3.2.31/src/entities/orderb2c.py
--rw-rw-rw-   0        0        0     3014 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/entities/pagamento.py
--rw-rw-rw-   0        0        0      351 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/entities/photos_sku.py
--rw-rw-rw-   0        0        0      407 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/entities/price.py
--rw-rw-rw-   0        0        0    10790 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/entities/product.py
--rw-rw-rw-   0        0        0     1959 2022-12-16 19:21:16.000000 oking_oz-3.2.31/src/entities/response.py
--rw-rw-rw-   0        0        0      940 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/entities/tracking.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:34:24.689138 oking_oz-3.2.31/src/jobs/
--rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.31/src/jobs/__init__.py
--rw-rw-rw-   0        0        0    18254 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/client_jobs.py
--rw-rw-rw-   0        0        0     8965 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/client_payment_plan_jobs.py
--rw-rw-rw-   0        0        0     2937 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/client_payment_plan_semaphore_jobs.py
--rw-rw-rw-   0        0        0    83964 2023-05-12 18:30:53.000000 oking_oz-3.2.31/src/jobs/order_jobs.py
--rw-rw-rw-   0        0        0    19666 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/price_jobs.py
--rw-rw-rw-   0        0        0    25107 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/products_jobs.py
--rw-rw-rw-   0        0        0     6841 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/representative_jobs.py
--rw-rw-rw-   0        0        0    12784 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/stock_jobs.py
--rw-rw-rw-   0        0        0     2003 2023-04-10 18:55:42.000000 oking_oz-3.2.31/src/jobs/system_jobs.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.614814 oking_oz-3.2.32/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/LICENSE
+-rw-rw-rw-   0        0        0       29 2022-06-03 11:48:57.000000 oking_oz-3.2.32/MANIFEST.in
+-rw-rw-rw-   0        0        0      935 2023-05-12 18:45:02.614814 oking_oz-3.2.32/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2022-06-03 12:55:44.000000 oking_oz-3.2.32/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/oking_oz.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1551 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-12 18:45:02.000000 oking_oz-3.2.32/oking_oz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-06-03 11:48:57.000000 oking_oz-3.2.32/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 18:45:02.614814 oking_oz-3.2.32/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-05-12 18:44:55.000000 oking_oz-3.2.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/src/
+-rw-rw-rw-   0        0        0     2979 2022-08-23 11:22:25.000000 oking_oz-3.2.32/src/__init__.py
+-rw-rw-rw-   0        0        0    25475 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/src/api/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.567535 oking_oz-3.2.32/src/api/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/entities/__init__.py
+-rw-rw-rw-   0        0        0     5097 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/api/entities/cliente.py
+-rw-rw-rw-   0        0        0     4496 2022-12-23 14:47:52.000000 oking_oz-3.2.32/src/api/entities/cliente_aprovado.py
+-rw-rw-rw-   0        0        0      249 2022-12-19 18:06:20.000000 oking_oz-3.2.32/src/api/entities/cliente_erp_code.py
+-rw-rw-rw-   0        0        0      932 2022-10-03 17:41:50.000000 oking_oz-3.2.32/src/api/entities/imposto_produto.py
+-rw-rw-rw-   0        0        0     1171 2022-10-03 17:41:50.000000 oking_oz-3.2.32/src/api/entities/lista_preco.py
+-rw-rw-rw-   0        0        0      390 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/api/entities/plano_pagamento_cliente.py
+-rw-rw-rw-   0        0        0      934 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/api/entities/representante.py
+-rw-rw-rw-   0        0        0      739 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/oking.py
+-rw-rw-rw-   0        0        0    20636 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/api/okvendas.py
+-rw-rw-rw-   0        0        0      886 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/api/slack.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.583169 oking_oz-3.2.32/src/database/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/database/__init__.py
+-rw-rw-rw-   0        0        0     2488 2022-08-23 11:22:25.000000 oking_oz-3.2.32/src/database/connection.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.583169 oking_oz-3.2.32/src/database/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/database/entities/__init__.py
+-rw-rw-rw-   0        0        0     1616 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/database/entities/client.py
+-rw-rw-rw-   0        0        0      253 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/database/entities/client_payment_plan.py
+-rw-rw-rw-   0        0        0     1077 2022-10-03 17:41:50.000000 oking_oz-3.2.32/src/database/entities/price_list.py
+-rw-rw-rw-   0        0        0      801 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/database/entities/product_tax.py
+-rw-rw-rw-   0        0        0      639 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/database/entities/representative.py
+-rw-rw-rw-   0        0        0    49121 2023-05-12 18:30:53.000000 oking_oz-3.2.32/src/database/queries.py
+-rw-rw-rw-   0        0        0      327 2022-07-04 16:40:47.000000 oking_oz-3.2.32/src/database/sqlserver_db.py
+-rw-rw-rw-   0        0        0     1106 2022-07-04 16:40:47.000000 oking_oz-3.2.32/src/database/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.601304 oking_oz-3.2.32/src/entities/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/__init__.py
+-rw-rw-rw-   0        0        0      628 2022-07-29 17:49:42.000000 oking_oz-3.2.32/src/entities/invoice.py
+-rw-rw-rw-   0        0        0      288 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/log.py
+-rw-rw-rw-   0        0        0     6846 2023-05-12 18:44:49.000000 oking_oz-3.2.32/src/entities/order.py
+-rw-rw-rw-   0        0        0    16869 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/entities/orderb2b.py
+-rw-rw-rw-   0        0        0     6823 2023-05-12 18:30:53.000000 oking_oz-3.2.32/src/entities/orderb2c.py
+-rw-rw-rw-   0        0        0     3014 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/pagamento.py
+-rw-rw-rw-   0        0        0      351 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/photos_sku.py
+-rw-rw-rw-   0        0        0      407 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/price.py
+-rw-rw-rw-   0        0        0    10790 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/entities/product.py
+-rw-rw-rw-   0        0        0     1959 2022-12-16 19:21:16.000000 oking_oz-3.2.32/src/entities/response.py
+-rw-rw-rw-   0        0        0      940 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/entities/tracking.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:45:02.614814 oking_oz-3.2.32/src/jobs/
+-rw-rw-rw-   0        0        0        0 2022-06-03 11:48:57.000000 oking_oz-3.2.32/src/jobs/__init__.py
+-rw-rw-rw-   0        0        0    18254 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/client_jobs.py
+-rw-rw-rw-   0        0        0     8965 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/client_payment_plan_jobs.py
+-rw-rw-rw-   0        0        0     2937 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/client_payment_plan_semaphore_jobs.py
+-rw-rw-rw-   0        0        0    83964 2023-05-12 18:30:53.000000 oking_oz-3.2.32/src/jobs/order_jobs.py
+-rw-rw-rw-   0        0        0    19666 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/price_jobs.py
+-rw-rw-rw-   0        0        0    25107 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/products_jobs.py
+-rw-rw-rw-   0        0        0     6841 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/representative_jobs.py
+-rw-rw-rw-   0        0        0    12784 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/stock_jobs.py
+-rw-rw-rw-   0        0        0     2003 2023-04-10 18:55:42.000000 oking_oz-3.2.32/src/jobs/system_jobs.py
```

### Comparing `oking_oz-3.2.31/PKG-INFO` & `oking_oz-3.2.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oking_oz
-Version: 3.2.31
+Version: 3.2.32
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
 Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
 License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
 Platform: UNKNOWN
```

### Comparing `oking_oz-3.2.31/README.md` & `oking_oz-3.2.32/README.md`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/oking_oz.egg-info/PKG-INFO` & `oking_oz-3.2.32/oking_oz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oking-oz
-Version: 3.2.31
+Version: 3.2.32
 Summary: Pacote de integração de produtos, preço, estoque e pedidos com o sistema OkVendas da Openk
 Home-page: UNKNOWN
 Author: Openk Tecnologia
 Author-email: <suporte.b2c@openk.com.br>
 License: UNKNOWN
 Keywords: python,oking,openk,okvendas,ok
 Platform: UNKNOWN
```

### Comparing `oking_oz-3.2.31/oking_oz.egg-info/SOURCES.txt` & `oking_oz-3.2.32/oking_oz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/setup.py` & `oking_oz-3.2.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #     f = open('version.txt', 'w')
 #     f.write(f'\tOking {v} - Openk Tecnologia')
 #     f.close()
 
 
 # Utilizar o padrão x.x.x.xxxx para caso precise subir versão de testes para o respositorio test-pypi
 # Utilizar o padrão x.x.x para subir em produção
-version = '3.2.31'
+version = '3.2.32'
 package_name = "oking_oz" if len([c for c in version if c == '.']) < 3 else 'okingtest'
 # save_version(version)
 setup(
     name=package_name,
     version=version,
     author="Openk Tecnologia",
     author_email="<suporte.b2c@openk.com.br>",
```

### Comparing `oking_oz-3.2.31/src/__init__.py` & `oking_oz-3.2.32/src/__init__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/__main__.py` & `oking_oz-3.2.32/src/__main__.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/entities/cliente.py` & `oking_oz-3.2.32/src/api/entities/cliente.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/entities/cliente_aprovado.py` & `oking_oz-3.2.32/src/api/entities/cliente_aprovado.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/entities/imposto_produto.py` & `oking_oz-3.2.32/src/api/entities/imposto_produto.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/entities/lista_preco.py` & `oking_oz-3.2.32/src/api/entities/lista_preco.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/entities/representante.py` & `oking_oz-3.2.32/src/api/entities/representante.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/oking.py` & `oking_oz-3.2.32/src/api/oking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/okvendas.py` & `oking_oz-3.2.32/src/api/okvendas.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/api/slack.py` & `oking_oz-3.2.32/src/api/slack.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/connection.py` & `oking_oz-3.2.32/src/database/connection.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/entities/client.py` & `oking_oz-3.2.32/src/database/entities/client.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/entities/price_list.py` & `oking_oz-3.2.32/src/database/entities/price_list.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/entities/product_tax.py` & `oking_oz-3.2.32/src/database/entities/product_tax.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/entities/representative.py` & `oking_oz-3.2.32/src/database/entities/representative.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/queries.py` & `oking_oz-3.2.32/src/database/queries.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/database/utils.py` & `oking_oz-3.2.32/src/database/utils.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/invoice.py` & `oking_oz-3.2.32/src/entities/invoice.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/order.py` & `oking_oz-3.2.32/src/entities/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,20 @@
         self.ibge_code: str = codigo_ibge
 
 
 class OrderItem:
     def __init__(self, sku_principal: str, sku_variacao: str, sku_reference: str, hierarquia_variacao: str, is_restock: bool, codigo_externo_restock: str,
                  ean: str, quantidade: int, value: float, valor_desconto: float, altura: float, comprimento: float, largura: float, peso: float, volume: float,
                  filial_expedicao: str, filial_faturamento: str, cnpj_filial_venda: str, unidade_medida: str = str(), valor_comissao_frete: float = 0.0, valor_frete: float = 0.0,
-                 percentual_comissao: float = 0.0, valor_comissao: float = 0.0, tipo_anuncio: str = ''):
+                 percentual_comissao: float = 0.0, valor_comissao: float = 0.0, tipo_anuncio: str = '', **kwargs):
         self.sku: str = sku_reference
         self.erp_code: str = sku_variacao
         self.measure_unity = unidade_medida
         self.quantity: int = quantidade
         self.ean: str = ean
         self.value: float = value
         self.discount: float = valor_desconto
         self.freight_value: float = valor_frete
         self.expedition_branch: str = filial_expedicao
         self.invoice_branch: str = filial_faturamento
         self.selling_branch_cnpj: str = cnpj_filial_venda
+        self.__dict__.update(kwargs)
```

### Comparing `oking_oz-3.2.31/src/entities/orderb2b.py` & `oking_oz-3.2.32/src/entities/orderb2b.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/orderb2c.py` & `oking_oz-3.2.32/src/entities/orderb2c.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/pagamento.py` & `oking_oz-3.2.32/src/entities/pagamento.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/product.py` & `oking_oz-3.2.32/src/entities/product.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/response.py` & `oking_oz-3.2.32/src/entities/response.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/entities/tracking.py` & `oking_oz-3.2.32/src/entities/tracking.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/client_jobs.py` & `oking_oz-3.2.32/src/jobs/client_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/client_payment_plan_jobs.py` & `oking_oz-3.2.32/src/jobs/client_payment_plan_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/client_payment_plan_semaphore_jobs.py` & `oking_oz-3.2.32/src/jobs/client_payment_plan_semaphore_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/order_jobs.py` & `oking_oz-3.2.32/src/jobs/order_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/price_jobs.py` & `oking_oz-3.2.32/src/jobs/price_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/products_jobs.py` & `oking_oz-3.2.32/src/jobs/products_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/representative_jobs.py` & `oking_oz-3.2.32/src/jobs/representative_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/stock_jobs.py` & `oking_oz-3.2.32/src/jobs/stock_jobs.py`

 * *Files identical despite different names*

### Comparing `oking_oz-3.2.31/src/jobs/system_jobs.py` & `oking_oz-3.2.32/src/jobs/system_jobs.py`

 * *Files identical despite different names*


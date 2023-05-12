# Comparing `tmp/eth-tester-0.8.0b3.tar.gz` & `tmp/eth-tester-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-tester-0.8.0b3.tar", last modified: Fri Dec 16 18:08:12 2022, max compression
+gzip compressed data, was "eth-tester-0.9.0b1.tar", last modified: Fri May 12 17:13:15 2023, max compression
```

## Comparing `eth-tester-0.8.0b3.tar` & `eth-tester-0.9.0b1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.696818 eth-tester-0.8.0b3/
--rw-r--r--   0 eve        (501) staff       (20)     1080 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      121 2022-08-25 19:50:54.000000 eth-tester-0.8.0b3/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)    35038 2022-12-16 18:08:12.696652 eth-tester-0.8.0b3/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)    34120 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.688585 eth-tester-0.8.0b3/eth_tester/
--rw-r--r--   0 eve        (501) staff       (20)      331 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.689832 eth-tester-0.8.0b3/eth_tester/backends/
--rw-r--r--   0 eve        (501) staff       (20)     1652 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2889 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)      540 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/backends/common.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.690973 eth-tester-0.8.0b3/eth_tester/backends/mock/
--rw-r--r--   0 eve        (501) staff       (20)       53 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/backends/mock/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      304 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/backends/mock/common.py
--rw-r--r--   0 eve        (501) staff       (20)    12860 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/backends/mock/factory.py
--rw-r--r--   0 eve        (501) staff       (20)     9480 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/backends/mock/main.py
--rw-r--r--   0 eve        (501) staff       (20)     2887 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/backends/mock/serializers.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.691850 eth-tester-0.8.0b3/eth_tester/backends/pyevm/
--rw-r--r--   0 eve        (501) staff       (20)      173 2021-11-18 18:37:46.000000 eth-tester-0.8.0b3/eth_tester/backends/pyevm/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    25336 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/backends/pyevm/main.py
--rw-r--r--   0 eve        (501) staff       (20)     8172 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/backends/pyevm/serializers.py
--rw-r--r--   0 eve        (501) staff       (20)      515 2021-11-18 18:37:46.000000 eth-tester-0.8.0b3/eth_tester/backends/pyevm/utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1702 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      413 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    29630 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/main.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.693179 eth-tester-0.8.0b3/eth_tester/normalization/
--rw-r--r--   0 eve        (501) staff       (20)      702 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/normalization/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3297 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/normalization/base.py
--rw-r--r--   0 eve        (501) staff       (20)      635 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/normalization/common.py
--rw-r--r--   0 eve        (501) staff       (20)     2665 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/normalization/default.py
--rw-r--r--   0 eve        (501) staff       (20)     3171 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/normalization/inbound.py
--rw-r--r--   0 eve        (501) staff       (20)     4874 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/normalization/outbound.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/rpc.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.693394 eth-tester-0.8.0b3/eth_tester/tools/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-10 19:15:57.000000 eth-tester-0.8.0b3/eth_tester/tools/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2235 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/tools/gas_burner_contract.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.695212 eth-tester-0.8.0b3/eth_tester/utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      152 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/utils/accounts.py
--rw-r--r--   0 eve        (501) staff       (20)      243 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/utils/address.py
--rw-r--r--   0 eve        (501) staff       (20)    64262 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/utils/backend_testing.py
--rw-r--r--   0 eve        (501) staff       (20)     9633 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/utils/emitter_contract.py
--rw-r--r--   0 eve        (501) staff       (20)      323 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/utils/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)     5244 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/utils/filters.py
--rw-r--r--   0 eve        (501) staff       (20)     4324 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/utils/math_contract.py
--rw-r--r--   0 eve        (501) staff       (20)      906 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/utils/module_loading.py
--rw-r--r--   0 eve        (501) staff       (20)     5035 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/utils/throws_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1191 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/utils/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.696263 eth-tester-0.8.0b3/eth_tester/validation/
--rw-r--r--   0 eve        (501) staff       (20)      658 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/validation/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2949 2021-11-04 18:08:25.000000 eth-tester-0.8.0b3/eth_tester/validation/base.py
--rw-r--r--   0 eve        (501) staff       (20)     5518 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/validation/common.py
--rw-r--r--   0 eve        (501) staff       (20)     2903 2021-03-31 18:03:15.000000 eth-tester-0.8.0b3/eth_tester/validation/default.py
--rw-r--r--   0 eve        (501) staff       (20)    10396 2022-08-31 17:39:35.000000 eth-tester-0.8.0b3/eth_tester/validation/inbound.py
--rw-r--r--   0 eve        (501) staff       (20)     8347 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/eth_tester/validation/outbound.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 18:08:12.689273 eth-tester-0.8.0b3/eth_tester.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)    35038 2022-12-16 18:08:12.000000 eth-tester-0.8.0b3/eth_tester.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1616 2022-12-16 18:08:12.000000 eth-tester-0.8.0b3/eth_tester.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-12-16 18:08:12.000000 eth-tester-0.8.0b3/eth_tester.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-12-16 18:08:12.000000 eth-tester-0.8.0b3/eth_tester.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)      994 2022-12-16 18:08:12.000000 eth-tester-0.8.0b3/eth_tester.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       11 2022-12-16 18:08:12.000000 eth-tester-0.8.0b3/eth_tester.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1055 2022-11-21 19:35:20.000000 eth-tester-0.8.0b3/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2022-12-16 18:08:12.696852 eth-tester-0.8.0b3/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     2532 2022-12-16 18:08:11.000000 eth-tester-0.8.0b3/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.097611 eth-tester-0.9.0b1/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1080 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/LICENSE
+-rw-r--r--   0 fselmo     (501) staff       (20)      121 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/MANIFEST.in
+-rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-05-12 17:13:15.097258 eth-tester-0.9.0b1/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)    34123 2023-04-27 17:15:42.000000 eth-tester-0.9.0b1/README.md
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.067687 eth-tester-0.9.0b1/eth_tester/
+-rw-r--r--   0 fselmo     (501) staff       (20)      331 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.072724 eth-tester-0.9.0b1/eth_tester/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1652 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/backends/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2889 2023-02-01 17:33:56.000000 eth-tester-0.9.0b1/eth_tester/backends/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/backends/common.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.076943 eth-tester-0.9.0b1/eth_tester/backends/mock/
+-rw-r--r--   0 fselmo     (501) staff       (20)       53 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      304 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    13229 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/factory.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9480 2023-05-11 22:08:22.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/mock/serializers.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.080301 eth-tester-0.9.0b1/eth_tester/backends/pyevm/
+-rw-r--r--   0 fselmo     (501) staff       (20)      173 2021-11-18 21:01:41.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    26621 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8556 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/serializers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      515 2021-11-18 21:01:41.000000 eth-tester-0.9.0b1/eth_tester/backends/pyevm/utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1725 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      413 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    29630 2023-02-01 17:33:56.000000 eth-tester-0.9.0b1/eth_tester/main.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.084919 eth-tester-0.9.0b1/eth_tester/normalization/
+-rw-r--r--   0 fselmo     (501) staff       (20)      702 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/normalization/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3297 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/normalization/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      636 2023-05-01 23:05:21.000000 eth-tester-0.9.0b1/eth_tester/normalization/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2665 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/normalization/default.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3171 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/normalization/inbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5366 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/normalization/outbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/rpc.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.086025 eth-tester-0.9.0b1/eth_tester/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-10 20:58:14.000000 eth-tester-0.9.0b1/eth_tester/tools/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2235 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/tools/gas_burner_contract.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.093400 eth-tester-0.9.0b1/eth_tester/utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      152 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/utils/accounts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      243 2021-07-08 21:12:50.000000 eth-tester-0.9.0b1/eth_tester/utils/address.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    64238 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/utils/backend_testing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9633 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/emitter_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      323 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/encoding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5244 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/filters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4324 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/math_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      906 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/module_loading.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5035 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/throws_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1191 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/utils/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.096555 eth-tester-0.9.0b1/eth_tester/validation/
+-rw-r--r--   0 fselmo     (501) staff       (20)      658 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/eth_tester/validation/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2949 2021-11-04 23:39:22.000000 eth-tester-0.9.0b1/eth_tester/validation/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5833 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/validation/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2903 2021-10-06 21:26:28.000000 eth-tester-0.9.0b1/eth_tester/validation/default.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11059 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/validation/inbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9124 2023-05-11 22:34:02.000000 eth-tester-0.9.0b1/eth_tester/validation/outbound.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-12 17:13:15.070441 eth-tester-0.9.0b1/eth_tester.egg-info/
+-rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     1616 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2022-11-21 22:09:50.000000 eth-tester-0.9.0b1/eth_tester.egg-info/not-zip-safe
+-rw-r--r--   0 fselmo     (501) staff       (20)      994 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/requires.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       11 2023-05-12 17:13:14.000000 eth-tester-0.9.0b1/eth_tester.egg-info/top_level.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)     1055 2023-02-01 16:36:02.000000 eth-tester-0.9.0b1/pyproject.toml
+-rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-05-12 17:13:15.097705 eth-tester-0.9.0b1/setup.cfg
+-rw-r--r--   0 fselmo     (501) staff       (20)     2532 2023-05-12 17:10:30.000000 eth-tester-0.9.0b1/setup.py
```

### Comparing `eth-tester-0.8.0b3/LICENSE` & `eth-tester-0.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/PKG-INFO` & `eth-tester-0.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.8.0b3
+Version: 0.9.0b1
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -193,15 +192,15 @@
 # Documentation
 
 ## Input and output data formats
 
 The ethereum tester library strictly enforces the following input formats and
 types.
 
-* Hexidecimal values **must** be text (not byte) strings.  The `0x` prefix is optional.
+* Hexadecimal values **must** be text (not byte) strings.  The `0x` prefix is optional.
 * Any address which contains mixed-case alpha characters will be validated as a checksummed address as specified by [EIP-55](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-55.md)
 * 32-byte hashes **must** be hexadecimal encoded.
 * Numeric values **must** be in their integer representation.
 
 Similarly, ethereum tester ensures that return values conform to similar rules.
 
 * 32-byte hashes will be returned in their hexadecimal encoded representation.
@@ -717,15 +716,15 @@
 
 See [the filtering guide](#guide-filtering) for detailed information on how to use filters.
 
 <a id="api-delete_filter"></a>
 
 #### `EthereumTester.delete_filter(filter_id)`
 
-Removes the filter for the provide `filter_id`.  If no filter is found for the
+Removes the filter for the provided `filter_id`.  If no filter is found for the
 given `filter_id`, raises [`FilterNotFound`](#errors-FilterNotFound).
 
 
 <a id="api-get_only_filter_changes"></a>
 
 #### `EthereumTester.get_only_filter_changes(filter_id) -> transaction_hash or block_hash or log_entry`
 
@@ -753,15 +752,15 @@
 
 
 <a id="api-revert_to_snapshot"></a>
 
 #### `EthereumTester.revert_to_snapshot(snapshot_id)`
 
 Reverts the chain to the chain state associated with the given `snapshot_id`.
-Raises [`SnapshotNotFound`](#errors-SnapshotNotFound) if no snapshot is know
+Raises [`SnapshotNotFound`](#errors-SnapshotNotFound) if no snapshot is known
 for the given id.
 
 ### Errors and Exceptions
 
 <a id="errors-TransactionNotFound"></a>
 
 #### `eth_tester.exceptions.TransactionNotFound`
@@ -887,15 +886,15 @@
 
 # Generates the following `dict`:
 
 # custom_genesis_params = {
 #     "coinbase": GENESIS_COINBASE,
 #     "difficulty": GENESIS_DIFFICULTY,
 #     "extra_data": GENESIS_EXTRA_DATA,
-#     "gas_limit": 4500000    # <<< Overidden Value <<<
+#     "gas_limit": 4500000    # <<< Overridden Value <<<
 #     "mix_hash": GENESIS_MIX_HASH,
 #     "nonce": GENESIS_NONCE,
 #     "receipt_root": BLANK_ROOT_HASH,
 #     "timestamp": int(time.time()),
 #     "transaction_root": BLANK_ROOT_HASH,
 # }
 ```
@@ -997,15 +996,15 @@
 ## Normalization and Validation
 
 > Beware! Here there be dragons...  This section of the documentation is only
 > relevant if you intend to build tooling on top of this library.
 
 The ethereum tester provides strong guarantees that backends can be swapped out
 seamlessly without effecting the data formats of both the input arguments and
-return values.  This is accomplished using a two step process of strict
+return values.  This is accomplished using a two-step process of strict
 *normalization* and *validation*.
 
 All inputs to the methods of the `EthereumTester` are first validated then
 normalized to a *canonical* format.  Return values are put through this process
 as well, first validating the data returned by the backend, and then
 normalizing it from the *canonical* format to the *normal* form before being
 returned.
@@ -1033,9 +1032,7 @@
 
 
 # Use with Web3.py
 
 See the [web3.py documentation](http://web3py.readthedocs.io/en/latest/) for
 information on the `EthereumTester` provider which integrates with this
 library.
-
-
```

### Comparing `eth-tester-0.8.0b3/README.md` & `eth-tester-0.9.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 # Documentation
 
 ## Input and output data formats
 
 The ethereum tester library strictly enforces the following input formats and
 types.
 
-* Hexidecimal values **must** be text (not byte) strings.  The `0x` prefix is optional.
+* Hexadecimal values **must** be text (not byte) strings.  The `0x` prefix is optional.
 * Any address which contains mixed-case alpha characters will be validated as a checksummed address as specified by [EIP-55](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-55.md)
 * 32-byte hashes **must** be hexadecimal encoded.
 * Numeric values **must** be in their integer representation.
 
 Similarly, ethereum tester ensures that return values conform to similar rules.
 
 * 32-byte hashes will be returned in their hexadecimal encoded representation.
@@ -688,15 +688,15 @@
 
 See [the filtering guide](#guide-filtering) for detailed information on how to use filters.
 
 <a id="api-delete_filter"></a>
 
 #### `EthereumTester.delete_filter(filter_id)`
 
-Removes the filter for the provide `filter_id`.  If no filter is found for the
+Removes the filter for the provided `filter_id`.  If no filter is found for the
 given `filter_id`, raises [`FilterNotFound`](#errors-FilterNotFound).
 
 
 <a id="api-get_only_filter_changes"></a>
 
 #### `EthereumTester.get_only_filter_changes(filter_id) -> transaction_hash or block_hash or log_entry`
 
@@ -724,15 +724,15 @@
 
 
 <a id="api-revert_to_snapshot"></a>
 
 #### `EthereumTester.revert_to_snapshot(snapshot_id)`
 
 Reverts the chain to the chain state associated with the given `snapshot_id`.
-Raises [`SnapshotNotFound`](#errors-SnapshotNotFound) if no snapshot is know
+Raises [`SnapshotNotFound`](#errors-SnapshotNotFound) if no snapshot is known
 for the given id.
 
 ### Errors and Exceptions
 
 <a id="errors-TransactionNotFound"></a>
 
 #### `eth_tester.exceptions.TransactionNotFound`
@@ -858,15 +858,15 @@
 
 # Generates the following `dict`:
 
 # custom_genesis_params = {
 #     "coinbase": GENESIS_COINBASE,
 #     "difficulty": GENESIS_DIFFICULTY,
 #     "extra_data": GENESIS_EXTRA_DATA,
-#     "gas_limit": 4500000    # <<< Overidden Value <<<
+#     "gas_limit": 4500000    # <<< Overridden Value <<<
 #     "mix_hash": GENESIS_MIX_HASH,
 #     "nonce": GENESIS_NONCE,
 #     "receipt_root": BLANK_ROOT_HASH,
 #     "timestamp": int(time.time()),
 #     "transaction_root": BLANK_ROOT_HASH,
 # }
 ```
@@ -968,15 +968,15 @@
 ## Normalization and Validation
 
 > Beware! Here there be dragons...  This section of the documentation is only
 > relevant if you intend to build tooling on top of this library.
 
 The ethereum tester provides strong guarantees that backends can be swapped out
 seamlessly without effecting the data formats of both the input arguments and
-return values.  This is accomplished using a two step process of strict
+return values.  This is accomplished using a two-step process of strict
 *normalization* and *validation*.
 
 All inputs to the methods of the `EthereumTester` are first validated then
 normalized to a *canonical* format.  Return values are put through this process
 as well, first validating the data returned by the backend, and then
 normalizing it from the *canonical* format to the *normal* form before being
 returned.
```

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/__init__.py` & `eth-tester-0.9.0b1/eth_tester/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/base.py` & `eth-tester-0.9.0b1/eth_tester/backends/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/common.py` & `eth-tester-0.9.0b1/eth_tester/backends/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/mock/factory.py` & `eth-tester-0.9.0b1/eth_tester/backends/mock/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,16 @@
         "gas_limit": 30029122,
         "gas_used": 0,
         "timestamp": int(time.time()),
         "transactions": [],
         "uncles": [],
         # base fee at London fork block 12965000 on mainnet
         "base_fee_per_gas": 1000000000,
+        "withdrawals": [],
+        "withdrawals_root": BLANK_ROOT_HASH,
     }
     if overrides is not None:
         genesis_block = merge_genesis_overrides(
             defaults=default_genesis_block, overrides=overrides
         )
     else:
         genesis_block = default_genesis_block
@@ -394,14 +396,24 @@
         yield "uncles", []
 
     if "base_fee_per_gas" in overrides:
         yield "base_fee_per_gas", overrides["base_fee_per_gas"]
     else:
         yield "base_fee_per_gas", _calculate_expected_base_fee_per_gas(parent_block)
 
+    if "withdrawals" in overrides:
+        yield "withdrawals", overrides["withdrawals"]
+    else:
+        yield "withdrawals", []
+
+    if "withdrawals_root" in overrides:
+        yield "withdrawals_root", overrides["withdrawals_root"]
+    else:
+        yield "withdrawals_root", BLANK_ROOT_HASH
+
 
 def _calculate_expected_base_fee_per_gas(parent_block) -> int:
     """py-evm logic for calculating the base fee from parent header"""
     parent_base_fee_per_gas = parent_block["base_fee_per_gas"]
 
     parent_gas_target = parent_block["gas_limit"] // BLOCK_ELASTICITY_MULTIPLIER
     parent_gas_used = parent_block["gas_used"]
```

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/mock/main.py` & `eth-tester-0.9.0b1/eth_tester/backends/mock/main.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/mock/serializers.py` & `eth-tester-0.9.0b1/eth_tester/backends/mock/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,21 @@
 def serialize_block(block, transaction_serializer, is_pending):
     serialized_transactions = tuple(
         transaction_serializer(
             transaction, block, transaction_index, is_pending=is_pending
         )
         for transaction_index, transaction in enumerate(block["transactions"])
     )
-    return assoc(block, "transactions", serialized_transactions)
+    block_with_transactions = assoc(block, "transactions", serialized_transactions)
+    block_with_withdrawals = assoc(
+        block_with_transactions,
+        "withdrawals",
+        block["withdrawals"],
+    )
+    return block_with_withdrawals
 
 
 def serialize_transaction_as_hash(transaction, block, transaction_index, is_pending):
     return transaction["hash"]
 
 
 def serialize_full_transaction(transaction, block, transaction_index, is_pending):
```

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/pyevm/main.py` & `eth-tester-0.9.0b1/eth_tester/backends/pyevm/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import absolute_import
 
 import os
 import time
+from typing import Dict, List, Union
 
 from eth_abi import abi
 from eth_abi.exceptions import DecodingError
 
 from eth_account.hdaccount import HDPath, seed_from_mnemonic
 
 from eth_utils import (
     encode_hex,
     int_to_big_endian,
+    to_bytes,
+    to_checksum_address,
     to_dict,
     to_tuple,
     to_wei,
     is_integer,
 )
 
 from eth_utils.decorators import replace_exceptions
@@ -39,38 +42,46 @@
 
 from .serializers import (
     serialize_block,
     serialize_transaction,
     serialize_transaction_receipt,
 )
 from .utils import is_supported_pyevm_version_available
+from ...validation.inbound import validate_inbound_withdrawals
+
 
 if is_supported_pyevm_version_available():
     from eth.constants import (
         GENESIS_PARENT_HASH,
         POST_MERGE_DIFFICULTY,
         POST_MERGE_MIX_HASH,
         POST_MERGE_NONCE,
     )
     from eth.exceptions import (
         HeaderNotFound as EVMHeaderNotFound,
         InvalidInstruction as EVMInvalidInstruction,
         Revert as EVMRevert,
     )
-    from eth.vm.forks import ParisVM
+    from eth.vm.forks import (
+        ParisVM,
+        ShanghaiVM,
+    )
     from eth.vm.spoof import SpoofTransaction as EVMSpoofTransaction
+    from eth.vm.forks.shanghai.withdrawals import Withdrawal
 else:
     EVMHeaderNotFound = None
     EVMInvalidInstruction = None
     EVMRevert = None
     GENESIS_PARENT_HASH = None
     ParisVM = None
     POST_MERGE_DIFFICULTY = None
     POST_MERGE_MIX_HASH = None
     POST_MERGE_NONCE = None
+    ShanghaiVM = None
+    Withdrawal = None
 
 
 ZERO_ADDRESS = 20 * b"\x00"
 ZERO_HASH32 = 32 * b"\x00"
 EIP838_SIG = b"\x08\xc3y\xa0"
 
 EMPTY_RLP_LIST_HASH = b"\x1d\xccM\xe8\xde\xc7]z\xab\x85\xb5g\xb6\xcc\xd4\x1a\xd3\x12E\x1b\x94\x8at\x13\xf0\xa1B\xfd@\xd4\x93G"  # noqa: E501
@@ -177,15 +188,15 @@
     from eth.consensus import (
         NoProofConsensus,
         ConsensusApplier,
     )
     from eth.db import get_db_backend
 
     if vm_configuration is None:
-        vm_config = ((0, ParisVM),)
+        vm_config = ((0, ShanghaiVM),)
     else:
         if len(vm_configuration) > 0:
             _genesis_block_num, genesis_vm = vm_configuration[0]
             if not issubclass(genesis_vm, ParisVM):
                 genesis_is_post_merge = False
         consensus_applier = ConsensusApplier(NoProofConsensus)
         vm_config = consensus_applier.amend_vm_configuration(vm_configuration)
@@ -654,14 +665,42 @@
     def send_transaction(self, transaction):
         signed_evm_transaction = self._get_normalized_and_signed_evm_transaction(
             transaction,
         )
         self.chain.apply_transaction(signed_evm_transaction)
         return signed_evm_transaction.hash
 
+    def apply_withdrawals(
+        self,
+        withdrawals_list: List[Dict[str, Union[int, str]]],
+    ) -> None:
+        """
+        Apply withdrawals to the state and mine the block that includes the withdrawals.
+        """
+        validate_inbound_withdrawals(withdrawals_list)
+
+        vm = _get_vm_for_block_number(self.chain, "latest")
+        if not isinstance(vm, ShanghaiVM):
+            raise ValidationError(
+                "Withdrawals are only supported after the Shanghai fork"
+            )
+
+        withdrawals = [
+            Withdrawal(
+                index=withdrawal_dict["index"],
+                validator_index=withdrawal_dict["validator_index"],
+                address=to_bytes(
+                    hexstr=to_checksum_address(withdrawal_dict["address"])
+                ),
+                amount=withdrawal_dict["amount"],
+            )
+            for withdrawal_dict in withdrawals_list
+        ]
+        self.chain.mine_all(transactions=[], withdrawals=withdrawals)
+
     def _max_available_gas(self):
         header = self.chain.get_block().header
         return header.gas_limit - header.gas_used
 
     @replace_exceptions(
         {EVMInvalidInstruction: TransactionFailed, EVMRevert: TransactionFailed}
     )
```

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/pyevm/serializers.py` & `eth-tester-0.9.0b1/eth_tester/backends/pyevm/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from .utils import is_supported_pyevm_version_available
 
 
 if is_supported_pyevm_version_available():
     from eth.rlp.transactions import BaseTransaction
     from eth.vm.forks.berlin.transactions import TypedTransaction
-    from eth.vm.forks.london.blocks import LondonBlock
 else:
     BaseTransaction = None
     TypedTransaction = None
 
 from eth_tester.exceptions import ValidationError
 from eth_tester.utils.address import (
     generate_contract_address,
@@ -63,20 +62,22 @@
         "gas_limit": block.header.gas_limit,
         "gas_used": block.header.gas_used,
         "timestamp": block.header.timestamp,
         "transactions": transactions,
         "uncles": [uncle.hash for uncle in block.uncles],
     }
 
-    # blocks after London should inherit from LondonBlock,
-    # so this should also work for future hard forks
-    if isinstance(block, LondonBlock):
+    if hasattr(block.header, "base_fee_per_gas"):
         base_fee = block.header.base_fee_per_gas
         block_info.update({"base_fee_per_gas": base_fee})
 
+    if hasattr(block.header, "withdrawals_root") and hasattr(block, "withdrawals"):
+        block_info.update({"withdrawals": serialize_block_withdrawals(block)})
+        block_info.update({"withdrawals_root": block.header.withdrawals_root})
+
     return block_info
 
 
 def serialize_transaction_hash(block, transaction, transaction_index, is_pending):
     return transaction.hash
 
 
@@ -136,15 +137,15 @@
         raise ValidationError("Invariant: code path should be unreachable")
 
     return merge(common_transaction_params, type_specific_params)
 
 
 def _field_in_transaction(transaction, field):
     """
-    There are many different classes of transactions, we have to be able to search for a
+    There are many classes of transactions, we have to be able to search for a
     particular field depending on the type of transaction - from dict, to legacy
     transaction classes, to *TypedTransaction classes.
     """
     if isinstance(transaction, dict):
         return field in transaction
     elif isinstance(transaction, BaseTransaction):
         # all legacy transactions inherit from BaseTransaction
@@ -229,7 +230,19 @@
         min(
             transaction.max_fee_per_gas,
             transaction.max_priority_fee_per_gas + block.header.base_fee_per_gas,
         )
         if transaction_type == "0x2"
         else transaction.gas_price
     )
+
+
+def serialize_block_withdrawals(block):
+    return [
+        {
+            "index": withdrawal.index,
+            "validator_index": withdrawal.validator_index,
+            "address": withdrawal.address,
+            "amount": withdrawal.amount,
+        }
+        for withdrawal in block.withdrawals
+    ]
```

### Comparing `eth-tester-0.8.0b3/eth_tester/backends/pyevm/utils.py` & `eth-tester-0.9.0b1/eth_tester/backends/pyevm/utils.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/constants.py` & `eth-tester-0.9.0b1/eth_tester/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import unicode_literals
 
 
 UINT256_MIN = 0
 UINT256_MAX = 2**256 - 1
+UINT64_MAX = 2**64 - 1
 UINT8_MAX = 2**8 - 1
 UINT2048_MAX = 2**2048 - 1
 
 
 ZERO_ADDRESS_HEX = "0x0000000000000000000000000000000000000000"
 BURN_ADDRESS = "0xdead000000000000000000000000000000000000"
```

### Comparing `eth-tester-0.8.0b3/eth_tester/main.py` & `eth-tester-0.9.0b1/eth_tester/main.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/normalization/__init__.py` & `eth-tester-0.9.0b1/eth_tester/normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/normalization/base.py` & `eth-tester-0.9.0b1/eth_tester/normalization/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/normalization/common.py` & `eth-tester-0.9.0b1/eth_tester/normalization/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         yield key, normalizer(item)
 
 
 @curry
 @to_tuple
 def normalize_array(value, normalizer):
     """
-    This is just `map` but it's nice to have it return a consisten type
+    This is just `map` but it's nice to have it return a consistent type
     (tuple).
     """
     for item in value:
         yield normalizer(item)
 
 
 @curry
```

### Comparing `eth-tester-0.8.0b3/eth_tester/normalization/default.py` & `eth-tester-0.9.0b1/eth_tester/normalization/default.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/normalization/inbound.py` & `eth-tester-0.9.0b1/eth_tester/normalization/inbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/normalization/outbound.py` & `eth-tester-0.9.0b1/eth_tester/normalization/outbound.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,29 +71,41 @@
     "r": identity,
     "s": identity,
     "v": identity,
 }
 normalize_transaction = partial(normalize_dict, normalizers=TRANSACTION_NORMALIZERS)
 
 
+WITHDRAWAL_NORMALIZERS = {
+    "index": identity,
+    "validator_index": identity,
+    "address": to_checksum_address,
+    "amount": identity,
+}
+normalize_withdrawal = partial(normalize_dict, normalizers=WITHDRAWAL_NORMALIZERS)
+
+
 def is_transaction_hash_list(value):
     return all(is_bytes(item) for item in value)
 
 
 def is_transaction_object_list(value):
     return all(is_dict(item) for item in value)
 
 
-def _remove_base_fee_if_none(block):
+def _remove_fork_specific_fields_if_none(block):
     """
-    A `None` value is set for `base_fee_per_gas` during validation for blocks that do
-    not have a base fee (pre-London blocks). Pop this value out here to normalize
-    pre-London blocks.
+    A `None` value is set for keys if they are not present during outbound block
+    validation. This means we are in a VM that has not yet been exposed to this new
+    field. Pop this value out here to normalize these older VM blocks.
     """
-    return block if block["base_fee_per_gas"] else dissoc(block, "base_fee_per_gas")
+    for key, value in list(block.items()):
+        if value is None:
+            block = dissoc(block, key)
+    return block
 
 
 BLOCK_NORMALIZERS = {
     "number": identity,
     "hash": encode_hex,
     "parent_hash": encode_hex,
     "nonce": encode_hex,
@@ -121,17 +133,20 @@
         partial(
             normalize_if,
             conditional_fn=is_transaction_object_list,
             normalizer=partial(normalize_array, normalizer=normalize_transaction),
         ),
     ),
     "uncles": partial(normalize_array, normalizer=encode_hex),
+    "withdrawals": partial(normalize_array, normalizer=normalize_withdrawal),
+    "withdrawals_root": encode_hex,
 }
 normalize_block = compose(
-    _remove_base_fee_if_none, partial(normalize_dict, normalizers=BLOCK_NORMALIZERS)
+    partial(normalize_dict, normalizers=BLOCK_NORMALIZERS),
+    _remove_fork_specific_fields_if_none,
 )
 
 
 LOG_ENTRY_NORMALIZERS = {
     "type": identity,
     "log_index": identity,
     "transaction_index": partial(
@@ -172,9 +187,10 @@
         normalizer=to_checksum_address,
     ),
     "logs": partial(normalize_array, normalizer=normalize_log_entry),
     "state_root": identity,
     "status": identity,
     "to": to_empty_or_checksum_address,
     "type": identity,
+    "base_fee_per_gas": identity,
 }
 normalize_receipt = partial(normalize_dict, normalizers=RECEIPT_NORMALIZERS)
```

### Comparing `eth-tester-0.8.0b3/eth_tester/tools/gas_burner_contract.py` & `eth-tester-0.9.0b1/eth_tester/tools/gas_burner_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/backend_testing.py` & `eth-tester-0.9.0b1/eth_tester/utils/backend_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
     "size",
     "extra_data",
     "gas_limit",
     "gas_used",
     "timestamp",
     "transactions",
     "uncles",
-    "base_fee_per_gas",
 }
 
 
 def _validate_serialized_block(block):
     missing_keys = BLOCK_KEYS.difference(block.keys())
     if missing_keys:
         error_message = "Serialized block is missing the following keys: {}".format(
```

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/emitter_contract.py` & `eth-tester-0.9.0b1/eth_tester/utils/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/filters.py` & `eth-tester-0.9.0b1/eth_tester/utils/filters.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/math_contract.py` & `eth-tester-0.9.0b1/eth_tester/utils/math_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/module_loading.py` & `eth-tester-0.9.0b1/eth_tester/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/throws_contract.py` & `eth-tester-0.9.0b1/eth_tester/utils/throws_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/utils/transactions.py` & `eth-tester-0.9.0b1/eth_tester/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/validation/__init__.py` & `eth-tester-0.9.0b1/eth_tester/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/validation/base.py` & `eth-tester-0.9.0b1/eth_tester/validation/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/validation/common.py` & `eth-tester-0.9.0b1/eth_tester/validation/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from __future__ import unicode_literals
 
 import math
 
 import functools
+from typing import (
+    Union,
+)
 
+from eth_typing import (
+    HexStr,
+)
 from eth_utils import (
+    is_address,
     is_bytes,
     is_hexstr,
     is_text,
     is_dict,
     is_integer,
     is_list_like,
     to_dict,
@@ -17,14 +24,15 @@
 
 from eth_utils.toolz import (
     curry,
 )
 
 from eth_tester.constants import (
     UINT256_MAX,
+    UINT64_MAX,
     UINT8_MAX,
 )
 from eth_tester.exceptions import (
     ValidationError,
 )
 
 
@@ -45,14 +53,15 @@
         bitsize = int(math.log2(max_val))
         raise ValidationError(
             f"Value exceeds maximum {bitsize:d} bit integer size:  {value}"
         )
 
 
 validate_uint256 = validate_uint(UINT256_MAX)
+validate_uint64 = validate_uint(UINT64_MAX)
 validate_uint8 = validate_uint(UINT8_MAX)
 
 
 def validate_bytes(value):
     if not is_bytes(value):
         raise ValidationError(
             "Value must be a byte string.  Got type: {}".format(type(value))
@@ -199,7 +208,12 @@
 def if_not_create_address(validator_fn):
     @functools.wraps(validator_fn)
     def inner(value):
         if value != b"":
             validator_fn(value)
 
     return inner
+
+
+def validate_address(value: Union[str, HexStr, bytes]):
+    if not is_address(value):
+        raise ValidationError(f"Value must be a valid address. Got: {value}")
```

### Comparing `eth-tester-0.8.0b3/eth_tester/validation/default.py` & `eth-tester-0.9.0b1/eth_tester/validation/default.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester/validation/inbound.py` & `eth-tester-0.9.0b1/eth_tester/validation/inbound.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from __future__ import unicode_literals
 
 import binascii
+from typing import (
+    Dict,
+    List,
+    Union,
+)
 
+from eth_typing import HexStr
 from eth_utils import (
     is_boolean,
     is_checksum_address,
     is_checksum_formatted_address,
     is_dict,
     is_hex,
     is_hex_address,
@@ -25,17 +31,20 @@
     BLOCK_NUMBER_META_VALUES,
 )
 from eth_tester.exceptions import (
     ValidationError,
 )
 
 from .common import (
+    validate_address,
+    validate_dict,
     validate_positive_integer,
     validate_transaction_type,
     validate_uint256,
+    validate_uint64,
     validate_uint8,
     validate_text,
 )
 
 
 def is_32byte_hex_string(value):
     return is_text(value) and is_hex(value) and len(remove_0x_prefix(value)) == 64
@@ -335,7 +344,25 @@
 
 def validate_raw_transaction(raw_transaction):
     if not is_text(raw_transaction) or not is_hex(raw_transaction):
         raise ValidationError(
             "Raw Transaction must be a hexadecimal encoded string.  Got: "
             "{}".format(raw_transaction)
         )
+
+
+INBOUND_WITHDRAWAL_VALIDATORS = {
+    "index": validate_uint64,
+    "validator_index": validate_uint64,
+    "address": validate_address,
+    "amount": validate_uint64,
+}
+
+
+def validate_inbound_withdrawals(
+    withdrawals_list: List[Dict[str, Union[int, str, HexStr, bytes]]],
+):
+    if len(withdrawals_list) == 0:
+        raise ValidationError("Withdrawals list must not be empty.")
+
+    for withdrawal_dict in withdrawals_list:
+        validate_dict(withdrawal_dict, key_validators=INBOUND_WITHDRAWAL_VALIDATORS)
```

### Comparing `eth-tester-0.8.0b3/eth_tester/validation/outbound.py` & `eth-tester-0.9.0b1/eth_tester/validation/outbound.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     validate_any,
     validate_array,
     validate_bytes,
     validate_positive_integer,
     validate_dict,
     validate_transaction_type,
     validate_uint256,
+    validate_uint64,
 )
 
 
 def validate_32_byte_string(value):
     validate_bytes(value)
     if len(value) != 32:
         raise ValidationError(
@@ -180,14 +181,23 @@
         partial(validate_dict, key_validators=LEGACY_TRANSACTION_VALIDATORS),
         partial(validate_dict, key_validators=ACCESS_LIST_TRANSACTION_VALIDATORS),
         partial(validate_dict, key_validators=DYNAMIC_FEE_TRANSACTION_VALIDATORS),
     ),
 )
 
 
+WITHDRAWAL_VALIDATORS = {
+    "index": validate_uint64,
+    "validator_index": validate_uint64,
+    "address": validate_canonical_address,
+    "amount": validate_uint64,
+}
+validate_withdrawal = partial(validate_dict, key_validators=WITHDRAWAL_VALIDATORS)
+
+
 def validate_status(value):
     validate_positive_integer(value)
     if value > 1:
         raise ValidationError(f"Invalid status value '{value}', only 0 or 1 allowed.")
 
 
 RECEIPT_VALIDATORS = {
@@ -207,15 +217,14 @@
     "type": validate_transaction_type,
 }
 validate_receipt = partial(validate_dict, key_validators=RECEIPT_VALIDATORS)
 
 
 BLOCK_VALIDATORS = {
     "number": validate_positive_integer,
-    "base_fee_per_gas": identity,  # validated separately via _validate_base_fee()
     "hash": validate_block_hash,
     "parent_hash": validate_block_hash,
     "nonce": validate_nonce,
     "sha3_uncles": validate_32_byte_string,
     "logs_bloom": validate_logs_bloom,
     "transactions_root": validate_32_byte_string,
     "receipts_root": validate_32_byte_string,
@@ -235,30 +244,44 @@
             partial(validate_array, validator=validate_32_byte_string),
             partial(validate_array, validator=validate_legacy_transaction),
             partial(validate_array, validator=validate_access_list_transaction),
             partial(validate_array, validator=validate_dynamic_fee_transaction),
         ),
     ),
     "uncles": partial(validate_array, validator=validate_32_byte_string),
+    # fork-specific fields, validated separately in `_validate_fork_specific_fields()`
+    "base_fee_per_gas": identity,
+    "withdrawals": identity,
+    "withdrawals_root": identity,
 }
 
 
-def _validate_base_fee(block):
+def _validate_fork_specific_fields(block):
     """
-    If `base_fee_per_gas` is present (post-London blocks), validate that the value is a
-    positive integer. For pre-London blocks, set to `None` during validation and pop it
-    back out during normalization.
+    If a fork-specific key is present, validate the value appropriately. For
+    blocks that are missing this key (before it was introduced via a fork), set the
+    value to `None` during validation and pop it back out during normalization.
     """
+    # London fork
     if "base_fee_per_gas" not in block:
         block["base_fee_per_gas"] = None
     else:
         validate_positive_integer(block["base_fee_per_gas"])
+
+    # Shanghai fork
+    if all(_ not in block for _ in ("withdrawals", "withdrawals_root")):
+        block["withdrawals"] = None
+        block["withdrawals_root"] = None
+    else:
+        partial(validate_array, validator=validate_withdrawal)(block["withdrawals"])
+        validate_32_byte_string(block["withdrawals_root"])
+
     return block
 
 
 validate_block = compose(
     partial(validate_dict, key_validators=BLOCK_VALIDATORS),
-    _validate_base_fee,
+    _validate_fork_specific_fields,
 )
 
 
 validate_accounts = partial(validate_array, validator=validate_canonical_address)
```

### Comparing `eth-tester-0.8.0b3/eth_tester.egg-info/PKG-INFO` & `eth-tester-0.9.0b1/eth_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.8.0b3
+Version: 0.9.0b1
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -193,15 +192,15 @@
 # Documentation
 
 ## Input and output data formats
 
 The ethereum tester library strictly enforces the following input formats and
 types.
 
-* Hexidecimal values **must** be text (not byte) strings.  The `0x` prefix is optional.
+* Hexadecimal values **must** be text (not byte) strings.  The `0x` prefix is optional.
 * Any address which contains mixed-case alpha characters will be validated as a checksummed address as specified by [EIP-55](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-55.md)
 * 32-byte hashes **must** be hexadecimal encoded.
 * Numeric values **must** be in their integer representation.
 
 Similarly, ethereum tester ensures that return values conform to similar rules.
 
 * 32-byte hashes will be returned in their hexadecimal encoded representation.
@@ -717,15 +716,15 @@
 
 See [the filtering guide](#guide-filtering) for detailed information on how to use filters.
 
 <a id="api-delete_filter"></a>
 
 #### `EthereumTester.delete_filter(filter_id)`
 
-Removes the filter for the provide `filter_id`.  If no filter is found for the
+Removes the filter for the provided `filter_id`.  If no filter is found for the
 given `filter_id`, raises [`FilterNotFound`](#errors-FilterNotFound).
 
 
 <a id="api-get_only_filter_changes"></a>
 
 #### `EthereumTester.get_only_filter_changes(filter_id) -> transaction_hash or block_hash or log_entry`
 
@@ -753,15 +752,15 @@
 
 
 <a id="api-revert_to_snapshot"></a>
 
 #### `EthereumTester.revert_to_snapshot(snapshot_id)`
 
 Reverts the chain to the chain state associated with the given `snapshot_id`.
-Raises [`SnapshotNotFound`](#errors-SnapshotNotFound) if no snapshot is know
+Raises [`SnapshotNotFound`](#errors-SnapshotNotFound) if no snapshot is known
 for the given id.
 
 ### Errors and Exceptions
 
 <a id="errors-TransactionNotFound"></a>
 
 #### `eth_tester.exceptions.TransactionNotFound`
@@ -887,15 +886,15 @@
 
 # Generates the following `dict`:
 
 # custom_genesis_params = {
 #     "coinbase": GENESIS_COINBASE,
 #     "difficulty": GENESIS_DIFFICULTY,
 #     "extra_data": GENESIS_EXTRA_DATA,
-#     "gas_limit": 4500000    # <<< Overidden Value <<<
+#     "gas_limit": 4500000    # <<< Overridden Value <<<
 #     "mix_hash": GENESIS_MIX_HASH,
 #     "nonce": GENESIS_NONCE,
 #     "receipt_root": BLANK_ROOT_HASH,
 #     "timestamp": int(time.time()),
 #     "transaction_root": BLANK_ROOT_HASH,
 # }
 ```
@@ -997,15 +996,15 @@
 ## Normalization and Validation
 
 > Beware! Here there be dragons...  This section of the documentation is only
 > relevant if you intend to build tooling on top of this library.
 
 The ethereum tester provides strong guarantees that backends can be swapped out
 seamlessly without effecting the data formats of both the input arguments and
-return values.  This is accomplished using a two step process of strict
+return values.  This is accomplished using a two-step process of strict
 *normalization* and *validation*.
 
 All inputs to the methods of the `EthereumTester` are first validated then
 normalized to a *canonical* format.  Return values are put through this process
 as well, first validating the data returned by the backend, and then
 normalizing it from the *canonical* format to the *normal* form before being
 returned.
@@ -1033,9 +1032,7 @@
 
 
 # Use with Web3.py
 
 See the [web3.py documentation](http://web3py.readthedocs.io/en/latest/) for
 information on the `EthereumTester` provider which integrates with this
 library.
-
-
```

### Comparing `eth-tester-0.8.0b3/eth_tester.egg-info/SOURCES.txt` & `eth-tester-0.9.0b1/eth_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/eth_tester.egg-info/requires.txt` & `eth-tester-0.9.0b1/eth_tester.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [dev]
 bumpversion<1.0.0,>=0.5.3
 tox<3.0.0,>=2.9.1
 wheel<1.0.0,>=0.30.0
 pytest<7,>=6.2.5
 pytest-xdist<3,>=2.0.0
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
-py-evm==0.6.1a2
+py-evm==0.7.0a2
 black<23,>=22
 flake8<4.0.0,>=3.5.0
 towncrier<22,>=21
 
 [dev:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
@@ -27,24 +27,24 @@
 towncrier<22,>=21
 
 [lint]
 black<23,>=22
 flake8<4.0.0,>=3.5.0
 
 [py-evm]
-py-evm==0.6.1a2
+py-evm==0.7.0a2
 
 [py-evm:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
 [py-evm:implementation_name == "pypy"]
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
 
 [pyevm]
-py-evm==0.6.1a2
+py-evm==0.7.0a2
 
 [pyevm:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
 [pyevm:implementation_name == "pypy"]
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
```

### Comparing `eth-tester-0.8.0b3/pyproject.toml` & `eth-tester-0.9.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-tester-0.8.0b3/setup.py` & `eth-tester-0.9.0b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "bumpversion>=0.5.3,<1.0.0",
         "tox>=2.9.1,<3.0.0",
         "wheel>=0.30.0,<1.0.0",
     ],
     "py-evm": [
         # Pin py-evm to exact version, until it leaves alpha.
         # EVM is very high velocity and might change API at each alpha.
-        "py-evm==0.6.1a2",
+        "py-evm==0.7.0a2",
         "eth-hash[pysha3]>=0.1.4,<1.0.0;implementation_name=='cpython'",
         "eth-hash[pycryptodome]>=0.1.4,<1.0.0;implementation_name=='pypy'",
     ],
     "docs": [
         "towncrier>=21,<22",
     ],
 }
@@ -45,15 +45,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="eth-tester",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.8.0-beta.3",
+    version="0.9.0-beta.1",
     description="""Tools for testing Ethereum applications.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/eth-tester",
     include_package_data=True,
```


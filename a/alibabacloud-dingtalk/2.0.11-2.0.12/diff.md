# Comparing `tmp/alibabacloud_dingtalk-2.0.11.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.11.tar", last modified: Tue May  9 01:56:59 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.12.tar", last modified: Fri May 12 10:18:21 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.11.tar` & `alibabacloud_dingtalk-2.0.12.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/
--rw-r--r--   0 root         (0) root         (0)    19362 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148888 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   274109 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   565599 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138548 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   328853 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   308062 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   429056 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89334 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133902 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87266 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130480 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129226 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157569 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260594 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   414815 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44880 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81308 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   147980 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53454 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118368 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175082 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   370377 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   459526 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   682489 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11743 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/
+-rw-r--r--   0 root         (0) root         (0)    19427 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   153926 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   284895 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   565599 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138548 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   328853 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220322 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   547684 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   523174 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   756557 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129226 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157569 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44880 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81308 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   147980 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53454 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118368 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175082 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   370377 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11743 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.11/ChangeLog.md` & `alibabacloud_dingtalk-2.0.12/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-09 Version: 2.0.11
+- Update AddOfficialAccountFollower.
+
 2023-04-28 Version: 2.0.10
 - Update AddOfficialAccountFollower.
 
 2023-04-26 Version: 2.0.0
 - Update AddOfficialAccountFollower.
 
 2023-04-26 Version: 2.0.0
```

### Comparing `alibabacloud_dingtalk-2.0.11/LICENSE` & `alibabacloud_dingtalk-2.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/PKG-INFO` & `alibabacloud_dingtalk-2.0.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.11
+Version: 2.0.12
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.11/README-CN.md` & `alibabacloud_dingtalk-2.0.12/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/README.md` & `alibabacloud_dingtalk-2.0.12/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1213,14 +1213,120 @@
         self,
         request: dingtalkattendance__1__0_models.GetCheckInSchemaTemplateRequest,
     ) -> dingtalkattendance__1__0_models.GetCheckInSchemaTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkattendance__1__0_models.GetCheckInSchemaTemplateHeaders()
         return await self.get_check_in_schema_template_with_options_async(request, headers, runtime)
 
+    def get_checkin_record_by_user_with_options(
+        self,
+        request: dingtalkattendance__1__0_models.GetCheckinRecordByUserRequest,
+        headers: dingtalkattendance__1__0_models.GetCheckinRecordByUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.GetCheckinRecordByUserResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.operator_user_id):
+            body['operatorUserId'] = request.operator_user_id
+        if not UtilClient.is_unset(request.start_time):
+            body['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.user_id_list):
+            body['userIdList'] = request.user_id_list
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetCheckinRecordByUser',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/checkin/records/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.GetCheckinRecordByUserResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_checkin_record_by_user_with_options_async(
+        self,
+        request: dingtalkattendance__1__0_models.GetCheckinRecordByUserRequest,
+        headers: dingtalkattendance__1__0_models.GetCheckinRecordByUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.GetCheckinRecordByUserResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.operator_user_id):
+            body['operatorUserId'] = request.operator_user_id
+        if not UtilClient.is_unset(request.start_time):
+            body['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.user_id_list):
+            body['userIdList'] = request.user_id_list
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetCheckinRecordByUser',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/checkin/records/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.GetCheckinRecordByUserResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_checkin_record_by_user(
+        self,
+        request: dingtalkattendance__1__0_models.GetCheckinRecordByUserRequest,
+    ) -> dingtalkattendance__1__0_models.GetCheckinRecordByUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.GetCheckinRecordByUserHeaders()
+        return self.get_checkin_record_by_user_with_options(request, headers, runtime)
+
+    async def get_checkin_record_by_user_async(
+        self,
+        request: dingtalkattendance__1__0_models.GetCheckinRecordByUserRequest,
+    ) -> dingtalkattendance__1__0_models.GetCheckinRecordByUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.GetCheckinRecordByUserHeaders()
+        return await self.get_checkin_record_by_user_with_options_async(request, headers, runtime)
+
     def get_closing_accounts_with_options(
         self,
         request: dingtalkattendance__1__0_models.GetClosingAccountsRequest,
         headers: dingtalkattendance__1__0_models.GetClosingAccountsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkattendance__1__0_models.GetClosingAccountsResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3011,14 +3011,346 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetCheckInSchemaTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetCheckinRecordByUserHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetCheckinRecordByUserRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        max_results: int = None,
+        next_token: int = None,
+        operator_user_id: str = None,
+        start_time: int = None,
+        user_id_list: List[str] = None,
+    ):
+        self.end_time = end_time
+        self.max_results = max_results
+        self.next_token = next_token
+        self.operator_user_id = operator_user_id
+        self.start_time = start_time
+        self.user_id_list = user_id_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.operator_user_id is not None:
+            result['operatorUserId'] = self.operator_user_id
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.user_id_list is not None:
+            result['userIdList'] = self.user_id_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('operatorUserId') is not None:
+            self.operator_user_id = m.get('operatorUserId')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('userIdList') is not None:
+            self.user_id_list = m.get('userIdList')
+        return self
+
+
+class GetCheckinRecordByUserResponseBodyResultPageListCustomDataList(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        label: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.label = label
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['key'] = self.key
+        if self.label is not None:
+            result['label'] = self.label
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('label') is not None:
+            self.label = m.get('label')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class GetCheckinRecordByUserResponseBodyResultPageList(TeaModel):
+    def __init__(
+        self,
+        checkin_time: int = None,
+        custom_data_list: List[GetCheckinRecordByUserResponseBodyResultPageListCustomDataList] = None,
+        detail_place: str = None,
+        image_list: List[str] = None,
+        latitude: str = None,
+        longitude: str = None,
+        place: str = None,
+        remark: str = None,
+        user_id: str = None,
+        visit_user: str = None,
+    ):
+        self.checkin_time = checkin_time
+        self.custom_data_list = custom_data_list
+        self.detail_place = detail_place
+        self.image_list = image_list
+        self.latitude = latitude
+        self.longitude = longitude
+        self.place = place
+        self.remark = remark
+        self.user_id = user_id
+        self.visit_user = visit_user
+
+    def validate(self):
+        if self.custom_data_list:
+            for k in self.custom_data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.checkin_time is not None:
+            result['checkinTime'] = self.checkin_time
+        result['customDataList'] = []
+        if self.custom_data_list is not None:
+            for k in self.custom_data_list:
+                result['customDataList'].append(k.to_map() if k else None)
+        if self.detail_place is not None:
+            result['detailPlace'] = self.detail_place
+        if self.image_list is not None:
+            result['imageList'] = self.image_list
+        if self.latitude is not None:
+            result['latitude'] = self.latitude
+        if self.longitude is not None:
+            result['longitude'] = self.longitude
+        if self.place is not None:
+            result['place'] = self.place
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.visit_user is not None:
+            result['visitUser'] = self.visit_user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('checkinTime') is not None:
+            self.checkin_time = m.get('checkinTime')
+        self.custom_data_list = []
+        if m.get('customDataList') is not None:
+            for k in m.get('customDataList'):
+                temp_model = GetCheckinRecordByUserResponseBodyResultPageListCustomDataList()
+                self.custom_data_list.append(temp_model.from_map(k))
+        if m.get('detailPlace') is not None:
+            self.detail_place = m.get('detailPlace')
+        if m.get('imageList') is not None:
+            self.image_list = m.get('imageList')
+        if m.get('latitude') is not None:
+            self.latitude = m.get('latitude')
+        if m.get('longitude') is not None:
+            self.longitude = m.get('longitude')
+        if m.get('place') is not None:
+            self.place = m.get('place')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('visitUser') is not None:
+            self.visit_user = m.get('visitUser')
+        return self
+
+
+class GetCheckinRecordByUserResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        next_token: int = None,
+        page_list: List[GetCheckinRecordByUserResponseBodyResultPageList] = None,
+    ):
+        self.next_token = next_token
+        self.page_list = page_list
+
+    def validate(self):
+        if self.page_list:
+            for k in self.page_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        result['pageList'] = []
+        if self.page_list is not None:
+            for k in self.page_list:
+                result['pageList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        self.page_list = []
+        if m.get('pageList') is not None:
+            for k in m.get('pageList'):
+                temp_model = GetCheckinRecordByUserResponseBodyResultPageList()
+                self.page_list.append(temp_model.from_map(k))
+        return self
+
+
+class GetCheckinRecordByUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: GetCheckinRecordByUserResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = GetCheckinRecordByUserResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class GetCheckinRecordByUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetCheckinRecordByUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetCheckinRecordByUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetClosingAccountsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5667,14 +5667,112 @@
         self,
         request: dingtalkexclusive__1__0_models.SaveAndSubmitAuthInfoRequest,
     ) -> dingtalkexclusive__1__0_models.SaveAndSubmitAuthInfoResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.SaveAndSubmitAuthInfoHeaders()
         return await self.save_and_submit_auth_info_with_options_async(request, headers, runtime)
 
+    def save_open_terminal_info_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.SaveOpenTerminalInfoRequest,
+        headers: dingtalkexclusive__1__0_models.SaveOpenTerminalInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.SaveOpenTerminalInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.log_source):
+            body['logSource'] = request.log_source
+        if not UtilClient.is_unset(request.log_type):
+            body['logType'] = request.log_type
+        if not UtilClient.is_unset(request.open_ext):
+            body['openExt'] = request.open_ext
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SaveOpenTerminalInfo',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/externalLogs/terminalInfos/save',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.SaveOpenTerminalInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def save_open_terminal_info_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.SaveOpenTerminalInfoRequest,
+        headers: dingtalkexclusive__1__0_models.SaveOpenTerminalInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.SaveOpenTerminalInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.log_source):
+            body['logSource'] = request.log_source
+        if not UtilClient.is_unset(request.log_type):
+            body['logType'] = request.log_type
+        if not UtilClient.is_unset(request.open_ext):
+            body['openExt'] = request.open_ext
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SaveOpenTerminalInfo',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/externalLogs/terminalInfos/save',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.SaveOpenTerminalInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def save_open_terminal_info(
+        self,
+        request: dingtalkexclusive__1__0_models.SaveOpenTerminalInfoRequest,
+    ) -> dingtalkexclusive__1__0_models.SaveOpenTerminalInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.SaveOpenTerminalInfoHeaders()
+        return self.save_open_terminal_info_with_options(request, headers, runtime)
+
+    async def save_open_terminal_info_async(
+        self,
+        request: dingtalkexclusive__1__0_models.SaveOpenTerminalInfoRequest,
+    ) -> dingtalkexclusive__1__0_models.SaveOpenTerminalInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.SaveOpenTerminalInfoHeaders()
+        return await self.save_open_terminal_info_with_options_async(request, headers, runtime)
+
     def save_white_app_with_options(
         self,
         request: dingtalkexclusive__1__0_models.SaveWhiteAppRequest,
         headers: dingtalkexclusive__1__0_models.SaveWhiteAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkexclusive__1__0_models.SaveWhiteAppResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12027,14 +12027,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SaveAndSubmitAuthInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SaveOpenTerminalInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SaveOpenTerminalInfoRequest(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        log_source: str = None,
+        log_type: str = None,
+        open_ext: str = None,
+    ):
+        self.corp_id = corp_id
+        self.log_source = log_source
+        self.log_type = log_type
+        self.open_ext = open_ext
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.log_source is not None:
+            result['logSource'] = self.log_source
+        if self.log_type is not None:
+            result['logType'] = self.log_type
+        if self.open_ext is not None:
+            result['openExt'] = self.open_ext
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('logSource') is not None:
+            self.log_source = m.get('logSource')
+        if m.get('logType') is not None:
+            self.log_type = m.get('logType')
+        if m.get('openExt') is not None:
+            self.open_ext = m.get('openExt')
+        return self
+
+
+class SaveOpenTerminalInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class SaveOpenTerminalInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SaveOpenTerminalInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SaveOpenTerminalInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SaveWhiteAppHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,100 @@
         self,
         request: dingtalkhrm__1__0_models.ECertQueryRequest,
     ) -> dingtalkhrm__1__0_models.ECertQueryResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkhrm__1__0_models.ECertQueryHeaders()
         return await self.e_cert_query_with_options_async(request, headers, runtime)
 
+    def esign_rollback_with_options(
+        self,
+        request: dingtalkhrm__1__0_models.EsignRollbackRequest,
+        headers: dingtalkhrm__1__0_models.EsignRollbackHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.EsignRollbackResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.opt_user_id):
+            query['optUserId'] = request.opt_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='EsignRollback',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/contracts/esign/rollback',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.EsignRollbackResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def esign_rollback_with_options_async(
+        self,
+        request: dingtalkhrm__1__0_models.EsignRollbackRequest,
+        headers: dingtalkhrm__1__0_models.EsignRollbackHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.EsignRollbackResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.opt_user_id):
+            query['optUserId'] = request.opt_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='EsignRollback',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/contracts/esign/rollback',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.EsignRollbackResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def esign_rollback(
+        self,
+        request: dingtalkhrm__1__0_models.EsignRollbackRequest,
+    ) -> dingtalkhrm__1__0_models.EsignRollbackResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.EsignRollbackHeaders()
+        return self.esign_rollback_with_options(request, headers, runtime)
+
+    async def esign_rollback_async(
+        self,
+        request: dingtalkhrm__1__0_models.EsignRollbackRequest,
+    ) -> dingtalkhrm__1__0_models.EsignRollbackResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.EsignRollbackHeaders()
+        return await self.esign_rollback_with_options_async(request, headers, runtime)
+
     def hrm_process_regular_with_options(
         self,
         request: dingtalkhrm__1__0_models.HrmProcessRegularRequest,
         headers: dingtalkhrm__1__0_models.HrmProcessRegularHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkhrm__1__0_models.HrmProcessRegularResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,14 +499,145 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ECertQueryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class EsignRollbackHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class EsignRollbackRequest(TeaModel):
+    def __init__(
+        self,
+        opt_user_id: str = None,
+    ):
+        self.opt_user_id = opt_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.opt_user_id is not None:
+            result['optUserId'] = self.opt_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('optUserId') is not None:
+            self.opt_user_id = m.get('optUserId')
+        return self
+
+
+class EsignRollbackResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class EsignRollbackResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: EsignRollbackResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = EsignRollbackResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class HrmProcessRegularHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,14 +617,104 @@
         feed_id: str,
         request: dingtalklive__1__0_models.EditFeedReplayRequest,
     ) -> dingtalklive__1__0_models.EditFeedReplayResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalklive__1__0_models.EditFeedReplayHeaders()
         return await self.edit_feed_replay_with_options_async(feed_id, request, headers, runtime)
 
+    def get_live_replay_url_with_options(
+        self,
+        request: dingtalklive__1__0_models.GetLiveReplayUrlRequest,
+        headers: dingtalklive__1__0_models.GetLiveReplayUrlHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalklive__1__0_models.GetLiveReplayUrlResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.live_id):
+            query['liveId'] = request.live_id
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetLiveReplayUrl',
+            version='live_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/live/lives/replayUrls',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalklive__1__0_models.GetLiveReplayUrlResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_live_replay_url_with_options_async(
+        self,
+        request: dingtalklive__1__0_models.GetLiveReplayUrlRequest,
+        headers: dingtalklive__1__0_models.GetLiveReplayUrlHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalklive__1__0_models.GetLiveReplayUrlResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.live_id):
+            query['liveId'] = request.live_id
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetLiveReplayUrl',
+            version='live_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/live/lives/replayUrls',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalklive__1__0_models.GetLiveReplayUrlResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_live_replay_url(
+        self,
+        request: dingtalklive__1__0_models.GetLiveReplayUrlRequest,
+    ) -> dingtalklive__1__0_models.GetLiveReplayUrlResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalklive__1__0_models.GetLiveReplayUrlHeaders()
+        return self.get_live_replay_url_with_options(request, headers, runtime)
+
+    async def get_live_replay_url_async(
+        self,
+        request: dingtalklive__1__0_models.GetLiveReplayUrlRequest,
+    ) -> dingtalklive__1__0_models.GetLiveReplayUrlResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalklive__1__0_models.GetLiveReplayUrlHeaders()
+        return await self.get_live_replay_url_with_options_async(request, headers, runtime)
+
     def get_user_all_live_list_with_options(
         self,
         request: dingtalklive__1__0_models.GetUserAllLiveListRequest,
         headers: dingtalklive__1__0_models.GetUserAllLiveListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalklive__1__0_models.GetUserAllLiveListResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -946,14 +946,180 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EditFeedReplayResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetLiveReplayUrlHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetLiveReplayUrlRequest(TeaModel):
+    def __init__(
+        self,
+        live_id: str = None,
+        union_id: str = None,
+    ):
+        self.live_id = live_id
+        self.union_id = union_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.live_id is not None:
+            result['liveId'] = self.live_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('liveId') is not None:
+            self.live_id = m.get('liveId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class GetLiveReplayUrlResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        replay_url: str = None,
+    ):
+        self.replay_url = replay_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.replay_url is not None:
+            result['replayUrl'] = self.replay_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('replayUrl') is not None:
+            self.replay_url = m.get('replayUrl')
+        return self
+
+
+class GetLiveReplayUrlResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: GetLiveReplayUrlResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = GetLiveReplayUrlResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class GetLiveReplayUrlResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetLiveReplayUrlResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetLiveReplayUrlResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetUserAllLiveListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,20 +729,20 @@
         project_id: str,
         request: dingtalkproject__1__0_models.CreateProjectCustomfieldStatusRequest,
         headers: dingtalkproject__1__0_models.CreateProjectCustomfieldStatusHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.CreateProjectCustomfieldStatusResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.customfield_id):
-            body['customfieldId'] = request.customfield_id
-        if not UtilClient.is_unset(request.customfield_instance_id):
-            body['customfieldInstanceId'] = request.customfield_instance_id
-        if not UtilClient.is_unset(request.customfield_name):
-            body['customfieldName'] = request.customfield_name
+        if not UtilClient.is_unset(request.custom_field_id):
+            body['customFieldId'] = request.custom_field_id
+        if not UtilClient.is_unset(request.custom_field_instance_id):
+            body['customFieldInstanceId'] = request.custom_field_instance_id
+        if not UtilClient.is_unset(request.custom_field_name):
+            body['customFieldName'] = request.custom_field_name
         if not UtilClient.is_unset(request.value):
             body['value'] = request.value
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -772,20 +772,20 @@
         project_id: str,
         request: dingtalkproject__1__0_models.CreateProjectCustomfieldStatusRequest,
         headers: dingtalkproject__1__0_models.CreateProjectCustomfieldStatusHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.CreateProjectCustomfieldStatusResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.customfield_id):
-            body['customfieldId'] = request.customfield_id
-        if not UtilClient.is_unset(request.customfield_instance_id):
-            body['customfieldInstanceId'] = request.customfield_instance_id
-        if not UtilClient.is_unset(request.customfield_name):
-            body['customfieldName'] = request.customfield_name
+        if not UtilClient.is_unset(request.custom_field_id):
+            body['customFieldId'] = request.custom_field_id
+        if not UtilClient.is_unset(request.custom_field_instance_id):
+            body['customFieldInstanceId'] = request.custom_field_instance_id
+        if not UtilClient.is_unset(request.custom_field_name):
+            body['customFieldName'] = request.custom_field_name
         if not UtilClient.is_unset(request.value):
             body['value'] = request.value
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -2955,18 +2955,18 @@
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.query):
             query['query'] = request.query
-        if not UtilClient.is_unset(request.stage_ids):
-            query['stageIds'] = request.stage_ids
         if not UtilClient.is_unset(request.task_list_id):
             query['taskListId'] = request.task_list_id
+        if not UtilClient.is_unset(request.task_stage_ids):
+            query['taskStageIds'] = request.task_stage_ids
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -3000,18 +3000,18 @@
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.query):
             query['query'] = request.query
-        if not UtilClient.is_unset(request.stage_ids):
-            query['stageIds'] = request.stage_ids
         if not UtilClient.is_unset(request.task_list_id):
             query['taskListId'] = request.task_list_id
+        if not UtilClient.is_unset(request.task_stage_ids):
+            query['taskStageIds'] = request.task_stage_ids
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -3058,28 +3058,26 @@
         user_id: str,
         request: dingtalkproject__1__0_models.SearchOranizationCustomfieldRequest,
         headers: dingtalkproject__1__0_models.SearchOranizationCustomfieldHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.SearchOranizationCustomfieldResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.customfield_ids):
-            query['customfieldIds'] = request.customfield_ids
+        if not UtilClient.is_unset(request.custom_field_ids):
+            query['customFieldIds'] = request.custom_field_ids
         if not UtilClient.is_unset(request.instance_ids):
             query['instanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.project_ids):
             query['projectIds'] = request.project_ids
         if not UtilClient.is_unset(request.query):
             query['query'] = request.query
-        if not UtilClient.is_unset(request.scope):
-            query['scope'] = request.scope
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -3106,28 +3104,26 @@
         user_id: str,
         request: dingtalkproject__1__0_models.SearchOranizationCustomfieldRequest,
         headers: dingtalkproject__1__0_models.SearchOranizationCustomfieldHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.SearchOranizationCustomfieldResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.customfield_ids):
-            query['customfieldIds'] = request.customfield_ids
+        if not UtilClient.is_unset(request.custom_field_ids):
+            query['customFieldIds'] = request.custom_field_ids
         if not UtilClient.is_unset(request.instance_ids):
             query['instanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.project_ids):
             query['projectIds'] = request.project_ids
         if not UtilClient.is_unset(request.query):
             query['query'] = request.query
-        if not UtilClient.is_unset(request.scope):
-            query['scope'] = request.scope
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -3173,28 +3169,26 @@
         project_id: str,
         request: dingtalkproject__1__0_models.SearchProjectCustomfieldRequest,
         headers: dingtalkproject__1__0_models.SearchProjectCustomfieldHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.SearchProjectCustomfieldResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.customfield_ids):
-            query['customfieldIds'] = request.customfield_ids
+        if not UtilClient.is_unset(request.custom_field_ids):
+            query['customFieldIds'] = request.custom_field_ids
         if not UtilClient.is_unset(request.instance_ids):
             query['instanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.query):
             query['query'] = request.query
-        if not UtilClient.is_unset(request.scenariofieldconfig_id):
-            query['scenariofieldconfigId'] = request.scenariofieldconfig_id
-        if not UtilClient.is_unset(request.scope):
-            query['scope'] = request.scope
+        if not UtilClient.is_unset(request.scenario_field_config_id):
+            query['scenarioFieldConfigId'] = request.scenario_field_config_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -3222,28 +3216,26 @@
         project_id: str,
         request: dingtalkproject__1__0_models.SearchProjectCustomfieldRequest,
         headers: dingtalkproject__1__0_models.SearchProjectCustomfieldHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.SearchProjectCustomfieldResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.customfield_ids):
-            query['customfieldIds'] = request.customfield_ids
+        if not UtilClient.is_unset(request.custom_field_ids):
+            query['customFieldIds'] = request.custom_field_ids
         if not UtilClient.is_unset(request.instance_ids):
             query['instanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.query):
             query['query'] = request.query
-        if not UtilClient.is_unset(request.scenariofieldconfig_id):
-            query['scenariofieldconfigId'] = request.scenariofieldconfig_id
-        if not UtilClient.is_unset(request.scope):
-            query['scope'] = request.scope
+        if not UtilClient.is_unset(request.scenario_field_config_id):
+            query['scenarioFieldConfigId'] = request.scenario_field_config_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -3706,14 +3698,16 @@
     ) -> dingtalkproject__1__0_models.SearchUserTaskResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.role_types):
+            query['roleTypes'] = request.role_types
         if not UtilClient.is_unset(request.tql):
             query['tql'] = request.tql
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -3746,14 +3740,16 @@
     ) -> dingtalkproject__1__0_models.SearchUserTaskResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.role_types):
+            query['roleTypes'] = request.role_types
         if not UtilClient.is_unset(request.tql):
             query['tql'] = request.tql
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -3961,18 +3957,18 @@
         task_id: str,
         request: dingtalkproject__1__0_models.UpdateCustomfieldValueRequest,
         headers: dingtalkproject__1__0_models.UpdateCustomfieldValueHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.UpdateCustomfieldValueResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.customfield_id):
-            body['customfieldId'] = request.customfield_id
-        if not UtilClient.is_unset(request.customfield_name):
-            body['customfieldName'] = request.customfield_name
+        if not UtilClient.is_unset(request.custom_field_id):
+            body['customFieldId'] = request.custom_field_id
+        if not UtilClient.is_unset(request.custom_field_name):
+            body['customFieldName'] = request.custom_field_name
         if not UtilClient.is_unset(request.value):
             body['value'] = request.value
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -4002,18 +3998,18 @@
         task_id: str,
         request: dingtalkproject__1__0_models.UpdateCustomfieldValueRequest,
         headers: dingtalkproject__1__0_models.UpdateCustomfieldValueHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.UpdateCustomfieldValueResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.customfield_id):
-            body['customfieldId'] = request.customfield_id
-        if not UtilClient.is_unset(request.customfield_name):
-            body['customfieldName'] = request.customfield_name
+        if not UtilClient.is_unset(request.custom_field_id):
+            body['customFieldId'] = request.custom_field_id
+        if not UtilClient.is_unset(request.custom_field_name):
+            body['customFieldName'] = request.custom_field_name
         if not UtilClient.is_unset(request.value):
             body['value'] = request.value
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -5645,16 +5641,16 @@
         headers: dingtalkproject__1__0_models.UpdateTaskTaskflowstatusHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.UpdateTaskTaskflowstatusResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.taskflow_status_id):
             body['taskflowStatusId'] = request.taskflow_status_id
-        if not UtilClient.is_unset(request.tfs_update_note):
-            body['tfsUpdateNote'] = request.tfs_update_note
+        if not UtilClient.is_unset(request.taskflow_status_update_note):
+            body['taskflowStatusUpdateNote'] = request.taskflow_status_update_note
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -5684,16 +5680,16 @@
         headers: dingtalkproject__1__0_models.UpdateTaskTaskflowstatusHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.UpdateTaskTaskflowstatusResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.taskflow_status_id):
             body['taskflowStatusId'] = request.taskflow_status_id
-        if not UtilClient.is_unset(request.tfs_update_note):
-            body['tfsUpdateNote'] = request.tfs_update_note
+        if not UtilClient.is_unset(request.taskflow_status_update_note):
+            body['taskflowStatusUpdateNote'] = request.taskflow_status_update_note
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1230,61 +1230,61 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('name') is not None:
             self.name = m.get('name')
         return self
 
 
-class CreateProjectResponseBodyResultCustomfieldsValue(TeaModel):
+class CreateProjectResponseBodyResultCustomFieldsValue(TeaModel):
     def __init__(
         self,
-        fieldvalue_id: str = None,
+        custom_field_value_id: str = None,
         meta_string: str = None,
         title: str = None,
     ):
-        self.fieldvalue_id = fieldvalue_id
+        self.custom_field_value_id = custom_field_value_id
         self.meta_string = meta_string
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
+        if self.custom_field_value_id is not None:
+            result['customFieldValueId'] = self.custom_field_value_id
         if self.meta_string is not None:
             result['metaString'] = self.meta_string
         if self.title is not None:
             result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('customFieldValueId') is not None:
+            self.custom_field_value_id = m.get('customFieldValueId')
         if m.get('metaString') is not None:
             self.meta_string = m.get('metaString')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
-class CreateProjectResponseBodyResultCustomfields(TeaModel):
+class CreateProjectResponseBodyResultCustomFields(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
+        custom_field_id: str = None,
         type: str = None,
-        value: List[CreateProjectResponseBodyResultCustomfieldsValue] = None,
+        value: List[CreateProjectResponseBodyResultCustomFieldsValue] = None,
     ):
-        self.customfield_id = customfield_id
+        self.custom_field_id = custom_field_id
         self.type = type
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
@@ -1292,44 +1292,44 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         if self.type is not None:
             result['type'] = self.type
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         if m.get('type') is not None:
             self.type = m.get('type')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
-                temp_model = CreateProjectResponseBodyResultCustomfieldsValue()
+                temp_model = CreateProjectResponseBodyResultCustomFieldsValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
 class CreateProjectResponseBodyResult(TeaModel):
     def __init__(
         self,
         created: str = None,
         creator_id: str = None,
-        customfields: List[CreateProjectResponseBodyResultCustomfields] = None,
+        custom_fields: List[CreateProjectResponseBodyResultCustomFields] = None,
         default_collection_id: str = None,
         is_archived: bool = None,
         is_suspended: bool = None,
         is_template: bool = None,
         logo: str = None,
         name: str = None,
         normal_type: str = None,
@@ -1338,15 +1338,15 @@
         source_id: str = None,
         unique_id_prefix: str = None,
         updated: str = None,
         visibility: str = None,
     ):
         self.created = created
         self.creator_id = creator_id
-        self.customfields = customfields
+        self.custom_fields = custom_fields
         self.default_collection_id = default_collection_id
         self.is_archived = is_archived
         self.is_suspended = is_suspended
         self.is_template = is_template
         self.logo = logo
         self.name = name
         self.normal_type = normal_type
@@ -1354,33 +1354,33 @@
         self.root_collection_id = root_collection_id
         self.source_id = source_id
         self.unique_id_prefix = unique_id_prefix
         self.updated = updated
         self.visibility = visibility
 
     def validate(self):
-        if self.customfields:
-            for k in self.customfields:
+        if self.custom_fields:
+            for k in self.custom_fields:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.created is not None:
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
-        result['customfields'] = []
-        if self.customfields is not None:
-            for k in self.customfields:
-                result['customfields'].append(k.to_map() if k else None)
+        result['customFields'] = []
+        if self.custom_fields is not None:
+            for k in self.custom_fields:
+                result['customFields'].append(k.to_map() if k else None)
         if self.default_collection_id is not None:
             result['defaultCollectionId'] = self.default_collection_id
         if self.is_archived is not None:
             result['isArchived'] = self.is_archived
         if self.is_suspended is not None:
             result['isSuspended'] = self.is_suspended
         if self.is_template is not None:
@@ -1407,19 +1407,19 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
-        self.customfields = []
-        if m.get('customfields') is not None:
-            for k in m.get('customfields'):
-                temp_model = CreateProjectResponseBodyResultCustomfields()
-                self.customfields.append(temp_model.from_map(k))
+        self.custom_fields = []
+        if m.get('customFields') is not None:
+            for k in m.get('customFields'):
+                temp_model = CreateProjectResponseBodyResultCustomFields()
+                self.custom_fields.append(temp_model.from_map(k))
         if m.get('defaultCollectionId') is not None:
             self.default_collection_id = m.get('defaultCollectionId')
         if m.get('isArchived') is not None:
             self.is_archived = m.get('isArchived')
         if m.get('isSuspended') is not None:
             self.is_suspended = m.get('isSuspended')
         if m.get('isTemplate') is not None:
@@ -1734,154 +1734,154 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class CreateProjectCustomfieldStatusRequestValue(TeaModel):
     def __init__(
         self,
-        fieldvalue_id: str = None,
+        custom_field_value_id: str = None,
         meta_string: str = None,
         title: str = None,
     ):
-        self.fieldvalue_id = fieldvalue_id
+        self.custom_field_value_id = custom_field_value_id
         self.meta_string = meta_string
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
+        if self.custom_field_value_id is not None:
+            result['customFieldValueId'] = self.custom_field_value_id
         if self.meta_string is not None:
             result['metaString'] = self.meta_string
         if self.title is not None:
             result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('customFieldValueId') is not None:
+            self.custom_field_value_id = m.get('customFieldValueId')
         if m.get('metaString') is not None:
             self.meta_string = m.get('metaString')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
 class CreateProjectCustomfieldStatusRequest(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
-        customfield_instance_id: str = None,
-        customfield_name: str = None,
+        custom_field_id: str = None,
+        custom_field_instance_id: str = None,
+        custom_field_name: str = None,
         value: List[CreateProjectCustomfieldStatusRequestValue] = None,
     ):
-        self.customfield_id = customfield_id
-        self.customfield_instance_id = customfield_instance_id
-        self.customfield_name = customfield_name
+        self.custom_field_id = custom_field_id
+        self.custom_field_instance_id = custom_field_instance_id
+        self.custom_field_name = custom_field_name
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
-        if self.customfield_instance_id is not None:
-            result['customfieldInstanceId'] = self.customfield_instance_id
-        if self.customfield_name is not None:
-            result['customfieldName'] = self.customfield_name
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
+        if self.custom_field_instance_id is not None:
+            result['customFieldInstanceId'] = self.custom_field_instance_id
+        if self.custom_field_name is not None:
+            result['customFieldName'] = self.custom_field_name
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
-        if m.get('customfieldInstanceId') is not None:
-            self.customfield_instance_id = m.get('customfieldInstanceId')
-        if m.get('customfieldName') is not None:
-            self.customfield_name = m.get('customfieldName')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
+        if m.get('customFieldInstanceId') is not None:
+            self.custom_field_instance_id = m.get('customFieldInstanceId')
+        if m.get('customFieldName') is not None:
+            self.custom_field_name = m.get('customFieldName')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
                 temp_model = CreateProjectCustomfieldStatusRequestValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
 class CreateProjectCustomfieldStatusResponseBodyResultValue(TeaModel):
     def __init__(
         self,
-        fieldvalue_id: str = None,
+        custom_field_value_id: str = None,
         meta_string: str = None,
         title: str = None,
     ):
-        self.fieldvalue_id = fieldvalue_id
+        self.custom_field_value_id = custom_field_value_id
         self.meta_string = meta_string
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
+        if self.custom_field_value_id is not None:
+            result['customFieldValueId'] = self.custom_field_value_id
         if self.meta_string is not None:
             result['metaString'] = self.meta_string
         if self.title is not None:
             result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('customFieldValueId') is not None:
+            self.custom_field_value_id = m.get('customFieldValueId')
         if m.get('metaString') is not None:
             self.meta_string = m.get('metaString')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
 class CreateProjectCustomfieldStatusResponseBodyResult(TeaModel):
     def __init__(
         self,
-        adv_cf_object_type: str = None,
-        customfield_id: str = None,
+        advanced_custom_field_object_type: str = None,
+        custom_field_id: str = None,
         name: str = None,
         original_id: str = None,
         type: str = None,
         value: List[CreateProjectCustomfieldStatusResponseBodyResultValue] = None,
     ):
-        self.adv_cf_object_type = adv_cf_object_type
-        self.customfield_id = customfield_id
+        self.advanced_custom_field_object_type = advanced_custom_field_object_type
+        self.custom_field_id = custom_field_id
         self.name = name
         self.original_id = original_id
         self.type = type
         self.value = value
 
     def validate(self):
         if self.value:
@@ -1891,36 +1891,36 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.adv_cf_object_type is not None:
-            result['advCfObjectType'] = self.adv_cf_object_type
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
+        if self.advanced_custom_field_object_type is not None:
+            result['advancedCustomFieldObjectType'] = self.advanced_custom_field_object_type
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         if self.name is not None:
             result['name'] = self.name
         if self.original_id is not None:
             result['originalId'] = self.original_id
         if self.type is not None:
             result['type'] = self.type
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('advCfObjectType') is not None:
-            self.adv_cf_object_type = m.get('advCfObjectType')
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
+        if m.get('advancedCustomFieldObjectType') is not None:
+            self.advanced_custom_field_object_type = m.get('advancedCustomFieldObjectType')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('originalId') is not None:
             self.original_id = m.get('originalId')
         if m.get('type') is not None:
             self.type = m.get('type')
         self.value = []
@@ -5130,61 +5130,61 @@
         if m.get('parentTaskId') is not None:
             self.parent_task_id = m.get('parentTaskId')
         if m.get('taskId') is not None:
             self.task_id = m.get('taskId')
         return self
 
 
-class GetTaskByIdsResponseBodyResultCustomfieldsValue(TeaModel):
+class GetTaskByIdsResponseBodyResultCustomFieldsValue(TeaModel):
     def __init__(
         self,
-        fieldvalue_id: str = None,
+        custom_field_value_id: str = None,
         meta_string: str = None,
         title: str = None,
     ):
-        self.fieldvalue_id = fieldvalue_id
+        self.custom_field_value_id = custom_field_value_id
         self.meta_string = meta_string
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
+        if self.custom_field_value_id is not None:
+            result['customFieldValueId'] = self.custom_field_value_id
         if self.meta_string is not None:
             result['metaString'] = self.meta_string
         if self.title is not None:
             result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('customFieldValueId') is not None:
+            self.custom_field_value_id = m.get('customFieldValueId')
         if m.get('metaString') is not None:
             self.meta_string = m.get('metaString')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
-class GetTaskByIdsResponseBodyResultCustomfields(TeaModel):
+class GetTaskByIdsResponseBodyResultCustomFields(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
+        custom_field_id: str = None,
         type: str = None,
-        value: List[GetTaskByIdsResponseBodyResultCustomfieldsValue] = None,
+        value: List[GetTaskByIdsResponseBodyResultCustomFieldsValue] = None,
     ):
-        self.customfield_id = customfield_id
+        self.custom_field_id = custom_field_id
         self.type = type
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
@@ -5192,102 +5192,102 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         if self.type is not None:
             result['type'] = self.type
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         if m.get('type') is not None:
             self.type = m.get('type')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
-                temp_model = GetTaskByIdsResponseBodyResultCustomfieldsValue()
+                temp_model = GetTaskByIdsResponseBodyResultCustomFieldsValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
 class GetTaskByIdsResponseBodyResult(TeaModel):
     def __init__(
         self,
         accomplish_time: str = None,
         ancestor_ids: List[str] = None,
         content: str = None,
         created: str = None,
         creator_id: str = None,
-        customfields: List[GetTaskByIdsResponseBodyResultCustomfields] = None,
+        custom_fields: List[GetTaskByIdsResponseBodyResultCustomFields] = None,
         due_date: str = None,
         executor_id: str = None,
         involve_members: List[str] = None,
         is_archived: bool = None,
         is_done: bool = None,
         note: str = None,
         parent_task_id: str = None,
         priority: int = None,
         project_id: str = None,
         recurrence: List[str] = None,
-        scenariofieldconfig_id: str = None,
+        scenario_field_config_id: str = None,
         sprint_id: str = None,
-        stage_id: str = None,
         start_date: str = None,
         story_point: str = None,
         tag_ids: List[str] = None,
         task_id: str = None,
         task_list_id: str = None,
-        taskflowstatus_id: str = None,
+        task_stage_id: str = None,
+        taskflow_status_id: str = None,
         unique_id: str = None,
         updated: str = None,
         visible: str = None,
     ):
         self.accomplish_time = accomplish_time
         self.ancestor_ids = ancestor_ids
         self.content = content
         self.created = created
         self.creator_id = creator_id
-        self.customfields = customfields
+        self.custom_fields = custom_fields
         self.due_date = due_date
         self.executor_id = executor_id
         self.involve_members = involve_members
         self.is_archived = is_archived
         self.is_done = is_done
         self.note = note
         self.parent_task_id = parent_task_id
         self.priority = priority
         self.project_id = project_id
         self.recurrence = recurrence
-        self.scenariofieldconfig_id = scenariofieldconfig_id
+        self.scenario_field_config_id = scenario_field_config_id
         self.sprint_id = sprint_id
-        self.stage_id = stage_id
         self.start_date = start_date
         self.story_point = story_point
         self.tag_ids = tag_ids
         self.task_id = task_id
         self.task_list_id = task_list_id
-        self.taskflowstatus_id = taskflowstatus_id
+        self.task_stage_id = task_stage_id
+        self.taskflow_status_id = taskflow_status_id
         self.unique_id = unique_id
         self.updated = updated
         self.visible = visible
 
     def validate(self):
-        if self.customfields:
-            for k in self.customfields:
+        if self.custom_fields:
+            for k in self.custom_fields:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5299,18 +5299,18 @@
             result['ancestorIds'] = self.ancestor_ids
         if self.content is not None:
             result['content'] = self.content
         if self.created is not None:
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
-        result['customfields'] = []
-        if self.customfields is not None:
-            for k in self.customfields:
-                result['customfields'].append(k.to_map() if k else None)
+        result['customFields'] = []
+        if self.custom_fields is not None:
+            for k in self.custom_fields:
+                result['customFields'].append(k.to_map() if k else None)
         if self.due_date is not None:
             result['dueDate'] = self.due_date
         if self.executor_id is not None:
             result['executorId'] = self.executor_id
         if self.involve_members is not None:
             result['involveMembers'] = self.involve_members
         if self.is_archived is not None:
@@ -5323,32 +5323,32 @@
             result['parentTaskId'] = self.parent_task_id
         if self.priority is not None:
             result['priority'] = self.priority
         if self.project_id is not None:
             result['projectId'] = self.project_id
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence
-        if self.scenariofieldconfig_id is not None:
-            result['scenariofieldconfigId'] = self.scenariofieldconfig_id
+        if self.scenario_field_config_id is not None:
+            result['scenarioFieldConfigId'] = self.scenario_field_config_id
         if self.sprint_id is not None:
             result['sprintId'] = self.sprint_id
-        if self.stage_id is not None:
-            result['stageId'] = self.stage_id
         if self.start_date is not None:
             result['startDate'] = self.start_date
         if self.story_point is not None:
             result['storyPoint'] = self.story_point
         if self.tag_ids is not None:
             result['tagIds'] = self.tag_ids
         if self.task_id is not None:
             result['taskId'] = self.task_id
         if self.task_list_id is not None:
             result['taskListId'] = self.task_list_id
-        if self.taskflowstatus_id is not None:
-            result['taskflowstatusId'] = self.taskflowstatus_id
+        if self.task_stage_id is not None:
+            result['taskStageId'] = self.task_stage_id
+        if self.taskflow_status_id is not None:
+            result['taskflowStatusId'] = self.taskflow_status_id
         if self.unique_id is not None:
             result['uniqueId'] = self.unique_id
         if self.updated is not None:
             result['updated'] = self.updated
         if self.visible is not None:
             result['visible'] = self.visible
         return result
@@ -5361,19 +5361,19 @@
             self.ancestor_ids = m.get('ancestorIds')
         if m.get('content') is not None:
             self.content = m.get('content')
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
-        self.customfields = []
-        if m.get('customfields') is not None:
-            for k in m.get('customfields'):
-                temp_model = GetTaskByIdsResponseBodyResultCustomfields()
-                self.customfields.append(temp_model.from_map(k))
+        self.custom_fields = []
+        if m.get('customFields') is not None:
+            for k in m.get('customFields'):
+                temp_model = GetTaskByIdsResponseBodyResultCustomFields()
+                self.custom_fields.append(temp_model.from_map(k))
         if m.get('dueDate') is not None:
             self.due_date = m.get('dueDate')
         if m.get('executorId') is not None:
             self.executor_id = m.get('executorId')
         if m.get('involveMembers') is not None:
             self.involve_members = m.get('involveMembers')
         if m.get('isArchived') is not None:
@@ -5386,32 +5386,32 @@
             self.parent_task_id = m.get('parentTaskId')
         if m.get('priority') is not None:
             self.priority = m.get('priority')
         if m.get('projectId') is not None:
             self.project_id = m.get('projectId')
         if m.get('recurrence') is not None:
             self.recurrence = m.get('recurrence')
-        if m.get('scenariofieldconfigId') is not None:
-            self.scenariofieldconfig_id = m.get('scenariofieldconfigId')
+        if m.get('scenarioFieldConfigId') is not None:
+            self.scenario_field_config_id = m.get('scenarioFieldConfigId')
         if m.get('sprintId') is not None:
             self.sprint_id = m.get('sprintId')
-        if m.get('stageId') is not None:
-            self.stage_id = m.get('stageId')
         if m.get('startDate') is not None:
             self.start_date = m.get('startDate')
         if m.get('storyPoint') is not None:
             self.story_point = m.get('storyPoint')
         if m.get('tagIds') is not None:
             self.tag_ids = m.get('tagIds')
         if m.get('taskId') is not None:
             self.task_id = m.get('taskId')
         if m.get('taskListId') is not None:
             self.task_list_id = m.get('taskListId')
-        if m.get('taskflowstatusId') is not None:
-            self.taskflowstatus_id = m.get('taskflowstatusId')
+        if m.get('taskStageId') is not None:
+            self.task_stage_id = m.get('taskStageId')
+        if m.get('taskflowStatusId') is not None:
+            self.taskflow_status_id = m.get('taskflowStatusId')
         if m.get('uniqueId') is not None:
             self.unique_id = m.get('uniqueId')
         if m.get('updated') is not None:
             self.updated = m.get('updated')
         if m.get('visible') is not None:
             self.visible = m.get('visible')
         return self
@@ -6190,45 +6190,39 @@
 
 
 class GetUserJoinedProjectResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         result: List[str] = None,
-        total_count: int = None,
     ):
         self.next_token = next_token
         self.result = result
-        self.total_count = total_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.result is not None:
             result['result'] = self.result
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('result') is not None:
             self.result = m.get('result')
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
         return self
 
 
 class GetUserJoinedProjectResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6352,61 +6346,61 @@
         if m.get('projectIds') is not None:
             self.project_ids = m.get('projectIds')
         if m.get('sourceId') is not None:
             self.source_id = m.get('sourceId')
         return self
 
 
-class QueryProjectResponseBodyResultCustomfieldsValue(TeaModel):
+class QueryProjectResponseBodyResultCustomFieldsValue(TeaModel):
     def __init__(
         self,
-        fieldvalue_id: str = None,
+        custom_field_value_id: str = None,
         meta_string: str = None,
         title: str = None,
     ):
-        self.fieldvalue_id = fieldvalue_id
+        self.custom_field_value_id = custom_field_value_id
         self.meta_string = meta_string
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
+        if self.custom_field_value_id is not None:
+            result['customFieldValueId'] = self.custom_field_value_id
         if self.meta_string is not None:
             result['metaString'] = self.meta_string
         if self.title is not None:
             result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('customFieldValueId') is not None:
+            self.custom_field_value_id = m.get('customFieldValueId')
         if m.get('metaString') is not None:
             self.meta_string = m.get('metaString')
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
-class QueryProjectResponseBodyResultCustomfields(TeaModel):
+class QueryProjectResponseBodyResultCustomFields(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
+        custom_field_id: str = None,
         type: str = None,
-        value: List[QueryProjectResponseBodyResultCustomfieldsValue] = None,
+        value: List[QueryProjectResponseBodyResultCustomFieldsValue] = None,
     ):
-        self.customfield_id = customfield_id
+        self.custom_field_id = custom_field_id
         self.type = type
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
@@ -6414,44 +6408,44 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         if self.type is not None:
             result['type'] = self.type
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         if m.get('type') is not None:
             self.type = m.get('type')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
-                temp_model = QueryProjectResponseBodyResultCustomfieldsValue()
+                temp_model = QueryProjectResponseBodyResultCustomFieldsValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
 class QueryProjectResponseBodyResult(TeaModel):
     def __init__(
         self,
         created: str = None,
         creator_id: str = None,
-        customfields: List[QueryProjectResponseBodyResultCustomfields] = None,
+        custom_fields: List[QueryProjectResponseBodyResultCustomFields] = None,
         description: str = None,
         end_date: str = None,
         is_archived: bool = None,
         is_suspended: bool = None,
         is_template: bool = None,
         logo: str = None,
         name: str = None,
@@ -6460,15 +6454,15 @@
         start_date: str = None,
         unique_id_prefix: str = None,
         updated: str = None,
         visibility: str = None,
     ):
         self.created = created
         self.creator_id = creator_id
-        self.customfields = customfields
+        self.custom_fields = custom_fields
         self.description = description
         self.end_date = end_date
         self.is_archived = is_archived
         self.is_suspended = is_suspended
         self.is_template = is_template
         self.logo = logo
         self.name = name
@@ -6476,33 +6470,33 @@
         self.project_id = project_id
         self.start_date = start_date
         self.unique_id_prefix = unique_id_prefix
         self.updated = updated
         self.visibility = visibility
 
     def validate(self):
-        if self.customfields:
-            for k in self.customfields:
+        if self.custom_fields:
+            for k in self.custom_fields:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.created is not None:
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
-        result['customfields'] = []
-        if self.customfields is not None:
-            for k in self.customfields:
-                result['customfields'].append(k.to_map() if k else None)
+        result['customFields'] = []
+        if self.custom_fields is not None:
+            for k in self.custom_fields:
+                result['customFields'].append(k.to_map() if k else None)
         if self.description is not None:
             result['description'] = self.description
         if self.end_date is not None:
             result['endDate'] = self.end_date
         if self.is_archived is not None:
             result['isArchived'] = self.is_archived
         if self.is_suspended is not None:
@@ -6529,19 +6523,19 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
-        self.customfields = []
-        if m.get('customfields') is not None:
-            for k in m.get('customfields'):
-                temp_model = QueryProjectResponseBodyResultCustomfields()
-                self.customfields.append(temp_model.from_map(k))
+        self.custom_fields = []
+        if m.get('customFields') is not None:
+            for k in m.get('customFields'):
+                temp_model = QueryProjectResponseBodyResultCustomFields()
+                self.custom_fields.append(temp_model.from_map(k))
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('endDate') is not None:
             self.end_date = m.get('endDate')
         if m.get('isArchived') is not None:
             self.is_archived = m.get('isArchived')
         if m.get('isSuspended') is not None:
@@ -7062,22 +7056,22 @@
 
 class SeachTaskStageRequest(TeaModel):
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
         query: str = None,
-        stage_ids: str = None,
         task_list_id: str = None,
+        task_stage_ids: str = None,
     ):
         self.max_results = max_results
         self.next_token = next_token
         self.query = query
-        self.stage_ids = stage_ids
         self.task_list_id = task_list_id
+        self.task_stage_ids = task_stage_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7086,32 +7080,32 @@
         result = dict()
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.query is not None:
             result['query'] = self.query
-        if self.stage_ids is not None:
-            result['stageIds'] = self.stage_ids
         if self.task_list_id is not None:
             result['taskListId'] = self.task_list_id
+        if self.task_stage_ids is not None:
+            result['taskStageIds'] = self.task_stage_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('query') is not None:
             self.query = m.get('query')
-        if m.get('stageIds') is not None:
-            self.stage_ids = m.get('stageIds')
         if m.get('taskListId') is not None:
             self.task_list_id = m.get('taskListId')
+        if m.get('taskStageIds') is not None:
+            self.task_stage_ids = m.get('taskStageIds')
         return self
 
 
 class SeachTaskStageResponseBodyResult(TeaModel):
     def __init__(
         self,
         created: str = None,
@@ -7181,19 +7175,17 @@
 
 
 class SeachTaskStageResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         result: List[SeachTaskStageResponseBodyResult] = None,
-        total_count: int = None,
     ):
         self.next_token = next_token
         self.result = result
-        self.total_count = total_count
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
@@ -7205,29 +7197,25 @@
         result = dict()
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         result['result'] = []
         if self.result is not None:
             for k in self.result:
                 result['result'].append(k.to_map() if k else None)
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         self.result = []
         if m.get('result') is not None:
             for k in m.get('result'):
                 temp_model = SeachTaskStageResponseBodyResult()
                 self.result.append(temp_model.from_map(k))
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
         return self
 
 
 class SeachTaskStageResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -7303,106 +7291,100 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class SearchOranizationCustomfieldRequest(TeaModel):
     def __init__(
         self,
-        customfield_ids: str = None,
+        custom_field_ids: str = None,
         instance_ids: str = None,
         max_results: int = None,
         next_token: str = None,
         project_ids: str = None,
         query: str = None,
-        scope: str = None,
     ):
-        self.customfield_ids = customfield_ids
+        self.custom_field_ids = custom_field_ids
         self.instance_ids = instance_ids
         self.max_results = max_results
         self.next_token = next_token
         self.project_ids = project_ids
         self.query = query
-        self.scope = scope
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_ids is not None:
-            result['customfieldIds'] = self.customfield_ids
+        if self.custom_field_ids is not None:
+            result['customFieldIds'] = self.custom_field_ids
         if self.instance_ids is not None:
             result['instanceIds'] = self.instance_ids
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.project_ids is not None:
             result['projectIds'] = self.project_ids
         if self.query is not None:
             result['query'] = self.query
-        if self.scope is not None:
-            result['scope'] = self.scope
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldIds') is not None:
-            self.customfield_ids = m.get('customfieldIds')
+        if m.get('customFieldIds') is not None:
+            self.custom_field_ids = m.get('customFieldIds')
         if m.get('instanceIds') is not None:
             self.instance_ids = m.get('instanceIds')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('projectIds') is not None:
             self.project_ids = m.get('projectIds')
         if m.get('query') is not None:
             self.query = m.get('query')
-        if m.get('scope') is not None:
-            self.scope = m.get('scope')
         return self
 
 
-class SearchOranizationCustomfieldResponseBodyResultAdvancedCustomfield(TeaModel):
+class SearchOranizationCustomfieldResponseBodyResultAdvancedCustomField(TeaModel):
     def __init__(
         self,
-        advanced_customfield_id: str = None,
+        advanced_custom_field_id: str = None,
         name: str = None,
         object_type: str = None,
     ):
-        self.advanced_customfield_id = advanced_customfield_id
+        self.advanced_custom_field_id = advanced_custom_field_id
         self.name = name
         self.object_type = object_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.advanced_customfield_id is not None:
-            result['advancedCustomfieldId'] = self.advanced_customfield_id
+        if self.advanced_custom_field_id is not None:
+            result['advancedCustomFieldId'] = self.advanced_custom_field_id
         if self.name is not None:
             result['name'] = self.name
         if self.object_type is not None:
             result['objectType'] = self.object_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('advancedCustomfieldId') is not None:
-            self.advanced_customfield_id = m.get('advancedCustomfieldId')
+        if m.get('advancedCustomFieldId') is not None:
+            self.advanced_custom_field_id = m.get('advancedCustomFieldId')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('objectType') is not None:
             self.object_type = m.get('objectType')
         return self
 
 
@@ -7438,101 +7420,99 @@
             self.value = m.get('value')
         return self
 
 
 class SearchOranizationCustomfieldResponseBodyResult(TeaModel):
     def __init__(
         self,
-        advanced_customfield: SearchOranizationCustomfieldResponseBodyResultAdvancedCustomfield = None,
+        advanced_custom_field: SearchOranizationCustomfieldResponseBodyResultAdvancedCustomField = None,
         choices: List[SearchOranizationCustomfieldResponseBodyResultChoices] = None,
         created: str = None,
         creator_id: str = None,
-        customfields_id: str = None,
+        custom_fields_id: str = None,
         name: str = None,
         payload: Dict[str, Any] = None,
         type: str = None,
     ):
-        self.advanced_customfield = advanced_customfield
+        self.advanced_custom_field = advanced_custom_field
         self.choices = choices
         self.created = created
         self.creator_id = creator_id
-        self.customfields_id = customfields_id
+        self.custom_fields_id = custom_fields_id
         self.name = name
         self.payload = payload
         self.type = type
 
     def validate(self):
-        if self.advanced_customfield:
-            self.advanced_customfield.validate()
+        if self.advanced_custom_field:
+            self.advanced_custom_field.validate()
         if self.choices:
             for k in self.choices:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.advanced_customfield is not None:
-            result['advancedCustomfield'] = self.advanced_customfield.to_map()
+        if self.advanced_custom_field is not None:
+            result['advancedCustomField'] = self.advanced_custom_field.to_map()
         result['choices'] = []
         if self.choices is not None:
             for k in self.choices:
                 result['choices'].append(k.to_map() if k else None)
         if self.created is not None:
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
-        if self.customfields_id is not None:
-            result['customfieldsId'] = self.customfields_id
+        if self.custom_fields_id is not None:
+            result['customFieldsId'] = self.custom_fields_id
         if self.name is not None:
             result['name'] = self.name
         if self.payload is not None:
             result['payload'] = self.payload
         if self.type is not None:
             result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('advancedCustomfield') is not None:
-            temp_model = SearchOranizationCustomfieldResponseBodyResultAdvancedCustomfield()
-            self.advanced_customfield = temp_model.from_map(m['advancedCustomfield'])
+        if m.get('advancedCustomField') is not None:
+            temp_model = SearchOranizationCustomfieldResponseBodyResultAdvancedCustomField()
+            self.advanced_custom_field = temp_model.from_map(m['advancedCustomField'])
         self.choices = []
         if m.get('choices') is not None:
             for k in m.get('choices'):
                 temp_model = SearchOranizationCustomfieldResponseBodyResultChoices()
                 self.choices.append(temp_model.from_map(k))
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
-        if m.get('customfieldsId') is not None:
-            self.customfields_id = m.get('customfieldsId')
+        if m.get('customFieldsId') is not None:
+            self.custom_fields_id = m.get('customFieldsId')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('payload') is not None:
             self.payload = m.get('payload')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
 class SearchOranizationCustomfieldResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         result: List[SearchOranizationCustomfieldResponseBodyResult] = None,
-        total_count: int = None,
     ):
         self.next_token = next_token
         self.result = result
-        self.total_count = total_count
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
@@ -7544,29 +7524,25 @@
         result = dict()
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         result['result'] = []
         if self.result is not None:
             for k in self.result:
                 result['result'].append(k.to_map() if k else None)
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         self.result = []
         if m.get('result') is not None:
             for k in m.get('result'):
                 temp_model = SearchOranizationCustomfieldResponseBodyResult()
                 self.result.append(temp_model.from_map(k))
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
         return self
 
 
 class SearchOranizationCustomfieldResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -7642,106 +7618,100 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class SearchProjectCustomfieldRequest(TeaModel):
     def __init__(
         self,
-        customfield_ids: str = None,
+        custom_field_ids: str = None,
         instance_ids: str = None,
         max_results: int = None,
         next_token: str = None,
         query: str = None,
-        scenariofieldconfig_id: str = None,
-        scope: str = None,
+        scenario_field_config_id: str = None,
     ):
-        self.customfield_ids = customfield_ids
+        self.custom_field_ids = custom_field_ids
         self.instance_ids = instance_ids
         self.max_results = max_results
         self.next_token = next_token
         self.query = query
-        self.scenariofieldconfig_id = scenariofieldconfig_id
-        self.scope = scope
+        self.scenario_field_config_id = scenario_field_config_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_ids is not None:
-            result['customfieldIds'] = self.customfield_ids
+        if self.custom_field_ids is not None:
+            result['customFieldIds'] = self.custom_field_ids
         if self.instance_ids is not None:
             result['instanceIds'] = self.instance_ids
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.query is not None:
             result['query'] = self.query
-        if self.scenariofieldconfig_id is not None:
-            result['scenariofieldconfigId'] = self.scenariofieldconfig_id
-        if self.scope is not None:
-            result['scope'] = self.scope
+        if self.scenario_field_config_id is not None:
+            result['scenarioFieldConfigId'] = self.scenario_field_config_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldIds') is not None:
-            self.customfield_ids = m.get('customfieldIds')
+        if m.get('customFieldIds') is not None:
+            self.custom_field_ids = m.get('customFieldIds')
         if m.get('instanceIds') is not None:
             self.instance_ids = m.get('instanceIds')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('query') is not None:
             self.query = m.get('query')
-        if m.get('scenariofieldconfigId') is not None:
-            self.scenariofieldconfig_id = m.get('scenariofieldconfigId')
-        if m.get('scope') is not None:
-            self.scope = m.get('scope')
+        if m.get('scenarioFieldConfigId') is not None:
+            self.scenario_field_config_id = m.get('scenarioFieldConfigId')
         return self
 
 
-class SearchProjectCustomfieldResponseBodyResultAdvancedCustomfield(TeaModel):
+class SearchProjectCustomfieldResponseBodyResultAdvancedCustomField(TeaModel):
     def __init__(
         self,
-        advanced_customfield_id: str = None,
+        advanced_custom_field_id: str = None,
         name: str = None,
         object_type: str = None,
     ):
-        self.advanced_customfield_id = advanced_customfield_id
+        self.advanced_custom_field_id = advanced_custom_field_id
         self.name = name
         self.object_type = object_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.advanced_customfield_id is not None:
-            result['advancedCustomfieldId'] = self.advanced_customfield_id
+        if self.advanced_custom_field_id is not None:
+            result['advancedCustomFieldId'] = self.advanced_custom_field_id
         if self.name is not None:
             result['name'] = self.name
         if self.object_type is not None:
             result['objectType'] = self.object_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('advancedCustomfieldId') is not None:
-            self.advanced_customfield_id = m.get('advancedCustomfieldId')
+        if m.get('advancedCustomFieldId') is not None:
+            self.advanced_custom_field_id = m.get('advancedCustomFieldId')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('objectType') is not None:
             self.object_type = m.get('objectType')
         return self
 
 
@@ -7777,92 +7747,92 @@
             self.value = m.get('value')
         return self
 
 
 class SearchProjectCustomfieldResponseBodyResult(TeaModel):
     def __init__(
         self,
-        advanced_customfield: SearchProjectCustomfieldResponseBodyResultAdvancedCustomfield = None,
+        advanced_custom_field: SearchProjectCustomfieldResponseBodyResultAdvancedCustomField = None,
         bound_to_object_id: str = None,
         choices: List[SearchProjectCustomfieldResponseBodyResultChoices] = None,
         created: str = None,
         creator_id: str = None,
-        customfiled_id: str = None,
+        custom_field_id: str = None,
         name: str = None,
         original_id: str = None,
         payload: Dict[str, Any] = None,
         type: str = None,
     ):
-        self.advanced_customfield = advanced_customfield
+        self.advanced_custom_field = advanced_custom_field
         self.bound_to_object_id = bound_to_object_id
         self.choices = choices
         self.created = created
         self.creator_id = creator_id
-        self.customfiled_id = customfiled_id
+        self.custom_field_id = custom_field_id
         self.name = name
         self.original_id = original_id
         self.payload = payload
         self.type = type
 
     def validate(self):
-        if self.advanced_customfield:
-            self.advanced_customfield.validate()
+        if self.advanced_custom_field:
+            self.advanced_custom_field.validate()
         if self.choices:
             for k in self.choices:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.advanced_customfield is not None:
-            result['advancedCustomfield'] = self.advanced_customfield.to_map()
+        if self.advanced_custom_field is not None:
+            result['advancedCustomField'] = self.advanced_custom_field.to_map()
         if self.bound_to_object_id is not None:
             result['boundToObjectId'] = self.bound_to_object_id
         result['choices'] = []
         if self.choices is not None:
             for k in self.choices:
                 result['choices'].append(k.to_map() if k else None)
         if self.created is not None:
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
-        if self.customfiled_id is not None:
-            result['customfiledId'] = self.customfiled_id
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         if self.name is not None:
             result['name'] = self.name
         if self.original_id is not None:
             result['originalId'] = self.original_id
         if self.payload is not None:
             result['payload'] = self.payload
         if self.type is not None:
             result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('advancedCustomfield') is not None:
-            temp_model = SearchProjectCustomfieldResponseBodyResultAdvancedCustomfield()
-            self.advanced_customfield = temp_model.from_map(m['advancedCustomfield'])
+        if m.get('advancedCustomField') is not None:
+            temp_model = SearchProjectCustomfieldResponseBodyResultAdvancedCustomField()
+            self.advanced_custom_field = temp_model.from_map(m['advancedCustomField'])
         if m.get('boundToObjectId') is not None:
             self.bound_to_object_id = m.get('boundToObjectId')
         self.choices = []
         if m.get('choices') is not None:
             for k in m.get('choices'):
                 temp_model = SearchProjectCustomfieldResponseBodyResultChoices()
                 self.choices.append(temp_model.from_map(k))
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
-        if m.get('customfiledId') is not None:
-            self.customfiled_id = m.get('customfiledId')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('originalId') is not None:
             self.original_id = m.get('originalId')
         if m.get('payload') is not None:
             self.payload = m.get('payload')
         if m.get('type') is not None:
@@ -7871,19 +7841,17 @@
 
 
 class SearchProjectCustomfieldResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         result: List[SearchProjectCustomfieldResponseBodyResult] = None,
-        total_count: int = None,
     ):
         self.next_token = next_token
         self.result = result
-        self.total_count = total_count
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
@@ -7895,29 +7863,25 @@
         result = dict()
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         result['result'] = []
         if self.result is not None:
             for k in self.result:
                 result['result'].append(k.to_map() if k else None)
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         self.result = []
         if m.get('result') is not None:
             for k in m.get('result'):
                 temp_model = SearchProjectCustomfieldResponseBodyResult()
                 self.result.append(temp_model.from_map(k))
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
         return self
 
 
 class SearchProjectCustomfieldResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -8543,19 +8507,17 @@
 
 
 class SearchTaskListResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         result: List[SearchTaskListResponseBodyResult] = None,
-        total_count: int = None,
     ):
         self.next_token = next_token
         self.result = result
-        self.total_count = total_count
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
@@ -8567,29 +8529,25 @@
         result = dict()
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         result['result'] = []
         if self.result is not None:
             for k in self.result:
                 result['result'].append(k.to_map() if k else None)
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         self.result = []
         if m.get('result') is not None:
             for k in m.get('result'):
                 temp_model = SearchTaskListResponseBodyResult()
                 self.result.append(temp_model.from_map(k))
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
         return self
 
 
 class SearchTaskListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -8915,20 +8873,22 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class SearchUserTaskRequest(TeaModel):
     def __init__(
         self,
-        max_results: int = None,
+        max_results: str = None,
         next_token: str = None,
+        role_types: str = None,
         tql: str = None,
     ):
         self.max_results = max_results
         self.next_token = next_token
+        self.role_types = role_types
         self.tql = tql
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8936,82 +8896,80 @@
             return _map
 
         result = dict()
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
+        if self.role_types is not None:
+            result['roleTypes'] = self.role_types
         if self.tql is not None:
             result['tql'] = self.tql
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
+        if m.get('roleTypes') is not None:
+            self.role_types = m.get('roleTypes')
         if m.get('tql') is not None:
             self.tql = m.get('tql')
         return self
 
 
-class SearchUserTaskResponseBodyResultCustomfieldsValue(TeaModel):
+class SearchUserTaskResponseBodyResultCustomFieldsValue(TeaModel):
     def __init__(
         self,
-        fieldvalue_id: str = None,
+        custom_field_value_id: str = None,
         meta_string: str = None,
         title: str = None,
-        total_count: int = None,
     ):
-        self.fieldvalue_id = fieldvalue_id
+        self.custom_field_value_id = custom_field_value_id
         self.meta_string = meta_string
         self.title = title
-        self.total_count = total_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
+        if self.custom_field_value_id is not None:
+            result['customFieldValueId'] = self.custom_field_value_id
         if self.meta_string is not None:
             result['metaString'] = self.meta_string
         if self.title is not None:
             result['title'] = self.title
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('customFieldValueId') is not None:
+            self.custom_field_value_id = m.get('customFieldValueId')
         if m.get('metaString') is not None:
             self.meta_string = m.get('metaString')
         if m.get('title') is not None:
             self.title = m.get('title')
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
         return self
 
 
-class SearchUserTaskResponseBodyResultCustomfields(TeaModel):
+class SearchUserTaskResponseBodyResultCustomFields(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
+        custom_field_id: str = None,
         type: str = None,
-        value: List[SearchUserTaskResponseBodyResultCustomfieldsValue] = None,
+        value: List[SearchUserTaskResponseBodyResultCustomFieldsValue] = None,
     ):
-        self.customfield_id = customfield_id
+        self.custom_field_id = custom_field_id
         self.type = type
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
@@ -9019,102 +8977,102 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         if self.type is not None:
             result['type'] = self.type
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         if m.get('type') is not None:
             self.type = m.get('type')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
-                temp_model = SearchUserTaskResponseBodyResultCustomfieldsValue()
+                temp_model = SearchUserTaskResponseBodyResultCustomFieldsValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
 class SearchUserTaskResponseBodyResult(TeaModel):
     def __init__(
         self,
         accomplish_time: str = None,
         ancestor_ids: List[str] = None,
         content: str = None,
         created: str = None,
         creator_id: str = None,
-        customfields: List[SearchUserTaskResponseBodyResultCustomfields] = None,
+        custom_fields: List[SearchUserTaskResponseBodyResultCustomFields] = None,
         due_date: str = None,
         executor_id: str = None,
         involve_members: List[str] = None,
         is_archived: bool = None,
         is_done: bool = None,
         note: str = None,
         parent_task_id: str = None,
         priority: int = None,
         project_id: str = None,
         recurrence: List[str] = None,
-        sfc_id: str = None,
+        scenario_field_config_id: str = None,
         sprint_id: str = None,
         start_date: str = None,
         story_point: str = None,
         tag_ids: List[str] = None,
         task_id: str = None,
         task_list_id: str = None,
-        taskflowstatus_id: str = None,
-        taskstage_id: str = None,
+        task_stage_id: str = None,
+        taskflow_status_id: str = None,
         unique_id: str = None,
         updated: str = None,
         visible: str = None,
     ):
         self.accomplish_time = accomplish_time
         self.ancestor_ids = ancestor_ids
         self.content = content
         self.created = created
         self.creator_id = creator_id
-        self.customfields = customfields
+        self.custom_fields = custom_fields
         self.due_date = due_date
         self.executor_id = executor_id
         self.involve_members = involve_members
         self.is_archived = is_archived
         self.is_done = is_done
         self.note = note
         self.parent_task_id = parent_task_id
         self.priority = priority
         self.project_id = project_id
         self.recurrence = recurrence
-        self.sfc_id = sfc_id
+        self.scenario_field_config_id = scenario_field_config_id
         self.sprint_id = sprint_id
         self.start_date = start_date
         self.story_point = story_point
         self.tag_ids = tag_ids
         self.task_id = task_id
         self.task_list_id = task_list_id
-        self.taskflowstatus_id = taskflowstatus_id
-        self.taskstage_id = taskstage_id
+        self.task_stage_id = task_stage_id
+        self.taskflow_status_id = taskflow_status_id
         self.unique_id = unique_id
         self.updated = updated
         self.visible = visible
 
     def validate(self):
-        if self.customfields:
-            for k in self.customfields:
+        if self.custom_fields:
+            for k in self.custom_fields:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9126,18 +9084,18 @@
             result['ancestorIds'] = self.ancestor_ids
         if self.content is not None:
             result['content'] = self.content
         if self.created is not None:
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
-        result['customfields'] = []
-        if self.customfields is not None:
-            for k in self.customfields:
-                result['customfields'].append(k.to_map() if k else None)
+        result['customFields'] = []
+        if self.custom_fields is not None:
+            for k in self.custom_fields:
+                result['customFields'].append(k.to_map() if k else None)
         if self.due_date is not None:
             result['dueDate'] = self.due_date
         if self.executor_id is not None:
             result['executorId'] = self.executor_id
         if self.involve_members is not None:
             result['involveMembers'] = self.involve_members
         if self.is_archived is not None:
@@ -9150,32 +9108,32 @@
             result['parentTaskId'] = self.parent_task_id
         if self.priority is not None:
             result['priority'] = self.priority
         if self.project_id is not None:
             result['projectId'] = self.project_id
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence
-        if self.sfc_id is not None:
-            result['sfcId'] = self.sfc_id
+        if self.scenario_field_config_id is not None:
+            result['scenarioFieldConfigId'] = self.scenario_field_config_id
         if self.sprint_id is not None:
             result['sprintId'] = self.sprint_id
         if self.start_date is not None:
             result['startDate'] = self.start_date
         if self.story_point is not None:
             result['storyPoint'] = self.story_point
         if self.tag_ids is not None:
             result['tagIds'] = self.tag_ids
         if self.task_id is not None:
             result['taskId'] = self.task_id
         if self.task_list_id is not None:
             result['taskListId'] = self.task_list_id
-        if self.taskflowstatus_id is not None:
-            result['taskflowstatusId'] = self.taskflowstatus_id
-        if self.taskstage_id is not None:
-            result['taskstageId'] = self.taskstage_id
+        if self.task_stage_id is not None:
+            result['taskStageId'] = self.task_stage_id
+        if self.taskflow_status_id is not None:
+            result['taskflowStatusId'] = self.taskflow_status_id
         if self.unique_id is not None:
             result['uniqueId'] = self.unique_id
         if self.updated is not None:
             result['updated'] = self.updated
         if self.visible is not None:
             result['visible'] = self.visible
         return result
@@ -9188,19 +9146,19 @@
             self.ancestor_ids = m.get('ancestorIds')
         if m.get('content') is not None:
             self.content = m.get('content')
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
-        self.customfields = []
-        if m.get('customfields') is not None:
-            for k in m.get('customfields'):
-                temp_model = SearchUserTaskResponseBodyResultCustomfields()
-                self.customfields.append(temp_model.from_map(k))
+        self.custom_fields = []
+        if m.get('customFields') is not None:
+            for k in m.get('customFields'):
+                temp_model = SearchUserTaskResponseBodyResultCustomFields()
+                self.custom_fields.append(temp_model.from_map(k))
         if m.get('dueDate') is not None:
             self.due_date = m.get('dueDate')
         if m.get('executorId') is not None:
             self.executor_id = m.get('executorId')
         if m.get('involveMembers') is not None:
             self.involve_members = m.get('involveMembers')
         if m.get('isArchived') is not None:
@@ -9213,91 +9171,79 @@
             self.parent_task_id = m.get('parentTaskId')
         if m.get('priority') is not None:
             self.priority = m.get('priority')
         if m.get('projectId') is not None:
             self.project_id = m.get('projectId')
         if m.get('recurrence') is not None:
             self.recurrence = m.get('recurrence')
-        if m.get('sfcId') is not None:
-            self.sfc_id = m.get('sfcId')
+        if m.get('scenarioFieldConfigId') is not None:
+            self.scenario_field_config_id = m.get('scenarioFieldConfigId')
         if m.get('sprintId') is not None:
             self.sprint_id = m.get('sprintId')
         if m.get('startDate') is not None:
             self.start_date = m.get('startDate')
         if m.get('storyPoint') is not None:
             self.story_point = m.get('storyPoint')
         if m.get('tagIds') is not None:
             self.tag_ids = m.get('tagIds')
         if m.get('taskId') is not None:
             self.task_id = m.get('taskId')
         if m.get('taskListId') is not None:
             self.task_list_id = m.get('taskListId')
-        if m.get('taskflowstatusId') is not None:
-            self.taskflowstatus_id = m.get('taskflowstatusId')
-        if m.get('taskstageId') is not None:
-            self.taskstage_id = m.get('taskstageId')
+        if m.get('taskStageId') is not None:
+            self.task_stage_id = m.get('taskStageId')
+        if m.get('taskflowStatusId') is not None:
+            self.taskflow_status_id = m.get('taskflowStatusId')
         if m.get('uniqueId') is not None:
             self.unique_id = m.get('uniqueId')
         if m.get('updated') is not None:
             self.updated = m.get('updated')
         if m.get('visible') is not None:
             self.visible = m.get('visible')
         return self
 
 
 class SearchUserTaskResponseBody(TeaModel):
     def __init__(
         self,
-        next_token: str = None,
         request_id: str = None,
         result: List[SearchUserTaskResponseBodyResult] = None,
-        total_size: int = None,
     ):
-        self.next_token = next_token
         self.request_id = request_id
         self.result = result
-        self.total_size = total_size
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
         if self.request_id is not None:
             result['requestId'] = self.request_id
         result['result'] = []
         if self.result is not None:
             for k in self.result:
                 result['result'].append(k.to_map() if k else None)
-        if self.total_size is not None:
-            result['totalSize'] = self.total_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
         if m.get('requestId') is not None:
             self.request_id = m.get('requestId')
         self.result = []
         if m.get('result') is not None:
             for k in m.get('result'):
                 temp_model = SearchUserTaskResponseBodyResult()
                 self.result.append(temp_model.from_map(k))
-        if m.get('totalSize') is not None:
-            self.total_size = m.get('totalSize')
         return self
 
 
 class SearchUserTaskResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -9666,59 +9612,59 @@
             self.title = m.get('title')
         return self
 
 
 class UpdateCustomfieldValueRequest(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
-        customfield_name: str = None,
+        custom_field_id: str = None,
+        custom_field_name: str = None,
         value: List[UpdateCustomfieldValueRequestValue] = None,
     ):
-        self.customfield_id = customfield_id
-        self.customfield_name = customfield_name
+        self.custom_field_id = custom_field_id
+        self.custom_field_name = custom_field_name
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
-        if self.customfield_name is not None:
-            result['customfieldName'] = self.customfield_name
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
+        if self.custom_field_name is not None:
+            result['customFieldName'] = self.custom_field_name
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
-        if m.get('customfieldName') is not None:
-            self.customfield_name = m.get('customfieldName')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
+        if m.get('customFieldName') is not None:
+            self.custom_field_name = m.get('customFieldName')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
                 temp_model = UpdateCustomfieldValueRequestValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
-class UpdateCustomfieldValueResponseBodyResultCustomfieldsValue(TeaModel):
+class UpdateCustomfieldValueResponseBodyResultCustomFieldsValue(TeaModel):
     def __init__(
         self,
         title: str = None,
     ):
         self.title = title
 
     def validate(self):
@@ -9737,87 +9683,87 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('title') is not None:
             self.title = m.get('title')
         return self
 
 
-class UpdateCustomfieldValueResponseBodyResultCustomfields(TeaModel):
+class UpdateCustomfieldValueResponseBodyResultCustomFields(TeaModel):
     def __init__(
         self,
-        customfield_id: str = None,
-        value: List[UpdateCustomfieldValueResponseBodyResultCustomfieldsValue] = None,
+        custom_field_id: str = None,
+        value: List[UpdateCustomfieldValueResponseBodyResultCustomFieldsValue] = None,
     ):
-        self.customfield_id = customfield_id
+        self.custom_field_id = custom_field_id
         self.value = value
 
     def validate(self):
         if self.value:
             for k in self.value:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
+        if self.custom_field_id is not None:
+            result['customFieldId'] = self.custom_field_id
         result['value'] = []
         if self.value is not None:
             for k in self.value:
                 result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
+        if m.get('customFieldId') is not None:
+            self.custom_field_id = m.get('customFieldId')
         self.value = []
         if m.get('value') is not None:
             for k in m.get('value'):
-                temp_model = UpdateCustomfieldValueResponseBodyResultCustomfieldsValue()
+                temp_model = UpdateCustomfieldValueResponseBodyResultCustomFieldsValue()
                 self.value.append(temp_model.from_map(k))
         return self
 
 
 class UpdateCustomfieldValueResponseBodyResult(TeaModel):
     def __init__(
         self,
-        customfields: List[UpdateCustomfieldValueResponseBodyResultCustomfields] = None,
+        custom_fields: List[UpdateCustomfieldValueResponseBodyResultCustomFields] = None,
     ):
-        self.customfields = customfields
+        self.custom_fields = custom_fields
 
     def validate(self):
-        if self.customfields:
-            for k in self.customfields:
+        if self.custom_fields:
+            for k in self.custom_fields:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['customfields'] = []
-        if self.customfields is not None:
-            for k in self.customfields:
-                result['customfields'].append(k.to_map() if k else None)
+        result['customFields'] = []
+        if self.custom_fields is not None:
+            for k in self.custom_fields:
+                result['customFields'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.customfields = []
-        if m.get('customfields') is not None:
-            for k in m.get('customfields'):
-                temp_model = UpdateCustomfieldValueResponseBodyResultCustomfields()
-                self.customfields.append(temp_model.from_map(k))
+        self.custom_fields = []
+        if m.get('customFields') is not None:
+            for k in m.get('customFields'):
+                temp_model = UpdateCustomfieldValueResponseBodyResultCustomFields()
+                self.custom_fields.append(temp_model.from_map(k))
         return self
 
 
 class UpdateCustomfieldValueResponseBody(TeaModel):
     def __init__(
         self,
         result: UpdateCustomfieldValueResponseBodyResult = None,
@@ -12532,25 +12478,25 @@
 
 class UpdateTaskStageResponseBodyResult(TeaModel):
     def __init__(
         self,
         accomplish_time: str = None,
         is_done: bool = None,
         project_id: str = None,
-        stage_id: str = None,
         task_id: str = None,
         task_list_id: str = None,
+        task_stage_id: str = None,
         updated: str = None,
     ):
         self.accomplish_time = accomplish_time
         self.is_done = is_done
         self.project_id = project_id
-        self.stage_id = stage_id
         self.task_id = task_id
         self.task_list_id = task_list_id
+        self.task_stage_id = task_stage_id
         self.updated = updated
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12560,38 +12506,38 @@
         result = dict()
         if self.accomplish_time is not None:
             result['accomplishTime'] = self.accomplish_time
         if self.is_done is not None:
             result['isDone'] = self.is_done
         if self.project_id is not None:
             result['projectId'] = self.project_id
-        if self.stage_id is not None:
-            result['stageId'] = self.stage_id
         if self.task_id is not None:
             result['taskId'] = self.task_id
         if self.task_list_id is not None:
             result['taskListId'] = self.task_list_id
+        if self.task_stage_id is not None:
+            result['taskStageId'] = self.task_stage_id
         if self.updated is not None:
             result['updated'] = self.updated
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('accomplishTime') is not None:
             self.accomplish_time = m.get('accomplishTime')
         if m.get('isDone') is not None:
             self.is_done = m.get('isDone')
         if m.get('projectId') is not None:
             self.project_id = m.get('projectId')
-        if m.get('stageId') is not None:
-            self.stage_id = m.get('stageId')
         if m.get('taskId') is not None:
             self.task_id = m.get('taskId')
         if m.get('taskListId') is not None:
             self.task_list_id = m.get('taskListId')
+        if m.get('taskStageId') is not None:
+            self.task_stage_id = m.get('taskStageId')
         if m.get('updated') is not None:
             self.updated = m.get('updated')
         return self
 
 
 class UpdateTaskStageResponseBody(TeaModel):
     def __init__(
@@ -12865,40 +12811,40 @@
         return self
 
 
 class UpdateTaskTaskflowstatusRequest(TeaModel):
     def __init__(
         self,
         taskflow_status_id: str = None,
-        tfs_update_note: str = None,
+        taskflow_status_update_note: str = None,
     ):
         self.taskflow_status_id = taskflow_status_id
-        self.tfs_update_note = tfs_update_note
+        self.taskflow_status_update_note = taskflow_status_update_note
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.taskflow_status_id is not None:
             result['taskflowStatusId'] = self.taskflow_status_id
-        if self.tfs_update_note is not None:
-            result['tfsUpdateNote'] = self.tfs_update_note
+        if self.taskflow_status_update_note is not None:
+            result['taskflowStatusUpdateNote'] = self.taskflow_status_update_note
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('taskflowStatusId') is not None:
             self.taskflow_status_id = m.get('taskflowStatusId')
-        if m.get('tfsUpdateNote') is not None:
-            self.tfs_update_note = m.get('tfsUpdateNote')
+        if m.get('taskflowStatusUpdateNote') is not None:
+            self.taskflow_status_update_note = m.get('taskflowStatusUpdateNote')
         return self
 
 
 class UpdateTaskTaskflowstatusResponseBodyResult(TeaModel):
     def __init__(
         self,
         updated: str = None,
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,120 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def app_login_code_gen_with_options(
+        self,
+        request: dingtalkyida__1__0_models.AppLoginCodeGenRequest,
+        headers: dingtalkyida__1__0_models.AppLoginCodeGenHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkyida__1__0_models.AppLoginCodeGenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.full_url):
+            query['fullUrl'] = request.full_url
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        body = {}
+        if not UtilClient.is_unset(request.app_key):
+            body['appKey'] = request.app_key
+        if not UtilClient.is_unset(request.sign_timestamp_str):
+            body['signTimestampStr'] = request.sign_timestamp_str
+        if not UtilClient.is_unset(request.signature):
+            body['signature'] = request.signature
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AppLoginCodeGen',
+            version='yida_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/yida/authorizations/appLoginCodes',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkyida__1__0_models.AppLoginCodeGenResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def app_login_code_gen_with_options_async(
+        self,
+        request: dingtalkyida__1__0_models.AppLoginCodeGenRequest,
+        headers: dingtalkyida__1__0_models.AppLoginCodeGenHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkyida__1__0_models.AppLoginCodeGenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.full_url):
+            query['fullUrl'] = request.full_url
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        body = {}
+        if not UtilClient.is_unset(request.app_key):
+            body['appKey'] = request.app_key
+        if not UtilClient.is_unset(request.sign_timestamp_str):
+            body['signTimestampStr'] = request.sign_timestamp_str
+        if not UtilClient.is_unset(request.signature):
+            body['signature'] = request.signature
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AppLoginCodeGen',
+            version='yida_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/yida/authorizations/appLoginCodes',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkyida__1__0_models.AppLoginCodeGenResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def app_login_code_gen(
+        self,
+        request: dingtalkyida__1__0_models.AppLoginCodeGenRequest,
+    ) -> dingtalkyida__1__0_models.AppLoginCodeGenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkyida__1__0_models.AppLoginCodeGenHeaders()
+        return self.app_login_code_gen_with_options(request, headers, runtime)
+
+    async def app_login_code_gen_async(
+        self,
+        request: dingtalkyida__1__0_models.AppLoginCodeGenRequest,
+    ) -> dingtalkyida__1__0_models.AppLoginCodeGenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkyida__1__0_models.AppLoginCodeGenHeaders()
+        return await self.app_login_code_gen_with_options_async(request, headers, runtime)
+
     def batch_get_form_data_by_id_list_with_options(
         self,
         request: dingtalkyida__1__0_models.BatchGetFormDataByIdListRequest,
         headers: dingtalkyida__1__0_models.BatchGetFormDataByIdListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkyida__1__0_models.BatchGetFormDataByIdListResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,168 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class AppLoginCodeGenHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class AppLoginCodeGenRequest(TeaModel):
+    def __init__(
+        self,
+        app_key: str = None,
+        sign_timestamp_str: str = None,
+        signature: str = None,
+        full_url: str = None,
+        user_id: str = None,
+    ):
+        self.app_key = app_key
+        self.sign_timestamp_str = sign_timestamp_str
+        self.signature = signature
+        self.full_url = full_url
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_key is not None:
+            result['appKey'] = self.app_key
+        if self.sign_timestamp_str is not None:
+            result['signTimestampStr'] = self.sign_timestamp_str
+        if self.signature is not None:
+            result['signature'] = self.signature
+        if self.full_url is not None:
+            result['fullUrl'] = self.full_url
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appKey') is not None:
+            self.app_key = m.get('appKey')
+        if m.get('signTimestampStr') is not None:
+            self.sign_timestamp_str = m.get('signTimestampStr')
+        if m.get('signature') is not None:
+            self.signature = m.get('signature')
+        if m.get('fullUrl') is not None:
+            self.full_url = m.get('fullUrl')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class AppLoginCodeGenResponseBody(TeaModel):
+    def __init__(
+        self,
+        login_code: str = None,
+    ):
+        self.login_code = login_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.login_code is not None:
+            result['loginCode'] = self.login_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('loginCode') is not None:
+            self.login_code = m.get('loginCode')
+        return self
+
+
+class AppLoginCodeGenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AppLoginCodeGenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AppLoginCodeGenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchGetFormDataByIdListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.11
+Version: 2.0.12
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.11/setup.py` & `alibabacloud_dingtalk-2.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 09/05/2023
+Created on 12/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```


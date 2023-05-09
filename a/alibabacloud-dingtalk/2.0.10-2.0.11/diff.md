# Comparing `tmp/alibabacloud_dingtalk-2.0.10.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.10.tar", last modified: Fri Apr 28 03:36:56 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.11.tar", last modified: Tue May  9 01:56:59 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.10.tar` & `alibabacloud_dingtalk-2.0.11.tar`

### file list

```diff
@@ -1,353 +1,357 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/
--rw-r--r--   0 root         (0) root         (0)    19297 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148888 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   274109 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   565599 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138548 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   328853 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34674 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   100519 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   387928 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   511378 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   308062 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   429056 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89334 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133902 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87266 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130480 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129226 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157291 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260594 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   414815 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10094 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26851 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   147980 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175082 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   370377 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   459526 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   682489 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11618 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/
+-rw-r--r--   0 root         (0) root         (0)    19362 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148888 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   274109 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   565599 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138548 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   328853 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220322 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   547684 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   308062 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   429056 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89334 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133902 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   523174 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   756557 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87266 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130480 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129226 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157569 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260594 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   414815 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44880 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81308 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   147980 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53454 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118368 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175082 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   370377 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   459526 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   682489 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11743 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-09 01:56:59.000000 alibabacloud_dingtalk-2.0.11/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.10/ChangeLog.md` & `alibabacloud_dingtalk-2.0.11/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-28 Version: 2.0.10
+- Update AddOfficialAccountFollower.
+
 2023-04-26 Version: 2.0.0
 - Update AddOfficialAccountFollower.
 
 2023-04-26 Version: 2.0.0
 - Update AddOfficialAccountFollower.
 
 2023-04-21 Version: 1.5.65
```

### Comparing `alibabacloud_dingtalk-2.0.10/LICENSE` & `alibabacloud_dingtalk-2.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/PKG-INFO` & `alibabacloud_dingtalk-2.0.11/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.10
+Version: 2.0.11
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.10/README-CN.md` & `alibabacloud_dingtalk-2.0.11/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/README.md` & `alibabacloud_dingtalk-2.0.11/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,16 @@
         headers: dingtalkcard__1__0_models.CreateAndDeliverHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcard__1__0_models.CreateAndDeliverResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.callback_route_key):
             body['callbackRouteKey'] = request.callback_route_key
+        if not UtilClient.is_unset(request.callback_type):
+            body['callbackType'] = request.callback_type
         if not UtilClient.is_unset(request.card_data):
             body['cardData'] = request.card_data
         if not UtilClient.is_unset(request.card_template_id):
             body['cardTemplateId'] = request.card_template_id
         if not UtilClient.is_unset(request.co_feed_open_deliver_model):
             body['coFeedOpenDeliverModel'] = request.co_feed_open_deliver_model
         if not UtilClient.is_unset(request.co_feed_open_space_model):
@@ -206,14 +208,16 @@
         headers: dingtalkcard__1__0_models.CreateAndDeliverHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcard__1__0_models.CreateAndDeliverResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.callback_route_key):
             body['callbackRouteKey'] = request.callback_route_key
+        if not UtilClient.is_unset(request.callback_type):
+            body['callbackType'] = request.callback_type
         if not UtilClient.is_unset(request.card_data):
             body['cardData'] = request.card_data
         if not UtilClient.is_unset(request.card_template_id):
             body['cardTemplateId'] = request.card_template_id
         if not UtilClient.is_unset(request.co_feed_open_deliver_model):
             body['coFeedOpenDeliverModel'] = request.co_feed_open_deliver_model
         if not UtilClient.is_unset(request.co_feed_open_space_model):
@@ -291,14 +295,16 @@
         headers: dingtalkcard__1__0_models.CreateCardHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcard__1__0_models.CreateCardResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.callback_route_key):
             body['callbackRouteKey'] = request.callback_route_key
+        if not UtilClient.is_unset(request.callback_type):
+            body['callbackType'] = request.callback_type
         if not UtilClient.is_unset(request.card_data):
             body['cardData'] = request.card_data
         if not UtilClient.is_unset(request.card_template_id):
             body['cardTemplateId'] = request.card_template_id
         if not UtilClient.is_unset(request.co_feed_open_space_model):
             body['coFeedOpenSpaceModel'] = request.co_feed_open_space_model
         if not UtilClient.is_unset(request.im_group_open_space_model):
@@ -348,14 +354,16 @@
         headers: dingtalkcard__1__0_models.CreateCardHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcard__1__0_models.CreateCardResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.callback_route_key):
             body['callbackRouteKey'] = request.callback_route_key
+        if not UtilClient.is_unset(request.callback_type):
+            body['callbackType'] = request.callback_type
         if not UtilClient.is_unset(request.card_data):
             body['cardData'] = request.card_data
         if not UtilClient.is_unset(request.card_template_id):
             body['cardTemplateId'] = request.card_template_id
         if not UtilClient.is_unset(request.co_feed_open_space_model):
             body['coFeedOpenSpaceModel'] = request.co_feed_open_space_model
         if not UtilClient.is_unset(request.im_group_open_space_model):
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1145,14 +1145,15 @@
         return self
 
 
 class CreateAndDeliverRequest(TeaModel):
     def __init__(
         self,
         callback_route_key: str = None,
+        callback_type: str = None,
         card_data: CreateAndDeliverRequestCardData = None,
         card_template_id: str = None,
         co_feed_open_deliver_model: CreateAndDeliverRequestCoFeedOpenDeliverModel = None,
         co_feed_open_space_model: CreateAndDeliverRequestCoFeedOpenSpaceModel = None,
         doc_open_deliver_model: CreateAndDeliverRequestDocOpenDeliverModel = None,
         im_group_open_deliver_model: CreateAndDeliverRequestImGroupOpenDeliverModel = None,
         im_group_open_space_model: CreateAndDeliverRequestImGroupOpenSpaceModel = None,
@@ -1164,14 +1165,15 @@
         private_data: Dict[str, PrivateDataValue] = None,
         top_open_deliver_model: CreateAndDeliverRequestTopOpenDeliverModel = None,
         top_open_space_model: CreateAndDeliverRequestTopOpenSpaceModel = None,
         user_id: str = None,
         user_id_type: int = None,
     ):
         self.callback_route_key = callback_route_key
+        self.callback_type = callback_type
         self.card_data = card_data
         self.card_template_id = card_template_id
         self.co_feed_open_deliver_model = co_feed_open_deliver_model
         self.co_feed_open_space_model = co_feed_open_space_model
         self.doc_open_deliver_model = doc_open_deliver_model
         self.im_group_open_deliver_model = im_group_open_deliver_model
         self.im_group_open_space_model = im_group_open_space_model
@@ -1218,14 +1220,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.callback_route_key is not None:
             result['callbackRouteKey'] = self.callback_route_key
+        if self.callback_type is not None:
+            result['callbackType'] = self.callback_type
         if self.card_data is not None:
             result['cardData'] = self.card_data.to_map()
         if self.card_template_id is not None:
             result['cardTemplateId'] = self.card_template_id
         if self.co_feed_open_deliver_model is not None:
             result['coFeedOpenDeliverModel'] = self.co_feed_open_deliver_model.to_map()
         if self.co_feed_open_space_model is not None:
@@ -1260,14 +1264,16 @@
             result['userIdType'] = self.user_id_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('callbackRouteKey') is not None:
             self.callback_route_key = m.get('callbackRouteKey')
+        if m.get('callbackType') is not None:
+            self.callback_type = m.get('callbackType')
         if m.get('cardData') is not None:
             temp_model = CreateAndDeliverRequestCardData()
             self.card_data = temp_model.from_map(m['cardData'])
         if m.get('cardTemplateId') is not None:
             self.card_template_id = m.get('cardTemplateId')
         if m.get('coFeedOpenDeliverModel') is not None:
             temp_model = CreateAndDeliverRequestCoFeedOpenDeliverModel()
@@ -1953,27 +1959,29 @@
         return self
 
 
 class CreateCardRequest(TeaModel):
     def __init__(
         self,
         callback_route_key: str = None,
+        callback_type: str = None,
         card_data: CreateCardRequestCardData = None,
         card_template_id: str = None,
         co_feed_open_space_model: CreateCardRequestCoFeedOpenSpaceModel = None,
         im_group_open_space_model: CreateCardRequestImGroupOpenSpaceModel = None,
         im_robot_open_space_model: CreateCardRequestImRobotOpenSpaceModel = None,
         open_dynamic_data_config: CreateCardRequestOpenDynamicDataConfig = None,
         out_track_id: str = None,
         private_data: Dict[str, PrivateDataValue] = None,
         top_open_space_model: CreateCardRequestTopOpenSpaceModel = None,
         user_id: str = None,
         user_id_type: int = None,
     ):
         self.callback_route_key = callback_route_key
+        self.callback_type = callback_type
         self.card_data = card_data
         self.card_template_id = card_template_id
         self.co_feed_open_space_model = co_feed_open_space_model
         self.im_group_open_space_model = im_group_open_space_model
         self.im_robot_open_space_model = im_robot_open_space_model
         self.open_dynamic_data_config = open_dynamic_data_config
         self.out_track_id = out_track_id
@@ -2004,14 +2012,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.callback_route_key is not None:
             result['callbackRouteKey'] = self.callback_route_key
+        if self.callback_type is not None:
+            result['callbackType'] = self.callback_type
         if self.card_data is not None:
             result['cardData'] = self.card_data.to_map()
         if self.card_template_id is not None:
             result['cardTemplateId'] = self.card_template_id
         if self.co_feed_open_space_model is not None:
             result['coFeedOpenSpaceModel'] = self.co_feed_open_space_model.to_map()
         if self.im_group_open_space_model is not None:
@@ -2034,14 +2044,16 @@
             result['userIdType'] = self.user_id_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('callbackRouteKey') is not None:
             self.callback_route_key = m.get('callbackRouteKey')
+        if m.get('callbackType') is not None:
+            self.callback_type = m.get('callbackType')
         if m.get('cardData') is not None:
             temp_model = CreateCardRequestCardData()
             self.card_data = temp_model.from_map(m['cardData'])
         if m.get('cardTemplateId') is not None:
             self.card_template_id = m.get('cardTemplateId')
         if m.get('coFeedOpenSpaceModel') is not None:
             temp_model = CreateCardRequestCoFeedOpenSpaceModel()
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4199,14 +4199,104 @@
         self,
         request: dingtalkdatacenter__1__0_models.QueryOfficialDatasetListRequest,
     ) -> dingtalkdatacenter__1__0_models.QueryOfficialDatasetListResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkdatacenter__1__0_models.QueryOfficialDatasetListHeaders()
         return await self.query_official_dataset_list_with_options_async(request, headers, runtime)
 
+    def query_official_form_data_with_options(
+        self,
+        request: dingtalkdatacenter__1__0_models.QueryOfficialFormDataRequest,
+        headers: dingtalkdatacenter__1__0_models.QueryOfficialFormDataHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdatacenter__1__0_models.QueryOfficialFormDataResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.param):
+            body['param'] = request.param
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
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
+            action='QueryOfficialFormData',
+            version='datacenter_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/datacenter/datas/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdatacenter__1__0_models.QueryOfficialFormDataResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_official_form_data_with_options_async(
+        self,
+        request: dingtalkdatacenter__1__0_models.QueryOfficialFormDataRequest,
+        headers: dingtalkdatacenter__1__0_models.QueryOfficialFormDataHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdatacenter__1__0_models.QueryOfficialFormDataResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.param):
+            body['param'] = request.param
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
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
+            action='QueryOfficialFormData',
+            version='datacenter_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/datacenter/datas/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdatacenter__1__0_models.QueryOfficialFormDataResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_official_form_data(
+        self,
+        request: dingtalkdatacenter__1__0_models.QueryOfficialFormDataRequest,
+    ) -> dingtalkdatacenter__1__0_models.QueryOfficialFormDataResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkdatacenter__1__0_models.QueryOfficialFormDataHeaders()
+        return self.query_official_form_data_with_options(request, headers, runtime)
+
+    async def query_official_form_data_async(
+        self,
+        request: dingtalkdatacenter__1__0_models.QueryOfficialFormDataRequest,
+    ) -> dingtalkdatacenter__1__0_models.QueryOfficialFormDataResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkdatacenter__1__0_models.QueryOfficialFormDataHeaders()
+        return await self.query_official_form_data_with_options_async(request, headers, runtime)
+
     def query_online_user_statistical_data_with_options(
         self,
         request: dingtalkdatacenter__1__0_models.QueryOnlineUserStatisticalDataRequest,
         headers: dingtalkdatacenter__1__0_models.QueryOnlineUserStatisticalDataHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkdatacenter__1__0_models.QueryOnlineUserStatisticalDataResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7861,14 +7861,157 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryOfficialDatasetListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryOfficialFormDataHeaders(TeaModel):
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
+class QueryOfficialFormDataRequest(TeaModel):
+    def __init__(
+        self,
+        param: str = None,
+        user_id: str = None,
+    ):
+        self.param = param
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
+        if self.param is not None:
+            result['param'] = self.param
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('param') is not None:
+            self.param = m.get('param')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryOfficialFormDataResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: str = None,
+        success: bool = None,
+    ):
+        self.result = result
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
+        if self.result is not None:
+            result['result'] = self.result
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class QueryOfficialFormDataResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryOfficialFormDataResponseBody = None,
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
+            temp_model = QueryOfficialFormDataResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryOnlineUserStatisticalDataHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2857,22 +2857,24 @@
 class ListInnerAppVersionResponseBodyAppVersionList(TeaModel):
     def __init__(
         self,
         app_version: str = None,
         app_version_id: int = None,
         app_version_type: int = None,
         create_time: str = None,
+        entrance_link: str = None,
         mini_app_id: str = None,
         mini_app_on_pc: bool = None,
         modify_time: str = None,
     ):
         self.app_version = app_version
         self.app_version_id = app_version_id
         self.app_version_type = app_version_type
         self.create_time = create_time
+        self.entrance_link = entrance_link
         self.mini_app_id = mini_app_id
         self.mini_app_on_pc = mini_app_on_pc
         self.modify_time = modify_time
 
     def validate(self):
         pass
 
@@ -2886,14 +2888,16 @@
             result['appVersion'] = self.app_version
         if self.app_version_id is not None:
             result['appVersionId'] = self.app_version_id
         if self.app_version_type is not None:
             result['appVersionType'] = self.app_version_type
         if self.create_time is not None:
             result['createTime'] = self.create_time
+        if self.entrance_link is not None:
+            result['entranceLink'] = self.entrance_link
         if self.mini_app_id is not None:
             result['miniAppId'] = self.mini_app_id
         if self.mini_app_on_pc is not None:
             result['miniAppOnPc'] = self.mini_app_on_pc
         if self.modify_time is not None:
             result['modifyTime'] = self.modify_time
         return result
@@ -2904,14 +2908,16 @@
             self.app_version = m.get('appVersion')
         if m.get('appVersionId') is not None:
             self.app_version_id = m.get('appVersionId')
         if m.get('appVersionType') is not None:
             self.app_version_type = m.get('appVersionType')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
+        if m.get('entranceLink') is not None:
+            self.entrance_link = m.get('entranceLink')
         if m.get('miniAppId') is not None:
             self.mini_app_id = m.get('miniAppId')
         if m.get('miniAppOnPc') is not None:
             self.mini_app_on_pc = m.get('miniAppOnPc')
         if m.get('modifyTime') is not None:
             self.modify_time = m.get('modifyTime')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.storage_2_0 import models as dingtalkstorage__2__0_models
+from alibabacloud_dingtalk.wiki_1_0 import models as dingtalkwiki__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,214 +25,178 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def commit_file_with_options(
+    def wiki_words_detail_with_options(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.CommitFileRequest,
-        headers: dingtalkstorage__2__0_models.CommitFileHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsDetailHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkstorage__2__0_models.CommitFileResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.union_id):
-            query['unionId'] = request.union_id
-        body = {}
-        if not UtilClient.is_unset(request.name):
-            body['name'] = request.name
-        if not UtilClient.is_unset(request.option):
-            body['option'] = request.option
-        if not UtilClient.is_unset(request.upload_key):
-            body['uploadKey'] = request.upload_key
+        if not UtilClient.is_unset(request.word_name):
+            query['wordName'] = request.word_name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query),
-            body=OpenApiUtilClient.parse_to_map(body)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CommitFile',
-            version='storage_2.0',
+            action='WikiWordsDetail',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/storage/spaces/files/{parent_dentry_uuid}/commit',
-            method='POST',
+            pathname=f'/v1.0/wiki/words/details',
+            method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkstorage__2__0_models.CommitFileResponse(),
+            dingtalkwiki__1__0_models.WikiWordsDetailResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def commit_file_with_options_async(
+    async def wiki_words_detail_with_options_async(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.CommitFileRequest,
-        headers: dingtalkstorage__2__0_models.CommitFileHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsDetailHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkstorage__2__0_models.CommitFileResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.union_id):
-            query['unionId'] = request.union_id
-        body = {}
-        if not UtilClient.is_unset(request.name):
-            body['name'] = request.name
-        if not UtilClient.is_unset(request.option):
-            body['option'] = request.option
-        if not UtilClient.is_unset(request.upload_key):
-            body['uploadKey'] = request.upload_key
+        if not UtilClient.is_unset(request.word_name):
+            query['wordName'] = request.word_name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query),
-            body=OpenApiUtilClient.parse_to_map(body)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CommitFile',
-            version='storage_2.0',
+            action='WikiWordsDetail',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/storage/spaces/files/{parent_dentry_uuid}/commit',
-            method='POST',
+            pathname=f'/v1.0/wiki/words/details',
+            method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkstorage__2__0_models.CommitFileResponse(),
+            dingtalkwiki__1__0_models.WikiWordsDetailResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def commit_file(
+    def wiki_words_detail(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.CommitFileRequest,
-    ) -> dingtalkstorage__2__0_models.CommitFileResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkstorage__2__0_models.CommitFileHeaders()
-        return self.commit_file_with_options(parent_dentry_uuid, request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsDetailHeaders()
+        return self.wiki_words_detail_with_options(request, headers, runtime)
 
-    async def commit_file_async(
+    async def wiki_words_detail_async(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.CommitFileRequest,
-    ) -> dingtalkstorage__2__0_models.CommitFileResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkstorage__2__0_models.CommitFileHeaders()
-        return await self.commit_file_with_options_async(parent_dentry_uuid, request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsDetailHeaders()
+        return await self.wiki_words_detail_with_options_async(request, headers, runtime)
 
-    def get_file_upload_info_with_options(
+    def wiki_words_parse_with_options(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.GetFileUploadInfoRequest,
-        headers: dingtalkstorage__2__0_models.GetFileUploadInfoHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsParseHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkstorage__2__0_models.GetFileUploadInfoResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.union_id):
-            query['unionId'] = request.union_id
         body = {}
-        if not UtilClient.is_unset(request.option):
-            body['option'] = request.option
-        if not UtilClient.is_unset(request.protocol):
-            body['protocol'] = request.protocol
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='GetFileUploadInfo',
-            version='storage_2.0',
+            action='WikiWordsParse',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/storage/spaces/files/{parent_dentry_uuid}/uploadInfos/query',
+            pathname=f'/v1.0/wiki/words/parse',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkstorage__2__0_models.GetFileUploadInfoResponse(),
+            dingtalkwiki__1__0_models.WikiWordsParseResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def get_file_upload_info_with_options_async(
+    async def wiki_words_parse_with_options_async(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.GetFileUploadInfoRequest,
-        headers: dingtalkstorage__2__0_models.GetFileUploadInfoHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsParseHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkstorage__2__0_models.GetFileUploadInfoResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.union_id):
-            query['unionId'] = request.union_id
         body = {}
-        if not UtilClient.is_unset(request.option):
-            body['option'] = request.option
-        if not UtilClient.is_unset(request.protocol):
-            body['protocol'] = request.protocol
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='GetFileUploadInfo',
-            version='storage_2.0',
+            action='WikiWordsParse',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/storage/spaces/files/{parent_dentry_uuid}/uploadInfos/query',
+            pathname=f'/v1.0/wiki/words/parse',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkstorage__2__0_models.GetFileUploadInfoResponse(),
+            dingtalkwiki__1__0_models.WikiWordsParseResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def get_file_upload_info(
+    def wiki_words_parse(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.GetFileUploadInfoRequest,
-    ) -> dingtalkstorage__2__0_models.GetFileUploadInfoResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkstorage__2__0_models.GetFileUploadInfoHeaders()
-        return self.get_file_upload_info_with_options(parent_dentry_uuid, request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsParseHeaders()
+        return self.wiki_words_parse_with_options(request, headers, runtime)
 
-    async def get_file_upload_info_async(
+    async def wiki_words_parse_async(
         self,
-        parent_dentry_uuid: str,
-        request: dingtalkstorage__2__0_models.GetFileUploadInfoRequest,
-    ) -> dingtalkstorage__2__0_models.GetFileUploadInfoResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkstorage__2__0_models.GetFileUploadInfoHeaders()
-        return await self.get_file_upload_info_with_options_async(parent_dentry_uuid, request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsParseHeaders()
+        return await self.wiki_words_parse_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,195 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
-class DentryAppPropertiesValue(TeaModel):
+class GetDingPortalDetailHeaders(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        value: str = None,
-        visibility: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.name = name
-        self.value = value
-        self.visibility = visibility
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        if self.value is not None:
-            result['value'] = self.value
-        if self.visibility is not None:
-            result['visibility'] = self.visibility
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('value') is not None:
-            self.value = m.get('value')
-        if m.get('visibility') is not None:
-            self.visibility = m.get('visibility')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CommitFileHeaders(TeaModel):
+class GetDingPortalDetailResponseBodyPages(TeaModel):
+    def __init__(
+        self,
+        all_visible: bool = None,
+        dept_ids: List[int] = None,
+        page_name: str = None,
+        page_uuid: str = None,
+        role_ids: List[int] = None,
+        userids: List[str] = None,
+    ):
+        self.all_visible = all_visible
+        self.dept_ids = dept_ids
+        self.page_name = page_name
+        self.page_uuid = page_uuid
+        self.role_ids = role_ids
+        self.userids = userids
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
+        if self.all_visible is not None:
+            result['allVisible'] = self.all_visible
+        if self.dept_ids is not None:
+            result['deptIds'] = self.dept_ids
+        if self.page_name is not None:
+            result['pageName'] = self.page_name
+        if self.page_uuid is not None:
+            result['pageUuid'] = self.page_uuid
+        if self.role_ids is not None:
+            result['roleIds'] = self.role_ids
+        if self.userids is not None:
+            result['userids'] = self.userids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('allVisible') is not None:
+            self.all_visible = m.get('allVisible')
+        if m.get('deptIds') is not None:
+            self.dept_ids = m.get('deptIds')
+        if m.get('pageName') is not None:
+            self.page_name = m.get('pageName')
+        if m.get('pageUuid') is not None:
+            self.page_uuid = m.get('pageUuid')
+        if m.get('roleIds') is not None:
+            self.role_ids = m.get('roleIds')
+        if m.get('userids') is not None:
+            self.userids = m.get('userids')
+        return self
+
+
+class GetDingPortalDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        app_uuid: str = None,
+        ding_portal_name: str = None,
+        pages: List[GetDingPortalDetailResponseBodyPages] = None,
+    ):
+        self.app_uuid = app_uuid
+        self.ding_portal_name = ding_portal_name
+        self.pages = pages
+
+    def validate(self):
+        if self.pages:
+            for k in self.pages:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_uuid is not None:
+            result['appUuid'] = self.app_uuid
+        if self.ding_portal_name is not None:
+            result['dingPortalName'] = self.ding_portal_name
+        result['pages'] = []
+        if self.pages is not None:
+            for k in self.pages:
+                result['pages'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appUuid') is not None:
+            self.app_uuid = m.get('appUuid')
+        if m.get('dingPortalName') is not None:
+            self.ding_portal_name = m.get('dingPortalName')
+        self.pages = []
+        if m.get('pages') is not None:
+            for k in m.get('pages'):
+                temp_model = GetDingPortalDetailResponseBodyPages()
+                self.pages.append(temp_model.from_map(k))
+        return self
+
+
+class GetDingPortalDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDingPortalDetailResponseBody = None,
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
+            temp_model = GetDingPortalDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetPluginPermissionPointHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -72,428 +214,395 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CommitFileRequestOptionAppProperties(TeaModel):
+class GetPluginPermissionPointRequest(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        value: str = None,
-        visibility: str = None,
+        mini_app_id: str = None,
     ):
-        self.name = name
-        self.value = value
-        self.visibility = visibility
+        self.mini_app_id = mini_app_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        if self.value is not None:
-            result['value'] = self.value
-        if self.visibility is not None:
-            result['visibility'] = self.visibility
+        if self.mini_app_id is not None:
+            result['miniAppId'] = self.mini_app_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('value') is not None:
-            self.value = m.get('value')
-        if m.get('visibility') is not None:
-            self.visibility = m.get('visibility')
+        if m.get('miniAppId') is not None:
+            self.mini_app_id = m.get('miniAppId')
         return self
 
 
-class CommitFileRequestOption(TeaModel):
+class GetPluginPermissionPointResponseBody(TeaModel):
     def __init__(
         self,
-        app_properties: List[CommitFileRequestOptionAppProperties] = None,
-        conflict_strategy: str = None,
-        convert_to_online_doc: bool = None,
-        convert_to_online_doc_target_document_type: str = None,
-        size: int = None,
+        permission_point_list: List[str] = None,
     ):
-        self.app_properties = app_properties
-        self.conflict_strategy = conflict_strategy
-        self.convert_to_online_doc = convert_to_online_doc
-        self.convert_to_online_doc_target_document_type = convert_to_online_doc_target_document_type
-        self.size = size
+        self.permission_point_list = permission_point_list
 
     def validate(self):
-        if self.app_properties:
-            for k in self.app_properties:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['appProperties'] = []
-        if self.app_properties is not None:
-            for k in self.app_properties:
-                result['appProperties'].append(k.to_map() if k else None)
-        if self.conflict_strategy is not None:
-            result['conflictStrategy'] = self.conflict_strategy
-        if self.convert_to_online_doc is not None:
-            result['convertToOnlineDoc'] = self.convert_to_online_doc
-        if self.convert_to_online_doc_target_document_type is not None:
-            result['convertToOnlineDocTargetDocumentType'] = self.convert_to_online_doc_target_document_type
-        if self.size is not None:
-            result['size'] = self.size
+        if self.permission_point_list is not None:
+            result['permissionPointList'] = self.permission_point_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.app_properties = []
-        if m.get('appProperties') is not None:
-            for k in m.get('appProperties'):
-                temp_model = CommitFileRequestOptionAppProperties()
-                self.app_properties.append(temp_model.from_map(k))
-        if m.get('conflictStrategy') is not None:
-            self.conflict_strategy = m.get('conflictStrategy')
-        if m.get('convertToOnlineDoc') is not None:
-            self.convert_to_online_doc = m.get('convertToOnlineDoc')
-        if m.get('convertToOnlineDocTargetDocumentType') is not None:
-            self.convert_to_online_doc_target_document_type = m.get('convertToOnlineDocTargetDocumentType')
-        if m.get('size') is not None:
-            self.size = m.get('size')
+        if m.get('permissionPointList') is not None:
+            self.permission_point_list = m.get('permissionPointList')
         return self
 
 
-class CommitFileRequest(TeaModel):
+class GetPluginPermissionPointResponse(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        option: CommitFileRequestOption = None,
-        upload_key: str = None,
-        union_id: str = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetPluginPermissionPointResponseBody = None,
     ):
-        self.name = name
-        self.option = option
-        self.upload_key = upload_key
-        self.union_id = union_id
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
 
     def validate(self):
-        if self.option:
-            self.option.validate()
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        if self.option is not None:
-            result['option'] = self.option.to_map()
-        if self.upload_key is not None:
-            result['uploadKey'] = self.upload_key
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('option') is not None:
-            temp_model = CommitFileRequestOption()
-            self.option = temp_model.from_map(m['option'])
-        if m.get('uploadKey') is not None:
-            self.upload_key = m.get('uploadKey')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPluginPermissionPointResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetPluginRuleCheckInfoHeaders(TeaModel):
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
         return self
 
 
-class CommitFileResponseBodyDentryProperties(TeaModel):
+class GetPluginRuleCheckInfoRequest(TeaModel):
     def __init__(
         self,
-        read_only: bool = None,
+        mini_app_id: str = None,
     ):
-        self.read_only = read_only
+        self.mini_app_id = mini_app_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.read_only is not None:
-            result['readOnly'] = self.read_only
+        if self.mini_app_id is not None:
+            result['miniAppId'] = self.mini_app_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('readOnly') is not None:
-            self.read_only = m.get('readOnly')
+        if m.get('miniAppId') is not None:
+            self.mini_app_id = m.get('miniAppId')
         return self
 
 
-class CommitFileResponseBodyDentryThumbnail(TeaModel):
+class GetPluginRuleCheckInfoResponseBody(TeaModel):
     def __init__(
         self,
-        height: int = None,
-        url: str = None,
-        width: int = None,
+        pack_code: str = None,
+        plugin_rule_check_detail: str = None,
     ):
-        self.height = height
-        self.url = url
-        self.width = width
+        self.pack_code = pack_code
+        self.plugin_rule_check_detail = plugin_rule_check_detail
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.height is not None:
-            result['height'] = self.height
-        if self.url is not None:
-            result['url'] = self.url
-        if self.width is not None:
-            result['width'] = self.width
+        if self.pack_code is not None:
+            result['packCode'] = self.pack_code
+        if self.plugin_rule_check_detail is not None:
+            result['pluginRuleCheckDetail'] = self.plugin_rule_check_detail
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('height') is not None:
-            self.height = m.get('height')
-        if m.get('url') is not None:
-            self.url = m.get('url')
-        if m.get('width') is not None:
-            self.width = m.get('width')
+        if m.get('packCode') is not None:
+            self.pack_code = m.get('packCode')
+        if m.get('pluginRuleCheckDetail') is not None:
+            self.plugin_rule_check_detail = m.get('pluginRuleCheckDetail')
         return self
 
 
-class CommitFileResponseBodyDentry(TeaModel):
+class GetPluginRuleCheckInfoResponse(TeaModel):
     def __init__(
         self,
-        app_properties: Dict[str, List[DentryAppPropertiesValue]] = None,
-        category: str = None,
-        create_time: str = None,
-        creator_id: str = None,
-        extension: str = None,
-        id: str = None,
-        modified_time: str = None,
-        modifier_id: str = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetPluginRuleCheckInfoResponseBody = None,
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
+            temp_model = GetPluginRuleCheckInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListWorkBenchGroupHeaders(TeaModel):
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
+class ListWorkBenchGroupRequest(TeaModel):
+    def __init__(
+        self,
+        ecological_corp_id: str = None,
+        group_type: str = None,
+        op_union_id: str = None,
+    ):
+        self.ecological_corp_id = ecological_corp_id
+        self.group_type = group_type
+        self.op_union_id = op_union_id
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
+        if self.ecological_corp_id is not None:
+            result['ecologicalCorpId'] = self.ecological_corp_id
+        if self.group_type is not None:
+            result['groupType'] = self.group_type
+        if self.op_union_id is not None:
+            result['opUnionId'] = self.op_union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ecologicalCorpId') is not None:
+            self.ecological_corp_id = m.get('ecologicalCorpId')
+        if m.get('groupType') is not None:
+            self.group_type = m.get('groupType')
+        if m.get('opUnionId') is not None:
+            self.op_union_id = m.get('opUnionId')
+        return self
+
+
+class ListWorkBenchGroupResponseBodyGroupList(TeaModel):
+    def __init__(
+        self,
+        component_id: str = None,
         name: str = None,
-        parent_id: str = None,
-        partition_type: str = None,
-        path: str = None,
-        properties: CommitFileResponseBodyDentryProperties = None,
-        size: int = None,
-        space_id: str = None,
-        status: str = None,
-        storage_driver: str = None,
-        thumbnail: CommitFileResponseBodyDentryThumbnail = None,
-        type: str = None,
-        uuid: str = None,
-        version: int = None,
-    ):
-        self.app_properties = app_properties
-        self.category = category
-        self.create_time = create_time
-        self.creator_id = creator_id
-        self.extension = extension
-        self.id = id
-        self.modified_time = modified_time
-        self.modifier_id = modifier_id
+    ):
+        self.component_id = component_id
         self.name = name
-        self.parent_id = parent_id
-        self.partition_type = partition_type
-        self.path = path
-        self.properties = properties
-        self.size = size
-        self.space_id = space_id
-        self.status = status
-        self.storage_driver = storage_driver
-        self.thumbnail = thumbnail
-        self.type = type
-        self.uuid = uuid
-        self.version = version
-
-    def validate(self):
-        if self.app_properties:
-            for v in self.app_properties.values():
-                for k1 in v:
-                    if k1:
-                        k1.validate()
-        if self.properties:
-            self.properties.validate()
-        if self.thumbnail:
-            self.thumbnail.validate()
+
+    def validate(self):
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['appProperties'] = {}
-        if self.app_properties is not None:
-            for k, v in self.app_properties.items():
-                l1 = []
-                for k1 in v:
-                    l1.append(k1.to_map() if k1 else None)
-                result['appProperties'][k] = l1
-        if self.category is not None:
-            result['category'] = self.category
-        if self.create_time is not None:
-            result['createTime'] = self.create_time
-        if self.creator_id is not None:
-            result['creatorId'] = self.creator_id
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.id is not None:
-            result['id'] = self.id
-        if self.modified_time is not None:
-            result['modifiedTime'] = self.modified_time
-        if self.modifier_id is not None:
-            result['modifierId'] = self.modifier_id
+        if self.component_id is not None:
+            result['componentId'] = self.component_id
         if self.name is not None:
             result['name'] = self.name
-        if self.parent_id is not None:
-            result['parentId'] = self.parent_id
-        if self.partition_type is not None:
-            result['partitionType'] = self.partition_type
-        if self.path is not None:
-            result['path'] = self.path
-        if self.properties is not None:
-            result['properties'] = self.properties.to_map()
-        if self.size is not None:
-            result['size'] = self.size
-        if self.space_id is not None:
-            result['spaceId'] = self.space_id
-        if self.status is not None:
-            result['status'] = self.status
-        if self.storage_driver is not None:
-            result['storageDriver'] = self.storage_driver
-        if self.thumbnail is not None:
-            result['thumbnail'] = self.thumbnail.to_map()
-        if self.type is not None:
-            result['type'] = self.type
-        if self.uuid is not None:
-            result['uuid'] = self.uuid
-        if self.version is not None:
-            result['version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.app_properties = {}
-        if m.get('appProperties') is not None:
-            for k, v in m.get('appProperties').items():
-                l1 = []
-                for k1 in v:
-                    temp_model = DentryAppPropertiesValue()
-                    l1.append(temp_model.from_map(k1))
-                self.app_properties['k'] = l1
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('createTime') is not None:
-            self.create_time = m.get('createTime')
-        if m.get('creatorId') is not None:
-            self.creator_id = m.get('creatorId')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('modifiedTime') is not None:
-            self.modified_time = m.get('modifiedTime')
-        if m.get('modifierId') is not None:
-            self.modifier_id = m.get('modifierId')
+        if m.get('componentId') is not None:
+            self.component_id = m.get('componentId')
         if m.get('name') is not None:
             self.name = m.get('name')
-        if m.get('parentId') is not None:
-            self.parent_id = m.get('parentId')
-        if m.get('partitionType') is not None:
-            self.partition_type = m.get('partitionType')
-        if m.get('path') is not None:
-            self.path = m.get('path')
-        if m.get('properties') is not None:
-            temp_model = CommitFileResponseBodyDentryProperties()
-            self.properties = temp_model.from_map(m['properties'])
-        if m.get('size') is not None:
-            self.size = m.get('size')
-        if m.get('spaceId') is not None:
-            self.space_id = m.get('spaceId')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('storageDriver') is not None:
-            self.storage_driver = m.get('storageDriver')
-        if m.get('thumbnail') is not None:
-            temp_model = CommitFileResponseBodyDentryThumbnail()
-            self.thumbnail = temp_model.from_map(m['thumbnail'])
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('uuid') is not None:
-            self.uuid = m.get('uuid')
-        if m.get('version') is not None:
-            self.version = m.get('version')
         return self
 
 
-class CommitFileResponseBody(TeaModel):
+class ListWorkBenchGroupResponseBody(TeaModel):
     def __init__(
         self,
-        dentry: CommitFileResponseBodyDentry = None,
+        group_list: List[ListWorkBenchGroupResponseBodyGroupList] = None,
     ):
-        self.dentry = dentry
+        self.group_list = group_list
 
     def validate(self):
-        if self.dentry:
-            self.dentry.validate()
+        if self.group_list:
+            for k in self.group_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.dentry is not None:
-            result['dentry'] = self.dentry.to_map()
+        result['groupList'] = []
+        if self.group_list is not None:
+            for k in self.group_list:
+                result['groupList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('dentry') is not None:
-            temp_model = CommitFileResponseBodyDentry()
-            self.dentry = temp_model.from_map(m['dentry'])
+        self.group_list = []
+        if m.get('groupList') is not None:
+            for k in m.get('groupList'):
+                temp_model = ListWorkBenchGroupResponseBodyGroupList()
+                self.group_list.append(temp_model.from_map(k))
         return self
 
 
-class CommitFileResponse(TeaModel):
+class ListWorkBenchGroupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CommitFileResponseBody = None,
+        body: ListWorkBenchGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -519,20 +628,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CommitFileResponseBody()
+            temp_model = ListWorkBenchGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetFileUploadInfoHeaders(TeaModel):
+class QueryComponentScopesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -557,270 +666,306 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetFileUploadInfoRequestOptionPreCheckParam(TeaModel):
+class QueryComponentScopesResponseBody(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        size: int = None,
+        dept_visible_scopes: List[int] = None,
+        user_visible_scopes: List[str] = None,
     ):
-        self.name = name
-        self.size = size
+        self.dept_visible_scopes = dept_visible_scopes
+        self.user_visible_scopes = user_visible_scopes
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        if self.size is not None:
-            result['size'] = self.size
+        if self.dept_visible_scopes is not None:
+            result['deptVisibleScopes'] = self.dept_visible_scopes
+        if self.user_visible_scopes is not None:
+            result['userVisibleScopes'] = self.user_visible_scopes
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('size') is not None:
-            self.size = m.get('size')
+        if m.get('deptVisibleScopes') is not None:
+            self.dept_visible_scopes = m.get('deptVisibleScopes')
+        if m.get('userVisibleScopes') is not None:
+            self.user_visible_scopes = m.get('userVisibleScopes')
+        return self
+
+
+class QueryComponentScopesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryComponentScopesResponseBody = None,
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
+            temp_model = QueryComponentScopesResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetFileUploadInfoRequestOption(TeaModel):
+class QueryShortcutScopesHeaders(TeaModel):
     def __init__(
         self,
-        pre_check_param: GetFileUploadInfoRequestOptionPreCheckParam = None,
-        prefer_intranet: bool = None,
-        prefer_region: str = None,
-        storage_driver: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.pre_check_param = pre_check_param
-        self.prefer_intranet = prefer_intranet
-        self.prefer_region = prefer_region
-        self.storage_driver = storage_driver
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
-        if self.pre_check_param:
-            self.pre_check_param.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.pre_check_param is not None:
-            result['preCheckParam'] = self.pre_check_param.to_map()
-        if self.prefer_intranet is not None:
-            result['preferIntranet'] = self.prefer_intranet
-        if self.prefer_region is not None:
-            result['preferRegion'] = self.prefer_region
-        if self.storage_driver is not None:
-            result['storageDriver'] = self.storage_driver
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('preCheckParam') is not None:
-            temp_model = GetFileUploadInfoRequestOptionPreCheckParam()
-            self.pre_check_param = temp_model.from_map(m['preCheckParam'])
-        if m.get('preferIntranet') is not None:
-            self.prefer_intranet = m.get('preferIntranet')
-        if m.get('preferRegion') is not None:
-            self.prefer_region = m.get('preferRegion')
-        if m.get('storageDriver') is not None:
-            self.storage_driver = m.get('storageDriver')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetFileUploadInfoRequest(TeaModel):
+class QueryShortcutScopesResponseBody(TeaModel):
     def __init__(
         self,
-        option: GetFileUploadInfoRequestOption = None,
-        protocol: str = None,
-        union_id: str = None,
+        dept_visible_scopes: List[int] = None,
+        user_visible_scopes: List[str] = None,
     ):
-        self.option = option
-        self.protocol = protocol
-        self.union_id = union_id
+        self.dept_visible_scopes = dept_visible_scopes
+        self.user_visible_scopes = user_visible_scopes
 
     def validate(self):
-        if self.option:
-            self.option.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.option is not None:
-            result['option'] = self.option.to_map()
-        if self.protocol is not None:
-            result['protocol'] = self.protocol
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.dept_visible_scopes is not None:
+            result['deptVisibleScopes'] = self.dept_visible_scopes
+        if self.user_visible_scopes is not None:
+            result['userVisibleScopes'] = self.user_visible_scopes
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('option') is not None:
-            temp_model = GetFileUploadInfoRequestOption()
-            self.option = temp_model.from_map(m['option'])
-        if m.get('protocol') is not None:
-            self.protocol = m.get('protocol')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('deptVisibleScopes') is not None:
+            self.dept_visible_scopes = m.get('deptVisibleScopes')
+        if m.get('userVisibleScopes') is not None:
+            self.user_visible_scopes = m.get('userVisibleScopes')
         return self
 
 
-class GetFileUploadInfoResponseBodyHeaderSignatureInfo(TeaModel):
+class QueryShortcutScopesResponse(TeaModel):
     def __init__(
         self,
-        expiration_seconds: int = None,
         headers: Dict[str, str] = None,
-        internal_resource_urls: List[str] = None,
-        region: str = None,
-        resource_urls: List[str] = None,
+        status_code: int = None,
+        body: QueryShortcutScopesResponseBody = None,
     ):
-        self.expiration_seconds = expiration_seconds
         self.headers = headers
-        self.internal_resource_urls = internal_resource_urls
-        self.region = region
-        self.resource_urls = resource_urls
+        self.status_code = status_code
+        self.body = body
 
     def validate(self):
-        pass
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.expiration_seconds is not None:
-            result['expirationSeconds'] = self.expiration_seconds
         if self.headers is not None:
             result['headers'] = self.headers
-        if self.internal_resource_urls is not None:
-            result['internalResourceUrls'] = self.internal_resource_urls
-        if self.region is not None:
-            result['region'] = self.region
-        if self.resource_urls is not None:
-            result['resourceUrls'] = self.resource_urls
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('expirationSeconds') is not None:
-            self.expiration_seconds = m.get('expirationSeconds')
         if m.get('headers') is not None:
             self.headers = m.get('headers')
-        if m.get('internalResourceUrls') is not None:
-            self.internal_resource_urls = m.get('internalResourceUrls')
-        if m.get('region') is not None:
-            self.region = m.get('region')
-        if m.get('resourceUrls') is not None:
-            self.resource_urls = m.get('resourceUrls')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryShortcutScopesResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetFileUploadInfoResponseBody(TeaModel):
+class UpdateDingPortalPageScopeHeaders(TeaModel):
     def __init__(
         self,
-        header_signature_info: GetFileUploadInfoResponseBodyHeaderSignatureInfo = None,
-        protocol: str = None,
-        storage_driver: str = None,
-        upload_key: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.header_signature_info = header_signature_info
-        self.protocol = protocol
-        self.storage_driver = storage_driver
-        self.upload_key = upload_key
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
+class UpdateDingPortalPageScopeRequest(TeaModel):
+    def __init__(
+        self,
+        all_visible: bool = None,
+        dept_ids: List[int] = None,
+        role_ids: List[int] = None,
+        userids: List[str] = None,
+    ):
+        self.all_visible = all_visible
+        self.dept_ids = dept_ids
+        self.role_ids = role_ids
+        self.userids = userids
 
     def validate(self):
-        if self.header_signature_info:
-            self.header_signature_info.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.header_signature_info is not None:
-            result['headerSignatureInfo'] = self.header_signature_info.to_map()
-        if self.protocol is not None:
-            result['protocol'] = self.protocol
-        if self.storage_driver is not None:
-            result['storageDriver'] = self.storage_driver
-        if self.upload_key is not None:
-            result['uploadKey'] = self.upload_key
+        if self.all_visible is not None:
+            result['allVisible'] = self.all_visible
+        if self.dept_ids is not None:
+            result['deptIds'] = self.dept_ids
+        if self.role_ids is not None:
+            result['roleIds'] = self.role_ids
+        if self.userids is not None:
+            result['userids'] = self.userids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headerSignatureInfo') is not None:
-            temp_model = GetFileUploadInfoResponseBodyHeaderSignatureInfo()
-            self.header_signature_info = temp_model.from_map(m['headerSignatureInfo'])
-        if m.get('protocol') is not None:
-            self.protocol = m.get('protocol')
-        if m.get('storageDriver') is not None:
-            self.storage_driver = m.get('storageDriver')
-        if m.get('uploadKey') is not None:
-            self.upload_key = m.get('uploadKey')
+        if m.get('allVisible') is not None:
+            self.all_visible = m.get('allVisible')
+        if m.get('deptIds') is not None:
+            self.dept_ids = m.get('deptIds')
+        if m.get('roleIds') is not None:
+            self.role_ids = m.get('roleIds')
+        if m.get('userids') is not None:
+            self.userids = m.get('userids')
         return self
 
 
-class GetFileUploadInfoResponse(TeaModel):
+class UpdateDingPortalPageScopeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetFileUploadInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
-        self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
             result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = GetFileUploadInfoResponseBody()
-            self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.10
+Version: 2.0.11
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.11/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -244,14 +244,17 @@
 alibabacloud_dingtalk/village_1_0/models.py
 alibabacloud_dingtalk/watt_1_0/__init__.py
 alibabacloud_dingtalk/watt_1_0/client.py
 alibabacloud_dingtalk/watt_1_0/models.py
 alibabacloud_dingtalk/wiki_1_0/__init__.py
 alibabacloud_dingtalk/wiki_1_0/client.py
 alibabacloud_dingtalk/wiki_1_0/models.py
+alibabacloud_dingtalk/wiki_2_0/__init__.py
+alibabacloud_dingtalk/wiki_2_0/client.py
+alibabacloud_dingtalk/wiki_2_0/models.py
 alibabacloud_dingtalk/wms_1_0/__init__.py
 alibabacloud_dingtalk/wms_1_0/client.py
 alibabacloud_dingtalk/wms_1_0/models.py
 alibabacloud_dingtalk/workbench_1_0/__init__.py
 alibabacloud_dingtalk/workbench_1_0/client.py
 alibabacloud_dingtalk/workbench_1_0/models.py
 alibabacloud_dingtalk/workflow_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.10/setup.py` & `alibabacloud_dingtalk-2.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 28/04/2023
+Created on 09/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```


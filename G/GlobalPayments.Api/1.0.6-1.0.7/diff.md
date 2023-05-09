# Comparing `tmp/GlobalPayments.Api-1.0.6.tar.gz` & `tmp/GlobalPayments.Api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlobalPayments.Api-1.0.6.tar", last modified: Thu Apr 20 12:36:27 2023, max compression
+gzip compressed data, was "GlobalPayments.Api-1.0.7.tar", last modified: Tue May  9 13:41:10 2023, max compression
```

## Comparing `GlobalPayments.Api-1.0.6.tar` & `GlobalPayments.Api-1.0.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.978104 GlobalPayments.Api-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.664688 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/
--rw-rw-rw-   0        0        0      910 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2023-04-20 12:36:27.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 12:36:26.000000 GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15439 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/LICENSE.md
--rw-rw-rw-   0        0        0      910 2023-04-20 12:36:27.976103 GlobalPayments.Api-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.672671 GlobalPayments.Api-1.0.6/globalpayments/
--rw-rw-rw-   0        0        0       36 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.678668 GlobalPayments.Api-1.0.6/globalpayments/api/
--rw-rw-rw-   0        0        0    10064 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.694668 GlobalPayments.Api-1.0.6/globalpayments/api/builders/
--rw-rw-rw-   0        0        0    13980 2023-04-13 15:28:43.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/__init__.py
--rw-rw-rw-   0        0        0     2807 2023-04-13 15:30:21.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/management_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.725690 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/
--rw-rw-rw-   0        0        0      322 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/__init__.py
--rw-rw-rw-   0        0        0     2742 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_clause.py
--rw-rw-rw-   0        0        0     1125 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_target.py
--rw-rw-rw-   0        0        0     2194 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validations.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.802850 GlobalPayments.Api-1.0.6/globalpayments/api/entities/
--rw-rw-rw-   0        0        0    15101 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/__init__.py
--rw-rw-rw-   0        0        0    18729 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/address.py
--rw-rw-rw-   0        0        0      176 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/batch_summary.py
--rw-rw-rw-   0        0        0      244 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/debit_mac.py
--rw-rw-rw-   0        0        0      658 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/ecommerce_info.py
--rw-rw-rw-   0        0        0      601 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/encryption_data.py
--rw-rw-rw-   0        0        0    12813 2023-04-13 17:43:34.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/enums.py
--rw-rw-rw-   0        0        0     1837 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/exceptions.py
--rw-rw-rw-   0        0        0      300 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/hosted_payment_data.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.834811 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/base_table_service_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/bump_status_collection.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/login_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/server_assignment_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/server_list_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/shift_assignments.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/table_service_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/table_service/ticket.py
--rw-rw-rw-   0        0        0      211 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/three_d_secure.py
--rw-rw-rw-   0        0        0      640 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/entities/transaction_summary.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.852836 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/
--rw-rw-rw-   0        0        0   100297 2023-04-14 18:53:27.000000 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/__init__.py
--rw-rw-rw-   0        0        0       81 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/gateway_response.py
--rw-rw-rw-   0        0        0       48 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/gateways/table_service_connector.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.911812 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/
--rw-rw-rw-   0        0        0      583 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/cash.py
--rw-rw-rw-   0        0        0     8601 2023-04-14 18:52:05.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/credit.py
--rw-rw-rw-   0        0        0     2256 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/debit.py
--rw-rw-rw-   0        0        0     2202 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/ebt.py
--rw-rw-rw-   0        0        0     1259 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/echeck.py
--rw-rw-rw-   0        0        0     3302 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/giftcard.py
--rw-rw-rw-   0        0        0     1274 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/payment_interfaces.py
--rw-rw-rw-   0        0        0      173 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/transaction_reference.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.966110 GlobalPayments.Api-1.0.6/globalpayments/api/services/
--rw-rw-rw-   0        0        0      220 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/__init__.py
--rw-rw-rw-   0        0        0      354 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/batch_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/credit_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/debit_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/device_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/ebt_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/gift_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/hosted_service.py
--rw-rw-rw-   0        0        0     1127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/recurring_service.py
--rw-rw-rw-   0        0        0      589 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/reporting_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/services/table_service.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:36:27.971143 GlobalPayments.Api-1.0.6/globalpayments/api/utils/
--rw-rw-rw-   0        0        0     6127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.6/globalpayments/api/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-20 12:36:27.980104 GlobalPayments.Api-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1159 2023-04-20 12:32:44.000000 GlobalPayments.Api-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.166307 GlobalPayments.Api-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.836821 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15439 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0      910 2023-05-09 13:41:10.165304 GlobalPayments.Api-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.841580 GlobalPayments.Api-1.0.7/globalpayments/
+-rw-rw-rw-   0        0        0       36 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.848567 GlobalPayments.Api-1.0.7/globalpayments/api/
+-rw-rw-rw-   0        0        0    10064 2023-05-01 21:16:30.000000 GlobalPayments.Api-1.0.7/globalpayments/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.862867 GlobalPayments.Api-1.0.7/globalpayments/api/builders/
+-rw-rw-rw-   0        0        0    13980 2023-05-08 13:15:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/__init__.py
+-rw-rw-rw-   0        0        0     2807 2023-04-13 15:30:21.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/management_builder.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.901020 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/
+-rw-rw-rw-   0        0        0      322 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/__init__.py
+-rw-rw-rw-   0        0        0     2742 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_clause.py
+-rw-rw-rw-   0        0        0     1125 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_target.py
+-rw-rw-rw-   0        0        0     2194 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validations.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.979662 GlobalPayments.Api-1.0.7/globalpayments/api/entities/
+-rw-rw-rw-   0        0        0    15101 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/__init__.py
+-rw-rw-rw-   0        0        0    18729 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/address.py
+-rw-rw-rw-   0        0        0      176 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/batch_summary.py
+-rw-rw-rw-   0        0        0      244 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/debit_mac.py
+-rw-rw-rw-   0        0        0      658 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/ecommerce_info.py
+-rw-rw-rw-   0        0        0      601 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/encryption_data.py
+-rw-rw-rw-   0        0        0    12813 2023-05-08 13:15:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/enums.py
+-rw-rw-rw-   0        0        0     1837 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/exceptions.py
+-rw-rw-rw-   0        0        0      300 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/hosted_payment_data.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.004209 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/base_table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/bump_status_collection.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/login_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/server_assignment_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/server_list_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/shift_assignments.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/ticket.py
+-rw-rw-rw-   0        0        0      211 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/three_d_secure.py
+-rw-rw-rw-   0        0        0      640 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/transaction_summary.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.046097 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/
+-rw-rw-rw-   0        0        0   100405 2023-05-09 13:22:20.000000 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/gateway_response.py
+-rw-rw-rw-   0        0        0       48 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/table_service_connector.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.108936 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/
+-rw-rw-rw-   0        0        0      583 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/cash.py
+-rw-rw-rw-   0        0        0     8601 2023-05-08 13:15:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/credit.py
+-rw-rw-rw-   0        0        0     2256 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/debit.py
+-rw-rw-rw-   0        0        0     2202 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/ebt.py
+-rw-rw-rw-   0        0        0     1259 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/echeck.py
+-rw-rw-rw-   0        0        0     3302 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/giftcard.py
+-rw-rw-rw-   0        0        0     1274 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/payment_interfaces.py
+-rw-rw-rw-   0        0        0      173 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/transaction_reference.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.155620 GlobalPayments.Api-1.0.7/globalpayments/api/services/
+-rw-rw-rw-   0        0        0      220 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/batch_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/credit_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/debit_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/device_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/ebt_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/gift_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/hosted_service.py
+-rw-rw-rw-   0        0        0     1127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/recurring_service.py
+-rw-rw-rw-   0        0        0      589 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/reporting_service.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/table_service.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.160301 GlobalPayments.Api-1.0.7/globalpayments/api/utils/
+-rw-rw-rw-   0        0        0     6127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 13:41:10.167305 GlobalPayments.Api-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2023-05-09 13:22:20.000000 GlobalPayments.Api-1.0.7/setup.py
```

### Comparing `GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/PKG-INFO` & `GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlobalPayments.Api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Global Payments Python SDK for integrating with Heartland and Global Payments merchant services APIs.
 Home-page: https://developer.heartlandpaymentsystems.com/
 Author: Heartland Payment Systems
 Author-email: EntApp_DevPortal@e-hps.com
 License: LICENSE.md
 License-File: LICENSE.md
```

### Comparing `GlobalPayments.Api-1.0.6/GlobalPayments.Api.egg-info/SOURCES.txt` & `GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/LICENSE.md` & `GlobalPayments.Api-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/PKG-INFO` & `GlobalPayments.Api-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlobalPayments.Api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Global Payments Python SDK for integrating with Heartland and Global Payments merchant services APIs.
 Home-page: https://developer.heartlandpaymentsystems.com/
 Author: Heartland Payment Systems
 Author-email: EntApp_DevPortal@e-hps.com
 License: LICENSE.md
 License-File: LICENSE.md
```

### Comparing `GlobalPayments.Api-1.0.6/README.txt` & `GlobalPayments.Api-1.0.7/README.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/__init__.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/builders/__init__.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/builders/management_builder.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/builders/management_builder.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_clause.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_clause.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validation_target.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_target.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/builders/validations/validations.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validations.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/__init__.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/address.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/address.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/ecommerce_info.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/ecommerce_info.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/encryption_data.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/encryption_data.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/enums.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/enums.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/exceptions.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/entities/transaction_summary.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/entities/transaction_summary.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/gateways/__init__.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/gateways/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,16 +104,18 @@
     @property
     def secret_api_key(self):
         return self._secret_api_key
 
     @secret_api_key.setter
     def secret_api_key(self, value):
         self._secret_api_key = value
-        encoded_value = base64.b64encode(bytearray(value.encode()))
-        self.headers['Authorization'] = 'Basic {}'.format(encoded_value.decode('ascii'))
+
+        if (value is not None):
+            encoded_value = base64.b64encode(bytearray(value.encode()))
+            self.headers['Authorization'] = 'Basic {}'.format(encoded_value.decode('ascii'))
 
     @property
     def supports_retrieval(self):
         return True
 
     @property
     def supports_update_payment_details(self):
@@ -727,19 +729,19 @@
 
             manual_entry = et.SubElement(card_data, 'TokenData'
                                          if has_token else 'ManualEntry')
             et.SubElement(manual_entry, 'TokenValue' if has_token else
                           'CardNbr').text = token_value or card.number
 
             if card.exp_month is not None:
-                et.SubElement(manual_entry, 'ExpMonth').text = card.exp_month
+                et.SubElement(manual_entry, 'ExpMonth').text = str(card.exp_month)
             if card.exp_year is not None:
-                et.SubElement(manual_entry, 'ExpYear').text = card.exp_year
+                et.SubElement(manual_entry, 'ExpYear').text = str(card.exp_year)
             if card.cvn is not None:
-                et.SubElement(manual_entry, 'CVV2').text = card.cvn
+                et.SubElement(manual_entry, 'CVV2').text = str(card.cvn)
 
             et.SubElement(
                 manual_entry,
                 'ReaderPresent').text = 'Y' if card.reader_present else 'N'
             et.SubElement(
                 manual_entry,
                 'CardPresent').text = 'Y' if card.card_present else 'N'
@@ -904,17 +906,17 @@
 
             # payment method stuff
             et.SubElement(block1, 'PaymentMethodKey').text = method.key
             if (method.payment_method is not None
                     and isinstance(method.payment_method, CreditCardData)):
                 card = method.payment_method
                 data = et.SubElement(block1, 'PaymentMethodKeyData')
-                et.SubElement(data, 'ExpMonth').text = card.exp_month
-                et.SubElement(data, 'ExpYear').text = card.exp_year
-                et.SubElement(data, 'CVV2').text = card.cvn
+                et.SubElement(data, 'ExpMonth').text = str(card.exp_month)
+                et.SubElement(data, 'ExpYear').text = str(card.exp_year)
+                et.SubElement(data, 'CVV2').text = str(card.cvn)
 
             # recurring data
             recurring = et.SubElement(block1, 'RecurringData')
             et.SubElement(recurring, 'ScheduleID').text = builder.schedule_id
             et.SubElement(
                 recurring,
                 'OneTime').text = 'Y' if builder.one_time_payment else 'N'
@@ -1124,29 +1126,29 @@
         version1 = et.SubElement(request, 'Ver1.0')
 
         # header
         header = et.SubElement(version1, 'Header')
         if self.secret_api_key is not None:
             et.SubElement(header, 'SecretAPIKey').text = self.secret_api_key
         if self.site_id is not None:
-            et.SubElement(header, 'SiteId').text = self.site_id
+            et.SubElement(header, 'SiteId').text = str(self.site_id)
         if self.license_id is not None:
-            et.SubElement(header, 'LicenseId').text = self.license_id
+            et.SubElement(header, 'LicenseId').text = str(self.license_id)
         if self.device_id is not None:
-            et.SubElement(header, 'DeviceId').text = self.device_id
+            et.SubElement(header, 'DeviceId').text = str(self.device_id)
         if self.username is not None:
-            et.SubElement(header, 'UserName').text = self.username
+            et.SubElement(header, 'UserName').text = str(self.username)
         if self.password is not None:
             et.SubElement(header, 'Password').text = self.password
         if self.developer_id is not None:
-            et.SubElement(header, 'DeveloperID').text = self.developer_id
+            et.SubElement(header, 'DeveloperID').text = str(self.developer_id)
         if self.version_number is not None:
-            et.SubElement(header, 'VersionNbr').text = self.version_number
+            et.SubElement(header, 'VersionNbr').text = str(self.version_number)
         if client_transaction_id is not None:
-            et.SubElement(header, 'ClientTxnId').text = client_transaction_id
+            et.SubElement(header, 'ClientTxnId').text = str(client_transaction_id)
 
         trans = et.SubElement(version1, 'Transaction')
         trans.append(transaction)
 
         return et.tostring(envelope)
 
     def _map_response(self, raw_response, payment_method):
```

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/__init__.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/credit.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/credit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/debit.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/debit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/ebt.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/ebt.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/echeck.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/echeck.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/giftcard.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/giftcard.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/payment_methods/payment_interfaces.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/payment_interfaces.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/services/recurring_service.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/services/recurring_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/services/reporting_service.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/services/reporting_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/globalpayments/api/utils/__init__.py` & `GlobalPayments.Api-1.0.7/globalpayments/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.6/setup.py` & `GlobalPayments.Api-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='GlobalPayments.Api',
-    version='1.0.6',
+    version='1.0.7',
     author='Heartland Payment Systems',
     author_email='EntApp_DevPortal@e-hps.com',
     packages=[
         'globalpayments', 'globalpayments.api', 'globalpayments.api.builders',
         'globalpayments.api.builders.validations',
         'globalpayments.api.entities',
         'globalpayments.api.entities.table_service',
```


# Comparing `tmp/cashfree_lrs_client-1.0.6.tar.gz` & `tmp/cashfree_lrs_client-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashfree_lrs_client-1.0.6.tar", max compression
+gzip compressed data, was "cashfree_lrs_client-1.0.7.tar", max compression
```

## Comparing `cashfree_lrs_client-1.0.6.tar` & `cashfree_lrs_client-1.0.7.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0     5265 2023-05-08 08:42:49.801334 cashfree_lrs_client-1.0.6/README.md
--rw-r--r--   0        0        0     1847 2023-05-08 08:42:49.825335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/__init__.py
--rw-r--r--   0        0        0       99 2023-05-08 08:42:49.829335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/__init__.py
--rw-r--r--   0        0        0    53538 2023-05-08 08:42:26.100904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/default_api.py
--rw-r--r--   0        0        0    54075 2023-05-08 08:42:49.785334 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/lrs_api.py
--rw-r--r--   0        0        0    30034 2023-05-08 08:42:49.837335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_client.py
--rw-r--r--   0        0        0      844 2023-05-08 08:42:49.837335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_response.py
--rw-r--r--   0        0        0      214 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/__init__.py
--rw-r--r--   0        0        0     1655 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/path_to_api.py
--rw-r--r--   0        0        0      246 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/beneficiaries.py
--rw-r--r--   0        0        0      121 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/fx_rate_details.py
--rw-r--r--   0        0        0      105 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders.py
--rw-r--r--   0        0        0      137 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders_documents_upload.py
--rw-r--r--   0        0        0      153 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
--rw-r--r--   0        0        0      136 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/orders_order_id_process.py
--rw-r--r--   0        0        0      111 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/remitters.py
--rw-r--r--   0        0        0      109 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/paths/webhooks.py
--rw-r--r--   0        0        0      306 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      308 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tags/lrs_api.py
--rw-r--r--   0        0        0    16079 2023-05-08 08:42:49.825335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/configuration.py
--rw-r--r--   0        0        0     2815 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
--rw-r--r--   0        0        0     2331 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderRequest.md
--rw-r--r--   0        0        0     1337 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderResponse.md
--rw-r--r--   0        0        0     2583 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateRemitterRequest.md
--rw-r--r--   0        0        0      389 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Currency.md
--rw-r--r--   0        0        0      859 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Error.md
--rw-r--r--   0        0        0     1656 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/FetchForexRateRequest.md
--rw-r--r--   0        0        0    59748 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/LrsApi.md
--rw-r--r--   0        0        0      343 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Purpose.md
--rw-r--r--   0        0        0     1239 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SetupWebhooksRequest.md
--rw-r--r--   0        0        0      896 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SuccessMessage.md
--rw-r--r--   0        0        0     5118 2023-05-08 08:42:49.833335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/exceptions.py
--rw-r--r--   0        0        0      353 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/__init__.py
--rw-r--r--   0        0        0      884 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.py
--rw-r--r--   0        0        0      815 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.pyi
--rw-r--r--   0        0        0    14903 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.py
--rw-r--r--   0        0        0    13066 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.pyi
--rw-r--r--   0        0        0    11475 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.py
--rw-r--r--   0        0        0    10572 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.pyi
--rw-r--r--   0        0        0     8398 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.py
--rw-r--r--   0        0        0     8166 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.pyi
--rw-r--r--   0        0        0    12349 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.py
--rw-r--r--   0        0        0    10785 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.pyi
--rw-r--r--   0        0        0     1192 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.py
--rw-r--r--   0        0        0     1031 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.pyi
--rw-r--r--   0        0        0     3384 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.py
--rw-r--r--   0        0        0     3384 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.pyi
--rw-r--r--   0        0        0     5805 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     5697 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
--rw-r--r--   0        0        0     1368 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.py
--rw-r--r--   0        0        0     1169 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.pyi
--rw-r--r--   0        0        0     3663 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.py
--rw-r--r--   0        0        0     3663 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.pyi
--rw-r--r--   0        0        0     2477 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.py
--rw-r--r--   0        0        0     2477 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.pyi
--rw-r--r--   0        0        0     1207 2023-05-08 08:42:49.829335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/__init__.py
--rw-r--r--   0        0        0      714 2023-05-08 08:42:49.533329 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/country.py
--rw-r--r--   0        0        0     1975 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary200_response.py
--rw-r--r--   0        0        0     5660 2023-05-08 08:42:49.545329 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary_request.py
--rw-r--r--   0        0        0     5041 2023-05-08 08:42:49.565330 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_request.py
--rw-r--r--   0        0        0     3426 2023-05-08 08:42:49.597330 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_response.py
--rw-r--r--   0        0        0     1951 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter200_response.py
--rw-r--r--   0        0        0     5347 2023-05-08 08:42:49.629331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter_request.py
--rw-r--r--   0        0        0      765 2023-05-08 08:42:49.637331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/currency.py
--rw-r--r--   0        0        0     2088 2023-05-08 08:42:49.641331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/error.py
--rw-r--r--   0        0        0     3279 2023-05-08 08:42:49.649331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     2775 2023-05-08 08:42:49.653331 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_response.py
--rw-r--r--   0        0        0     2903 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/order_response.py
--rw-r--r--   0        0        0      780 2023-05-08 08:42:49.661332 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/purpose.py
--rw-r--r--   0        0        0     1943 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks200_response.py
--rw-r--r--   0        0        0     2361 2023-05-08 08:42:49.669332 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks_request.py
--rw-r--r--   0        0        0     1909 2023-05-08 08:42:49.673332 cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/success_message.py
--rw-r--r--   0        0        0      644 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/__init__.py
--rw-r--r--   0        0        0    12582 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.py
--rw-r--r--   0        0        0    12396 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.pyi
--rw-r--r--   0        0        0      326 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/__init__.py
--rw-r--r--   0        0        0    11760 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.py
--rw-r--r--   0        0        0    11604 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.pyi
--rw-r--r--   0        0        0      309 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/__init__.py
--rw-r--r--   0        0        0    13005 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.py
--rw-r--r--   0        0        0    12789 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.pyi
--rw-r--r--   0        0        0      343 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
--rw-r--r--   0        0        0    12334 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.py
--rw-r--r--   0        0        0    12148 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
--rw-r--r--   0        0        0      361 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
--rw-r--r--   0        0        0    15715 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
--rw-r--r--   0        0        0    15469 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
--rw-r--r--   0        0        0      343 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
--rw-r--r--   0        0        0     8093 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.py
--rw-r--r--   0        0        0     7937 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
--rw-r--r--   0        0        0      315 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/__init__.py
--rw-r--r--   0        0        0    12525 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.py
--rw-r--r--   0        0        0    12339 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.pyi
--rw-r--r--   0        0        0      313 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    11939 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.py
--rw-r--r--   0        0        0    11783 2023-05-08 08:42:26.104905 cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.pyi
--rw-r--r--   0        0        0    12769 2023-05-08 08:42:49.841335 cashfree_lrs_client-1.0.6/cashfree_lrs_client/rest.py
--rw-r--r--   0        0        0    97649 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/schemas.py
--rw-r--r--   0        0        0        0 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/__init__.py
--rw-r--r--   0        0        0     2694 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_beneficiary_request.py
--rw-r--r--   0        0        0     2292 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_request.py
--rw-r--r--   0        0        0     1952 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_response.py
--rw-r--r--   0        0        0     2486 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_remitter_request.py
--rw-r--r--   0        0        0      738 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_currency.py
--rw-r--r--   0        0        0     1439 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_error.py
--rw-r--r--   0        0        0     1860 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
--rw-r--r--   0        0        0     1845 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_lrs_api.py
--rw-r--r--   0        0        0      731 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_purpose.py
--rw-r--r--   0        0        0     1737 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_setup_webhooks_request.py
--rw-r--r--   0        0        0     1493 2023-05-08 08:42:26.108904 cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_success_message.py
--rw-r--r--   0        0        0      683 2023-05-08 08:42:49.817335 cashfree_lrs_client-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6168 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     5331 2023-05-09 07:23:12.793233 cashfree_lrs_client-1.0.7/README.md
+-rw-r--r--   0        0        0     1942 2023-05-09 07:23:12.821234 cashfree_lrs_client-1.0.7/cashfree_lrs_client/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-09 07:23:12.825234 cashfree_lrs_client-1.0.7/cashfree_lrs_client/api/__init__.py
+-rw-r--r--   0        0        0    53538 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/api/default_api.py
+-rw-r--r--   0        0        0    54075 2023-05-09 07:23:12.781232 cashfree_lrs_client-1.0.7/cashfree_lrs_client/api/lrs_api.py
+-rw-r--r--   0        0        0    30034 2023-05-09 07:23:12.837235 cashfree_lrs_client-1.0.7/cashfree_lrs_client/api_client.py
+-rw-r--r--   0        0        0      844 2023-05-09 07:23:12.841235 cashfree_lrs_client-1.0.7/cashfree_lrs_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/__init__.py
+-rw-r--r--   0        0        0     1655 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      246 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/beneficiaries.py
+-rw-r--r--   0        0        0      121 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/fx_rate_details.py
+-rw-r--r--   0        0        0      105 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/orders.py
+-rw-r--r--   0        0        0      137 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/orders_documents_upload.py
+-rw-r--r--   0        0        0      153 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
+-rw-r--r--   0        0        0      136 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/orders_order_id_process.py
+-rw-r--r--   0        0        0      111 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/remitters.py
+-rw-r--r--   0        0        0      109 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/paths/webhooks.py
+-rw-r--r--   0        0        0      306 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      308 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/tags/lrs_api.py
+-rw-r--r--   0        0        0    16079 2023-05-09 07:23:12.817234 cashfree_lrs_client-1.0.7/cashfree_lrs_client/configuration.py
+-rw-r--r--   0        0        0     2815 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
+-rw-r--r--   0        0        0     2331 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateOrderRequest.md
+-rw-r--r--   0        0        0     1337 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateOrderResponse.md
+-rw-r--r--   0        0        0     2583 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateRemitterRequest.md
+-rw-r--r--   0        0        0      389 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/Currency.md
+-rw-r--r--   0        0        0      859 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/Error.md
+-rw-r--r--   0        0        0     1656 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/FetchForexRateRequest.md
+-rw-r--r--   0        0        0    59748 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/LrsApi.md
+-rw-r--r--   0        0        0      343 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/Purpose.md
+-rw-r--r--   0        0        0     1239 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/SetupWebhooksRequest.md
+-rw-r--r--   0        0        0      896 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/SuccessMessage.md
+-rw-r--r--   0        0        0     5118 2023-05-09 07:23:12.829234 cashfree_lrs_client-1.0.7/cashfree_lrs_client/exceptions.py
+-rw-r--r--   0        0        0      353 2023-05-09 07:22:47.011977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/amount.py
+-rw-r--r--   0        0        0      815 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/amount.pyi
+-rw-r--r--   0        0        0    14903 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_beneficiary_request.py
+-rw-r--r--   0        0        0    13066 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_beneficiary_request.pyi
+-rw-r--r--   0        0        0    11475 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_request.py
+-rw-r--r--   0        0        0    10572 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_request.pyi
+-rw-r--r--   0        0        0     8398 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_response.py
+-rw-r--r--   0        0        0     8166 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_response.pyi
+-rw-r--r--   0        0        0    12349 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_remitter_request.py
+-rw-r--r--   0        0        0    10785 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_remitter_request.pyi
+-rw-r--r--   0        0        0     1192 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/currency.py
+-rw-r--r--   0        0        0     1031 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/currency.pyi
+-rw-r--r--   0        0        0     3384 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/error.py
+-rw-r--r--   0        0        0     3384 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/error.pyi
+-rw-r--r--   0        0        0     5805 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     5697 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
+-rw-r--r--   0        0        0     1368 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/purpose.py
+-rw-r--r--   0        0        0     1169 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/purpose.pyi
+-rw-r--r--   0        0        0     3663 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/setup_webhooks_request.py
+-rw-r--r--   0        0        0     3663 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/setup_webhooks_request.pyi
+-rw-r--r--   0        0        0     2477 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/success_message.py
+-rw-r--r--   0        0        0     2477 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/success_message.pyi
+-rw-r--r--   0        0        0     1302 2023-05-09 07:23:12.825234 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-09 07:23:12.421215 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/country.py
+-rw-r--r--   0        0        0     1975 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_beneficiary200_response.py
+-rw-r--r--   0        0        0     5660 2023-05-09 07:23:12.441216 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_beneficiary_request.py
+-rw-r--r--   0        0        0     5041 2023-05-09 07:23:12.457216 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_order_request.py
+-rw-r--r--   0        0        0     3426 2023-05-09 07:23:12.469217 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_order_response.py
+-rw-r--r--   0        0        0     1951 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_remitter200_response.py
+-rw-r--r--   0        0        0     5347 2023-05-09 07:23:12.481218 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_remitter_request.py
+-rw-r--r--   0        0        0      765 2023-05-09 07:23:12.485218 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/currency.py
+-rw-r--r--   0        0        0     2088 2023-05-09 07:23:12.493218 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/error.py
+-rw-r--r--   0        0        0     3279 2023-05-09 07:23:12.505219 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     3077 2023-05-09 07:23:12.525220 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/fetch_forex_rate_response.py
+-rw-r--r--   0        0        0     5240 2023-05-09 07:23:12.537220 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/fetch_forex_rate_response_tcs.py
+-rw-r--r--   0        0        0     2903 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/order_response.py
+-rw-r--r--   0        0        0      780 2023-05-09 07:23:12.565222 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/purpose.py
+-rw-r--r--   0        0        0     1943 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/setup_webhooks200_response.py
+-rw-r--r--   0        0        0     2361 2023-05-09 07:23:12.593223 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/setup_webhooks_request.py
+-rw-r--r--   0        0        0     1909 2023-05-09 07:23:12.609224 cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/success_message.py
+-rw-r--r--   0        0        0      644 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/beneficiaries/__init__.py
+-rw-r--r--   0        0        0    12582 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/beneficiaries/post.py
+-rw-r--r--   0        0        0    12396 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/beneficiaries/post.pyi
+-rw-r--r--   0        0        0      326 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/fx_rate_details/__init__.py
+-rw-r--r--   0        0        0    11760 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/fx_rate_details/post.py
+-rw-r--r--   0        0        0    11604 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/fx_rate_details/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders/__init__.py
+-rw-r--r--   0        0        0    13005 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders/post.py
+-rw-r--r--   0        0        0    12789 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
+-rw-r--r--   0        0        0    12334 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_documents_upload/post.py
+-rw-r--r--   0        0        0    12148 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
+-rw-r--r--   0        0        0    15715 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
+-rw-r--r--   0        0        0    15469 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
+-rw-r--r--   0        0        0     8093 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_process/post.py
+-rw-r--r--   0        0        0     7937 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/remitters/__init__.py
+-rw-r--r--   0        0        0    12525 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/remitters/post.py
+-rw-r--r--   0        0        0    12339 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/remitters/post.pyi
+-rw-r--r--   0        0        0      313 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    11939 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/webhooks/post.py
+-rw-r--r--   0        0        0    11783 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0    12769 2023-05-09 07:23:12.845235 cashfree_lrs_client-1.0.7/cashfree_lrs_client/rest.py
+-rw-r--r--   0        0        0    97649 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_beneficiary_request.py
+-rw-r--r--   0        0        0     2292 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_order_request.py
+-rw-r--r--   0        0        0     1952 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_order_response.py
+-rw-r--r--   0        0        0     2486 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_remitter_request.py
+-rw-r--r--   0        0        0      738 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_currency.py
+-rw-r--r--   0        0        0     1439 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_error.py
+-rw-r--r--   0        0        0     1860 2023-05-09 07:22:47.015977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     1845 2023-05-09 07:22:47.019977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_lrs_api.py
+-rw-r--r--   0        0        0      731 2023-05-09 07:22:47.019977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_purpose.py
+-rw-r--r--   0        0        0     1737 2023-05-09 07:22:47.019977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_setup_webhooks_request.py
+-rw-r--r--   0        0        0     1493 2023-05-09 07:22:47.019977 cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_success_message.py
+-rw-r--r--   0        0        0      683 2023-05-09 07:23:12.813234 cashfree_lrs_client-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.7/PKG-INFO
```

### Comparing `cashfree_lrs_client-1.0.6/README.md` & `cashfree_lrs_client-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.6
-- Package version: 1.0.6
+- API version: 1.0.7
+- Package version: 1.0.7
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -123,14 +123,15 @@
  - [CreateOrderRequest](docs/CreateOrderRequest.md)
  - [CreateOrderResponse](docs/CreateOrderResponse.md)
  - [CreateRemitterRequest](docs/CreateRemitterRequest.md)
  - [Currency](docs/Currency.md)
  - [Error](docs/Error.md)
  - [FetchForexRateRequest](docs/FetchForexRateRequest.md)
  - [FetchForexRateResponse](docs/FetchForexRateResponse.md)
+ - [FetchForexRateResponseTcs](docs/FetchForexRateResponseTcs.md)
  - [Purpose](docs/Purpose.md)
  - [SetupWebhooksRequest](docs/SetupWebhooksRequest.md)
  - [SuccessMessage](docs/SuccessMessage.md)
 
 
 ## Documentation For Authorization
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/__init__.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 # import apis into sdk package
 from cashfree_lrs_client.api.lrs_api import LrsApi
 
 # import ApiClient
 from cashfree_lrs_client.api_response import ApiResponse
 from cashfree_lrs_client.api_client import ApiClient
@@ -37,10 +37,11 @@
 from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.currency import Currency
 from cashfree_lrs_client.models.error import Error
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
 from cashfree_lrs_client.models.fetch_forex_rate_response import FetchForexRateResponse
+from cashfree_lrs_client.models.fetch_forex_rate_response_tcs import FetchForexRateResponseTcs
 from cashfree_lrs_client.models.purpose import Purpose
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
 from cashfree_lrs_client.models.success_message import SuccessMessage
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/default_api.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api/lrs_api.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/api/lrs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_client.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.6/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/api_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/api_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/path_to_api.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/apis/tags/lrs_api.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/apis/tags/lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/configuration.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -411,16 +411,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.6\n"\
-               "SDK Package Version: 1.0.6".\
+               "Version of the API: 1.0.7\n"\
+               "SDK Package Version: 1.0.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderRequest.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateOrderRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateOrderResponse.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateOrderResponse.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/CreateRemitterRequest.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/CreateRemitterRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/Error.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/Error.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/FetchForexRateRequest.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/FetchForexRateRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/LrsApi.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/LrsApi.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SetupWebhooksRequest.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/SetupWebhooksRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/docs/SuccessMessage.md` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/docs/SuccessMessage.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/exceptions.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/amount.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/amount.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/amount.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_beneficiary_request.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_beneficiary_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_request.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_order_response.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_order_response.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/create_remitter_request.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/create_remitter_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/currency.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/currency.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/error.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/error.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/fetch_forex_rate_request.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/fetch_forex_rate_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/purpose.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/purpose.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/setup_webhooks_request.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/setup_webhooks_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/model/success_message.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/model/success_message.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/__init__.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -20,10 +20,11 @@
 from cashfree_lrs_client.models.create_order_request import CreateOrderRequest
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.currency import Currency
 from cashfree_lrs_client.models.error import Error
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
 from cashfree_lrs_client.models.fetch_forex_rate_response import FetchForexRateResponse
+from cashfree_lrs_client.models.fetch_forex_rate_response_tcs import FetchForexRateResponseTcs
 from cashfree_lrs_client.models.purpose import Purpose
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
 from cashfree_lrs_client.models.success_message import SuccessMessage
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/country.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/country.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary200_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_beneficiary200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_beneficiary_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_order_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_order_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_order_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter200_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_remitter200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/create_remitter_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/create_remitter_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/currency.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/error.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/fetch_forex_rate_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/fetch_forex_rate_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/fetch_forex_rate_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -17,20 +17,21 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt
+from cashfree_lrs_client.models.fetch_forex_rate_response_tcs import FetchForexRateResponseTcs
 
 class FetchForexRateResponse(BaseModel):
     """
     FetchForexRateResponse
     """
-    tcs: StrictInt = Field(...)
+    tcs: FetchForexRateResponseTcs = Field(...)
     gst: Union[StrictFloat, StrictInt] = Field(...)
     to_amount: Union[StrictFloat, StrictInt] = Field(...)
     fx_rate: Union[StrictFloat, StrictInt] = Field(...)
     amount_to_pay: Union[StrictFloat, StrictInt] = Field(...)
     handling_charges: Union[StrictFloat, StrictInt] = Field(...)
     __properties = ["tcs", "gst", "to_amount", "fx_rate", "amount_to_pay", "handling_charges"]
 
@@ -52,35 +53,37 @@
         """Create an instance of FetchForexRateResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
-                            "tcs",
                             "gst",
                             "to_amount",
                             "fx_rate",
                             "amount_to_pay",
                             "handling_charges",
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of tcs
+        if self.tcs:
+            _dict['tcs'] = self.tcs.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> FetchForexRateResponse:
         """Create an instance of FetchForexRateResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return FetchForexRateResponse.parse_obj(obj)
 
         _obj = FetchForexRateResponse.parse_obj({
-            "tcs": obj.get("tcs"),
+            "tcs": FetchForexRateResponseTcs.from_dict(obj.get("tcs")) if obj.get("tcs") is not None else None,
             "gst": obj.get("gst"),
             "to_amount": obj.get("to_amount"),
             "fx_rate": obj.get("fx_rate"),
             "amount_to_pay": obj.get("amount_to_pay"),
             "handling_charges": obj.get("handling_charges")
         })
         return _obj
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/order_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/purpose.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/purpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks200_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/setup_webhooks200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/setup_webhooks_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/models/success_message.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/models/success_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/__init__.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/beneficiaries/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/beneficiaries/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/beneficiaries/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/fx_rate_details/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/fx_rate_details/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/fx_rate_details/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_process/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/orders_order_id_process/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/orders_order_id_process/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/remitters/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/remitters/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/remitters/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/paths/webhooks/post.pyi` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/rest.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.6
+    The version of the OpenAPI document: 1.0.7
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/schemas.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/schemas.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_beneficiary_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_order_response.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_create_remitter_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_currency.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_error.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_lrs_api.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_purpose.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_setup_webhooks_request.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/cashfree_lrs_client/test/test_success_message.py` & `cashfree_lrs_client-1.0.7/cashfree_lrs_client/test/test_success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.6/pyproject.toml` & `cashfree_lrs_client-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "cashfree_lrs_client"
-version = "1.0.6"
+version = "1.0.7"
 description = "Cashfree LRS"
 authors = ["CashFree Care <nextgenapi@cashfree.com>"]
 license = "NoLicense"
 readme = "README.md"
-repository = "https://github.com/GIT_REPO_ID/GIT_USER_ID"
+repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Cashfree LRS"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
```

### Comparing `cashfree_lrs_client-1.0.6/PKG-INFO` & `cashfree_lrs_client-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cashfree-lrs-client
-Version: 1.0.6
+Version: 1.0.7
 Summary: Cashfree LRS
-Home-page: https://github.com/GIT_REPO_ID/GIT_USER_ID
+Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,Cashfree LRS
 Author: CashFree Care
 Author-email: nextgenapi@cashfree.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aenum (>=3.1.11)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: urllib3 (>=1.25.3)
-Project-URL: Repository, https://github.com/GIT_REPO_ID/GIT_USER_ID
+Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
 Description-Content-Type: text/markdown
 
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.6
-- Package version: 1.0.6
+- API version: 1.0.7
+- Package version: 1.0.7
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -147,14 +147,15 @@
  - [CreateOrderRequest](docs/CreateOrderRequest.md)
  - [CreateOrderResponse](docs/CreateOrderResponse.md)
  - [CreateRemitterRequest](docs/CreateRemitterRequest.md)
  - [Currency](docs/Currency.md)
  - [Error](docs/Error.md)
  - [FetchForexRateRequest](docs/FetchForexRateRequest.md)
  - [FetchForexRateResponse](docs/FetchForexRateResponse.md)
+ - [FetchForexRateResponseTcs](docs/FetchForexRateResponseTcs.md)
  - [Purpose](docs/Purpose.md)
  - [SetupWebhooksRequest](docs/SetupWebhooksRequest.md)
  - [SuccessMessage](docs/SuccessMessage.md)
 
 
 ## Documentation For Authorization
```


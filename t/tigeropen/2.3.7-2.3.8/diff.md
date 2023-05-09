# Comparing `tmp/tigeropen-2.3.7.tar.gz` & `tmp/tigeropen-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-2.3.7.tar", last modified: Tue Apr 18 08:29:48 2023, max compression
+gzip compressed data, was "tigeropen-2.3.8.tar", last modified: Tue May  9 12:42:33 2023, max compression
```

## Comparing `tigeropen-2.3.7.tar` & `tigeropen-2.3.8.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.101903 tigeropen-2.3.7/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.7/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-04-18 08:29:48.101671 tigeropen-2.3.7/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.7/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.7/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-04-18 08:29:48.101977 tigeropen-2.3.7/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.3.7/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.027768 tigeropen-2.3.7/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.030847 tigeropen-2.3.7/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.033441 tigeropen-2.3.7/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.7/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    18954 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.7/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2945 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.7/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.035800 tigeropen-2.3.7/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-02-16 07:36:42.000000 tigeropen-2.3.7/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.7/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.7/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.7/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.039547 tigeropen-2.3.7/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.040220 tigeropen-2.3.7/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.040548 tigeropen-2.3.7/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.041054 tigeropen-2.3.7/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.041931 tigeropen-2.3.7/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.045929 tigeropen-2.3.7/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.7/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.7/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.048777 tigeropen-2.3.7/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.052043 tigeropen-2.3.7/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.071329 tigeropen-2.3.7/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.7/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)     8946 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.072200 tigeropen-2.3.7/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.076959 tigeropen-2.3.7/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9598 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    76032 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.077894 tigeropen-2.3.7/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    33338 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.093978 tigeropen-2.3.7/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.7/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.7/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.7/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1129 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.7/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.7/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.094816 tigeropen-2.3.7/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.096677 tigeropen-2.3.7/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     4117 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)     9811 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.097528 tigeropen-2.3.7/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    32706 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.101366 tigeropen-2.3.7/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6736 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4864 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40415 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.029840 tigeropen-2.3.7/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7360 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.050021 tigeropen-2.3.8/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.8/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-05-09 12:42:33.049900 tigeropen-2.3.8/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.8/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.8/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-05-09 12:42:33.050056 tigeropen-2.3.8/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.3.8/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.021745 tigeropen-2.3.8/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.023597 tigeropen-2.3.8/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.025205 tigeropen-2.3.8/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.8/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.8/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.8/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.027026 tigeropen-2.3.8/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-2.3.8/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.8/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.8/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.8/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028027 tigeropen-2.3.8/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028300 tigeropen-2.3.8/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028435 tigeropen-2.3.8/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028558 tigeropen-2.3.8/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028794 tigeropen-2.3.8/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.029713 tigeropen-2.3.8/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.8/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.8/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.030432 tigeropen-2.3.8/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.031873 tigeropen-2.3.8/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.038467 tigeropen-2.3.8/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.8/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.038728 tigeropen-2.3.8/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.040394 tigeropen-2.3.8/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    76884 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.040626 tigeropen-2.3.8/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.045946 tigeropen-2.3.8/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.8/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.8/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.8/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.3.8/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.3.8/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.8/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.8/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.046194 tigeropen-2.3.8/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.047640 tigeropen-2.3.8/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4529 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9811 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.047887 tigeropen-2.3.8/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32706 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.049697 tigeropen-2.3.8/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6736 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4864 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40415 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.022603 tigeropen-2.3.8/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7360 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-2.3.7/PKG-INFO` & `tigeropen-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.7
+Version: 2.3.8
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.7/README.md` & `tigeropen-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/setup.py` & `tigeropen-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/__init__.py` & `tigeropen-2.3.8/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/filter_fields.py` & `tigeropen-2.3.8/tigeropen/common/consts/filter_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,46 +68,40 @@
     VolumeRatio = 21, "volumeRatio"
     # 委比*（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     BidAskRatio = 22, "committee"
     # 下次财报日期 *
     EarningDate = 23, "earningDate"
     # 市盈率* TTM（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     PeTTM = 24, "peRate"
-    # 市净率*（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
-    PbRate = 25, "pbRate"
     # 股息   hermes $
-    DividePrice = 26, "dividePrice"
+    DividePrice = 26, "dividePriceVal"
     # 股息收益率 选股服务自身计算
-    DivideRate = 27, "divideRate"
+    DivideRate = 27, "divideRateVal"
     # 股票交易市场
     Exchange = 29, "exchange"
     # 换手率*（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     TurnoverRate = 30, "turnoverRate"
     # 上市时间
     ListingDate = 31, "listingDate"
-    # 市盈率LYR* TTM（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
-    LyrPeRate = 32, "LyrPeRate"
     # 总股本*
     Share = 33, "shares"
     # 上市价格*
     ListingPrice = 34, "listingPrice"
-    # 交易币种*
-    TradeCurrency = 35, "tradeCurrency"
     # 最新价-发行价*
     DiffBetweenLastPriceAndListPrice = 36, "DiffBetweenLastPriceAndListPrice"
     # 每股收益 lyr=Last Year Ratio 静态市盈率
     lyr_Eps = 37, "lyrEps"
     # 未平仓做空量
-    Open_Short_Interest = 38, "OpenShortInterest"
+    Open_Short_Interest = 38, "OpenShortInterestVal"
     # 未平仓做空比例 = 未平仓做空量/总股本
     Open_Short_Interest_Ratio = 39, "OpenShortInterestRatio"
     # 产权比率 = Liability/Equity 总负债/股东
-    Equity_Ratio = 40, "EquityRatio"
+    Equity_Ratio = 40, "totalDebtToEquity"
     # 权益乘数 = Asset/Equity
-    Equity_Multiplier = 41, "EquityMultiplier"
+    Equity_Multiplier = 41, "totalLiabilitiesToTotalAssets"
     # 最新股东数
     Holder_Nums = 42, "holderNums"
     # 最新股东户数增长率
     Holder_Nums_Ratio = 43, "holderRatio"
     # 户均持股数量
     Per_Hold_Nums = 44, "perHolderNums"
     # 户均持股金额
@@ -124,29 +118,38 @@
     Top10_Composition_Rate = 50, "Top10CompoRate"
     # 成分股Top15 占比 - ETF
     Top15_Composition_Rate = 51, "Top15CompoRate"
     # 成分股Top20 占比 - ETF
     Top20_Composition_Rate = 52, "Top20CompoRate"
     # 溢价率(折扣率) - ETF
     DiscountPremium = 53, "discountPremium"
-    # 股息率 - ETF
-    dividend_Rate = 54, "dividendRate"
     # 资产规模-净值 - ETF
     Net_Worth_Aum = 55, "aum"
     # 资产规模-现价 - ETF
     assetSize = 56, "assetSize"
     # 振幅
     Amplitude = 57, "Amplitude"
-
+    #  盘前涨跌幅 
+    Pre_ChangeRate = 58, "preChangeRate"
+    # 盘中涨跌幅 */
+    current_ChangeRate = 59, "curChangeRate"
+    # 盘后涨跌幅 */
+    Post_ChangeRate = 60, "postChangeRate"
+    # 成分变动 - etf */
+    ETF_LastHoldingChangeDay = 61, "LastHoldingChangeDay"
+    # 持仓数量 - etf */
+    ETF_HoldingCount = 62, "etfHoldingCount"
+    # 净利润 不带周期 */
+    Net_Income = 63, "netIncomeVal"
 
 class AccumulateField(FilterField):
     # 涨跌幅*（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     ChangeRate = 1, "changeRate"
     # 涨跌额*（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
-    ChangeValue = 2, "change"
+    ChangeValue = 2, "changeVal"
     # 总负债增长率
     TotalLiabilities_Ratio_Annual = 3, "totalLiabilitiesRatio"
     # 净资产增长率
     TotalCommonEquity_Ratio_Annual = 4, "totalCommonEquityRatio"
     # 每股收益同比增长率
     BasicEps_Ratio_Annual = 5, "basicEpsRatio"
     # 净利润同比增长率
@@ -163,65 +166,60 @@
     Operating_Income = 11, "operatingIncome"
     # 营业收入
     Total_Revenue = 12, "total_revenue"
     # ROE = 资产回报率
     ROE = 13, "ROE"
     # ROA = 净资产收益率
     ROA = 14, "ROA"
-    # 股息   hermes $
-    DividePrice = 15, "dividePrice"
-    # 股息收益率 选股服务自身计算
-    DivideRate = 16, "divideRate"
     # 毛利率
     GrossProfitRate = 17, "grossMargin"
     # 净利率*
     NetProfitRate = 18, "netIncomeMargin"
     # 总资产*
     TotalAssets = 19, "totalAssets"
     # 流动比率
     CurrentRatio = 20, "currentRatio"
     # 速动比率
     QuickRatio = 21, "quickRatio"
-    # 经营现金流
-    CashFromOps = 22, "cash4Ops"
+    # 经营现金流比率
+    CashFromOpsRatio = 22, "cash4OpsRatio"
     # 投资现金流
     CashFromInvesting = 23, "cash4Invest"
     # 筹资现金流
     CashFromFinancing = 24, "cash4Finance"
     # 资产负债率
     TotalLiabilitiesToTotalAssets = 25, "allLiabAndAssets"
     # 经营现金流同比增长率; （T期CFO-T-1期CFO）/T-1期CFO *100%
     CashFromOps_yearOnYear_Ratio = 26, "cash4OpsYearOnYearRatio"
     # 净资产收益率ROE同比增长率  （T期ROE-T-1期ROE）/T-1期ROE *100%
     ROE_yearOnYear_Ratio = 27, "netIncomeYearOnYearRatio"
-
+    # 营业利润占比
+    Operating_Profits_Ratio = 28, "OperatingProfitsRatio"
+    # 经营现金流
+    CashFromOpsVal = 29, "cash4OpsVal"
 
 class FinancialField(FilterField):
     # 毛利率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
-    GrossProfitRate = 1, "grossMargin"
+    GrossProfitRate = 1, "grossMarginVal"
     # 净利率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
-    NetProfitRate = 2, "netIncomeMargin"
+    NetProfitRate = 2, "netIncomeMarginVal"
     # 扣非净利润率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     EarningsFromContOpsMargin = 3, "earningsFromContOpsMargin"
-    # 总负债/股东权益 (单位：元)
-    TotalDebtToEquity = 4, "totalDebtToEquity"
     # 长期负债/股东权益
     LongTermDebtToEquity = 5, "ltDebtToEquity"
     # EBIT/利息支出
     EbitToInterestExp = 6, "ebitToInterestExp"
-    # 总负债/总资产
-    TotalLiabilitiesToTotalAssets = 7, "totalLiabilitiesToTotalAssets"
     # 总资产周转率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     TotalAssetTurnover = 8, "totalAssetTurnover"
     # 应收帐款周转率
     AccountsReceivableTurnover = 9, "accountsReceivableTurnover"
     # 存货周转率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     InventoryTurnover = 10, "inventoryTurnover"
     # 流动比率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
-    CurrentRatio = 11, "currentRatio"
+    CurrentRatio = 11, "currentRatioVal"
     # 速动比率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     QuickRatio = 12, "quickRatio"
     # 资产回报率 总资产收益率 *$ TTM（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     ROATTM = 13, "roa"
     # 净资产收益率 $（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     ReturnOnEquityRate = 14, "roe"
     # 营业收入一年增长率 或者 营收增长率
@@ -234,15 +232,15 @@
     AccountsReceivable1YrGrowth = 18, "accountsReceivable1YrGrowth"
     # 存货一年增长率
     Inventory1YrGrowth = 19, "inventory1YrGrowth"
     # 总资产一年增长率
     TotalAssets1YrGrowth = 20, "totalAssets1YrGrowth"
     # 有形资产一年增长率
     TangibleBookValue1YrGrowth = 21, "tangibleBookValue1YrGrowth"
-    # 经营现金流一年增长率
+    # 经营现金流一年增长率  = 经营现金流同比增长率
     CashFromOperations1YrGrowth = 22, "cashFromOperations1YrGrowth"
     # 资本开支一年增长率
     CapitalExpenditures1YrGrowth = 23, "capitalExpenditures1YrGrowth"
     # 营业收入三年增长率 或者叫 营收3年复合增长率
     TotalRevenues3YrCagr = 24, "totalRevenues3YrCagr"
     # 毛利润率三年增长率
     GrossProfit3YrCagr = 25, "grossProfit3YrCagr"
@@ -265,41 +263,37 @@
     # 经营现金流
     CashFromOperations = 34, "cashFromOps"
     # 投资现金流
     CashFromInvesting = 35, "cashFromInvesting"
     # 筹资现金流
     CashFromFinancing = 36, "cashFromFinancing"
     # 净利润2年复合增长率
-    NormalizedNetIncome2YrCagr = 37, "normalizedNetIncome2YrCagr"
+    NormalizedNetIncome2YrCagr = 37, "netIncome2YrCagr"
     # 营收2年复合增长率
     TotalRevenues2YrCagr = 38, "totalRevenues2YrCagr"
     # 净利润5年复合增长率
     NetIncome5YrCagr = 39, "netIncome5YrCagr"
     # 营收5年复合增长率
     TotalRevenues5YrCagr = 40, "totalRevenues5YrCagr"
     # 总资产
-    TotalAssets = 41, "totalAssets"
+    TotalAssets = 41, "totalAssetsVal"
     # 固定资产周转率（精确到小数点后 3 位，超出部分会被舍弃）例如填写 [0.005,0.01] 值区间
     FixedAssetTurnover = 42, "fixedAssetTurnover"
     # 营业利润
-    OperatingIncome = 43, "operatingIncome"
+    OperatingIncome = 43, "operatingIncomeVal"
     # 营业总收入
     TotalRevenue = 44, "totalRevenue"
     # 市盈率LYR PE =price-to-earnings ratio
     LYR_PE = 45, "LyrPE"
     # 市盈率TTM PE =price-to-earnings ratio
     TTM_PE = 46, "ttmPE"
     # 市销率LYR PS =Price-to-sales Ratio
     LYR_PS = 47, "LyrPS"
     # 市销率TTM PS =Price-to-sales Ratio
     TTM_PS = 48, "ttmPS"
-    # 市净率LYR PB =price/book value ratio
-    LYR_PB = 47, "LyrPB"
-    # 市净率TTM PB =price/book value ratio
-    TTM_PB = 48, "ttmPB"
     # 当日主力净流入额
     LargeInflowAmountToday = 49, "largeInflowAmountToday"
     # 当日主力增仓占比
     LargeInflowAmountTodayPre = 50, "largeInflowAmountTodayPre"
     # 未平仓做空量
     ShortInterest = 51, "shortInterest"
     # 未平仓做空比例
@@ -332,15 +326,18 @@
     ListingAnnualVolatility = 65, "listingAnnualVolatility"
     # 近1年年化波动率  ETF
     LstYearAnnualVolatility = 66, "lstYearAnnualVolatility"
     # 近2年年化波动率  ETF
     Lst2YearAnnualVolatility = 67, "lst2YearAnnualVolatility"
     # 近5年年化波动率  ETF
     Lst5YearAnnualVolatility = 68, "lst5YearAnnualVolatility"
-
+    # 市净率LYR PB =price/book value ratio
+    LYR_PB = 69, "LyrPB"
+    # 市净率TTM PB =price/book value ratio
+    TTM_PB = 70, "ttmPB"
 
 class MultiTagField(FilterField):
     # 所属行业
     Industry = 1, "industry"
     # 所属概念
     Concept = 2, "concept"
     # 是否为otc股票.1=是，0=否
@@ -370,15 +367,22 @@
     Today_HistoryLow = 15, "todayHistoryLow"
     # 股票包
     Stock_Package = 16, "StockPkg"
     # 52周最高 0 否 1是*
     Week52HighFlag = 17, "week52HighFlag"
     # 52周最低 0 否 1是
     Week52LowFlag = 18, "week52LowFlag"
-
+    # 交易币种, 需要具体币种
+    TradeCurrency = 19, "tradeCurrency"
+    # ETF类型，需要具体类型
+    ETF_TYPE = 20, "etfType"
+    # 股票市场，支持多个市场
+    Market_Name = 21, "marketName"
+    # 一级行业级别, 需要传递具体sectorId
+    One_Sectors_Level = 22, "oneSectorsLevel"
 
 class FieldBelongType(Enum):
     """选股排序字段对应的filter类别
     """
     def __new__(cls, field_type, *args, **kwargs):
         obj = object.__new__(cls)
         obj._value_ = field_type
```

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-2.3.8/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/params.py` & `tigeropen-2.3.8/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/push_types.py` & `tigeropen-2.3.8/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/quote_keys.py` & `tigeropen-2.3.8/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/service_types.py` & `tigeropen-2.3.8/tigeropen/common/consts/service_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 QUOTE_REAL_TIME = "quote_real_time"
 QUOTE_DELAY = "quote_delay"
 QUOTE_SHORTABLE_STOCKS = "quote_shortable_stocks"
 QUOTE_STOCK_TRADE = "quote_stock_trade"
 QUOTE_DEPTH = "quote_depth"  # level2 深度行情
 GRAB_QUOTE_PERMISSION = "grab_quote_permission"  # 抢占行情
 MARKET_SCANNER = "market_scanner"  # 选股器
+MARKET_SCANNER_TAGS = "market_scanner_tags"
 GET_QUOTE_PERMISSION = "get_quote_permission"
 TRADING_CALENDAR = "trading_calendar"
 STOCK_BROKER = "stock_broker"  # 港股股票实时经纪队列
 CAPITAL_DISTRIBUTION = "capital_distribution"  # 股票当日资金分布
 CAPITAL_FLOW = "capital_flow"  # 股票资金流向
 WARRANT_FILTER = "warrant_filter"
 WARRANT_REAL_TIME_QUOTE = "warrant_real_time_quote"
```

### Comparing `tigeropen-2.3.7/tigeropen/common/consts/tick_constants.py` & `tigeropen-2.3.8/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/model.py` & `tigeropen-2.3.8/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/request.py` & `tigeropen-2.3.8/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/response.py` & `tigeropen-2.3.8/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/common_utils.py` & `tigeropen-2.3.8/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/contract_utils.py` & `tigeropen-2.3.8/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/order_utils.py` & `tigeropen-2.3.8/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/price_util.py` & `tigeropen-2.3.8/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/signature_utils.py` & `tigeropen-2.3.8/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/string_utils.py` & `tigeropen-2.3.8/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/tick_util.py` & `tigeropen-2.3.8/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/common/util/web_utils.py` & `tigeropen-2.3.8/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/client_config.py` & `tigeropen-2.3.8/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/nasdaq100.py` & `tigeropen-2.3.8/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-2.3.8/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/push_client_demo.py` & `tigeropen-2.3.8/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-2.3.8/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/quote_client_demo.py` & `tigeropen-2.3.8/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/examples/trade_client_demo.py` & `tigeropen-2.3.8/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/request/model.py` & `tigeropen-2.3.8/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-2.3.8/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-2.3.8/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-2.3.8/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-2.3.8/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-2.3.8/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/fundamental/response/industry_response.py` & `tigeropen-2.3.8/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/__init__.py` & `tigeropen-2.3.8/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/network/connect.py` & `tigeropen-2.3.8/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/network/exception.py` & `tigeropen-2.3.8/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/network/listener.py` & `tigeropen-2.3.8/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/network/protocal.py` & `tigeropen-2.3.8/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/network/transport.py` & `tigeropen-2.3.8/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/network/utils.py` & `tigeropen-2.3.8/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/AssetData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/PositionData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/PushData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/Request.proto` & `tigeropen-2.3.8/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-2.3.8/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-2.3.8/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/pb/util.py` & `tigeropen-2.3.8/tigeropen/push/pb/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 
 class ProtoMessageUtil:
 
     increment_count = 0
 
     @classmethod
-    @property
     def increment(cls):
         cls.increment_count += 1
         return cls.increment_count
 
     @classmethod
     def extract_heart_beat(cls, resp):
         if resp.command == SocketCommon_pb2.SocketCommon.CONNECTED and "heart-beat" in resp.msg:
@@ -47,15 +46,15 @@
 
     @classmethod
     def build_connect_message(cls, tiger_id, sign, version='3', send_interval=0, receive_interval=0):
         if send_interval < 0 or receive_interval < 0:
             raise ValueError("sendInterval < 0 or receiveInterval < 0")
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.CONNECT
-        request.id = cls.increment
+        request.id = cls.increment()
 
         con = Request_pb2.Request.Connect()
         con.acceptVersion = version
         con.sdkVersion = P_SDK_VERSION_PREFIX + __VERSION__  # Replace with the appropriate SDK version
         con.tigerId = tiger_id
         con.sign = sign
         con.sendInterval = send_interval
@@ -63,44 +62,44 @@
         request.connect.CopyFrom(con)
         return request
 
     @classmethod
     def build_disconnect_message(cls):
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.DISCONNECT
-        request.id = cls.increment
+        request.id = cls.increment()
         return request
 
     @classmethod
     def build_send_message(cls):
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.SEND
-        request.id = cls.increment
+        request.id = cls.increment()
         return request
 
     @classmethod
     def build_heart_beat_message(cls):
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.HEARTBEAT
-        request.id = cls.increment
+        request.id = cls.increment()
         return request
 
     @classmethod
     def build_subscribe_trade_message(cls, data_type, account):
         return cls.build_trade_message(data_type, account, SocketCommon_pb2.SocketCommon.SUBSCRIBE)
 
     @classmethod
     def build_unsubscribe_trade_message(cls, data_type, account):
         return cls.build_trade_message(data_type, account, SocketCommon_pb2.SocketCommon.UNSUBSCRIBE)
 
     @classmethod
     def build_subscribe_query_message(cls):
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.SEND
-        request.id = cls.increment
+        request.id = cls.increment()
         return request
 
     @classmethod
     def build_subscribe_quote_message(cls, symbols, data_type=SocketCommon_pb2.SocketCommon.Quote):
         return cls.build_quote_message(data_type, symbols, SocketCommon_pb2.SocketCommon.SUBSCRIBE)
 
     @classmethod
@@ -131,40 +130,40 @@
     def build_unsubscribe_market_message(cls, market):
         return cls.build_market_quote_message(market, SocketCommon_pb2.SocketCommon.UNSUBSCRIBE)
 
     @classmethod
     def build_quote_message(cls, data_type, symbols, command):
         request = Request_pb2.Request()
         request.command = command
-        request.id = cls.increment
+        request.id = cls.increment()
 
         sub = Request_pb2.Request.Subscribe()
         sub.dataType = data_type
         if symbols:
             sub.symbols = ','.join(symbols) if isinstance(symbols, list) else symbols
         request.subscribe.CopyFrom(sub)
         return request
 
     @classmethod
     def build_market_quote_message(cls, market, command):
         request = Request_pb2.Request()
         request.command = command
-        request.id = cls.increment
+        request.id = cls.increment()
 
         sub = Request_pb2.Request.Subscribe()
         sub.dataType = SocketCommon_pb2.SocketCommon.Quote
         sub.market = market
         request.subscribe.CopyFrom(sub)
         return request
 
     @classmethod
     def build_trade_message(cls, data_type, account, command):
         request = Request_pb2.Request()
         request.command = command
-        request.id = cls.increment
+        request.id = cls.increment()
 
         sub = Request_pb2.Request.Subscribe()
         sub.dataType = data_type
         if account:
             sub.account = account
         request.subscribe.CopyFrom(sub)
         return request
```

### Comparing `tigeropen-2.3.7/tigeropen/push/protobuf_push_client.py` & `tigeropen-2.3.8/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/push_client.py` & `tigeropen-2.3.8/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/push/stomp_push_client.py` & `tigeropen-2.3.8/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/domain/filter.py` & `tigeropen-2.3.8/tigeropen/quote/domain/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.period = period
 
     def to_dict(self):
         return {
             'field_name': self.field.index,
             'field_type': self.field.field_type_request_name,
             'sort_dir': self.sort_dir.value,
-            'period': self.period.value
+            'period': self.period.value if self.period else None
         }
 
 
 class StockFilter:
     def __init__(self, field, filter_min=None, filter_max=None, is_no_filter=False, accumulate_period=None,
                  financial_period=None, tag_list=None):
         """
```

### Comparing `tigeropen-2.3.7/tigeropen/quote/domain/quote_brief.py` & `tigeropen-2.3.8/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/domain/stock_broker.py` & `tigeropen-2.3.8/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/quote_client.py` & `tigeropen-2.3.8/tigeropen/quote/quote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from tigeropen.common.consts import Market, QuoteRight, BarPeriod, OPEN_API_SERVICE_VERSION_V3, \
     OPEN_API_SERVICE_VERSION_V1
 from tigeropen.common.consts import THREAD_LOCAL, SecurityType, CorporateActionType, IndustryLevel
 from tigeropen.common.consts.filter_fields import FieldBelongType
 from tigeropen.common.consts.service_types import GRAB_QUOTE_PERMISSION, QUOTE_DELAY, GET_QUOTE_PERMISSION, \
     HISTORY_TIMELINE, FUTURE_CONTRACT_BY_CONTRACT_CODE, TRADING_CALENDAR, FUTURE_CONTRACTS, MARKET_SCANNER, \
-    STOCK_BROKER, CAPITAL_FLOW, CAPITAL_DISTRIBUTION, WARRANT_REAL_TIME_QUOTE, WARRANT_FILTER
+    STOCK_BROKER, CAPITAL_FLOW, CAPITAL_DISTRIBUTION, WARRANT_REAL_TIME_QUOTE, WARRANT_FILTER, MARKET_SCANNER_TAGS
 from tigeropen.common.consts.service_types import MARKET_STATE, ALL_SYMBOLS, ALL_SYMBOL_NAMES, BRIEF, \
     TIMELINE, KLINE, TRADE_TICK, OPTION_EXPIRATION, OPTION_CHAIN, FUTURE_EXCHANGE, OPTION_BRIEF, \
     OPTION_KLINE, OPTION_TRADE_TICK, FUTURE_KLINE, FUTURE_TICK, FUTURE_CONTRACT_BY_EXCHANGE_CODE, \
     FUTURE_TRADING_DATE, QUOTE_SHORTABLE_STOCKS, FUTURE_REAL_TIME_QUOTE, \
     FUTURE_CURRENT_CONTRACT, QUOTE_REAL_TIME, QUOTE_STOCK_TRADE, FINANCIAL_DAILY, FINANCIAL_REPORT, CORPORATE_ACTION, \
     QUOTE_DEPTH, INDUSTRY_LIST, INDUSTRY_STOCKS, STOCK_INDUSTRY, STOCK_DETAIL
 from tigeropen.common.exceptions import ApiException
@@ -59,15 +59,15 @@
 from tigeropen.quote.response.quote_brief_response import QuoteBriefResponse
 from tigeropen.quote.response.quote_delay_briefs_response import DelayBriefsResponse
 from tigeropen.quote.response.quote_depth_response import DepthQuoteResponse
 from tigeropen.quote.response.quote_grab_permission_response import QuoteGrabPermissionResponse
 from tigeropen.quote.response.quote_ticks_response import TradeTickResponse
 from tigeropen.quote.response.quote_timeline_history_response import QuoteTimelineHistoryResponse
 from tigeropen.quote.response.quote_timeline_response import QuoteTimelineResponse
-from tigeropen.quote.response.market_scanner_response import MarketScannerResponse
+from tigeropen.quote.response.market_scanner_response import MarketScannerResponse, MarketScannerTagsResponse
 from tigeropen.quote.response.stock_briefs_response import StockBriefsResponse
 from tigeropen.quote.response.stock_broker_response import StockBrokerResponse
 from tigeropen.quote.response.stock_details_response import StockDetailsResponse
 from tigeropen.quote.response.stock_short_interest_response import ShortInterestResponse
 from tigeropen.quote.response.stock_trade_meta_response import TradeMetaResponse
 from tigeropen.quote.response.symbol_names_response import SymbolNamesResponse
 from tigeropen.quote.response.symbols_response import SymbolsResponse
@@ -1369,15 +1369,15 @@
         :param sort_field_data: tigeropen.quote.domain.filter.FilterSortData
         :param page: page begin number
         :param page_size: page size limit
         :return:
         """
         params = MarketScannerParams()
         params.version = OPEN_API_SERVICE_VERSION_V1
-        params.market = market.value
+        params.market = get_enum_value(market)
         if filters is not None:
             params.base_filter_list = list()
             params.accumulate_filter_list = list()
             params.financial_filter_list = list()
             params.multi_tags_filter_list = list()
             for f in filters:
                 if f.field_belong_type == FieldBelongType.BASE:
@@ -1398,14 +1398,31 @@
             response = MarketScannerResponse()
             response.parse_response_content(response_content)
             if response.is_success():
                 return response.result
             else:
                 raise ApiException(response.code, response.message)
 
+    def get_market_scanner_tags(self, market=Market.US, tag_fields=None):
+        """
+        :param market: tigeropen.common.consts.Market
+        :param tag_fields: tigeropen.common.consts.filter_fields.MultiTagField
+        """
+        params = MarketScannerParams()
+        params.market = get_enum_value(market)
+        params.multi_tags_fields = tag_fields
+        request = OpenApiRequest(MARKET_SCANNER_TAGS, biz_model=params)
+        response_content = self.__fetch_data(request)
+        if response_content:
+            response = MarketScannerTagsResponse()
+            response.parse_response_content(response_content)
+            if response.is_success():
+                return response.result
+            else:
+                raise ApiException(response.code, response.message)
     def grab_quote_permission(self):
         """
         抢占行情权限
         :return: 权限列表。expire_at 为-1时表示长期有效
         示例: [{'name': 'usQuoteBasic', 'expire_at': 1621931026000},
               {'name': 'usStockQuoteLv2Totalview', 'expire_at': 1621931026000},
               {'name': 'usOptionQuote', 'expire_at': 1621931026000},
```

### Comparing `tigeropen-2.3.7/tigeropen/quote/request/model.py` & `tigeropen-2.3.8/tigeropen/quote/request/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -846,15 +846,15 @@
         self._base_filter_list = None
         self._accumulate_filter_list = None
         self._financial_filter_list = None
         self._multi_tags_filter_list = None
         self._sort_field_data = None
         self._page = None
         self._page_size = None
-
+        self._multi_tags_fields = None
     @property
     def market(self):
         return self._market
 
     @market.setter
     def market(self, value):
         self._market = value
@@ -911,14 +911,22 @@
     def page_size(self):
         return self._page_size
 
     @page_size.setter
     def page_size(self, value):
         self._page_size = value
 
+    @property
+    def multi_tags_fields(self):
+        return self._multi_tags_fields
+
+    @multi_tags_fields.setter
+    def multi_tags_fields(self, value):
+        self._multi_tags_fields = value
+
     def to_openapi_dict(self):
         """
         example
         {"accumulate_filter_list":
             [{"field_name":"AccumulateField_ChangeRate","filter_max":1,"filter_min":0.01,"is_no_filter":false,"period":"Last_Year"}],
         "base_filter_list":
             [{"field_name":"StockField_FloatShare","filter_max":10000000000000.0,"filter_min":10000000.0,"is_no_filter":true},
@@ -946,14 +954,16 @@
             params['multi_tags_filter_list'] = self.multi_tags_filter_list
         if self.sort_field_data:
             params['sort_field_data'] = self.sort_field_data.to_dict()
         if self.page is not None:
             params['page'] = self.page
         if self.page_size is not None:
             params['page_size'] = self.page_size
+        if self.multi_tags_fields:
+            params['multi_tag_field_list'] = [f.index for f in self.multi_tags_fields]
         return params
 
 
 class StockBrokerParams(BaseParams):
     def __init__(self):
         super().__init__()
         self._symbol = None
```

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/future_contract_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/market_scanner_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 # 
 # @Date    : 2021/11/18
 # @Author  : sukai
+import json
+
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util.string_utils import camel_to_underline_obj
 from tigeropen.quote.domain.filter import ScannerResult
 
 
 class MarketScannerResponse(TigerResponse):
     def __init__(self):
@@ -21,7 +23,25 @@
             data = camel_to_underline_obj(self.data)
             self.result = ScannerResult(page=data.get('page'),
                                         page_size=data.get('page_size'),
                                         total_page=data.get('total_page'),
                                         total_count=data.get('total_count'),
                                         items=data.get('items'))
         return self.result
+
+
+class MarketScannerTagsResponse(TigerResponse):
+    def __init__(self):
+        super(MarketScannerTagsResponse, self).__init__()
+        self.result = None
+        self._is_success = None
+
+    def parse_response_content(self, response_content):
+        response = super(MarketScannerTagsResponse, self).parse_response_content(response_content)
+        if 'is_success' in response:
+            self._is_success = response['is_success']
+        if self.data:
+            if isinstance(self.data, str):
+                self.data = json.loads(self.data)
+            data = camel_to_underline_obj(self.data)
+            self.result = data
+        return self.result
```

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/market_status_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/option_chains_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/stock_details_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/symbols_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-2.3.8/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/tiger_open_client.py` & `tigeropen-2.3.8/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/tiger_open_config.py` & `tigeropen-2.3.8/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/domain/account.py` & `tigeropen-2.3.8/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/domain/contract.py` & `tigeropen-2.3.8/tigeropen/trade/domain/contract.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  local_symbol=None, expiry=None, strike=None, put_call=None, multiplier=None, name=None,
                  short_margin=None, short_initial_margin=None, short_maintenance_margin=None,
                  short_fee_rate=None, shortable=None, shortable_count=None, long_initial_margin=None,
                  long_maintenance_margin=None, contract_month=None, identifier=None, primary_exchange=None,
                  market=None, min_tick=None, trading_class=None, status=None, continuous=None, trade=None,
                  marginable=None, close_only=None,
                  last_trading_date=None, first_notice_date=None, last_bidding_close_time=None, tick_sizes=None,
-                 is_etf=None, etf_leverage=None):
+                 is_etf=None, etf_leverage=None, **kwargs):
         self.contract_id = contract_id
         self.symbol = symbol
         self.currency = get_enum_value(currency)
         self.sec_type = get_enum_value(sec_type)
         self.exchange = exchange
         self.origin_symbol = origin_symbol
         self.local_symbol = local_symbol
@@ -79,14 +79,20 @@
         # 期货专有，竞价截止时间
         self.last_bidding_close_time = last_bidding_close_time
         # 是否是ETF
         self.is_etf = is_etf
         # ETF杠杆倍数
         self.etf_leverage = etf_leverage
 
+        self.discounted_day_initial_margin = kwargs.get('discounted_day_initial_margin')
+        self.discounted_day_maintenance_margin = kwargs.get('discounted_day_maintenance_margin')
+        self.discounted_time_zone_code = kwargs.get('discounted_time_zone_code')
+        self.discounted_start_at = kwargs.get('discounted_start_at')
+        self.discounted_end_at = kwargs.get('discounted_end_at')
+
     @property
     def right(self):
         return self.put_call
 
     def __repr__(self):
         identifier = self.identifier if self.identifier else self.symbol
         if self.sec_type == SecurityType.FUT.value:
```

### Comparing `tigeropen-2.3.7/tigeropen/trade/domain/order.py` & `tigeropen-2.3.8/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/domain/position.py` & `tigeropen-2.3.8/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/domain/prime_account.py` & `tigeropen-2.3.8/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/request/model.py` & `tigeropen-2.3.8/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/__init__.py` & `tigeropen-2.3.8/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/account_profile_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/assets_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/contracts_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/forex_order_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/order_id_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/order_preview_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/orders_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/positions_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/response/transactions_response.py` & `tigeropen-2.3.8/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen/trade/trade_client.py` & `tigeropen-2.3.8/tigeropen/trade/trade_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.7/tigeropen.egg-info/PKG-INFO` & `tigeropen-2.3.8/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.7
+Version: 2.3.8
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.7/tigeropen.egg-info/SOURCES.txt` & `tigeropen-2.3.8/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

